---
title: Versionsinformation för Adobe GenStudio for Performance Marketing Beta
description: Läs om de senaste funktionerna och förbättringarna i Adobe GenStudio for Performance Marketing.
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: c95a99d4fa8030a35b7fe3690235102e1827422f
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# Versionsinformation för Adobe GenStudio for Performance Marketing Beta

Dessa kommentarer belyser viktiga Adobe GenStudio for Performance Marketing-korrigeringar och förbättringar för den vecka som slutar den 27 september.

## Nya funktioner och förbättringar

* GenStudio kan nu extrahera persona och produktinformation från ett överfört PDF och fylla i relaterade fält. <!-- GS-3806 -->

* Användare kan nu filtrera [!DNL Content] resurser och upplevelser efter namnet på den användare som överförde resursen. <!-- GS-1808 -->

* Inloggningsflödet för metadata innehåller nu en **[!UICONTROL Refresh]**-knapp som gör att användare kan ta bort blockering av popup-fönster under inloggning.

* Avsnittet [!DNL Additional details] togs bort från detaljsidan för [!DNL Persona]. <!-- GS-5133 5134 -->

* Namnet på avsnittet [!DNL Additional details] ändrades till [!DNL Messaging preferences] på detaljsidan för [!DNL Products]. <!-- GS-5133 5134 -->

* En [!DNL Add persona]-knapp har lagts till på sidan _Lägg till din första profil_. <!-- GS-5132 -->

## Kända fel

Följande kända fel är schemalagda för lösning i GenStudio for Performance Marketing GA-versionen.

* Mallar kan överföras men inte visas. **Tillfällig lösning**: Överför en resurs med fältet **[!UICONTROL Campaigns]** ifyllt. Ladda sedan upp mallen igen. <!-- GS-4815 5650-->

* Användare kan inte beskära Meta-annonser manuellt efter att de har ändrat storlek. <!-- GS-5871 -->

* Användare kan skapa en ny [!DNL Campaign] från [!DNL Content]-arbetsflöden. <!-- GS-5650 -->

* Användare måste logga in två gånger till ett Meta-annonskonto i en kanal när de också är inloggade på Facebook. Tillfällig lösning: Logga ut från Facebook innan du loggar in på ett kanalkonto för Meta-annonser. <!-- GS-3009 -->

### Ytterligare förbättringar och åtgärdade problem

* Problem med återkommande latens för vissa [!DNL Create] arbetsyteåtgärder har lösts. <!-- GS-5203 -->

* Användare behöver inte längre logga in två gånger på ett Meta-annonskonto i en kanal när de också är inloggade på Facebook. <!-- GS-4806 -->

* E-postgenereringen resulterar nu längre i ett ofullständigt e-postmeddelande. <!-- GS-5209 -->

* När du skapar en kampanj i mallarbetsflödet sparas nu ID:n som förväntat.  <!-- GS-4923 -->

* Väljaren för flera databaser visar nu databaser i alfabetisk ordning. <!-- GS-5553 -->

* Problem med CSV-exportfilformat för icke-engelska språk har åtgärdats. <!-- GS-5141 -->

* Användare kan nu klicka på knappen [!DNL Create] _Senaste arbete_ **[!UICONTROL View all drafts]** när utkast läses in. Om du tidigare klickade på den här knappen innan alla utkast hade lästs in, lästes bara ett fåtal utkast in och knappen **[!UICONTROL View all drafts]** blev inte tillgänglig. <!-- GS-3938 -->

* På arbetsytan i [!DNL Create] visas nu knappen **[!UICONTROL View all drafts]** som förväntat när mer än fyra utkast visas på arbetsytan. <!-- GS-5588 -->

* Sökfunktionen fungerar nu som förväntat på fliken _Attribut_. <!-- GS-5658 -->

* Skalanimeringen skalas nu korrekt när upplevelsen läses in. <!-- GS-5574 -->

* Miniatyrförhandsvisningar av e-postmeddelanden med flera delar återges nu som förväntat i [!DNL Content]. <!-- GS-5258 -->

* Ett Workfront-relaterat problem med knappen **[!UICONTROL Send for approval]** har korrigerats. <!-- GS-5847 -->

* Problem med inläsning av Shimmer i vyn [!DNL Create] Senaste arbete har korrigerats. <!-- GS-5589 -->

* Om du anger en sökterm får du nu bara ett sökanrop som förväntat.  <!-- GS-2999 -->

* Korrigerad bildåtergivning av Meta-annonsbilder efter export. <!-- GS-5749 -->

* Symbolen `%` återges nu korrekt i DEU-, FRA- och ESP-språkversioner när användare zoomar in eller zoomar ut från e-postvarianter på C[!DNL Create] Canvas. <!-- GS-5007 -->


#### Lokalisering

Den här versionen innehåller förbättringar av lokaliseringen i hela produktgränssnittet, särskilt i hela [!DNL Create]. Följande gränssnittskomponenter har lokaliserats: <!-- GS-5295 -->

* Alla strängar i området _Fråga_ (parametertitel, alternativnamn i listrutan och platshållartext) <!-- GS-5027 -->

* Alla strängar i fönstret _Ändra storlek_ för genererade Meta-annonser i [!DNL Create] <!-- GS-5035 -->

* Alla strängar i området _Senaste arbete_ i [!DNL Create] <!-- GS-5037 -->

* Alternativsträngarna Varumärke, Personas och Produkt i listrutan i området Fråga <!-- GS-5293 -->

* Strängen **Zooma för att passa skärmen** som visas under generering av e-post och metaannonser <!-- GS-5063 -->

* Datum- och tidsformat, strängen **Namnlöst utkast** och felmeddelanden i e-post- och metaannonsnamn <!-- GS-5023 5022 5048-->

* Flikgalleriet [!DNL Content] _Assets_ visar strängar och procentsymbol (%) <!-- GS-4983 4984-->

* Procentsymbolen (%) som används i Insights > Experiences klickfrekvens <!-- GS-4279 -->

* Ett felmeddelande visas när ett systemfel inträffar när e-post eller Meta ads skapas <!-- GS-5061 -->

* Decimalavgränsare för frasen &quot;Antal ord per mening&quot; på informationssidan för Insights Experience <!-- GS-4986 -->

* Strängar på menyn Exportera för en Meta-annons som skapats med en mall. <!-- GS-5031 -->

