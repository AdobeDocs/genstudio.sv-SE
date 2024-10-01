---
title: Anpassa en mall
description: Lär dig hur du anpassar och optimerar din mall för Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Templates, Content
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: 54fd20fec553b545b2f5d64cdf9327098b16580f
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 0%

---

# Anpassa en mall

Anpassa HTML-mallarna för Adobe GenStudio for Performance Marketing med hjälp av mallspråket _Handlebars_ . Syntaxen [!DNL Handlebars] använder vanlig text med dubbla klammerparenteser som innehållsplatshållare. Läs [`What is [!DNL Handlebars]?`](https://handlebarsjs.com/guide/#what-is-handlebars) i _Handlebars språkguide_ om du vill lära dig hur du förbereder mallen.

I de följande avsnitten beskrivs hur du lägger till platshållare för innehåll, döljer onödiga element från förhandsgranskning och hanterar länkar till statiskt innehåll. När mallen är klar kan du [överföra den till GenStudio for Performance Marketing](use-templates.md#upload-a-template) och börja generera anpassade e-postmeddelanden baserat på din anpassade mall.

## Platshållare för innehåll

GenStudio for Performance Marketing känner igen vissa [element](use-templates.md#template-elements) i en mall, men bara om du identifierar dem med ett känt fältnamn.

I mallens huvud eller brödtext kan du använda syntaxen [!DNL Handlebars] som en innehållsplatshållare där du kräver att GenStudio for Performance Marketing ska fylla i mallen med faktiskt innehåll. GenStudio for Performance Marketing känner igen och tolkar platshållarna för innehåll baserat på det [identifierade _fältnamnet_](#recognized-field-names).

Du kan till exempel använda `{{ headline }}` med syntaxen [!DNL Handlebars] för att ange var rubriken i e-postmeddelandet ska placeras:

```handlebars
<div>{{headline}}</div>
```

### Identifierade fältnamn

I följande tabell visas de fältnamn som GenStudio for Performance Marketing har identifierat för ifyllning i mallar. Lägg till de här fältnamnen med syntaxen [!DNL Handlebars] i mallen där du behöver GenStudio for Performance Marketing för att generera innehåll.

| Fält | Roll | Kanalmall |
| -------------- | ---------------------- | ------------------------------ |
| `pre_header` | Förrubrik | e-post |
| `headline` | Headline | e-post <br>Meta ad |
| `body` | Body copy | e-post <br>Meta ad |
| `cta` | Uppmaning | e-post <br>Meta ad |
| `on_image_text` | På bildtext | Meta ad |
| `image` | Bild | e-post <br>Meta ad |
| `brand_logo` | Logotyp för markerat varumärke<br>Se [Fältnamn för logotyp för varumärke](#brand-logo-field-name) för rekommenderad användning. | e-post<br>Meta ad |

GenStudio for Performance Marketing fyller i vissa fält automatiskt i följande mallar:

- **E-postmallen** kräver inte att du identifierar fältet `subject`
- **Meta Ads-mallen** kräver inte att du identifierar fälten `headline`, `body` och `CTA`

<!--
- **Display Ads template** does not require you to idenitify the `CTA` field
-->

>[!WARNING]
>
>För Instagram-annonser visas den genererade rubriken inte i den slutliga versionen.

Det finns en gräns på 20 fält när en mall överförs till GenStudio for Performance Marketing. Eftersom fältet `subject` genereras automatiskt i ett e-postmeddelande räknas det som ett fält. Det innebär att 19 fält tillåts i en e-postmall.

>[!TIP]
>
>Du kan verifiera mallen med [mallförhandsgranskning](#template-preview) i GenStudio for Performance Marketing.

#### Fältnamn för märkeslogotyp

För närvarande kan du inte välja logotypen för mallöverföringen. I följande exempel visas två metoder som villkorligt återger varumärkeslogotypen. Varje metod verifierar källan, ger en standardbild eller alternativ bild om logotypen inte är tillgänglig och använder en stil:

**Exempel 1**: Använder [!DNL Handlebars] villkor för inbyggda hjälpredor direkt i HTML-attributet `img src`:

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**Exempel 2**: Använder [!DNL Handlebars] inbyggd villkorssats för att kapsla in HTML-taggen `img`:

```handlebars
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

#### Manuella fältnamn

Alla andra fältnamn behandlas som manuellt ifyllda fält.

Om du vill skapa ett redigerbart avsnitt lägger du till dubbla hakparenteser runt avsnittsnamnet:

```handlebars
{{customVariable}}
```

### Avsnitt eller grupper

_Avsnitt_ informerar GenStudio for Performance Marketing om att fälten i det här avsnittet kräver hög grad av konsekvens. Genom att etablera relationen kan AI generera innehåll som matchar de kreativa elementen i avsnittet.

Använd ett prefix som du väljer i fältnamnet för att ange att ett fält är en del av ett avsnitt eller en grupp. Du kan till exempel markera innehåll som visas i ett markerat område:

- `pod1_headline`
- `pod1_body`

Varje avsnitt kan bara använda en av varje fälttyp. I exemplet ovan kan avsnittet `pod1` bara använda ett `pod1_headline`-fält.

En mall kan innehålla upp till tre avsnitt:

- `headline`
- `body`
- `pod1_headline`
- `pod1_body`
- `pod2_headline`
- `pod2_body`

GenStudio for Performance Marketing förstår att `pod1_headline` är närmare relaterat till `pod1_body` än till `pod2_body`.

## Förhandsgranska mall

När du [överför en mall](use-templates.md#upload-a-template) söker GenStudio for Performance Marketing igenom filen HTML efter identifierade fält. Använd förhandsgranskningen för att granska dina [mallelement](use-templates.md#template-elements) och bekräfta att du har identifierat dem korrekt med de [igenkända fältnamnen](#recognized-field-names).

Exempel på Förhandsgranska för en e-postmall:

![Förhandsgranskningsfält har identifierats](../../assets/template-detected-fields.png){width="650"}

### Förhandsgranska kontroll

Du kan styra visningen av specialinnehåll med hjälp av inbyggda hjälpredor (specialuttryck i mallspråket [!DNL Handlebars] som utför vissa åtgärder). Du kan till exempel lägga till en villkorssats som lägger till spårningsparametrar till länkar i den exporterade mallen samtidigt som förhandsgranskningslänkarna hålls rena.

Värdet `_genStudio.browser` anges när en mall återges och värdet `genStudio.export` anges när en mall exporteras. Du kan välja att ta med visst innehåll högst upp i ett e-postmeddelande med en villkorlig omslutning, till exempel när mallen används för export:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Ett annat exempel kan vara att förhindra att spårningskoder används när en mall förhandsgranskas i GenStudio for Performance Marketing. I följande exempel visas hur du lägger till spårningsparametrar till länkar i den exporterade mallen, samtidigt som du håller förhandsgranskningslänkarna rena:

```handlebars
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## Statiskt innehåll

E-post- och metamallar länkar ofta till bilder och CSS-filer som lagras utanför GenStudio for Performance Marketing. När GenStudio for Performance Marketing genererar miniatyrbilder för dessa mallar eller de upplevelser som härleds från dem, kan dessa externa resurser ignoreras om de inte har rätt CORS-rubriker (Cross-Origin Resource Sharing).

Om du vill vara säker på att de här resurserna är tillgängliga när du genererar miniatyrbilder bör du överväga två alternativ:

1. **Använd CORS-huvuden**: Värdservern måste skicka svar med ett `Access-Control-Allow-Origin`-huvud inställt på `https://experience.adobe.com` för produktionsmiljöer. Med den här metoden kan GenStudio for Performance Marketing komma åt och inkludera resurserna.

1. **Använd data-URL:er**: Bädda in de externa resurserna direkt i mallen med data-URL:er. Den här metoden åsidosätter CORS-begränsningar och ser till att resurserna är tillgängliga under genereringen av miniatyrbilder.

## Exempel på mallar

+++Exempel: E-postmall med ett avsnitt

Nedan följer ett grundläggande exempel på en HTML-mall för ett e-postmeddelande som innehåller ett avsnitt. Huvudet innehåller enkel, infogad CSS för formatering. Innehållet innehåller en `pre-header`, `headline` och `image` [platshållare](#content-placeholders) som GenStudio for Performance Marketing kan använda för att mata in innehåll under e-postgenereringsprocessen.

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
    <!-- Pod1 -->
        <div class="pod">
            <h2>{{ pod1_header }}</h2>
            <p>{{ pod1_body }}</p>
        </div>
        <!-- End of Pod1 -->
    <!-- Pod2 -->
        <div class="pod">
            <h2>{{ pod2_header }}</h2>
            <p>{{ pod2_body }}</p>
        </div>
        <!-- End of Pod2 -->
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
