---
title: Attribut - översikt
description: Lär dig hur du utvärderar prestandan för specifika attribut i Adobe GenStudio for Performance Marketing.
feature: Insights, Assets
source-git-commit: 6ba029f46a37c159ec48676a158a6a9b8fb5465d
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---

# Attribut - översikt

Vyn [!DNL Insights] _[!UICONTROL Attributes]_visar en lista med attribut som används i annonskampanjer för det valda kanalkontot.

Tabellen _[!UICONTROL Attributes]_är ordnad med namnet [!UICONTROL Attribute]. Du kan växla mellan listtyperna med knappen **[!UICONTROL Images]**och knappen **[!UICONTROL Video]**. Klicka på inställningsikonen ovanför den högra sidan av tabellen för att växla mellan de kolumner som kan visas.

Filterikonen (tratten) ovanför tabellens vänstra sida öppnar menyn **[!UICONTROL Filter]** där du kan välja mellan [!UICONTROL Account] och [!UICONTROL Attribute category] för att filtrera attributen i tabellen. I följande exempel visas en lista med attribut i kategorin `Lighting Condition`.

![Attributfilter och tabell](/help/assets/insights-attributes-filter.png){zoomable="yes"}

## Attributinformation

Attribut hjälper till att identifiera resurser genom deras inneboende detaljer, som färg, komposition, visuella element och andra egenskaper.

I vyn för attributdetaljer kan du se vilka upplevelser som använder det valda attributet. Detaljerna innehåller totala attributprestanda och en uppdelning av prestandamätningarna för varje upplevelse.

