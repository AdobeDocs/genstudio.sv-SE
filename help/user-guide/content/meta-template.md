---
title: Förbered en mall för Meta-annonser för GenStudio
description: Lär dig hur du skapar en anpassad mall för Meta-annonser för GenStudio.
level: Intermediate
feature: Templates, Content
source-git-commit: 31f02218e02b1400ca9f32472acdecae03dbd304
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---


# Förbered Meta ad-mall för GenStudio

När du skapar en mall för Meta-annonser används en strukturerad metod som är anpassad för sociala medier. När du har utformat och testat en mall för Meta-annonser kan du förbereda den för överföring och användning i GenStudio.

## Lägg till riktlinjer

Innan du förbereder en mall för Meta-annonser måste du se till att du har lagt till [riktlinjer](/help/user-guide/guidelines/overview.md) i din GenStudio och fyllt i dem med omfattande information om relevanta varumärken. [varumärkesriktlinjerna](/help/user-guide/guidelines/brands.md) påverkar det genererade innehållet direkt.

**Exempel**: Om du vill att innehållet i en Meta ad-mall inte ska vara längre än 500 tecken lägger du till det kravet i [kanalriktlinjerna](/help/user-guide/guidelines/brands.md#channel-guidelines) för fältet &quot;body&quot;.

Om inga riktlinjer läggs till i GenStudio används standardvärden.

## Utforma en mall

Vanligtvis skapar en designer den visuella designen för en mall i ett designprogram som Adobe XD.

Se [Anatomi en mall](/help/user-guide/content/use-templates.md#anatomy-of-a-template) och [Mallexempel](/help/user-guide/content/customize-template.md#template-examples).

### Annonsspecifikationer

GenStudio har stöd för dessa proportioner för Meta-annonser:

* Fyrkant (1:1): 1 080 x 1 080 pixlar
* Lodrät (4:5): 1 080 x 1 350 pixlar
* Artikel (9:16): 1 080 x 1 920 pixlar

Om annonsen inte är utformad i någon av dessa proportioner beskärs bilden automatiskt i lämplig storlek av GenStudio.

## Testa en mall för Meta-annonser

Testa mallen med Metas Creative Hub för att se hur annonsen ser ut på olika platser, till exempel i en feed eller som en berättelse.

Använd din e-postleverantör eller korrekturplattform för att testa din e-post och verifiera att den återges korrekt på olika e-postklienter och enheter.

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