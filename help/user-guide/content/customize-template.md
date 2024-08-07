---
title: Anpassa mallar
description: Lär dig hur du skapar en anpassad mall för GenStudio.
level: Intermediate
feature: Templates, Content
source-git-commit: 423956d6fdbf5b31041d44eb434f90d55a87d7c0
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 0%

---


# Anpassa mallar

Du kan anpassa dina HTML-mallar för GenStudio med hjälp av mallspråket _Handlebars_ . I Handlebars syntax används vanlig text med dubbla klammerparenteser som innehållsplatshållare. Läs [`What is Handlebars?`](https://handlebarsjs.com/guide/#what-is-handlebars) i _Handlebars språkguide_ om du vill lära dig hur du förbereder mallen.

## Mallstruktur

<!-- This is for email. In the future, maybe use tabs to provide guidance for other template types.
-->

Om du inte har någon HTML-mall som kan användas i GenStudio kan du börja med att definiera e-postmeddelandets struktur med hjälp av HTML-taggarna: `DOCTYPE`, `html`, `head` och `body`. Du kan inkludera CSS-format för att anpassa utseendet på e-postmeddelandet.

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

>[!TIP]
>
>I de följande avsnitten lägger du till platshållare för innehåll för e-postfält, döljer onödiga element från förhandsgranskning och hanterar länkar till statiskt innehåll. När mallen är klar kan du [överföra den till GenStudio](use-templates.md#upload-a-template) och börja generera anpassade e-postmeddelanden baserat på din anpassade mall.

## Platshållare för innehåll

I mallens huvud eller brödtext kan du använda Handlebars syntax för att infoga platshållare för innehåll där du kräver att GenStudio fyller i e-postmeddelandet med faktiskt innehåll. GenStudio känner igen och tolkar platshållarna för innehållet automatiskt baserat på fältnamnet.

Du kan till exempel använda `{{ headline }}` för att ange var rubriken i e-postmeddelandet ska placeras:

```handlebars
<div>{{ headline }}</div>
```

Det högsta antalet fält som tillåts i en anpassad mall är tjugo.

**Identifierade fältnamn**:

| Fält | Roll | Kanalmall |
| -------------- | ---------------------- | -------------------- |
| `pre_header` | Förrubrik | e-post |
| `headline` | Headline | e-post<br>social annons |
| `body` | Body copy | e-post<br>social annons |
| `cta` | Uppmaning | e-post<br>social annons |
| `on_image_text` | På bildtext | social annonsering |
| `image` | Bild | e-post<br>social annons |
| `brand_logo` | Det valda varumärkets logotyp | social annonsering |

>[!IMPORTANT]
>
>GenStudio förser e-postmallen automatiskt med ett `subject`-fält under [!DNL Create]-processen, så du behöver inte ta med ämnesfältet i din e-postmall.

+++Exempel: Grundläggande mall

Här följer ett grundläggande exempel på en HTML-mall för e-post. Huvudet innehåller enkel, infogad CSS för formatering. Innehållet innehåller en `pre-header`-, `headline`- och `image`-platshållare som GenStudio kan använda för att mata in innehåll under e-postgenereringsprocessen.

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

### Bakgrundsbild

När du utformar en annons för Meta är det viktigt att använda en bakgrundsbild som kompletteras med text och en logotypövertäckning. För att garantera korrekt skalning av bilden måste du ange `aspect ratio` i Meta- och annonsmallarna. I det här sammanhanget kan du bara ange ett bildfält.

## Avsnitt eller grupper

_Avsnitt_ är ett sätt att informera GenStudio om att fält som tillhör ett avsnitt kräver hög grad av konsekvens. Genom att etablera relationen kan AI generera innehåll som matchar de kreativa elementen i avsnittet. En mall kan innehålla upp till tre avsnitt.

Använd ett prefix som du väljer i fältnamnet för att ange att det här fältet är en del av ett avsnitt eller en grupp. Du kan till exempel markera innehåll som visas i ett markerat område. Du kan välja att identifiera innehållet för det här området med ett vanligt prefix:

- `spotlight_headline`
- `spotlight_body`

Varje avsnitt kan bara ha en fälttyp. Exempelgruppen ovan med prefixet `spotlight` kan till exempel bara ha ett `spotlight_headline`-fält.

När du har flera avsnitt (max tre):

- `headline`
- `body`
- `spotlight_headline`
- `spotlight_body`
- `news_headline`
- `news_body`

GenStudio förstår att `spotlight_headline` är närmare relaterat till `spotlight_body` än till `news_body`.

+++Exempel: Mall med flera avsnitt

Följande är samma HTML-mall i exemplet ovan, men med ytterligare två avsnitt. Huvudet innehåller infogad CSS för formatering av en ruta. I brödtexten används två streck med platshållare för innehåll med ett prefix.

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

## Förhandsgranska mall

E-postmallar innehåller ibland särskilt innehåll som inte är nödvändigt för förhandsgranskning i GenStudio. Du kan styra synligheten för det här innehållet med hjälp av inbyggda hjälpredor, som är specialuttryck i mallspråket Handlebars som hjälper dig att utföra vissa åtgärder.

Värdet `_genStudio.browser` anges när en mall återges och värdet `genStudio.export` anges när en mall exporteras. Du kan välja att inkludera visst innehåll högst upp i e-postmeddelandena med en villkorlig omslutning, till exempel när mallen används för export:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Ett annat exempel kan vara att förhindra användning av spårningskoder när du förhandsgranskar en e-postmall i GenStudio. I det här exemplet visas hur du lägger till spårningsparametrar till länkar i den exporterade mallen, samtidigt som du håller förhandsgranskningslänkarna rena:

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
