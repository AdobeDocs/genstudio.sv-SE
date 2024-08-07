---
title: Skapa en e-postupplevelse
description: Lär dig hur du skapar e-postupplevelser i Adobe [!DNL GenStudio].
feature: Content, Brands Service, Guidelines, Content Generation
role: User
level: Beginner
type: Tutorial
recommendations: noDisplay
source-git-commit: fa89422db3e1679516a377c9bfd9f05ab6e63428
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 0%

---


# Skapa en e-postupplevelse

I den här självstudiekursen visas hur du skapar varumärkesanpassade e-postupplevelser med GenStudio [[!DNL Create]](/help/user-guide/create/overview.md) (penselikonen i det vänstra navigeringsområdet).

Om du vill skapa en effektiv e-postupplevelse rekommenderar vi att du [lägger till riktlinjer i GenStudio](/help/user-guide/guidelines/add-guidelines.md) och penselredigerar [grunderna för att skapa en fråga](/help/user-guide/effective-prompts.md) innan du börjar.

## Välj en mall

Om du vill komma igång med att skapa en ny e-postupplevelse kan du använda en tillgänglig mall för att tillhandahålla ramverket för ditt innehåll.

**Så här väljer du en e-postmall**:

1. I _[!DNL Create]_klickar du på&#x200B;**[!UICONTROL Email]**i_&quot;Vad vill du skapa idag?&quot;avsnittet _.
1. I vyn _Välj mall_ växlar du filtret _Kanaler_ till **[!UICONTROL Email]**.
1. Använd sökalternativet bredvid _Filter_ för att hitta en viss e-postmall.
1. Klicka för att välja en e-postmall eller för att växla mellan flera e-postmallar och klicka på **[!UICONTROL Use]**. Om du väljer flera mallar används alla valda mallar när varianterna genereras.

   Arbetsytan, innehållscenter, visas.

## Lägg till parametrar

Att lägga till parametrar för riktlinjer lägger grunden till innehållsgenereringsprocessen och är ett viktigt förberedelsesteg för att skapa en e-postupplevelse.

**Så här lägger du till parametrar och resurser**:

1. Klicka på ikonen _Parametrar_ för att utöka parameteralternativen och lägga till referensparametrar och resurser.
1. I avsnittet _Parametrar_ väljer du riktlinjer - Varumärke, Persona och Produkt - för att informera om hur du skapar innehåll.

   Om det inte finns några varumärken, profiler eller produkter tillgängliga från dessa menyer [lägger du till riktlinjer i din GenStudio](/help/user-guide/guidelines/add-guidelines.md).

1. I avsnittet _Innehåll_ lägger du till innehåll som ska användas i upplevelsen *och* för att påverka innehållsgenereringen. Det finns tre sätt att lägga till resurser:
   * Klicka på **[!UICONTROL Select from content]** för att välja resurser (bilder eller video) som redan har publicerats till [!DNL Content]. Använd filtren för att begränsa sökresultaten ytterligare.
   * Klicka på **[!UICONTROL Upload]** för att bläddra bland dina filer och välja resurser som ska användas. Du kan även importera från Microsoft OneDrive eller Dropbox.
   * Dra och släpp resurser i avsnittet _Innehåll_.

   När du väljer resurser från GenStudio-innehåll väljer du bland resurser som redan har sparats i [[!DNL Content]](/help/user-guide/content/overview.md). Du kan filtrera efter kanal, produkt, språk med mera för att snabbt hitta de resurser du behöver.

När du är klar med att lägga till parametrar kan du komprimera avsnitten *Parametrar* och *Innehåll* genom att klicka på ikonen _Parametrar_ igen.

## Använda en uppmaning

När du har valt riktlinjer kan du snabbt börja generera innehåll för din nya e-postupplevelse med det naturliga språket.

Läs [Skriv effektiva uppmaningar](/help/user-guide/effective-prompts.md) om du vill veta mer om hur du skriver uppmaningar.

**Så här använder du en fråga**:

1. Ange en uppmaning i rutan _&quot;Beskriv de upplevelser du vill generera&quot;_ .
   <!-- If the prompt box is not visible, click **[!UICONTROL Open to prompt]** to expand it. -->

