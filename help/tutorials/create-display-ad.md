---
title: Skapa en webbannonsupplevelse
description: Lär dig hur du skapar webbannonsupplevelser i Adobe [!DNL GenStudio] för Performance Marketers.
feature: Brands Service, Guidelines, Content Generation, Generative AI, Create, Experiences, Variant Generation
role: User
level: Beginner
type: Tutorial
recommendations: noDisplay
source-git-commit: 9624429977e21af614173c5078c6b470c8b5a147
workflow-type: tm+mt
source-wordcount: '790'
ht-degree: 0%

---

# Skapa en webbannonsupplevelse

I den här självstudiekursen visas hur du skapar varumärkesanpassade annonsupplevelser med GenStudio för Performance Marketers [[!DNL Create]](/help/user-guide/create/overview.md) (penselikonen i det vänstra navigeringsområdet).

Om du vill skapa en övertygande webbannonsupplevelse rekommenderar vi att du [lägger till riktlinjer i GenStudio för Performance Marketers](/help/user-guide/guidelines/add-guidelines.md) och penseldrar på [grunderna för skrivande av uppmaningar](/help/user-guide/effective-prompts.md) innan du börjar.

## Välj en mall

Om du vill skapa en webbannonsupplevelse använder du en tillgänglig mall för att tillhandahålla ramverket för ditt innehåll.

**Så här väljer du en visningsannonsmall**:

1. I _[!DNL Create]_klickar du på&#x200B;**[!UICONTROL Display ads]**i_&quot;Vad vill du skapa idag?&quot;avsnittet _.
1. Använd sökalternativet, bredvid _Filter_, för att hitta en specifik mall för visningsannons.
1. I vyn _Välj mall_ klickar du på en mall för visningsannons.
1. Klicka på **[!UICONTROL Use]**.

   Arbetsytan, som fungerar som nav för att skapa innehåll, visas.

## Lägg till parametrar

Om du lägger till [riktlinjer](/help/user-guide/guidelines/overview.md) och resurser i _Parametrar_ i promptområdet överbelastas innehållsgenereringsprocessen och är ett viktigt förberedelsesteg för att generera en e-postupplevelse.

**Så här lägger du till parametrar och resurser**:

1. Klicka på ikonen _Parametrar_ för att utöka promptområdet.
1. I avsnittet _Parametrar_ väljer du riktlinjer -[!DNL Brands], [!DNL Personas] och [!DNL Products] - för att informera om hur du skapar innehåll.

   Om det inte finns några varumärken, profiler eller produkter tillgängliga från de här menyerna [lägger du till riktlinjer i din GenStudio för Performance Marketers](/help/user-guide/guidelines/add-guidelines.md).

1. Klicka på **[!UICONTROL Select content]** om du vill lägga till innehåll som ska användas i upplevelsen *och* om du vill påverka innehållsgenereringen.
   * Klicka på **[!UICONTROL Select from content]** för att välja resurser (bilder) som redan har publicerats till [!DNL Content]. Använd filtren för att begränsa sökresultaten ytterligare.
   * Klicka på **[!UICONTROL Upload]** för att bläddra bland dina filer och välja resurser som ska användas. Du kan importera från Microsoft OneDrive eller Dropbox tillsammans med att bläddra på enheten.
   * Dra och släpp resurser i avsnittet _Innehåll_.
1. Klicka på **[!UICONTROL Use]**.

När du är klar med att lägga till parametrar komprimerar du frågeområdet genom att klicka på ikonen _Parametrar_ igen.

## Ange en uppmaning

När du har valt riktlinjer kan du snabbt skapa innehåll för den nya webbannonsupplevelsen med hjälp av det naturliga språket. För att förbättra kvaliteten på den genererade webbannonsupplevelsen är det viktigt att skapa detaljerade och beskrivande uppmaningar.

Läs [Skriv effektiva uppmaningar](/help/user-guide/effective-prompts.md) om du vill veta mer om hur du skriver uppmaningar.

**Så här skriver du en fråga**:

1. Ange en uppmaning i rutan _&quot;Beskriv de upplevelser du vill generera&quot;_ .
1. Klicka på **[!UICONTROL Generate]**.

