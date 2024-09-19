---
title: Adobe GenStudio för Performance Marketers Beta versionsinformation
description: Läs om de senaste funktionerna och förbättringarna av Adobe GenStudion för Performance Marketers.
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: 7085fa5a12a6ed36c9310f8f691969d9c1366d36
workflow-type: tm+mt
source-wordcount: '1341'
ht-degree: 0%

---

# Adobe GenStudio för Performance Marketers Beta versionsinformation

Dessa kommentarer belyser viktig Adobe GenStudio för korrigeringar och förbättringar av Performance Marketers för den vecka som slutar den 19 september.

## Nya funktioner och förbättringar

* **Integrering med Adobe Experience Manager Assets**. Skrivskyddad åtkomst till Adobe Experience Manager Assets finns nu. <!-- GS-2432 -->

* **Förbättringar av arbetsflödet Uppdatera mall**.  Användare som uppdaterar mallar väljer nu den kanal som de vill använda mallen för. <!-- GS-4029 -->

* **Förbättrad prestanda vid sidinläsning**. Oanvända beroenden har tagits bort från sidinläsningsprocessen. <!-- GS-3630 -->

* **Stöd för e-post i flera avsnitt**. Redigerare kan nu generera e-postmeddelanden som innehåller flera avsnitt och bilder. De kan också återskapa specifika fragment av ett genererat e-postmeddelande (till exempel en rubrik). <!-- GS-2436 -->

* **Växla mellan skrivbordsvyn och mobilvyn när du skapar**. Användarna kan nu växla mellan datorvyn och mobilvyn för att förhandsgranska varianter av e-postupplevelsen. <!-- GS-4314 -->

* Innehåll genererar nu bilder med beskärningsdimensioner som är relativa till de ursprungliga objektdimensionerna. <!-- GS-3150 -->

* Användarna kan nu välja genererade bildvarianter och använda funktionen Justera beskärning för att beskära dem under arbetsflödet. <!-- GS-5538 2342 -->

* I detaljvyn för en godkänd upplevelse visas nu en miniatyrbild och statusen för alla resurser som refereras till i den upplevelsen. <!-- GS-3783 -->

## Kända fel

Följande kända fel är schemalagda för lösning i GenStudio for Performance Marketers GA-versionen.

* Problem med återkommande fördröjning påverkar vissa [!DNL Create] arbetsyteåtgärder. <!-- GS-5203 -->

* E-postgenereringen resulterar i ett ofullständigt e-postmeddelande. **Tillfällig lösning**: Uppdatera sidan och återskapa den. <!-- GS-5209 -->

* Mallar kan överföras men inte visas. **Tillfällig lösning**: Överför en resurs med fältet **[!UICONTROL Campaigns]** ifyllt. Ladda sedan upp mallen igen. <!-- GS-4815 -->

* Användare måste logga in två gånger till ett Meta-annonskonto i en kanal när de också är inloggade på Facebook. **Tillfällig lösning**: Logga ut från Facebook innan du loggar in på ett kanalkonto för Meta-annonser. <!-- GS-4806 -->

### Ytterligare förbättringar och åtgärdade problem

* Dra och släpp fungerar nu som väntat i promptområdet. <!-- GS-3977 -->

* Problem med att använda tabbtangenten för att navigera bland element i det vänstra navigeringsfältet har korrigerats. Tidigare krävdes flera klick för att navigera från ett element till nästa aktiva element.  <!-- GS-2639 -->

* GenStudio sparar nu upplevelsenamn när användare redigerar namnet medan upplevelsen läses in. <!-- GS-5242 -->

* Användarna kan nu redigera en upplevelsetitel. Tidigare var rubriktexten densamma som den ursprungliga texten när en användare försökte redigera den. <!-- GS-5246 -->
* De valda bilderna återges nu på arbetsytan som förväntat när flera e-postmeddelanden skapas. <!-- GS-5263 -->

* Alla strängar på detaljsidan för [!DNL Content] upplevelser är nu lokaliserade. <!-- GS-5016 -->

* Användare kan nu ta bort en produkt vars detaljvy är öppen i [!DNL Products]. <!-- GS-5057 -->

* Det meddelande som GenStudio visar när en sökning inte ger några matchande resultat har förbättrats. <!-- GS-4544 -->

* `aria-label` attributvärden för sökfiltervärden översätts nu som förväntat. <!-- GS-5388 -->

* Användare kan nu ta bort duplicerade resurser i frågerutan [!DNL Create] i arbetsytan.  <!-- GS-5233 -->

* Filtret Konto fungerar nu som väntat med upplevelser, resurser och attribut. <!-- GS-4812 -->

* Teckensnittsproblem i Meta-annonsmallar har lösts för att förbättra läsbarheten och tillgängligheten. <!-- GS-5354 -->

* Ändringar i utkastsrubriker bevaras nu som förväntat. Tidigare återgick rubrikerna till standardnamnet efter redigering. <!-- GS-2951 -->

#### Mallkorrigeringar

* Storleksförändringsfunktionen fungerar nu som väntat med flera bilder i Meta-annonsmallar. Tidigare storleksändrades inte bilder i GenStudio för alla valda mallar. <!-- GS-4696 -->

* Om du tar bort en mall uppdateras sidan [!DNL Content] som förväntat. <!-- GS-5397 -->

