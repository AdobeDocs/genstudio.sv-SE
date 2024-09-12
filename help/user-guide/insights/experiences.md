---
title: Översikt över upplevelser
description: Se en översikt över kundengagemang, budget och utgifter för upplevelser och tillgångsprestanda i Adobe GenStudio för Performance Marketers.
feature: Insights, Experiences
source-git-commit: 70ce82b026b2ee1f088cda75caa22bbb1b9c5ef3
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%

---


# Översikt över upplevelser

Vyn [!DNL Insights] _[!UICONTROL Experiences]_visar en lista med annonser och upplevelser för det anslutna kanalannonskontot.

Tabellen [!UICONTROL Experiences] är ordnad med [!UICONTROL Ad names]. Filterikonen (trattikonen) ovanför tabellens vänstra sida öppnar menyn **[!UICONTROL Filter]** där du kan välja i listorna [!UICONTROL Account] och [!UICONTROL Campaign] för att filtrera annonsnamnen i tabellen.

![Upplevelsfilter och tabell](../../assets/insights-experiences-filter.png)

## Annonsinformation

När du väljer ett annonsnamn kan du visa mått och attribut för annonsprestanda, som gör att du kan analysera en upplevelses mått baserat på annonsplaceringen inom ett visst datumintervall.

Detaljvyn innehåller ett helhetsmått för annonsen `click-through rate`, `cost per click` och hur mycket av budgeten som har varit `spent`. Eftersom annonser kan ha flera placeringar, t.ex. en feed eller en banner, kan du se en uppdelning av samma mätvärden för varje annonsplacering. Använd vänster- och högerpilarna under **[!UICONTROL Performance by ad placement]** för att bläddra igenom mätvärdena för annonsplacering.

![Lägg till information med mått och annonsplaceringar](../../assets/insights-ad-details.png)

### Textattribut

Under annonsen visas en lista med [!UICONTROL Text attributes] som är associerad med annonsen. När resurser och upplevelser har godkänts och lagrats i [!DNL Content] genererar GenStudio for Performance Marketers taggar baserat på deras inneboende funktioner. Mer information om systemmetadata finns i [Resursinformation](../content/asset-details.md#system-metadata).

### Annonsplaceringar

När du skapade en kampanj med Meta Ads kan du ha valt var annonserna ska köras baserat på kampanjens [mål](channels.md#objectives). Annonsplaceringar breddar räckvidden för era annonser.

GenStudio for Performance Marketers har stöd för annonsformat som resursflöden, länkannonser och enskild bild eller video. Nedan följer en lista över annonsformat per plattform:

| Instagram | Facebook/Meta | Messenger | Målgruppsnätverk |
| --- | --- | --- | --- |
| Utforska<br>Utforska startsidan<br>Utforska startsidan för stödraster<br>Feed<br>Reels<br>Profilfeed<br>Sök<br>Handla<br>Artiklar | Business Explore<br>Feed<br>Inströmsvideo<br>Marketplace<br>Reels<br>Reels Overlay<br>Right-column<br>Search<br>Stories<br>Video Feeds<br>Ads on Facebook Reels | Inkorg<br>artiklar | Intern video, banderoll och interstitiell<br>inbyggd<br>återgiven video |

## Mått

Insikter kan hjälpa er att utvärdera vilka upplevelser som bidrar till framgången för en kampanj och vilka annonsplaceringar som är mest effektiva.

### Mätvärdesdetalj

Följande tabell innehåller definitioner och insikter för viktiga mätvärden för digital marknadsföring i vyn [!UICONTROL Experiences]. Varje mätvärde innehåller en kort definition av annonsnamn, hur mätvärdet beräknas och en eller flera insikter som hjälper till att förstå dess betydelse och påverkan på en upplevelse.

| Mått | Definition | Insikt |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Campaign]** | En kampanj är en uppsättning upplevelser och annonser som utformats för att uppnå ett visst mål. | |
| **[!UICONTROL Ad placements]** | Antal annonsplaceringar för annonsen eller upplevelsen. | Annonsplaceringar ökar publikens räckvidd. |
| **[!UICONTROL Assets]** | Antal resurser som används i annonsen eller upplevelsen. | |
| **[!UICONTROL Impressions]** | Impressions räknas varje gång innehållet läses in på skärmen, oavsett interaktion eller visning. | Ett högt visningsvärde kan visa på bred synlighet, men för verkliga prestandainsikter bör du överväga andra engagemangsmått. |
| **[!UICONTROL Clicks]** | Antal gånger som användare interagerar med ett klickbart element i en annons. Du kan klicka på en sidprofil eller bild, skicka svar, dela, kommentera eller expandera media till helskärm. | Ett högt klickningsantal visar starkt intresse och engagemang för innehållet, vilket kan vara effektivt och nå rätt målgrupp. |
| **[!UICONTROL CTR]** | Procentandel (%) av användarna som klickade på en annons.<br>**Beräkning**: `clicks` delat med `impressions` | En hög klickfrekvens visar att innehållet är mycket relevant och motiverat för målgruppen i budskapen och designen och att det effektivt riktar sig till målgruppens intressen. |
| **[!UICONTROL CPM]** | Resultatmätning för kostnad ($) per tusen annonsvisningar.<br>**Beräkning**: totalt belopp `spent` dividerat med räckvidd, multiplicerat med 1000 | Ett lågt värde kan indikera kostnadseffektiv synlighet, särskilt om det kombineras med en hög klickfrekvens. |
| **[!UICONTROL CPC]** | Genomsnittskostnad ($) som associeras med varje klick i en upplevelse.<br>**Beräkning**: totalt belopp `spent` delat med `clicks` | Lägre genomsnittliga kostnader kan tyda på kostnadseffektiva annonskostnader, särskilt om man jämför med en ökning av antalet konverteringar. |
| **[!UICONTROL Spend]** | Det belopp som har använts från budgeten under en viss tidsperiod. | Ett högt utgiftsbelopp under en kort period kan tyda på snabb användning, vilket kan leda till att resurser tar slut i förtid. Spåra utgiftsbeloppet mot nyckeltal för att övervaka den totala avkastningen på investeringen. |
