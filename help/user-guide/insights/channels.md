---
title: Översikt över kanaler
description: Se en översikt över kundengagemang, resultat, budget och utgifter för marknadsföringskampanjer i Adobe GenStudio för Performance Marketers.
feature: Insights, Channels
source-git-commit: 2e76eadcc3281ea935dca383eb3db8c41b83e679
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---


# Översikt över kanaler

Vyn [!DNL Insights] _[!UICONTROL Channels]_visar en lista med kampanjer för det anslutna kanalannonskontot.

>[!TIP]
>
>GenStudio för Performance Marketers kräver att du ansluter till ett kanalkonto för att börja ta emot data. Se [Anslut kanalkonto](connect-channel.md).

Tabellen [!UICONTROL Channels] är organiserad med den kanalbaserade annonskampanjen. Filterikonen (trattikonen) ovanför den vänstra sidan av tabellen öppnar menyn **[!UICONTROL Filter]** där du kan välja i listorna [!UICONTROL Account], [!UICONTROL Status] och [!UICONTROL Objective] för att filtrera kampanjer i tabellen.

![Kanalfilter och tabell](../../assets/insights-channel-filter.png)

När du väljer en kampanj öppnas fliken [!UICONTROL Experiences] med en lista över annonsnamn som är associerade med kampanjen.

## Mål

När ni skapade en kampanj med Meta Ads kan ni ha valt ett mål som är anpassat till era affärsmål. Det finns sex mål från Meta Ads som är synliga i GenStudio för Performance Marketers:

1. **Kännedom**: Nå ut till största möjliga publik och nå ut till ert företag.
1. **Trafik**: Öka trafiken till din webbplats eller ditt program.
1. **Engagemang**: Interagera med befintliga och potentiella kunder.
1. **Leads**: Skapa anslutningar för att utöka er målgrupp.
1. **Appkampanj**: Befordra ditt program.
1. **Försäljning**: Fokusera på att nå de personer som mest sannolikt kommer att använda din produkt.

## Mått

Beroende på era prestationsmål kan Insights-mätvärden hjälpa er att utvärdera om ni uppfyller era mål.

Om du till exempel har som mål att öka medvetenheten kan en ökning av hastigheten `impressions` tyda på att du utökar din räckvidd. Om du vill förstå om det uppnår ditt mål kan du titta på mätvärden som anger att ditt innehåll är engagerande, till exempel `clicks` eller `video plays`. Hur effektivt interagerar er målgrupp med ert innehåll?

### Mätvärdesdetalj

Följande tabell innehåller definitioner och insikter för viktiga mätvärden för digital marknadsföring i kanalvyn. Varje mätvärde innehåller en kort definition vad gäller kanaler, hur mätvärdet beräknas och en eller flera insikter som hjälper till att förstå dess betydelse och påverkan på marknadsföringskampanjer.

| Mått | Definition | Insikt |
| ----------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Launch]** | Det datum då kampanjen släpptes eller publicerades på marknaden. | Ett högt antal visningar kan tyda på att annonsen når den avsedda målgruppen. |
| **[!UICONTROL Impressions]** | Impressions räknas varje gång innehållet läses in på skärmen, oavsett interaktion eller visning. | Ett högt visningsvärde kan visa på bred synlighet, men för verkliga prestandainsikter bör du överväga andra engagemangsmått. |
| **[!UICONTROL Clicks]** | Antal gånger som användare interagerar med ett klickbart element, till exempel en länk eller en annons. | Ett högt klickningsantal visar starkt intresse och engagemang för innehållet, vilket kan vara effektivt och nå rätt målgrupp. |
| **[!UICONTROL CTR]** | Procentandel (%) av användarna som klickade på en annons, ett sökresultat eller länkar i ett e-postmeddelande.<br>**Beräkning**: `clicks` delat med `impressions` | En hög klickfrekvens visar att innehållet är mycket relevant och motiverat för målgruppen i budskapen och designen och att det effektivt riktar sig till målgruppens intressen. |
| **[!UICONTROL CPM]** | Resultatmätning för kostnad ($) per tusen annonsvisningar.<br>**Beräkning**: totalt belopp `spent` dividerat med räckvidd, multiplicerat med 1000 | Ett lågt värde kan indikera kostnadseffektiv synlighet, särskilt om det kombineras med en hög klickfrekvens. |
| **[!UICONTROL CPC]** | Genomsnittskostnad ($) som associeras med varje klick i en upplevelse.<br>**Beräkning**: totalt belopp `spent` delat med `clicks` | Lägre genomsnittliga kostnader kan tyda på kostnadseffektiva annonskostnader, särskilt om man jämför med en ökning av antalet konverteringar. |
| **[!UICONTROL Video plays]** | Procentandel av tittarna som tittade på en video till slutet. | Ett stort antal videouppspelningar kan tyda på att videon fångar uppmärksamheten och kan betyda att miniatyren, titeln eller placeringen ritas effektivt i visningsprogrammen. Höga uppspelningshastigheter tyder på att videomaterialet är övertygande och relevant. |
| **[!UICONTROL Budget]** | Totala medel ($) som anslagits för en annonskampanj för att uppnå kampanjmålen. | En hög budget innebär mer resurser för en bredare räckvidd och potentiellt större påverkan. |
| **[!UICONTROL Spend]** | Det belopp som har använts från budgeten under en viss tidsperiod. | Ett högt utgiftsbelopp under en kort period kan tyda på snabb användning, vilket kan leda till att resurser tar slut i förtid. Spåra utgiftsbeloppet mot nyckeltal för att övervaka den totala avkastningen på investeringen. |