* Användarna kan nu bara välja värden för [!DNL Personas], [!DNL Brands] eller [!DNL Products] i listrutan. I dialogrutan _Mallöverföring_ kan användare ange valfritt [!DNL Persona]-, [!DNL Brand]- eller [!DNL Product]-namn. <!-- GS-5072 5071-->

* Knappen **[!UICONTROL Back]** är nu inaktiverad under mallöverföringen. <!-- GS-5358 -->

* Alla strängar i vyn [!DNL Create] Välj mallinformation är nu lokaliserade. <!-- GS-5025 -->

## Tidigare versioner av Beta

Tidigare versioner av Beta innehöll följande programfixar och markeringar.

### Högdagrar

* Innehållsväljaren [!DNL Create] har omarbetats för att förbättra resursinläsningen. <!-- GS-2586 -->

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

* **Metaannonser Ändra storlek**: Redigerare kan ändra storlek på metadata och proportioner. (fast 8/16)

* **Begränsade [!DNL Insights] inloggningskonton**: Inloggningen [!DNL Insights] har nu bara stöd för ett konto per kund. (fast 8/16)

### Ytterligare förbättringar och åtgärdade problem

* Arbetsytan [!DNL Create] återger nu bilder i Meta-annonser korrekt. (fast 9/13) <!-- GS-4864 -->

* Även om det finns skillnader mellan förhandsvisningar av arbetsytan i Meta-annonser och exporterade vyer fungerar exporterade upplevelser som förväntat. (fast 9/13) <!-- GS-4492 4401 -->

* Överförda bilder innehåller nu de förväntade smarta taggarna. (fast 9/13) <!-- GS-4856 -->

* CSV-filen för export av metaannonser innehåller nu bilder som förväntat. Tidigare innehöll ZIP-filen CSV-exportfilen och NULL-filer i stället för bilder. (fast 9/13) <!-- GS-5107 -->

* Användare kan nu ange text i malldetaljsvyn **[!UICONTROL Uploaded by]** som förväntat. Tidigare hindrade ikonen för inläsning användarna från att skriva text. (fast 9/13) <!-- GS-4887 -->

* Användare omdirigeras inte längre till detaljvyn för ett varumärke efter att varumärket har tagits bort. (fast 9/13) <!-- GS-2663 -->

* Redigerare får inte längre följande fel när varianter skickas för granskning och godkännande: `You have no access to view comments on this Object`. (fast 9/13) <!-- GS-5140 -->

* Uppdaterade e-postmallen som används i arbetsflödet för granskning och godkännande. (fast 9/13) <!-- GS-5239 -->

* GenStudio visar nu ett felmeddelande när ett nätverksfel inträffar när mallväljaren läses in. (fast 9/13) <!-- GS-4682 -->

* Löste problem med att navigera från en resurs, en upplevelse eller ett mallkort till det valda objektet. (fast 9/13) <!-- GS-4390 -->

* Popup-fönstret _Lägg till Assets_ är nu lokaliserat när det öppnas från Skapa arbetsyta. (fast 9/13) <!-- GS-4867 -->

* Varumärkesvalidering aktiveras nu för återskapade varianter. Tidigare aktiverades inte valideringen om en redigerare genererade om varianter av ett befintligt utkast. (fast 9/13) <!-- GS-3971 -->

* Popup-fönstret _Lägg till Assets_ är nu lokaliserat som förväntat. (fast 9/5) <!-- GS-3834 -->

* Problem med skalning av mallen Meta Adds Experience har lösts. (fast 9/5) <!-- GS-4174 -->

* Textfält i CSV-exportfilen för e-post med flera delar ordnas nu som förväntat. (fast 9/5) <!-- GS-4013 -->

* Sökfältet [!DNL Content] försvinner inte längre när en användare trycker på tangenten **Backsteg** upprepade gånger för att radera texten i sökfältet. (fast 9/5) <!-- GS-4543 -->

* GenStudio for Performance Marketers läser nu in användare som förväntat när en medarbetare lägger till en `@`-händelse till en kommentar. Tidigare lästes inte användarna in och ett fel visades: `Unable to load users. Refresh the page`. (fast 29/8) <!-- GS-4113 -->

* GenStudio visar inte längre meddelandet **Något gick fel** när en redigerare klickar på **Välj innehåll** när e-postmeddelandet skapades i promptområdet. <!-- GS-4879 -->

* Sidfeedplaceringsnamnet _Experience Detail_ anger nu Facebook- eller Instagram-feed. (fast 8/16)

* Det är nu konsekvent att beskära större bilder och videoklipp när användaren navigerar från vyn _Resursöversikt_ till vyn _Resursdetaljer_. (fast 8/16)

* Resultatantal för attributskärmssökning visas inte längre `0 of` innan en användare loggar in. (fast 8/16) <!-- GS-3665 -->

* När du klickar på fältet **[!UICONTROL [!DNL Insights]]** > **[!UICONTROL Asset]** rensas inte längre inställningarna för sökning och filter. (fast 8/16) <!-- GS-3476 -->

* Ett fel visas i GenStudio när en användare försöker ange inloggningsuppgifter i vyn [!DNL Insights]. (fast 29/8) <!-- GS-4689 -->

* Det går inte att överföra varumärkesriktlinjer på grund av problem med lagringsplattformen i AVS. (fast 8/22) <!-- GS-4369 -->

* I listrutan Fråga [!DNL Brands] visas en rotationsruta i slutet av listan [!DNL Brands] när e-postmeddelanden skapas. (fast 8/22) <!-- GS-4077 -->
