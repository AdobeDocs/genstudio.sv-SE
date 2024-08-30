---
title: Arbeta med mallar
description: Upptäck hur ni kan använda mallar effektivt för att effektivisera er kreativa process i Adobe GenStudio för Performance Marketers.
feature: Templates, Content
source-git-commit: 192568a65bbd5c8c2e9cfc050462eb2c3465245d
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 0%

---


# Arbeta med mallar

Med GenStudio for Performance Marketers kan innehållsskapare snabbt producera enhetligt marknadsföringsmaterial på varumärke med hjälp av _mallar_. En mall minskar tiden och arbetet som krävs för att generera nytt innehåll avsevärt genom att tillhandahålla en startpunkt som inkluderar förkonfigurerade layouter och designelement.

## Mallelement

En mall är en uppsättning instruktioner som definieras med HTML och infogad CSS som kan användas för att skapa en e-post- eller metaannons.

Nedan följer en lista över element som används i mallar och en del detaljer om deras egenskaper.

- **Förrubrik**

   - Fungerar som en sekundär ämnesrad i ett e-postmeddelande och förbättrar ämnesraden
   - Mellan 40 och 50 tecken
   - Visas i inkorgen bredvid motivet innan e-postmeddelandet öppnas
   - Används i e-postmallar

- **Sidhuvud**

   - Övre delen av e-postmeddelandet som mottagaren ser när han/hon öppnar e-postmeddelandet
   - Anger tonen och ger sammanhang för det inkluderade innehållet
   - Används i e-postmallar

- **Rubrik**

   - Första innehållet som mottagaren ser
   - Bör vara lockande att fånga intresset
   - Används i metadatamallar

- **Brödtext**

   - Huvudsakligt innehållsområde där det primära meddelandet överförs
   - Möjlighet att inkludera text, bilder och andra medier
   - Används i mallar för e-post och metaannonser

- **CTA (Call-to-Action)**

   - Uppmuntrade mottagaren att utföra en viss åtgärd, som att klicka på en länk eller göra ett köp
   - Används i mallar för e-post och metaannonser

- **Bilder**

   - Förbättrar den visuella effekten
   - Dela upp text
   - Stöd meddelandet
   - Bör vara högkvalitativ och uppseendeväckande
   - Används i mallar för e-post och metaannonser

- **Sidfot**

   - Avsnittet längst ned som innehåller ytterligare innehåll, t.ex. kontaktinformation, länkar till sociala medier, ansvarsfriskrivningar och alternativ för att avbryta prenumerationen
   - Används i e-postmallar

- **Textövertäckning**

   - Text på en bild
   - Använd för att stödja och förbättra rubriken och brödtexten
   - Används i metadatamallar

>[!TIP]
>
>Se de [identifierade fältnamnen](customize-template.md#recognized-field-names) som GenStudio for Performance Marketers stöder för mallar av varje kanaltyp.

## Konfigurera kanalriktlinjer

Det är en god vana att konfigurera [kanalriktlinjer](../guidelines/brands.md#channel-guidelines) för varje varumärke innan du använder mallar i GenStudio för Performance Marketers. Kanalriktlinjerna påverkar direkt vilken typ av innehåll som skapas när mallen används. Du kan t.ex. ange teckenbegränsningar för brödtexten i ett e-postmeddelande.

![Specifikationer för brödtext](/help/assets/channel-email-body.png)

## Anpassa mall

Du [anpassar mallen](customize-template.md) så att den kan användas i GenStudio för Performance Marketers genom att infoga platshållare för innehåll, eller fält, som används av den generativa AI-filen för att infoga innehåll. GenStudio for Performance Marketers känner igen vissa fält, till exempel fältet `body`, och följer kanalriktlinjerna som konfigurerats för det valda varumärket.

>[!TIP]
>
>Följ [hjälpmedelsriktlinjerna för att skapa mallar](accessibility-for-templates.md) så att du kan nå fler av din publik och få en optimal upplevelse.

## Överföra en mall

Använd [Anpassa mallar](customize-template.md) som guide när du förbereder en mall för GenStudio för Performance Marketers. Mer information om hur du får en bättre upplevelse för alla målgrupper finns i [Riktlinjer för hjälpmedel för mallar](accessibility-for-templates.md).

**Så här lägger du till en mall**:

1. I _[!DNL Content]_väljer du avsnittet **[!UICONTROL Templates]**.

1. Klicka på **[!UICONTROL Add template]**.

1. I rutan _[!UICONTROL Add your approved template]_bläddrar du efter mallfilen HTML eller drar HTML-mallfilen till släppområdet. Klicka på&#x200B;**[!UICONTROL Next]**.

1. Granska de identifierade fälten i rutan _[!UICONTROL Review discovered fields]_. Kontrollera att du använder rätt mall och att all information är som förväntat. Klicka på&#x200B;**[!UICONTROL Next]**.

   Exempel på Förhandsgranska för en e-postmall:

   ![Förhandsgranskningsfält har identifierats](../../assets/template-detected-fields.png){width="650"}

   >[!TIP]
   >
   >Om mallen inte är korrekt klickar du på **[!UICONTROL Back]** och går tillbaka till föregående steg. Överför den korrigerade mallfilen.

1. I rutan _[!UICONTROL Provide template details and upload]_ger du mallen ett namn och väljer en **[!UICONTROL Channel]**-typ.

   Mallnamn och kanaltyp krävs. Ytterligare krav kan vara:

   - **Meta**: kräver proportioner
   <!-- - **Display ads**: requires Dimensions -->

1. Lägg till så många detaljer du kan för att förbättra identifiering av mallar i sökningar och filtrering.

1. Klicka på **[!UICONTROL Done]**.

## Skapa med en mall

Hitta och använd en befintlig mall i GenStudio för Performance Marketers för att skapa fler upplevelser.

**Så här skapar du en upplevelse med en mall**:

1. I _[!DNL Content]_väljer du avsnittet **[!UICONTROL Templates]**.

   ![Listan Innehållsmall](../../assets/content-templates.png){width="650" zoomable="yes"}

1. Välj en mall för en fullständig vy och en lista med detaljer.

1. Klicka på **[!UICONTROL Create Experience]** (penselverktyget) i det övre högra hörnet om du vill använda mallen.

1. Fortsätt med [självstudiekurser](/help/tutorials/tutorials.md) för att skapa en upplevelse.
