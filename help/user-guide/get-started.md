---
title: Kom igång med Adobe GenStudio för Performance Marketers
description: Lär dig hur du konfigurerar din GenStudio for Performance Marketers för att generera nytt varumärkesanpassat marknadsföringsmaterial.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
exl-id: bcb03198-bbcb-45ae-af01-25c1e834b563
source-git-commit: dab19da0063d6f4f4497112c4063bfc9c285e651
workflow-type: tm+mt
source-wordcount: '1106'
ht-degree: 0%

---

# Kom igång med Adobe GenStudio för Performance Marketers

GenStudio for Performance Marketers är en heltäckande plattform för att skapa, utvärdera och hantera marknadsföringsupplevelser som speglar och följer varumärkesidentiteten.

Intressentåtkomsten till dess många funktioner styrs av tilldelade _användarroller_. Din tilldelade användarroll avgör vilka uppgifter du kan utföra i GenStudio för Performance Marketers. En Adobe-systemadministratör tilldelar dina behörigheter i GenStudio för Performance Marketers-produktprofilen i Adobe Admin Console. Ditt välkomstmeddelande identifierar din tilldelade roll.

Om du är nybörjare på att skapa AI-baserade verktyg eller bara är nyfiken på GenStudio för Performance Marketers grundprinciper kan du läsa [Koncept](concepts.md) och [Skriv effektiva uppmaningar](effective-prompts.md).

## Användarroller

Att skapa och driftsätta moderna marknadsföringskampanjer kräver samarbete mellan intressenter med varierande ansvarsområden och kompetenser.

Tre typer av GenStudio för Performance Marketers-användarroller har stöd för denna mångfald av organisationsroller. Behörigheterna är skräddarsydda för var och en av dessa användartyper och stöder varje användares ansvar i marknadsföringsorganisationen.

**De tre användarrolltyperna är**:

* **Redigerare** använder GenStudio för Performance Marketers generativa AI-funktioner för att skapa marknadsföringskampanjresurser, begära granskning och godkännande av innehåll och publicera godkända utkast av det här innehållet. Alla GenStudio-användare kan komma åt och använda en resurs när den som skapat den har sparat den i Innehåll.

* **Medarbetare** är det bredaste urvalet av GenStudio för Performance Marketers-användare. Medarbetare kan visa och godkänna innehåll och är en viktig del av arbetsflödet som säkerställer att det innehåll du genererar matchar organisationens behov och standarder.

* **Systemhanterare** har den bredaste behörighetsuppsättningen inom GenStudio för Performance Marketers. Systemansvariga utför den grundläggande startuppgiften att skapa skyddsutkast för att skapa och driftsätta kampanjresurser. Systemansvariga implementerar skyddsprofilerna genom att överföra varumärkes- och organisationsspecifik information, till exempel [varumärkesriktlinjer](/help/user-guide/guidelines/overview.md). GenStudio systemansvariga har behörighet att skapa och publicera varumärken, men saknar administratörsbehörighet.

>[!NOTE]
>Innan några användare etableras i de här rollerna måste en Adobe-systemadministratör utses i Adobe Admin Console för att kunna utföra engångsinstallationsuppgifter. Administratörsrollen för Adobe fungerar endast i Adobe Admin Console. Den har ingen roll i GenStudio för Performance Marketers plattformsgränssnitt.

### GenStudio Editors

**Redigerare** har de behörigheter som krävs för att skapa GenStudio för Performance Marketers [!DNL Brands]-, [!DNL Campaigns]- och [!DNL Content]-resurser. De kan också redigera och ta bort resurser som de har skapat. GenStudio for Performance Marketers har stöd för att snabbt skapa hundratals innehållsdelar. Dessa användare kan generera innehållsavsnitt eller hela upplevelser som orkestrerar separata delar av godkänt innehåll för att uppfylla kraven för specifika marknadsföringskampanjer.

Redigerare interagerar med GenStudio för Performance Marketers generativa AI-tekniker genom att _fråga_. I promptområdet på arbetsytan finns verktyg som du kan använda för att ställa frågor i samband med en viss kampanjs riktlinjer. Därför beror kvaliteten och framgången för det genererade innehållet delvis på kvaliteten på de varumärkesriktlinjer som organisationen har överfört och på hur specifik uppmaningen är.

Se [Skriv aktuella uppmaningar](effective-prompts.md).

I följande tabell visas standardredigerarens behörigheter:

| Funktion | Skapa | Uppdatera | Ta bort | Visa |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | no | no | no | ja |
| [!DNL Campaigns] | ja | ja | ja | ja |
| [!DNL Content] | ja | ja | ja | ja |
| [!DNL Insights] | kan bara konfigurera annonsanslutningar |    |     | ja |
| [!DNL Personas] | ja | ja | ja | ja |
| [!DNL Products] | ja | ja | ja | ja |
| [!DNL Reviews and approvals] | ja | ja | ja | ja |