Som standard genereras och visas fyra varianter på arbetsytan, som alla föds av uppmaningen, riktlinjer och innehåll som du har lagt till.

## Revidera genererade displayannonser

Innan du väljer vad som ska skickas för godkännande eller publicering till [!DNL Content] kan du redigera visnings- och textavsnitt eller ta bort en genererad variant.

**Så här granskar du genererade varianter**:

* **Om du vill [redigera namnet för visning och utkast](/help/user-guide/create/manage-variants.md#change-draft-name)** klickar du i titeln _Namnlöst utkast_ längst upp på arbetsytan och anger en ny titel.
* **Om du vill [redigera en visningsannons manuellt](/help/user-guide/create/manage-variants.md#manually-edit-text)** dubbelklickar du i något av avsnitten eller fälten i displayannonsen (t.ex. ämnesraden, huvudet eller brödtexten) och redigerar efter behov.
* **Om du vill [ändra storlek och proportioner för annonsen](/help/user-guide/create/manage-variants.md#change-aspect-ratio)** klickar du på knappen _[!UICONTROL Resize]_(ruta med en knappikon till vänster om arbetsytan) och väljer en ny storlek och proportioner som ska användas för alla varianter. Varianterna dupliceras och storleksändras.

<!-- # Preview for device

When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.

**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. -->

## Verifiera varumärkesjustering

Om du vill optimera de annonser som skapas och säkerställa strikt överensstämmelse med varumärkesidentiteten kan du utnyttja kraften i kontrollen [_Varumärkesriktlinjer_](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) - som ger en sammanfattning av varumärkesjusteringen för en variant - och [_Varumärkesvalideringspanelen_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel) - och som visar omfattande information om varumärkesvalidering och upplysta förbättringsområden.

**Så här verifierar du varumärkesjustering**:

1. Klicka på ikonen [**[!UICONTROL [!DNL Brand] guidelines check]**](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) för en variant och se en sammanfattning av hur varianten fungerar när den kontrolleras mot ditt varumärke.
1. Klicka **[!UICONTROL Review]** _eller_ på ikonen för validering av varumärke i den övre menyraden för att visa information om de fragment och riktlinjer som behöver förbättras, så att [_panelen för validering av varumärke_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel) visas.

1. Se hur ni kan förbättra det genererade innehållet så att det blir mer varumärkesanpassat.
1. [Granska annonser manuellt](#revise-generated-display-ads) för att säkerställa att dina e-postmeddelanden är i linje med ditt varumärke.

Se [Varumärkesvalidering](/help/user-guide/guidelines/brand-validation.md).

## Få recensioner och godkännanden

Använd panelen Godkännanden, som finns på den övre menyraden på arbetsytan, för att få granskningskommentarer, spåra granskningskommentarer och få godkännanden från intressenter.

**Så här får du granskningar och godkännanden**:

1. [Starta en godkännandebegäran](/help/user-guide/approvals/request-review.md) för att begära ett [godkännande av utkast till e-postupplevelser](/help/user-guide/approvals/approve-content.md).
1. [Ta bort eller lägg till granskare](/help/user-guide/approvals/review-and-edit.md#manage-approvals) under granskningsprocessen.
1. [Få åtkomst till innehållet för granskning](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) och visa begäranden om revision.
1. Redigera utkasten per granskningskommentarer och [publicera dina e-postupplevelser](#publish-and-export-experience).

Se [Recensioner och godkännanden](/help/user-guide/approvals/overview.md).

## Publish och exportupplevelser

Om du vill göra de genererade webbannonserna tillgängliga för aktuell och framtida användning publicerar du dem på [!UICONTROL Content] och exporterar dem för användning i dina marknadsföringskampanjer.

1. **Klicka **[!UICONTROL Publish]**i det övre verktygsfältet om du vill publicera dina nya visningsannonsupplevelser**.
1. **Klicka **[!UICONTROL Export]**i det övre verktygsfältet om du vill exportera dina nya visnings- och annonsupplevelser**.
   1. Markera formatet (endast JPG och PNG) och klicka på **[!UICONTROL Export]**.

Se [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