<!-- 1. Optionally, click one of the prompt suggestions visible just above the prompt text box. Clicking a suggestion auto-fills the suggested prompt in the prompt box. -->
1. Klicka på **[!UICONTROL Generate]**.

Som standard visas fyra genererade variationer - som alla följs av uppmaningen, riktlinjer och innehåll som du har lagt till - på arbetsytan.

## Granska genererade e-postmeddelanden

Innan du väljer vad som ska skickas för godkännande eller publicering till [!DNL Content] kan du redigera e-postfragment eller ta bort en variant från uppsättningen genererade e-postmeddelanden.

**Så här granskar du genererade varianter**:

* **Om du vill redigera ett e-postmeddelande** manuellt dubbelklickar du på något av e-postfragmenten (till exempel ämnesraden, huvudet eller brödtexten) och redigerar efter behov.

  Subject line and preheader only require a single click to edit, while the header, body copy, and call to action require a double click.

* **Om du vill ta bort ett e-postmeddelande** klickar du för att markera e-posttiteln (till exempel&quot;E-post 1/4&quot;) och klickar på **[!UICONTROL Delete variant]**.

## Verifiera varumärkesjustering

Om du vill optimera de genererade e-postmeddelandena och säkerställa strikt efterlevnad av varumärkesidentiteten kan du utnyttja kraften i kontrollen [_Varumärkesriktlinjer_](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) - som ger en sammanfattning av varumärkeskontraktionen för en variant - och [_Varumärkesvalideringspanelen_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel) - som visar omfattande information om varumärkesvalidering och upplysta förbättringsområden.

Du kan redigera enskilda e-postfragment manuellt eller [generera förfinade varianter](/help/user-guide/create/generate-variants.md) av det ursprungliga resultatet för att anpassa dig efter ditt varumärke.

**Så här verifierar du varumärkesjustering**:

1. Klicka på ikonen [**[!UICONTROL [!DNL Brand] guidelines check]**](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) för en variant och se en sammanfattning av hur varianten fungerar när den kontrolleras mot ditt varumärke.
1. Klicka **[!UICONTROL Review]** _eller_ på ikonen för validering av varumärke i den övre menyraden för att visa information om de fragment och riktlinjer som behöver förbättras, så att [_panelen för validering av varumärke_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel) visas.

1. Växla mellan e-postmeddelanden för att se hur ni kan förbättra det genererade innehållet så att det blir mer varumärkesanpassat.
1. [Granska e-postmeddelanden ](#revise-generated-emails) manuellt eller [generera varianter](/help/user-guide/create/generate-variants.md) för att vara säker på att e-postmeddelandena är i linje med ert varumärke.

Se [Varumärkesvalidering](/help/user-guide/guidelines/brand-validation.md).

## Få recensioner och godkännanden

Använd panelen Godkännanden, som finns på den övre menyraden på arbetsytan, för att få granskningskommentarer, spåra granskningskommentarer och få godkännanden från intressenter.

**Så här får du granskningar och godkännanden**:

1. [Starta en godkännandebegäran](/help/user-guide/approvals/request-review.md) för att begära ett [godkännande av utkast till e-postupplevelser](/help/user-guide/approvals/approve-content.md).
1. [Ta bort eller lägg till granskare](/help/user-guide/approvals/review-and-edit.md#manage-approvals) under granskningsprocessen.
1. [Få åtkomst till innehållet för granskning](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) och visa begäranden om revision.
1. Redigera utkasten per granskningskommentarer och [publicera dina e-postupplevelser](#publish-and-export-experience).

Mer information finns i [Recensioner och godkännanden](/help/user-guide/approvals/overview.md).

## Publish och exportupplevelser

Om du vill göra de genererade e-postmeddelandena tillgängliga för aktuell och framtida användning publicerar du dem på [!UICONTROL Content] och exporterar dem för användning i dina marknadsföringskampanjer.

1. **Om du vill publicera dina nya e-postupplevelser** klickar du på **[!UICONTROL Publish]** i det övre verktygsfältet.
1. **Om du vill exportera dina nya e-postupplevelser** klickar du på **[!UICONTROL Export]** i det övre verktygsfältet.
   1. Markera formatet (endast CSV och bilder eller HTML) och klicka på **[!UICONTROL Export]**.

Mer information finns i [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