### GenStudio medarbetare

**Medarbetare** kan visa resurser i GenStudio för Performance Marketers men inte skapa, redigera eller ta bort dessa resurser. Medarbetarna arbetar bland annat med intressenter som är viktiga för att gransknings- och godkännandeprocessen ska lyckas, men som inte behöver skapa eller redigera innehåll direkt. Juridiska experter och chefer för kreatörer är exempel på potentiella medarbetare. Medarbetare på GenStudio för Performance Marketers kan ha behörighet att skapa och visa resurser i andra Creative Cloud-produkter.

I följande tabell visas standardbehörigheter för medarbetare:

| Funktion | Skapa | Uppdatera | Ta bort | Visa |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | no | no | no | ja |
| [!DNL Campaigns] | no | no | no | ja |
| [!DNL Content] | no | no | no | ja |
| [!DNL Insights] | no | no | no | ja |
| [!DNL Personas] | no | no | no | ja |
| [!DNL Products] | no | no | no | ja |
| [!DNL Reviews and approvals] | no | no | no | ja |

### GenStudio systemansvariga

**GenStudio systemhanterare** har slutfört de initiala åtgärder som förbereder din organisation för att distribuera GenStudio för Performance Marketers.

I följande tabell visas standardbehörigheterna för GenStudio systemhanterare:

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

GenStudio systemansvariga förbereder sin organisations GenStudio for Performance Marketers-miljö för att redaktörer och medarbetare ska kunna skapa kampanjresurser. Dessa preliminära installationsuppgifter omfattar:

1. [Lägg till riktlinjer](./guidelines/overview.md) för [!DNL Brands], [!DNL Products] och [!DNL Personas]. Att bygga upp de viktigaste byggstenarna i organisationens varumärkesidentitet är en nödvändig förutsättning för det arbete som utförs av kreatörer och medarbetare. Du kan antingen överföra varumärkesriktlinjer eller ange varumärkesinformation manuellt.
   * **Förbered dina riktlinjer**. Ju mer beskrivande och omfattande varumärkesriktlinjerna är, desto bättre blir resultatet. Ta med korta exempel på funktioner som du anser vara viktiga för ert varumärke och lägg till beskrivningar av beteenden som du vill utesluta från att skapa innehåll. GenStudio for Performance Marketers extraherar information från dessa överförda dokument och börjar bygga upp ert varumärke. Information som varumärkesröst, kanal och riktlinjer för bilder fylls i när GenStudio for Performance Marketers sätter ihop varje riktlinje från dina överförda dokument.
   * **Redigera eller komplettera varumärkesstödfält efter behov**. Omfattande varumärkesriktlinjer utgör grunden för GenStudio när det gäller Performance Marketers förståelse för er organisations varumärke. När GenStudio for Performance Marketers har extraherat den information som behövs från varumärkesriktlinjerna uppmanas du att redigera eller fylla i fält med extraherad information manuellt. Ange enskilda produktfokusområden för innehållsskapande genom att lägga till en [!DNL Product]. [!DNL Personas]-riktlinjer hjälper dig att skräddarsy innehållsskapande för definierade kundsegment.

   Även om det kan vara en engångsåtgärd att upprätta en organisations varumärkesriktlinjer kan du behöva revidera och förbättra dessa riktlinjer baserat på din organisations volatilitet, tillväxt och förändrade marknadsförhållanden.

1. **[Överför mallar](./content/use-templates.md)**. Mallar ger genvägar och gör att det går snabbare att skapa innehåll. En mall innehåller godkända funktioner, t.ex. sidhuvuden och sidfötter, och skyddsutkast för att skapa innehåll. Systemansvariga överför och hanterar vanligtvis mallar för sin organisation. Skaparna använder mallar för att snabbt komma igång med processen att skapa innehåll inom de gränser som fastställts av organisationens varumärke.

1. **[Överför godkända resurser](./content/manage-assets.md)**. Godkända resurser i [!DNL Content] är tillgängliga för alla som skapar Performance Marketers i GenStudio. Du kan skapa nya upplevelser eller resurser för [!DNL Content] med resurser som skapare kan använda.

1. **[Anslut till ett Meta-konto (Facebook)](./insights/connect-channel.md)**. Konfigurera en anslutning mellan GenStudio för Performance Marketers och organisationens sociala konton för att ta emot data från era aktiva marknadsföringskampanjer, resurser och upplevelser. [[!DNL Insights]](./insights/overview.md) innehåller verktyg för att analysera kanalhärledda data.