![Attribut för prestandamått](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketing identifierar vissa funktioner och använder rätt attribut för en resurs eller upplevelse som en tagg. Se [Kategorier](#categories) om du vill se exempel på de här taggarna. Om du vill visa alla attribut som är kopplade till en upplevelse klickar du på inställningsikonen (cog) ovanför den högra sidan av tabellen för att markera kolumnen **[!UICONTROL Attributes]**.

## Kategorier

GenStudio for Performance Marketing känner igen vissa funktioner i bilder, videoklipp och text och lägger till en funktionstagg i resursen. En _kategori_ är en uppsättning funktioner som delar en specifik egenskap. Ett exempelvärde för _bildorientering_ är `landscape`.

Attribut som identifieras och tillämpas automatiskt kan inte redigeras.

<!--
Select any of the following to open a detailed list of feature categories:

+++**Image features**

| Category               | Values                              |
| ---------------------- | ----------------------------------- |
| Background Colors      | 14 colors |
| Camera Position        | - `low angle`, `high angle`, `dutch angle`<br>- `overhead view`, `eye level`,`bird's eye view` |
| Camera Proximity       | `close up`, `mid shot`, `long shot` |
| Camera Setting         | - `fast shutter speed`, `long exposure`, `double exposure`<br>- `normal mode`, `flash`, `macro`, `wide-angle`<br>- `black and white`, `surreal`<br>- `bokeh blur`, `motion blur`, `tilt-shift blur` |
| Foreground Colors      | 14 colors |
| Image Type             | `photograph`, `sketch`, `painting`, `digital cartoon`, `infographics`, `graphic design`, `collage`, `screenshot` |
| Lighting Condition     | golden hour, blue hour, midday, overcast, night, high-key, low-key, daylight, incandescent, fluorescent, colorful, studio |
| Objects                | The items, entities, and elements that are visible, such as `lighthouse`, `orchid`, or `tunnel`. |
| Orientation            | Examples: `landscape`, `portrait`, `square` |
| Overall Tone           | `warm`, `cool`, `neutral` |
| People Categories      | Examples: `person`, `social group`, `people`, `kid` |
| Photography Styles     | `aerial photography`, `aerial photography`, `architectural photography`, `astrophotography`, `black and white photography`, `business photography`, `cityscape photography`, `commercial photography`, `composite photography`, `creative photography`, `editorial photography`, `event photography`, `family photography`, `fashion photography`, `fine art photography`, `food photography`, `holiday photography`, `indoor photography`, `landscape photography`, `lifestyle photography`, `macro photography`, `minimalist photography`, `night photography`, `outdoor photography`, `pet photography`, `portrait photography`, `product photography`, `real estate photography`, `seascape photography`, `sports photography`, `still-life photography`, `street photography`, `travel photography`, `underwater photography`, `wildlife photography` |
| Scenes                 | Examples: `city`, `island`, `living room` |
| Tags                   | Examples: `gaming`, `law`, `yoga` |
| Visual Attention Spread| The level of viewer attention spread across an image: `high`, `low` |
| Visual Content Density | The amount of information or detail in an image: `high`, `low` |

+++

+++**Video features**

| Category               | Values                              |
| ---------------------- | ----------------------------------- |
| Audio Genre  | |
| Audio Genre Category  | |
| Audio Mood  | |
| Audio Types| |
| Objects  | |
| Orientation  | |
| People Categories  | |
| Scenes  | |
| Styles  | |
| Tags   | |
| Video Category  | |
| Video Type  | |

+++

+++**Text features**

| Category               | Values                              |
| ---------------------- | ----------------------------------- |
| Emojis Count  | |
| HashTags Count  | |
| Keywords  | |
| Marketing Emotions  | |
| Narratives  |  |
| Persuasion Strategies  |  |
| Readability  | |
| Sentences Count  | |
| Stop Words Ratio  | |
| Text Quotes Count  | |
| Tones  | |
| Words Count  | |
| Words Count Per Sentence  | |

+++

-->

## Attributmått

Insikter kan hjälpa er att utvärdera vilka attribut som inspirerar till mer kundengagemang.

### Mätvärdesdetalj

Följande tabell innehåller definitioner och insikter för viktiga mätvärden för digital marknadsföring i vyn [!UICONTROL Attributes]. Varje mätvärde innehåller en kort definition av vad den avser en mediefil, hur mätvärdet beräknas och en eller flera insikter som hjälper till att förstå dess betydelse och påverkan på en annonskampanj.

| Mått | Definition | Insikt |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Attribute]** | Attributnamnet. | Sortera tabellen genom att klicka på kolumnrubriken för något av nyckelmåtten. |
| **[!UICONTROL Category]** | Den [kategori](#categories) som representerar den inbyggda kvaliteten för ett attribut. |  |
| **[!UICONTROL # of images]** | Antal bilder med detta attribut. |  |
| **[!UICONTROL # of videos]** | Antal videor med det här attributet. |  |
| **[!UICONTROL Impressions]** | En mängd varje gång en bild eller videor med det här attributet läses in i kanalen, oavsett interaktion eller visning. | Ett högt visningsvärde kan visa på bred synlighet, men för verkliga prestandainsikter bör du överväga andra engagemangsmått. |
| **[!UICONTROL Clicks]** | Antal gånger som användare interagerar med en bild eller video med det här attributet. | Ett högt klickningsantal visar starkt intresse och engagemang för innehållet, vilket kan vara effektivt och nå rätt målgrupp. |
| **[!UICONTROL CTR]**<br>_Genomklickningsfrekvens _ | Procentandel (%) av visningar som resulterade i klickningar på bilder eller videor med det här attributet.<br>**Beräkning**: `clicks` delat med `impressions` | En hög klickfrekvens visar att innehållet är mycket relevant och motiverat för målgruppen i budskapen och designen och att det effektivt riktar sig till målgruppens intressen. |
| **[!UICONTROL CPM]**<br>_Kostnad per tusen _ | Kostnad ($) för varje tusen annonsvisningar av en bild eller video med det här attributet.<br>**Beräkning**: totalt belopp `spent` dividerat med räckvidd, multiplicerat med 1000 | Ett lågt värde kan indikera kostnadseffektiv synlighet, särskilt om det kombineras med en hög klickfrekvens. |
| **[!UICONTROL CPC]**<br>_Kostnad per klick _ | Genomsnittskostnad ($) som associeras med varje klick på bilder eller videor med det här attributet.<br>**Beräkning**: totalt belopp `spent` delat med `clicks` | Lägre genomsnittliga kostnader kan tyda på kostnadseffektiva annonskostnader, särskilt om man jämför med en ökning av antalet konverteringar. |
| **[!UICONTROL Spend]** | Det belopp ($) som spenderas från budgeten i förhållande till attribut under en viss tidsperiod. | Ett högt utgiftsbelopp under en kort period kan tyda på snabb användning, vilket kan leda till att resurser tar slut i förtid. Spåra utgiftsbeloppet mot nyckeltal för att övervaka den totala avkastningen på investeringen. |
