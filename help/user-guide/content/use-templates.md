---
title: Arbeta med mallar
description: Lär dig hur du använder mallar för att skapa engagerande upplevelser i Adobe GenStudio för Performance Marketers.
feature: Templates, Content
source-git-commit: 0cd877737f8ed4d38201c832d454795206505de2
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---


# Arbeta med mallar

Med GenStudio mallar kan kreatörer snabbt producera enhetligt marknadsföringsmaterial. När du använder mallar minskas tiden och arbetet avsevärt för att generera nytt innehåll genom att du får en startpunkt som inkluderar förkonfigurerade layouter och designelement.

Den här handboken innehåller detaljerad information om hur du:

* Förbered en [e-postmall](email-template.md) eller en mall för meta-annons
* [Anpassa mallar](customize-template.md) för GenStudio för Performance Marketers
* Följ vägledningen i [Skapa tillgängliga mallar](accessibility-for-templates.md)
* [Överför mallar](#upload-a-template) till GenStudio för Performance Marketers
* [Använd mallar för att skapa upplevelser](#use-a-template)

## Anatomi för en mall

Grundläggande malldesign innehåller följande element:

| Element | Funktion | Kanalmall |
| ------------ | ---------------------- | -------------------- |
| Förrubrik | Mellan 40 och 50 tecken <br>Fungerar som en sekundär ämnesrad som förbättrar huvudämnesraden <br>Visas i inkorgen bredvid motivet innan e-postmeddelandet öppnas | e-post |
| Sidhuvud | Det vanligaste avsnittet i e-postmeddelandet visas när e-postmeddelandet <br>Ställer in ton och anger kontext för inkluderat innehåll | e-post |
| Headline | Det första innehållet som mottagaren ser <br>Bör vara intressant att fånga intresset | Meta ad |
| Brödtext | Huvudsakligt innehållsområde där det primära meddelandet förmedlas <br>Kan innehålla text, bilder och andra media | e-post<br>Meta ad |
| CTA | Uppmaning till mottagare att vidta specifika åtgärder, som att klicka på en länk eller göra ett köp | e-post<br>Meta ad |
| Bilder | Förbättrat utseende <br>Bryter upp text <br>Stöder meddelande <br>Ska vara högkvalitativt och uppseendeväckande | e-post<br>Meta ad |
| Sidfot | Fotosektion som innehåller ytterligare innehåll som kontaktinformation, länkar till sociala medier, ansvarsfriskrivningar och alternativ för att avbryta prenumerationen | e-post |
| Textövertäckning | Text på en bild <br>Ska stöda och förbättra rubrik och brödtext | Meta ad |

>[!NOTE]
>
>Vi rekommenderar att du inkluderar specifika fält i varje kanals innehåll för att säkerställa att GenStudio for Performance Marketers kan generera text för platshållare för innehåll. Se [Identifierade fältnamn](customize-template.md#recognized-field-names) för att se vilka fält som rekommenderas för inkludering.

## Överföra en mall

GenStudio for Performance Marketers accepterar mallar i HTML-format.

**Så här lägger du till en mall**:

1. I _[!DNL Content]_väljer du avsnittet **[!UICONTROL Templates]**.

1. Klicka på **[!UICONTROL Add template]**.

1. I rutan _[!UICONTROL Add your approved template]_bläddrar du efter mallfilen HTML eller drar HTML-mallfilen till släppområdet. Klicka på&#x200B;**[!UICONTROL Next]**.

1. I rutan _[!UICONTROL Review structure detail]_kontrollerar du att du använder rätt mall och att all information är som förväntat. Klicka på&#x200B;**[!UICONTROL Next]**.

1. I rutan _[!UICONTROL Add your template details]_ger du mallen ett namn och väljer en **[!UICONTROL Channel]**-typ.

   Mallnamn och kanaltyp krävs.

   * **Meta**: kräver proportioner
   <!-- **Display ads**: requires Dimensions -->

1. Lägg till så många detaljer du kan för att förbättra identifiering av mallar i sökningar och filtrering.

1. Klicka på **[!UICONTROL Done]**.

## Använda en mall

Hitta och använd en befintlig mall för att skapa upplevelser.

**Så här skapar du en upplevelse med en mall**:

1. I _[!DNL Content]_väljer du avsnittet **[!UICONTROL Templates]**.

   ![Listan Innehållsmall](../../assets/content-templates.png){width="650" zoomable="yes"}

1. Välj en mall för en fullständig vy och en lista med detaljer.

>[!TIP]
>
>Se [[!DNL Create] en e-postupplevelse](/help/tutorials/create-email-experience.md) eller [[!DNL Create] en metadataannonsupplevelse](/help/tutorials/create-meta-ad.md) för fullständiga självstudiekurser med hjälp av mallar.
<!--  The create button in Content Template view does not work yet.
1. Click **[!UICONTROL Create Experience]** (paintbrush) from the upper right corner to use the template.
-->
