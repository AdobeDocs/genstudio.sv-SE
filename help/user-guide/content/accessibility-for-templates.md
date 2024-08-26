---
title: Skapa tillgängliga mallar
description: Bygg mallar som kan nå alla målgrupper för användning i Adobe GenStudio för Performance Marketers.
feature: Templates, Content
source-git-commit: 26d1b9c7b392e93e87ffcd9444f391c2980d1c3c
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---


# Skapa tillgängliga mallar

Adobe strävar efter att tillhandahålla en optimal upplevelse för alla målgrupper. Mer information finns i [Tillgänglighetsinitiativ på Adobe](https://www.adobe.com/trust/accessibility/initiatives.html).

I GenStudio for Performance Marketers kan du överföra resurser och mallar som gör att du kan skapa innehåll för en mängd olika upplevelser. Genom att följa tillgänglighetsstandarder kan ert innehåll nå er avsedda målgrupp.

Använd följande rekommendationer för att förbereda mallarna med hjälp av optimala tillgänglighetsstandarder.

## Alternativ text

Ange textalternativ för innehåll som inte är text, till exempel bilder.

```html
<img alt="Collage of ideas, books, man holding giant pencil, computer" src="card-create-assets.png">
```

![Idékollage, böcker, man som håller en enorm penna, dator](../../assets/card-create-assets.png){width="400"}

## Länksyfte (endast länk)

Skapa tydlig länktext som beskriver länkens syfte och plats.

Om du till exempel använder länktext som&quot;Klicka här&quot; eller&quot;Läs mer&quot; beskrivs inte syftet med länken tydligt:

```html
<a href="product-site.html">Click here</a>
```

Det bästa sättet är att använda text som tydligt beskriver var länken går. I ett bättre exempel kan namnet på länkkällan och syftet användas:

```html
<a href="product-site.html">Explore Product Site</a>
```

## Språk

Många produkter och tjänster använder språket på ett kreativt eller unikt sätt. Undvik jargon, långa meningar och komplexa fraser. Använd ett tydligt, koncist och lättläst språk som är kompatibelt med målgruppen.

- Använd tydliga beskrivningar, textbundna definitioner eller relaterade exempel när det är möjligt. Det kan vara svårt att översätta ett unikt språk.

- Skriv ut eller länka till en definition för de första förekomsterna av en akronym eller förkortning. Det kan vara svårt att översätta förkortningar.

- Använd visuella element för att komplettera text eller komplexa idéer när det är möjligt.
