---
title: Adobe GenStudio för Performance Marketers Beta versionsinformation
description: Läs om de senaste funktionerna och förbättringarna av Adobe GenStudion.
source-git-commit: 382026b07e123a1e49813b766f69496f6a8f38eb
workflow-type: tm+mt
source-wordcount: '387'
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

* _Bildgenerering: Kategorival_: Användare kan nu välja riktlinjer för bilder som är specifika för deras behov av bildåtergivning.

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

### Varumärke

* Den som skapar varumärket kan publicera det, men organisationens medlemmar kan inte se varumärket. <!-- XI-2197 -->

### Skapa

* Bildbeskärning i Meta-annonser är inkonsekvent. <!-- GS-3739 -->

* Mallar som består av flera grupper av sidelement kan inte valideras. <!-- GS-4037 -->

### Insikter

* Åtkomst nekas fel med slutpunkten `/admin/addOffer` (etableringstjänsten). **Löst 8/12**. <!-- GS-4047 -->

* **Utgifterna på kampanjnivå** är inte korrekta. Data är för närvarande inte konsekventa mellan Facebook Ads Manager och datasjön. <!-- GS-3202 -->

### Recensioner och godkännanden

* Skapare kan ändra resurser efter godkännande innan de publicerar det. Godkännare meddelas inte om dessa ändringar.
