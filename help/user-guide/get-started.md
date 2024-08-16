---
title: Kom igång med Adobe GenStudio för Performance Marketers
description: Lär dig hur du konfigurerar din GenStudio for Performance Marketers för att generera nytt varumärkesanpassat marknadsföringsmaterial.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
source-git-commit: c9d09801f0bd3732611b01d4a98cc7ebf38884d7
workflow-type: tm+mt
source-wordcount: '1117'
ht-degree: 0%

---


# Kom igång med Adobe GenStudio för Performance Marketers

GenStudio for Performance Marketers är en heltäckande plattform för att skapa, utvärdera och hantera marknadsföringsupplevelser som speglar och följer varumärkesidentiteten.

Intressenternas åtkomst till deras många funktioner styrs av tilldelade användarroller. Din tilldelade användarroll avgör vilka uppgifter du kan utföra i GenStudio för Performance Marketers. En administratör anger dina behörigheter, som definieras i ditt välkomstmeddelande.

Om du är nybörjare på att skapa AI-baserade verktyg eller bara är nyfiken på GenStudio för prestandamarknadsförarnas grundprinciper kan du läsa [Koncept](concepts.md) och [Skriv effektiva uppmaningar](effective-prompts.md).

## Användarroller

Att skapa och driftsätta moderna marknadsföringskampanjer kräver samarbete mellan intressenter med varierande ansvarsområden och kompetenser.

Tre typer av GenStudio för Performance Marketers-användarroller har stöd för denna mångfald av organisationsroller. Behörigheterna är skräddarsydda för var och en av dessa användartyper och stöder varje användares ansvar i marknadsföringsorganisationen.

**De tre användarrolltyperna är**:

* **Skapare** använder GenStudio för Performance Marketers generativa AI-funktioner för att skapa marknadsföringskampanjresurser, begära granskning och godkännande av innehåll och publicera godkända utkast av det här innehållet. Alla GensStudio-användare kan komma åt och använda en mediefil när den som skapat den har sparat den i Innehåll.

* **Medarbetare** är det bredaste urvalet av GenStudio för Performance Marketers-användare. Medarbetare kan visa och godkänna innehåll och är en viktig del av arbetsflödet som säkerställer att det innehåll ni skapar matchar organisationens behov och standarder.

* **Systemadministratörer** har den bredaste behörighetsuppsättningen inom GenStudio för Performance Marketers. Systemadministratörer kan lägga till och ta bort användare och innehåll. Administratörer utför den grundläggande introduktionsuppgiften att skapa grundläggande skyddsutkast för att skapa och distribuera kampanjresurser. Administratörer implementerar skyddsprofilerna genom att överföra varumärkes- och organisationsspecifik information, till exempel [varumärkesriktlinjer](/help/user-guide/guidelines/overview.md).

>[!NOTE]
>Innan några användare etableras i de här rollerna måste en administratör utses till superanvändare i Admin Console i Adobe för att kunna utföra engångsinstallationsåtgärder. Den här superanvändarrollen fungerar bara i Adobe Admin Console. Den har ingen roll i GenStudio för Performance Marketers plattformsgränssnitt. Det finns inget koncept för superanvändare i GenStudio för rolltilldelningar för Performance Marketers.

### Skapare

**Skapare** har de behörigheter som krävs för att skapa GenStudio för Performance Marketers [!DNL Brands]-, [!DNL Campaigns]- och [!DNL Content]-resurser. De kan också redigera och ta bort resurser som de har skapat. GenStudio for Performance Marketers har stöd för att snabbt skapa hundratals innehållsdelar. Dessa användare kan generera innehållsfragment eller hela upplevelser som orkestrerar separata delar av godkänt innehåll för specifika marknadsföringskampanjer.

Skaparna interagerar med GenStudio för Performance Marketers generativa AI-tekniker genom att _fråga_. I promptområdet på arbetsytan finns verktyg som du kan använda för att ställa frågor i samband med en viss kampanjs riktlinjer. Därför beror kvaliteten och framgången för det genererade innehållet delvis på kvaliteten på de varumärkesriktlinjer som organisationen har överfört och på hur specifik uppmaningen är.

Se [Skriv aktuella uppmaningar](effective-prompts.md).

I följande tabell visas standardbehörigheterna för att skapa:

| Funktion | Skapa | Uppdatera | Ta bort | Visa |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | no | no | no | ja |
| [!DNL Campaigns] | ja | ja | ja | ja |
| [!DNL Content] | ja | ja | ja | ja |
| [!DNL Insights] | kan bara konfigurera annonsanslutningar |    |     | ja |
| [!DNL Personas] | ja | ja | ja | ja |
| [!DNL Products] | ja | ja | ja | ja |
| [!DNL Reviews and approvals] | ja | ja | ja | ja |

### Medarbetare

