---
title: Resursinformation
description: Adobe GenStudio för Performance Marketers lagrar godkänt innehåll med omfattande metadata för sökbarhet och prestandaspårning.
feature: Attributes, Assets
source-git-commit: c9d09801f0bd3732611b01d4a98cc7ebf38884d7
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---


# Resursinformation

Adobe GenStudio för Performance Marketers lagrar godkänt innehåll med omfattande metadata för upptäckt och prestandaspårning.

Varje resurs (inklusive upplevelser och mallar) har associerad _information_ (metadata) som hjälper till att identifiera, spåra, använda och lära sig av innehållsprestanda.

Metadatatyperna för resurser omfattar [systemmetadata](#system-metadata) och [användardefinierade metadata](#user-defined-metadata).

## Systemmetadata

Vissa metadata för resurser samlas in automatiskt när en resurs överförs. Du kan inte redigera standardsystemmetadata.

Standardmetadata som lagras och hämtas för en resurs är filens namn, dimensioner, källa med mera.

### Genererade taggar

När resurser har godkänts och lagrats i [!DNL Content] använder GenStudio för Performance Marketers funktioner för Adobe AI och maskininlärning för att generera taggar baserat på resursfunktioner, som färg och ton, eller nyckelord som identifierar resursfunktioner. Du kan inte redigera taggar.

### Metadata för genererat innehåll

Den information som används för att generera en ny resurs eller upplevelse blir metadata, till exempel den fråga som användes. Du kan inte redigera frågan när innehållet har godkänts, men du kan använda den som startpunkt för att generera något nytt.

## Användardefinierade metadata

Användardefinierade metadata lägger till marknadsföringssammanhang till resursens innehåll, vilket gör att marknadsförarna bättre kan förstå hur de ska använda och interagera med resursen.

När du [överför en resurs](/help/user-guide/content/manage-assets.md#add-assets) kan du definiera en uppsättning med valfri resursinformation som finns i GenStudio för Performance Marketers som metadata.

### Metadatainformation

Följande tabell innehåller metadata (resursinformation) som du kan definiera när du skapar en resurs.

| Fält | Beskrivning | Redigerbar | Obligatoriskt |
| ------------- | ----------- | -------- | -------- |
| Kampanjnamn (projektnamn) | Standardmetadata som hämtas och lagras med resursen | Y | N |
| Märkesnamn | [[!DNL Brands]](/help/user-guide/guidelines/brands.md) har lagts till i GenStudio för Performance Marketers och publicerats för användning | Y | N |
| [!DNL Products] | [[!DNL Products]](/help/user-guide/guidelines/products.md) har lagts till i GenStudio för Performance Marketers för användning | Y | N |
| [!DNL Personas] | [[!DNL Personas]](/help/user-guide/guidelines/personas.md) har lagts till i GenStudio för Performance Marketers för användning | Y | N |
| Kanaler | Innehållstyper i GenStudio för Performance Marketers som resursen används för, som e-post- och metaannonser | Y | N |
| Tidsram | Tidsram som resursen användes för, t.ex. kvartal, årstid, år. Exempel: `Winter 2023` | Y | N |
| Län | Områden som tillgången används för. Exempel: `North America`, `APAC`, `Italy` | Y | N |
| Språk | Språk som resursen används för. Exempel: `Spanish` | Y | N |
| Nyckelord | Nyckelord som används för att identifiera tillgångssyfte | Y | N |

## Visa tillgångsinformation

**Om du vill visa resursinformation**:

1. Välj en resurs i _[!DNL Content]_.

1. Granska avsnittet _[!UICONTROL Details]_till höger i resursvyn.

   Om avsnittet _[!UICONTROL Details]_inte visas klickar du på ikonen **[!UICONTROL Information]**(i).

>[!TIP]
>
>Du kan även visa resursinformation från [!DNL Insights]. [!DNL Insights] tillhandahåller användningsstatistik och prestandakontext för olika upplevelser. I _[!DNL Insights]_väljer du avsnittet **[!UICONTROL Assets]**.

<!-- ## History

Expand the _[!UICONTROL History]_ section to view a timeline of approvals and activity.

list other activity, show screenshot?
-->
