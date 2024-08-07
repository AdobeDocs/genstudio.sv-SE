---
title: Anpassa mallar
description: Lär dig hur du skapar en anpassad mall för GenStudio.
level: Intermediate
feature: Templates, Content
source-git-commit: 6870f1b7056219d03cabbcc4e5ddbfa436b1a56d
workflow-type: tm+mt
source-wordcount: '788'
ht-degree: 0%

---


# Anpassa mallar

Du kan anpassa dina HTML-mallar för GenStudio med hjälp av mallspråket _Handlebars_ . I Handlebars syntax används vanlig text med dubbla klammerparenteser som innehållsplatshållare. Läs [`What is Handlebars?`](https://handlebarsjs.com/guide/#what-is-handlebars) i _Handlebars språkguide_ om du vill lära dig hur du förbereder mallen.

<!-- This is for email. In the future, maybe use tabs to provide guidance for other template types.
-->If you do not have an HTML template ready to use in GenStudio, you can start by defining the structure of your email using HTML tags: `DOCTYPE`, `html`, `head`, and `body`. You can include CSS styles to customize the appearance of your email.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Title</title>
    <style>
    </style>
</head>
<body>
</body>
</html>
```

Se [Mallexempel](#template-examples).

>[!TIP]
>
>I de följande avsnitten lägger du till platshållare för innehåll för e-postfält, läser exempelmallar, döljer onödiga element från förhandsgranskning och hanterar länkar till statiskt innehåll. När mallen är klar kan du [överföra den till GenStudio](use-templates.md#upload-a-template) och börja generera anpassade e-postmeddelanden baserat på din anpassade mall.

## Platshållare för innehåll

I mallens huvud eller brödtext kan du använda Handlebars syntax för att infoga platshållare för innehåll där du kräver att GenStudio ska fylla i mallen med det faktiska innehållet. GenStudio känner igen och tolkar platshållarna för innehållet automatiskt baserat på fältnamnet.

Du kan till exempel använda `{{ headline }}` för att ange var rubriken i e-postmeddelandet ska placeras:

```handlebars
<div>{{ headline }}</div>
```

### Fältnamn

Det högsta antalet fält som tillåts i en anpassad mall är tjugo.

#### Identifierade fältnamn

I följande tabell visas de fältnamn som GenStudio har identifierat för ifyllning i mallar.

| Fält | Roll | Kanalmall |
| -------------- | ---------------------- | -------------------- |
| `pre_header` | Förrubrik | e-post (rekommenderas) |
| `headline` | Headline | e-post (rekommenderas)<br>Meta ad |
| `body` | Body copy | e-post (rekommenderas)<br>Meta ad |
| `cta` | Uppmaning | e-post (rekommenderas)<br>Meta ad |
| `on_image_text` | På bildtext | Meta ad (rekommenderas) |
| `image` | Bild | e-post (rekommenderas)<br>Meta ad (rekommenderas) |
| `brand_logo` | Det valda varumärkets logotyp | Meta ad |

GenStudio fyller automatiskt i vissa fält i mallar, så du behöver inte ta med dem i malldesignen:

* fältet `subject` (e-postmall)
* `headline`, `body` och `CTA` fält (Meta ad template)

>[!WARNING]
>
>För Instagram-annonser visas den genererade rubriken inte i den slutliga versionen.

#### Manuella fältnamn

Alla andra fältnamn behandlas som manuellt ifyllda fält. Om du vill att ett avsnitt ska kunna redigeras lägger du till dubbla hakparenteser runt det avsnitt du vill redigera.

> Exempel: ``{{customVariable}}`` (customVariable är det manuellt redigerbara avsnittet)

## Avsnitt eller grupper

_Avsnitt_ informerar GenStudio om att fält i det här avsnittet kräver hög grad av konsekvens. Genom att etablera relationen kan AI generera innehåll som matchar de kreativa elementen i avsnittet.

Använd ett prefix som du väljer i fältnamnet för att ange att ett fält är en del av ett avsnitt eller en grupp.

Du kan till exempel markera innehåll som visas i ett markerat område:

* `spotlight_headline`
* `spotlight_body`

Varje avsnitt kan bara ha en av varje fälttyp. I exemplet ovan kan prefixet `spotlight` bara ha ett `spotlight_headline`-fält.

En mall kan innehålla upp till tre avsnitt:

* `headline`
* `body`
* `spotlight_headline`
* `spotlight_body`
* `news_headline`
* `news_body`

GenStudio förstår att `spotlight_headline` är närmare relaterat till `spotlight_body` än till `news_body`.

## Exempel på mallar

+++Exempel: E-postmall med ett avsnitt

Nedan följer ett grundläggande exempel på en HTML-mall för ett e-postmeddelande som innehåller ett avsnitt. Huvudet innehåller enkel, infogad CSS för formatering. Innehållet innehåller en `pre-header`, `headline` och `image` [platshållare](#content-placeholders) som GenStudio kan använda för att mata in innehåll under e-postgenereringsprocessen.

```handlebars {line-numbers="true" highlight="13"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    </div>
</body>
</html>
```

+++

+++Exempel: E-postmall med flera avsnitt

Följande är samma HTML-mall i exemplet ovan, men med ytterligare två avsnitt. Huvudet innehåller infogad CSS för att formatera en grupp. Brödtexten använder två grupper med [platshållare för innehåll](#content-placeholders) som använder ett prefix.

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
        .pod {
            background-color: #f8f8f8;
            margin: 10px;
            padding: 20px;
            border-radius: 5px;
        }
        .pod h2 {
            color: #333;
        }
        .pod p {
            color: #666;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
        <div class="pod">
            <h2>{{ pod1_headline }}</h2>
            <p>This is Pod 1 content.</p>
        </div>
        <div class="pod">
            <h2>{{ pod2_headline }}</h2>
            <p>This is Pod 2 content.</p>
        </div>
    </div>
</body>
</html>
```

+++

+++Exempel: Meta ad template

Följande är ett grundläggande exempel på en Meta-annonsmall. Huvudet innehåller infogad CSS för formatering. Brödtexten använder [platshållare för innehåll](#content-placeholders) med ett prefix.

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Adobe</title>
    <style>
        .ad-container {
            width: 300px;
            border: 1px solid #ddd;
            padding: 16px;
            font-family: Arial, sans-serif;
        }
        .ad-image {
            width: 100%;
            height: auto;
        }
        .ad-headline {
            font-size: 18px;
            font-weight: bold;
            margin: 12px 0;
        }
        .ad-body {
            font-size: 14px;
            margin: 12px 0;
        }
        .ad-cta {
            display: inline-block;
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            text-decoration: none;
            border-radius: 4px;
            text-align: center;
        }
    </style>
</head>
<body>
<div class="ad-container">
    <img src="{{ image }}" alt="Ad Image" class="ad-image">
    <div class="ad-headline">"{{ headline }}"</div>
    <div class="ad-body">"{{ body }}"</div>
    <a href="(https://example.com)" class="ad-cta">"{{ CTA }}"</a>
</div>

</body>
</html>
```

+++

## Förhandsgranska mall

Kontrollera synligheten för specialinnehåll med hjälp av inbyggda hjälpredor (specialuttryck i mallspråket Handlebars som utför vissa åtgärder). Du kan till exempel lägga till spårningsparametrar till länkar i den exporterade mallen samtidigt som förhandsgranskningslänkarna hålls rena.

Värdet `_genStudio.browser` anges när en mall återges och värdet `genStudio.export` anges när en mall exporteras. Du kan välja att ta med visst innehåll högst upp i ett e-postmeddelande med en villkorlig omslutning, till exempel när mallen används för export:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Ett annat exempel kan vara att förhindra att spårningskoder används när en mall förhandsgranskas i GenStudio. I det här exemplet visas hur du lägger till spårningsparametrar till länkar i den exporterade mallen, samtidigt som du håller förhandsgranskningslänkarna rena:

```handlebars
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## Statiskt innehåll

E-post- och metamallar länkar ofta till bilder och CSS-filer som lagras utanför GenStudio. När GenStudio genererar miniatyrbilder för dessa mallar eller de upplevelser som härleds från dem, kan dessa externa resurser ignoreras om de inte har rätt CORS-rubriker (Cross-Origin Resource Sharing).

Om du vill vara säker på att de här resurserna är tillgängliga när du genererar miniatyrbilder bör du överväga två alternativ:

1. **Använd CORS-huvuden**: Värdservern måste skicka svar med ett `Access-Control-Allow-Origin`-huvud inställt på `https://experience.adobe.com` för produktionsmiljöer. Med den här metoden kan GenStudio komma åt och inkludera resurserna.
1. **Använd data-URL:er**: Bädda in de externa resurserna direkt i mallen med data-URL:er. Den här metoden åsidosätter CORS-begränsningar och ser till att resurserna är tillgängliga under genereringen av miniatyrbilder.
