---
title: Adobe GenStudio för Performance Marketers Beta versionsinformation
description: Läs om de senaste funktionerna och förbättringarna av Adobe GenStudion för Performance Marketers.
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: 62793ab56b635f17e037b63beb56c09ff2d45621
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 0%

---

# Adobe GenStudio för Performance Marketers Beta versionsinformation

Dessa kommentarer belyser viktig Adobe GenStudio för korrigeringar och förbättringar av Performance Marketers för den vecka som slutar 6 september.

## Nya funktioner

* GenStudio har nu stöd för alternativet att förhandsgranska medieresurser i [!DNL Insights]-tabell- och gallerivyer. Videominiatyrbilder innehåller en **uppspelningsknapp** med ett ljudavstängningsalternativ. <!-- GS-4398 -->

## Kända fel

Följande kända fel är schemalagda för lösning i GenStudio for Performance Marketers GA-versionen.

* Redigerare stöter ibland på ett felmeddelande om att något gick fel på [!DNL Create Canvas] under bildgenereringen. **Tillfällig lösning**: Om felet upprepas kan användaren logga ut, logga in på GenStudio igen och återskapa bilden.  <!-- GS-4813 -->

* [!DNL Create Canvas] återger bilder i Meta-annonser felaktigt. <!-- GS-4864 -->

* Assets utan kampanjer kan överföras till [!DNL Content], men är kanske inte synligt för användarna. <!-- GS-4815 -->

* Det finns skillnader mellan förhandsvisningar av MetaAds Canvas och exporterade vyer. <!-- GS-4492 4401 -->

* Kampanjminiatyrer saknas i [!DNL Insights]. <!-- GS-4648 -->

* Användarna kan för närvarande välja små resurser som kräver storleksändring, men det går inte att förstora dessa resurser. <!-- GS-3131 -->

* Användare måste logga in två gånger till ett Meta Ads-kanalkonto när de också är inloggade på Facebook. **Tillfällig lösning**: Logga ut från Facebook innan du loggar in på ett Meta Ads-kanalkonto.

* Överförda bilder innehåller inte alltid de förväntade smarta taggarna. <!-- GS-4856 -->

### Ytterligare förbättringar och åtgärdade problem

* Popup-fönstret _Lägg till Assets_ är nu lokaliserat som förväntat. <!-- GS-3834 -->

* Problem med skalning av mallen Meta Adds Experience har lösts. <!-- GS-4174 -->

* Modeller för innehållsfragment som skapats för mallar kan nu återges korrekt i AEM. <!-- GS-4716 -->

* Textfält i CSV-exportfilen för e-post med flera delar ordnas nu som förväntat. <!-- GS-4013 -->

* Sökfältet [!DNL Content] försvinner inte längre när en användare trycker på tangenten **Backsteg** upprepade gånger för att radera texten i sökfältet.  <!-- GS-4543 -->

* GenStudio läser nu in användare som förväntat när en medarbetare lägger till ett @-omnämnande i en kommentar. Tidigare lästes inte användare in i GenStudio och följande fel visades: `Unable to load users. Refresh the page`. <!-- GS-4113 -->

* GenStudio visar inte längre meddelandet **Något gick fel** när en redigerare klickar på **Välj innehåll** när e-postmeddelandet skapades i promptområdet. <!-- GS-4879 -->

## Tidigare versioner av Beta

Tidigare versioner av Beta innehöll följande programfixar och markeringar.

### Högdagrar

* Instagram och Facebook kanalriktlinjer har kombinerats i Metas varumärkesriktlinjer.

* [!DNL Create] arbetsytans navigeringselement har strömlinjeformats. På [!DNL Create]-landningssidan visas den vänstra navigeringspanelen, men användarna använder nu en **[!UICONTROL Back]**-knapp för att navigera till det här utrymmet från andra [!DNL Create] arbetsytor.

* Navigeringselementen har förbättrats för att ge stöd åt användarfokus när man utför uppgifter i hela produkten, inklusive följande produktområden:

   * Resurs, upplevelse, mallinformation i [!DNL Content]
   * Upplevelse, resurs, attributdetaljer i [!DNL Insights]
   * Märkesinformation i [!DNL Brands]
   * Produkt- och personinformation i Produkter och Personas

* Användare behöver inte längre klicka på knappen **[!UICONTROL Refresh]** för att se uppdateringar av upplevelser i [!DNL Content].

* Sidan _Upplevelseinformation_ återger nu externa miniatyrbilder av resurser som HTML.

* Fördröjningen för användargränssnitt efter att Assets och Experience har lagts till eller tagits bort har förbättrats.

* Mallförhandsvisningar innehåller nu mer beskrivande standardtext. Se [Anpassa en mall](https://experienceleague.adobe.com/en/docs/genstudio/user-guide/content/templates/customize-template#template-preview).

* **Procentandel av valideringspoäng**: I varumärkesvalideringen visas nu varumärkesvalideringspoängen i procent i stället för ett godkänt/underkänt värde. (fast 8/16)

* **Uppdaterat gränssnitt för varumärkesextrahering**: Extraheringen visar nu att extraheringsprocessen har slutförts i procent. (fast 8/16)

* **Inkrementell varumärkesbelastning under extrahering**: Riktlinjer för varumärket läses nu in stegvis i användargränssnittet. (fast 8/16)

* **Skapa e-post i flera avsnitt**: Användare kan nu skapa e-postmeddelanden som består av separata rubriker, bilder, brödtext och CTA-element. (fast 8/16)

* **Storleksändring för metaannonser**: Redigerare kan ändra storlek på metadata och proportioner. (fast 8/16)

* **Begränsade [!DNL Insights] inloggningskonton**: Inloggningen [!DNL Insights] har nu bara stöd för ett konto per kund. (fast 8/16)

### Ytterligare förbättringar och åtgärdade problem

* Sidfeedplaceringsnamnet _Experience Detail_ anger nu Facebook- eller Instagram-feed. (fast 8/16)

* Det är nu konsekvent att beskära större bilder och videoklipp när användaren navigerar från vyn _Resursöversikt_ till vyn _Resursdetaljer_. (fast 8/16)

* Resultatantal för attributskärmssökning visas inte längre `0 of` innan en användare loggar in. (fast 8/16) <!-- GS-3665 -->

* När du klickar på fältet **[!UICONTROL [!DNL Insights]]** > **[!UICONTROL Asset]** rensas inte längre inställningarna för sökning och filter. (fast 8/16) <!-- GS-3476 -->

### Kända problem som lösts i tidigare versioner av Beta

* Ett fel visas i GenStudio när en användare försöker ange inloggningsuppgifter i vyn [!DNL Insights]. (fast 29/8) <!-- GS-4689 -->

* Det går inte att överföra varumärkesriktlinjer på grund av problem med lagringsplattformen i AVS. (fast 8/22) <!-- GS-4369 -->

* I listrutan Fråga [!DNL Brands] visas en rotationsruta i slutet av listan [!DNL Brands] när e-postmeddelanden skapas. (fast 8/22) <!-- GS-4077 -->
