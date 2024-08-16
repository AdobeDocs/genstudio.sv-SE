---
title: Adobe GenStudio för Performance Marketers Beta versionsinformation
description: Läs om de senaste funktionerna och förbättringarna av Adobe GenStudion för Performance Marketers.
source-git-commit: cbae3aeb1b8282fb64f2a6405a7ad9e07a48dbbd
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---


# Adobe GenStudio för Performance Marketers Beta versionsinformation

I dessa kommentarer beskrivs viktiga korrigeringar och förbättringar av Adobe GenStudion för den vecka som slutar den 16 augusti.

## Högdagrar

Funktionsutvecklingen är snabb och kontinuerlig. Några viktiga nya funktioner:

### [!DNL Brands]

Valideringspanelen [!DNL Brand] har förbättrats för att förbättra användarupplevelsen, inklusive följande ändringar:

* **Procentandel av valideringspoäng**: I varumärkesvalideringen visas nu varumärkesvalideringspoängen i procent i stället för ett godkänt/underkänt värde.

* **Uppdaterat gränssnitt för varumärkesextrahering**: Extraheringen visar nu att extraheringsprocessen har slutförts i procent.

* **Inkrementell varumärkesbelastning under extrahering**: Riktlinjer för varumärket läses nu in stegvis i användargränssnittet.

* **Förenkling av schemat för Kopiera stödlinje**: Fälten `unique attributes` och `frequent keywords` har tagits bort från schemat Kopiera stödlinje, vilket förenklar processen för att konfigurera stödlinjer.

### [!DNL Create]

* **Skapa e-post i flera avsnitt**: Användare kan nu skapa e-postmeddelanden som består av separata rubriker, bilder, brödtext och CTA-element.

* **Storleksändring för metaannonser**: Skapare kan ändra storlek på metadata och proportioner.

### [!DNL Insights]

* **Begränsade Insights-inloggningskonton**: Inloggningen för Insights har nu bara stöd för ett konto per kund.

## Förbättringar och åtgärdade problem

Den här versionen innehåller följande ytterligare korrigeringar.

### [!DNL Insights]

* Sidfeedplaceringsnamnet _Experience Detail_ anger nu Facebook- eller Instagram-feed.

* Beskärning av större bilder och videor är nu konsekvent när användaren navigerar från vyn _Resursöversikt_ till vyn _Resursdetaljer_ .

* Resultatantal för attributskärmssökning visas inte längre `0 of` innan en användare loggar in. <!-- GS- 3665 -->

* När du klickar på fältet **[!UICONTROL [!DNL Insights]]** > **[!UICONTROL Asset]** rensas inte längre inställningarna för sökning och filter. <!-- GS-3476 -->

## Kända fel

Följande kända problem kommer att åtgärdas med GenStudio for Performance Marketers GA-versionen.

### Analyser

* Åtgärder som utlöses av knapparna **[!UICONTROL Add templates]** och **[!UICONTROL Upload]** spåras inte för närvarande. <!-- GS-3505 -->

### [!DNL Insights]

* Det går inte att spela upp videofilmer från _Assets_. <!-- GS-3846 -->

* Användarna måste logga in två gånger när de också är inloggade på Facebook. **Tillfällig lösning**: Logga ut från Facebook innan du loggar in på [!DNL Insights].

* **Utgifterna på kampanjnivå** är inte korrekta. Data är för närvarande inte konsekventa mellan Facebook Ads Manager och datasjön. <!-- GS-3202 -->

### [!DNL Reviews and Approvals]

* Upphovsmannen kan ändra materialet efter att ha godkänt det innan det publiceras. Godkännare meddelas inte om dessa ändringar.

