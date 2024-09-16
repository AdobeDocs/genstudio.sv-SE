---
title: Adobe GenStudio för Performance Marketers Beta versionsinformation
description: Läs om de senaste funktionerna och förbättringarna av Adobe GenStudion för Performance Marketers.
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: d1904bfe6e5775f71290c2fc7aa185ac2a4a4668
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Adobe GenStudio för Performance Marketers Beta versionsinformation

Dessa kommentarer belyser viktig Adobe GenStudio för korrigeringar och förbättringar av Performance Marketers för den vecka som slutar den 13 september.

## Förbättringar

* Innehållsväljaren [!DNL Create] har omarbetats för att förbättra resursinläsningen. <!-- GS-2586 -->

## Kända fel

Följande kända fel är schemalagda för lösning i GenStudio for Performance Marketers GA-versionen.

* Problem med återkommande fördröjning påverkar vissa [!DNL Create] arbetsyteåtgärder. <!-- GS-5203 -->

* E-postgenereringen resulterar i ett ofullständigt e-postmeddelande. **Tillfällig lösning**: Uppdatera sidan och återskapa den. <!-- GS-5209 -->

* Mallar kan överföras men inte visas. **Tillfällig lösning**: Skapa eller överför en resurs och ange ett namn på en resursgrupp i fältet **[!UICONTROL Campaigns]**. Om du tilldelar resursen till ett [!DNL Campaign] läggs metadatavärdet för gruppnamnet till. Ladda sedan upp mallen igen. <!-- GS-4815 -->

* Kampanjminiatyrer saknas i [!DNL Insights]. <!-- GS-4648 -->

* Användare måste logga in två gånger till ett Meta Ads-kanalkonto när de också är inloggade på Facebook. **Tillfällig lösning**: Logga ut från Facebook innan du loggar in på ett Meta Ads-kanalkonto. <!-- GS-4806 -->

### Ytterligare förbättringar och åtgärdade problem

* Arbetsytan [!DNL Create] återger nu bilder i Meta Ads korrekt. <!-- GS-4864 -->

* Även om det kan finnas skillnader mellan förhandsvisningar för Meta Ads Canvas och exporterade vyer fungerar exporterade upplevelser som förväntat. <!-- GS-4492 4401 -->

* Överförda bilder innehåller nu de förväntade smarta taggarna. <!-- GS-4856 -->

* CSV-filen för export av meta Ads innehåller nu bilder som förväntat. Tidigare innehöll ZIP-filen CSV-exportfilen och NULL-filer i stället för bilder.  <!-- GS-5107 -->

* Användare kan nu ange text i malldetaljsvyn **[!UICONTROL Uploaded by]** som förväntat. Tidigare hindrade ikonen för inläsning användarna från att skriva text. <!-- GS-4887 -->

* Användare omdirigeras inte längre till detaljvyn för ett varumärke efter att varumärket har tagits bort. <!-- GS-2663 -->

* Redigerare får inte längre följande fel när varianter skickas för granskning och godkännande: `You have no access to view comments on this Object`. <!-- GS-5140 -->

* Uppdaterade e-postmallen som används i arbetsflödet för granskning och godkännande. <!-- GS-5239 -->

* GenStudio visar nu ett felmeddelande när ett nätverksfel inträffar när mallväljaren läses in. <!-- GS-4682 -->

* Löste problem med att navigera från en resurs, en upplevelse eller ett mallkort till det valda objektet. <!-- GS-4390 -->

* Popup-fönstret _Lägg till Assets_ är nu lokaliserat när det öppnas från Skapa arbetsyta.  <!-- GS-4867 -->

* Varumärkesvalidering aktiveras nu för återskapade varianter. Tidigare aktiverades inte valideringen om en redigerare genererade om varianter av ett befintligt utkast. <!-- GS-3971 -->

## Tidigare versioner av Beta

Tidigare versioner av Beta innehöll följande programfixar och markeringar.

### Högdagrar

* GenStudio har nu stöd för alternativet att förhandsgranska medieresurser i [!DNL Insights]-tabell- och gallerivyer. Videominiatyrbilder innehåller en **uppspelningsknapp** med ett ljudavstängningsalternativ. <!-- GS-4398 -->

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

* **MetaAds Ändra storlek**: Redigerare kan ändra storlek på MetaAd-proportioner. (fast 8/16)

* **Begränsade [!DNL Insights] inloggningskonton**: Inloggningen [!DNL Insights] har nu bara stöd för ett konto per kund. (fast 8/16)

### Ytterligare förbättringar och åtgärdade problem

* Popup-fönstret _Lägg till Assets_ är nu lokaliserat som förväntat. <!-- GS-3834 -->

* Problem med skalning av mallen Meta Adds Experience har lösts. <!-- GS-4174 -->

* Textfält i CSV-exportfilen för e-post med flera delar ordnas nu som förväntat. <!-- GS-4013 -->

* Sökfältet [!DNL Content] försvinner inte längre när en användare trycker på tangenten **Backsteg** upprepade gånger för att radera texten i sökfältet.  <!-- GS-4543 -->

* GenStudio for Performance Marketers läser nu in användare som förväntat när en medarbetare lägger till en `@`-händelse till en kommentar. Tidigare lästes inte användarna in och ett fel visades: `Unable to load users. Refresh the page`. <!-- GS-4113 -->

* GenStudio visar inte längre meddelandet **Något gick fel** när en redigerare klickar på **Välj innehåll** när e-postmeddelandet skapades i promptområdet. <!-- GS-4879 -->

* Sidfeedplaceringsnamnet _Experience Detail_ anger nu Facebook- eller Instagram-feed. (fast 8/16)

* Det är nu konsekvent att beskära större bilder och videoklipp när användaren navigerar från vyn _Resursöversikt_ till vyn _Resursdetaljer_. (fast 8/16)

* Resultatantal för attributskärmssökning visas inte längre `0 of` innan en användare loggar in. (fast 8/16) <!-- GS-3665 -->

* När du klickar på fältet **[!UICONTROL [!DNL Insights]]** > **[!UICONTROL Asset]** rensas inte längre inställningarna för sökning och filter. (fast 8/16) <!-- GS-3476 -->

* Ett fel visas i GenStudio när en användare försöker ange inloggningsuppgifter i vyn [!DNL Insights]. (fast 29/8) <!-- GS-4689 -->

* Det går inte att överföra varumärkesriktlinjer på grund av problem med lagringsplattformen i AVS. (fast 8/22) <!-- GS-4369 -->

* I listrutan Fråga [!DNL Brands] visas en rotationsruta i slutet av listan [!DNL Brands] när e-postmeddelanden skapas. (fast 8/22) <!-- GS-4077 -->