**Medarbetare** kan visa resurser i GenStudio för Performance Marketers men inte skapa, redigera eller ta bort dessa resurser. Medarbetarna arbetar bland annat med intressenter som är viktiga för att gransknings- och godkännandeprocessen ska lyckas, men som inte behöver skapa eller redigera innehåll direkt. Juridiska experter och chefer för kreatörer är exempel på potentiella medarbetare. Medarbetare på GenStudio för Performance Marketers kan ha behörighet att skapa och visa resurser i andra Creative Cloud-produkter.

I följande tabell visas standardbehörigheter för medarbetare:

| Funktion | Skapa | Uppdatera | Ta bort | Visa |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | ja | ja | ja | ja |
| [!DNL Campaigns] | ja | ja | ja | ja |
| [!DNL Content] | ja | ja | ja | ja |
| [!DNL Insights] | no | no | no | ja |
| [!DNL Personas] | ja | ja | ja | ja |
| [!DNL Products] | ja | ja | ja | ja |
| [!DNL Reviews and approvals] | no | no | no | ja |

### Administratörer

**Administratörer** skapar och tilldelar användare till någon av de roller som stöds av GenStudio för Performance Marketers. De kan tilldela enskilda skapare eller medarbetare nya behörigheter efter behov. Deras viktigaste uppgift är att slutföra de inledande introduktionsuppgifterna som förbereder organisationen för att driftsätta GenStudio för Performance Marketers.

I följande tabell visas standardbehörigheterna för systemadministratörer:

| Funktion | Skapa | Uppdatera | Ta bort | Visa |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | ja | ja | ja | ja |
| [!DNL Campaigns] | ja | ja | ja | ja |
| [!DNL Content] | ja | ja | ja | ja |
| [!DNL Insights] | ja | ja | ja | ja |
| [!DNL Personas] | ja | ja | ja | ja |
| [!DNL Products] | ja | ja | ja | ja |
| [!DNL Reviews and approvals] | ja | ja | ja | ja |


## Förbered GenStudio för Performance Marketers för att generera innehåll

Systemadministratörer förbereder organisationens GenStudio för Performance Marketers-miljö så att skapare och medarbetare kan skapa kampanjresurser. Dessa preliminära installationsuppgifter omfattar:

1. [Lägg till riktlinjer](./guidelines/overview.md) för [!DNL Brands], [!DNL Products] och [!DNL Personas]. Att bygga upp de viktigaste byggstenarna i organisationens varumärkesidentitet är en nödvändig förutsättning för det arbete som utförs av kreatörer och medarbetare. Du kan antingen överföra varumärkesriktlinjer eller ange varumärkesinformation manuellt.
   * **Förbered dina riktlinjer**. Ju mer beskrivande och omfattande varumärkesriktlinjerna är, desto bättre blir resultatet. Ta med korta exempel på funktioner som du anser vara viktiga för ert varumärke och lägg till beskrivningar av beteenden som du vill utesluta när du skapar innehåll. GenStudio for Performance Marketers extraherar information från dessa överförda dokument och börjar bygga upp ert varumärke. Information som varumärkesröst, kanal och riktlinjer för bilder fylls i när GenStudio for Performance Marketers sätter ihop varje riktlinje från dina överförda dokument.
   * **Redigera eller komplettera varumärkesstödfält efter behov**. Omfattande varumärkesriktlinjer utgör grunden för GenStudio när det gäller Performance Marketers förståelse för er organisations varumärke. När GenStudio for Performance Marketers har extraherat den information som behövs från varumärkesriktlinjerna uppmanas du att redigera eller fylla i fält med extraherad information manuellt. Ange enskilda produktfokusområden för innehållsskapande genom att lägga till en [!DNL Product]. [!DNL Personas]-riktlinjer hjälper dig att skräddarsy innehållsskapande för definierade kundsegment.

   Även om det kan vara en engångsåtgärd att upprätta en organisations varumärkesriktlinjer kan du behöva revidera och förbättra dessa riktlinjer baserat på din organisations volatilitet, tillväxt och förändrade marknadsförhållanden.

1. **[Överför mallar](./content/use-templates.md)**. Mallar ger genvägar och gör att det går snabbare att skapa innehåll. En mall innehåller godkända funktioner, t.ex. sidhuvuden och sidfötter, och skyddsutkast för att skapa innehåll. Administratörer överför och hanterar vanligtvis mallar för sin organisation. Skaparna använder mallar för att snabbt komma igång med att skapa innehåll inom de etablerade gränserna för ett visst varumärke.

1. **[Överför godkända resurser](./content/manage-assets.md)**. Godkända resurser i [!DNL Content] är tillgängliga för alla som skapar Performance Marketers i GenStudio. Du kan skapa nya upplevelser eller resurser för [!DNL Content] med resurser som skapare kan använda.

1. **[Anslut till ett Meta-konto (Facebook)](./insights/connect-channel.md)**. Du måste konfigurera en anslutning mellan GenStudio för Performance Marketers och organisationens sociala konton för att kunna ta emot data från era aktiva marknadsföringskampanjer, resurser och upplevelser. [[!DNL Insights]](./insights/overview.md) innehåller verktyg för att analysera kanalhärledda data.
