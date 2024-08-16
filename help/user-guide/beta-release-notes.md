---
title: Adobe GenStudio för Performance Marketers Beta versionsinformation
description: Läs om de senaste funktionerna och förbättringarna av Adobe GenStudion.
source-git-commit: 5505e3fdc78e217dd1eb73ed5bffa5e43d4f3084
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---


# Adobe GenStudio för Performance Marketers Beta versionsinformation

I dessa kommentarer beskrivs viktiga korrigeringar och förbättringar av Adobe GenStudion för den vecka som slutar den 16 augusti.

## Högdagrar

GenStudio funktionsutveckling går snabbt och kontinuerligt. Några viktiga nya funktioner:

### Varumärke

Valideringspanelen för varumärket har förbättrats för att förbättra användarupplevelsen, bland annat:

* _Procentandel av valideringspoäng_: I varumärkesvalideringen visas nu varumärkesvalideringspoängen i procent i stället för ett godkänt/underkänt värde.

* _Uppdaterat gränssnitt för varumärkesextrahering_: Extraheringen visar nu att extraheringsprocessen har slutförts i procent.

* _Inkrementell varumärkesbelastning under extrahering_: Riktlinjer för varumärket läses nu in stegvis i användargränssnittet.

* _Förenkling av schemat för Kopiera stödlinje_: Fälten `unique attributes` och `frequent keywords` har tagits bort från schemat Kopiera stödlinje, vilket förenklar processen för att konfigurera stödlinjer.

### Skapa

* **Skapa e-post i flera avsnitt**: Användare kan nu skapa e-postmeddelanden som består av separata rubriker, bilder, brödtext och CTA-element.

* **Storleksändring för metaannonser**: Skapare kan ändra storlek på metadata och proportioner.

### Insikter

* **Begränsade Insights-inloggningskonton**: Inloggningen för Insights har nu bara stöd för ett konto per kund.

## Förbättringar och åtgärdade problem

Den här versionen innehåller följande ytterligare korrigeringar.

### Insikter

* Sidfeedplaceringsnamnet _Experience Detail_ anger nu Facebook- eller Instagram-feed.

* Beskärning av större bilder och videor är nu konsekvent när användaren navigerar från vyn _Resursöversikt_ till vyn _Resursdetaljer_ .

* Resultatantal för attributskärmssökning visas inte längre `0 of` innan en användare loggar in. <!-- GS- 3665 -->

* När du klickar på fältet **[!UICONTROL Insight]** > **[!UICONTROL Asset]** rensas inte längre inställningarna för sökning och filter. <!-- GS-3476 -->

## Kända fel

Följande kända problem kommer att åtgärdas med GenStudio for Performance Marketers GA-versionen.

### Analyser

* Åtgärder som utlöses av knapparna **[!UICONTROL Add templates]** och **[!UICONTROL Upload]** spåras inte för närvarande. <!-- GS-3505 -->

### Insikter

* Det går inte att spela upp videofilmer från _Assets_. <!-- GS-3846 -->

* Användarna måste logga in två gånger när de också är inloggade på Facebook. **Tillfällig lösning**: Logga ut från Facebook innan du loggar in på Insights.

* **Utgifterna på kampanjnivå** är inte korrekta. Data är för närvarande inte konsekventa mellan Facebook Ads Manager och datasjön. <!-- GS-3202 -->

### Recensioner och godkännanden

* Upphovsmannen kan ändra materialet efter att ha godkänt det innan det publiceras. Godkännare meddelas inte om dessa ändringar.

