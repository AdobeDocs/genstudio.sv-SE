---
title: Resursinformation
description: Adobe GenStudio för Performance Marketers lagrar godkänt innehåll med omfattande metadata för sökbarhet och prestandaspårning.
feature: Attributes, Assets
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
source-git-commit: 95eb7c2eaeeceedf3abe5ab16e1e7c2de7bf8117
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Resursinformation

Adobe GenStudio för Performance Marketers lagrar godkänt innehåll med omfattande metadata för upptäckt och prestandaspårning.

Varje resurs (inklusive upplevelser och mallar) har associerad _information_ (metadata) som hjälper till att identifiera, spåra, använda och lära sig av innehållsprestanda.

**Så här visar du resursinformation**:

1. I _[!DNL Content]_väljer du en resurs, upplevelse eller mall. När du klickar på en resurs öppnas en fokuserad vy över resursen.

1. Granska avsnittet _[!UICONTROL Details]_till höger i resursvyn.

   >[!TIP]
   >
   >Om avsnittet _[!UICONTROL Details]_inte visas klickar du på ikonen **[!UICONTROL Information]**(i).

Resursinformationen innehåller metadata som används vid skapande eller överföring. Metadatatyperna för resurser omfattar [systemmetadata](#system-metadata) och [användardefinierade metadata](#user-defined-metadata).

>[!NOTE]
>
>Assets från AEM visar olika metadata. Mer information om hur du konfigurerar resursinformation för AEM Assets Content Hub finns i [Konfigurera resurssynlighet](connect-aem-repo.md#step-4-configure-asset-visibility).

## Systemmetadata

Vissa metadata för resurser samlas in automatiskt när en resurs överförs. Du kan inte redigera standardsystemmetadata.

Standardmetadata som lagras och hämtas för en resurs är filens namn, dimensioner, källa med mera.

### Genererade taggar

När du lagrar en godkänd resurs i [!DNL Content] använder GenStudio for Performance Marketers funktioner för Adobe AI och maskininlärning för att studera resursen och tillämpa taggar baserat på resursfunktionerna. En bild på en katt kan till exempel resultera i smarta taggar som `pet photography` eller `cat`, och färgtaggar som identifierar dominerande färger i bilden. Du kan inte redigera taggar.

### Metadata för genererat innehåll

Den information som används för att generera en ny resurs eller upplevelse blir metadata, till exempel den fråga som användes. Du kan inte redigera frågan när innehållet har godkänts, men du kan använda den som startpunkt för att generera något nytt.

## Användardefinierade metadata

Användardefinierade metadata lägger till marknadsföringssammanhang till resursens innehåll, vilket gör att marknadsförarna kan förstå hur de ska använda och interagera med resursen.

När du [överför en resurs](/help/user-guide/content/manage-assets.md#add-assets) kan du definiera en uppsättning med valfri resursinformation som finns i GenStudio för Performance Marketers som metadata. Om du tar med mer information kan det bli enklare att identifiera resurser i sökningar och filtrering.

### Metadatainformation

Följande tabell visar vilka metadata (resursinformation) du kan definiera när du skapar en resurs.

| Fält | Beskrivning |
| ------------- | ----------- |
| Kampanjer (projektnamn) | Standardmetadata som hämtas och lagras med resursen |
| [!DNL Brands] | [[!DNL Brands]](/help/user-guide/guidelines/brands.md) har lagts till i GenStudio för Performance Marketers och publicerats för användning |
| [!DNL Products] | [[!DNL Products]](/help/user-guide/guidelines/products.md) har lagts till i GenStudio för Performance Marketers för användning |
| [!DNL Personas] | [[!DNL Personas]](/help/user-guide/guidelines/personas.md) har lagts till i GenStudio för Performance Marketers för användning |
| Kanaler | Innehållstyper i GenStudio för Performance Marketers som resursen används för, som e-post- och metaannonser |
| Tidsram | Tidsram som resursen användes för, t.ex. kvartal, årstid, år. Exempel: `Winter 2023` |
| Län | Områden som tillgången används för. Exempel: `North America`, `APAC`, `Italy` |
| Språk | Språk som resursen används för. Exempel: `Spanish` |
| Nyckelord | Nyckelord som används för ytterligare identifiering av tillgångars egenskaper och syfte |

<!-- ## History

Expand the _[!UICONTROL History]_ section to view a timeline of approvals and activity.

list other activity, show screenshot?
-->
