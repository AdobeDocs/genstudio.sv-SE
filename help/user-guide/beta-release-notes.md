---
title: Adobe GenStudio för Performance Marketers Beta versionsinformation
description: Läs om de senaste funktionerna och förbättringarna av Adobe GenStudion för Performance Marketers.
source-git-commit: 16f44baf646d696da3572ac2c17a5efb7c8f7fc6
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---


# Adobe GenStudio för Performance Marketers Beta versionsinformation

Dessa kommentarer belyser viktig Adobe GenStudio för korrigeringar och förbättringar av Performance Marketers för den vecka som slutar 6 september.

## Kända fel

Följande kända fel är schemalagda för lösning i GenStudio for Performance Marketers GA-versionen.

* Redigerare stöter ibland på ett felmeddelande om att något gick fel på [!DNL Create Canvas] under bildgenereringen. **Tillfällig lösning**: Om felet upprepas kan användaren logga ut, logga in på GenStudio igen och återskapa bilden.  <!-- GS-4813 -->

* [!DNL Create Canvas] återger bilder i Meta-annonser felaktigt. <!-- GS-4864 -->

* Assets utan kampanjer kan överföras till [!DNL Content], men är kanske inte synligt för användarna. <!-- GS-4815 -->

* Det finns skillnader mellan förhandsvisningar av MetaAds Canvas och exporterade vyer. <!-- GS-4492 4401 -->

* Kampanjminiatyrer saknas i [!DNL Insights]. <!-- GS-4648 -->

* Användarna kan för närvarande välja små resurser som kräver storleksändring, men det går inte att förstora dessa resurser. <!-- GS-3131 -->

* Användare måste logga in två gånger till ett Meta Ads-kanalkonto när de också är inloggade på Facebook. **Tillfällig lösning**: Logga ut från Facebook innan du loggar in på ett Meta Ads-kanalkonto.

### Lösta kända fel

* Ett fel visas i GenStudio när en användare försöker ange inloggningsuppgifter i vyn [!DNL Insights]. (fast 29/8) <!-- GS-4689 -->

## Tidigare versioner av Beta

Tidigare versioner av Beta innehöll följande programfixar och markeringar.

### Högdagrar

* **Procentandel av valideringspoäng**: I varumärkesvalideringen visas nu varumärkesvalideringspoängen i procent i stället för ett godkänt/underkänt värde. (fast 8/16)

* **Uppdaterat gränssnitt för varumärkesextrahering**: Extraheringen visar nu att extraheringsprocessen har slutförts i procent. (fast 8/16)

* **Inkrementell varumärkesbelastning under extrahering**: Riktlinjer för varumärket läses nu in stegvis i användargränssnittet. (fast 8/16)

* **Skapa e-post i flera avsnitt**: Användare kan nu skapa e-postmeddelanden som består av separata rubriker, bilder, brödtext och CTA-element. (fast 8/16)

* **Storleksändring för metaannonser**: Redigerare kan ändra storlek på metadata och proportioner. (fast 8/16)

* **Begränsade Insights-inloggningskonton**: Inloggningen för Insights har nu bara stöd för ett konto per kund. (fast 8/16)

### Ytterligare förbättringar och åtgärdade problem

* Sidfeedplaceringsnamnet _Experience Detail_ anger nu Facebook- eller Instagram-feed. (fast 8/16)

* Det är nu konsekvent att beskära större bilder och videoklipp när användaren navigerar från vyn _Resursöversikt_ till vyn _Resursdetaljer_. (fast 8/16)

* Resultatantal för attributskärmssökning visas inte längre `0 of` innan en användare loggar in. (fast 8/16) <!-- GS-3665 -->

* När du klickar på fältet **[!UICONTROL [!DNL Insights]]** > **[!UICONTROL Asset]** rensas inte längre inställningarna för sökning och filter. (fast 8/16) <!-- GS-3476 -->

### Kända problem som lösts i tidigare versioner av Beta

* Det går inte att överföra varumärkesriktlinjer på grund av problem med lagringsplattformen i AVS. (fast 8/22) <!-- GS-4369 -->

* I listrutan Fråga [!DNL Brands] visas en rotationsruta i slutet av listan [!DNL Brands] när e-postmeddelanden skapas. (fast 8/22) <!-- GS-4077 -->

