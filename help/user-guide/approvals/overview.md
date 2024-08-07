---
title: GenStudio granskningar och godkännanden
description: Läs mer om GenStudio granskning och godkännande.
feature: Approval
source-git-commit: c9bd8bf434e493696e674900f403307260a65b02
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---


# GenStudio granskningar och godkännanden

GenStudio arbetsflöde för granskning och godkännande säkerställer att alla intressenter - från kreativa team till juridiska experter - effektivt kan granska och godkänna kampanjkomponenter, inklusive generativa AI-producerade varumärkesresurser.

## [!DNL Review and Approval] fördelar med arbetsflödet

* **Stöd för robust, iterativt generativt AI-innehåll**. Att skapa och distribuera varumärkesanpassat innehåll i en organisation är en mycket iterativ process. GenStudio generativa AI-funktioner gör det enkelt att snabbt skapa hundratals tillgångsvarianter. Varje granskare kan begära flera ändringar av ett tillgångsutkast innan han eller hon godkänner det. Ju fler granskare, desto fler möjliga iterationer innan alla intressenter kommer överens om en slutgiltig variant.

* **Stöd för kreativ integritet**. Godkännanden skyddar ert varumärkes kreativa integritet genom att de som skapar materialet deltar i godkännandeprocessen. Genom att involvera kreativa intressenter (till exempel innehållsskapare och creative directors) i gransknings- och godkännandeprocessen ser du till att slutresultatet överensstämmer med din vision och varumärkesidentitet.

* **Följer Campaign-målen och de juridiska kraven**. Godkännandeprocessen hjälper till att verifiera att innehållet stöder kampanjmål. Det säkerställer att innehållet uppfyller kraven på juridisk autenticitet, vilket minimerar riskerna och potentiella juridiska problem.

## Livscykel för granskning och godkännande

De huvudsakliga faserna i arbetsflödet för granskning och godkännande omfattar:

[Begär granskning och godkännande av innehåll du skapat](./request-review.md)

[Granska och redigera innehåll](./review-and-edit.md)

[Godkänn innehåll](./approve-content.md)

[Publish content](./publish-content.md)

## Vem kan begära en granskning eller godkänna innehåll?

Om du har skapat en resurs eller upplevelse kan du be andra i din organisations godkännandekedja att formellt granska och kommentera ditt arbete. Endast de utsedda godkännarna kan granska utkastet.

## Om [!DNL Content] utkast

_Utkast_ är preliminära versioner av resurser eller upplevelser som inte har genomgått gransknings- och godkännandeprocessen. Utkaststatus identifierar var utkastet befinner sig i gransknings- och godkännandeprocessen. Ett unikt utkast-ID identifierar varje utkast. Det här ID:t är giltigt tills ett utkast har godkänts och publicerats till [!DNL Content]. Granskningskommentarer och godkännanden för ett utkast är kopplade till detta enskilda utkast-ID.

När ett utkast slutför gransknings- och godkännandeprocessen och publiceras till [!DNL Content], förfaller utkast-ID:t och GenStudio sparar inte associerade kommentarer och godkännandestatus. Utkast-URL:en är inte längre giltig.

Utkaststatus fångar statusen för innehållsutkastet när det går igenom gransknings- och godkännandeprocessen. Alla utsedda granskare meddelas om förändringar i status för det innehåll de granskar. Granskarna ändrar utkaststatus för att ange om ett utkast behöver ändras ytterligare eller kan godkännas. Alla utsedda godkännare måste godkänna en mediefil eller upplevelse innan den kan publiceras.

Tillgängliga statusvärden för utkast:

**Meddelande**: Den som skapat innehållet har startat granskningsprocessen genom att meddela granskarna att ett utkast är klart för granskning.
**Behöver arbete**: Anger att en eller flera granskare har begärt ändringar av innehållsutkastet. Innehåll med den här statusen kan inte sparas till [!DNL Content].
**Godkänd**: Alla utsedda godkännare har godkänt resursen eller upplevelsen. Innehållsskaparen kan nu lägga till metadata till resursen eller upplevelsen och spara den i [!DNL Content].

## Meddelanden

GenStudio produktmeddelanden uppdaterar godkännare och innehållsskapare i realtid om resursstatusändringar och granskar kommentarerna. Aviseringar ger snabb redigering genom flera gransknings-, redigerings- och godkännandecykler.

Åtgärder som vidtas av godkännandedeltagare utlöser automatiska meddelanden i produkten och e-postmeddelanden. När du startar en godkännandeprocess får utsedda godkännare meddelanden både via e-post och i produkten. Du hålls kvar med meddelanden i produkten varje gång en godkännare lägger till kommentarer eller godkänner. Meddelanden innehåller länkar till innehållsutkastet.

Om du initierade gransknings- och godkännandeprocessen för innehåll meddelas du om alla godkännanden och granskningskommentarer. Godkännare meddelas dock endast om kommentarer som innehåller dem med en `@mention`.
