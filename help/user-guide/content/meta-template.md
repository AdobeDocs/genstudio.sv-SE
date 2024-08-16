---
title: Förbered en mall för metaannonser för Adobe GenStudio för Performance Marketers
description: Lär dig hur du skapar en anpassad mall för Meta-annonser för Adobe GenStudio för Performance Marketers.
level: Intermediate
feature: Templates, Content
source-git-commit: c9d09801f0bd3732611b01d4a98cc7ebf38884d7
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---


# Förbered Meta ad-mall för Adobe GenStudio för Performance Marketers

När du skapar en mall för Meta-annonser används en strukturerad metod som är anpassad för sociala medier. När du har utformat och testat en mall för Meta-annonser kan du förbereda den för överföring och användning i GenStudio för Performance Marketers.

## Lägg till riktlinjer

Innan du förbereder en mall för Meta-annonser måste du se till att du har lagt till [riktlinjer](/help/user-guide/guidelines/overview.md) i din GenStudio för Performance Marketers och fyllt i dem med omfattande information om relevanta varumärken. [varumärkesriktlinjerna](/help/user-guide/guidelines/brands.md) påverkar det genererade innehållet direkt.

**Exempel**: Om du vill att innehållet i en Meta ad-mall inte ska vara längre än 500 tecken lägger du till det kravet i [kanalriktlinjerna](/help/user-guide/guidelines/brands.md#channel-guidelines) för fältet &quot;body&quot;.

Om inga riktlinjer läggs till i GenStudio för Performance Marketers används standardvärden.

## Utforma en mall

Vanligtvis skapar en designer den visuella designen för en mall i ett designprogram som Adobe XD.

Se [Anatomi en mall](/help/user-guide/content/use-templates.md#anatomy-of-a-template) och [Mallexempel](/help/user-guide/content/customize-template.md#template-examples).

### Annonsspecifikationer

GenStudio for Performance Marketers stöder dessa proportioner för Meta-annonser:

* Fyrkant (1:1): 1 080 x 1 080 pixlar
* Lodrät (4:5): 1 080 x 1 350 pixlar
* Artikel (9:16): 1 080 x 1 920 pixlar

Om annonsen inte är utformad i någon av dessa proportioner beskär GenStudio för Performance Marketers automatiskt bilden till lämplig storlek.

## Testa en mall för Meta-annonser

Testa mallen med Metas Creative Hub för att se hur annonsen ser ut på olika platser, till exempel i en feed eller som en berättelse.

Använd din e-postleverantör eller korrekturplattform för att testa din e-post och verifiera att den återges korrekt på olika e-postklienter och enheter.

## Definiera genererade innehållsområden

Definiera de områden i e-postmallen som ska fyllas i dynamiskt med innehåll från GenStudio för Performance Marketers.

Så här definierar du genererade innehållsområden:

* Identifiera textelementen i mallen som GenStudio for Performance Marketers ska generera automatiskt, till exempel rubriken eller CTA.
* Anpassa HTML-mallen genom att infoga platshållare i den med syntaxen Handblebars.

Se [Platshållare för innehåll](/help/user-guide/content/customize-template.md#content-placeholders).

## Förhandsgranska mallen

Kontrollera synligheten för specifika innehållsområden med hjälp av inbyggda stödfunktioner. Du kan till exempel inkludera spårningsparametrar till länkar i en exporterad mall samtidigt som du behåller rena förhandsgranskningslänkar.

Se [Förhandsvisning av mall](/help/user-guide/content/customize-template.md#template-preview).

## Överför och använd mall

När mallen har designats, kodats, testats och förhandsgranskats kan du överföra den till GenStudio för Performance Marketers och använda den för att generera helt nytt marknadsföringsmaterial.

Se [Arbeta med mallar](use-templates.md).
