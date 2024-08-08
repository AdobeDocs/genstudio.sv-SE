---
title: Förbered en e-postmall för GenStudio
description: Lär dig hur du skapar en anpassad e-postmall för GenStudio.
level: Intermediate
feature: Templates, Content
source-git-commit: 31f02218e02b1400ca9f32472acdecae03dbd304
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---


# Förbered e-postmall för GenStudio

Vanligtvis skapar en designer den visuella designen för en mall i ett designprogram som Adobe XD. När du har utformat, kodat och testat en e-postmall kan du förbereda den för överföring och användning i GenStudio.

Se [Anatomi för en mall](/help/user-guide/content/use-templates.md#anatomy-of-a-template).

## Lägg till riktlinjer

Innan du förbereder en mall för Meta-annonser måste du se till att du har lagt till [riktlinjer](/help/user-guide/guidelines/overview.md) i din GenStudio och fyllt i dem med omfattande information om relevanta varumärken. [varumärkesriktlinjerna](/help/user-guide/guidelines/brands.md) påverkar det genererade innehållet direkt.

**Exempel**: Om du vill att brödtexten i en e-postmall inte ska vara längre än 500 tecken lägger du till det kravet i [kanalriktlinjerna](/help/user-guide/guidelines/brands.md#channel-guidelines) för fältet&quot;brödtext&quot;.

Om inga riktlinjer läggs till i GenStudio används standardvärden.

## Koda en e-postmall

När en mall har designats kodas den med HTML och infogad CSS. Koden ska vara ren och responsiv för olika enheter.

Se [Mallexempel](/help/user-guide/content/customize-template.md#template-examples).

## Testa en e-postmall

Använd din e-postleverantör eller korrekturplattform för att testa din e-post och verifiera att den återges korrekt på olika e-postklienter och enheter.

Testa om e-postmallen uppfyller följande:

* Layouten justeras för olika skärmstorlekar med CSS-mediefrågor
* Knapparna går att klicka på och navigerar till den avsedda platsen
* E-postmallen kan läsas och användas på mobila enheter

## Definiera genererade innehållsområden

Definiera de områden i e-postmallen som ska fyllas i dynamiskt med innehåll från GenStudio.

Så här definierar du genererade innehållsområden:

* Identifiera textelementen i mallen som GenStudio ska generera automatiskt, till exempel rubriken eller CTA.
* Anpassa HTML-mallen genom att infoga platshållare i den med syntaxen Handblebars.

Se [Platshållare för innehåll](/help/user-guide/content/customize-template.md#content-placeholders).

## Förhandsgranska mallen

Kontrollera synligheten för specifika innehållsområden med hjälp av inbyggda stödfunktioner. Du kan till exempel inkludera spårningsparametrar till länkar i en exporterad mall samtidigt som du behåller rena förhandsgranskningslänkar.

Se [Förhandsvisning av mall](/help/user-guide/content/customize-template.md#template-preview).

## Överför och använd mall

När mallen har designats, kodats, testats och förhandsgranskats kan du överföra den till GenStudio för att använda den för att generera helt nytt marknadsföringsmaterial.

Se [Arbeta med mallar](use-templates.md).
