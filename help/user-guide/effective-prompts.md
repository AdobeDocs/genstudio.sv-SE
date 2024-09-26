---
title: Skriv effektiva uppmaningar
description: Lär dig hur du skriver effektiva uppmaningar om Adobe GenStudio för Performance Marketers.
feature: Prompt, Generative AI, Brands Service, Personas Service, Products Service, Guidelines
exl-id: 0cd4db4f-d031-4c1f-a4e7-adc220f947fc
source-git-commit: 016cd2b5415651ed3cf157244f868315234330fa
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Skriv effektiva uppmaningar

Att kommunicera med den generativa AI-miljön är nödvändigt för att man ska kunna arbeta effektivt i Adobe GenStudio för Performance Marketers.

GenStudio for Performance Marketers ger en generativ AI-fråga varje gång det finns möjlighet att ändra en resurs. Komponenterna i en effektiv prompt ska innehålla beskrivande språk, exempel och information som inte tillhandahålls via dina konfigurerade riktlinjer.

Som en god praxis är det att förse GenStudio for Performance Marketers med din varumärkesinformation med [riktlinjer](/help/user-guide/guidelines/overview.md), så kan du utnyttja den generativa AI:n fullt ut för att skapa varumärkesanpassade innehållsupplevelser.

## Beskrivning

Ni kan använda naturligt språk för att uttrycka era idéer och skapa upplevelser. Din uppmaning leder AI till att skapa kanalinnehåll som är personaliserat och bilder som kompletterar din vision. Ju mer detaljerad information du ger, desto större chans att skapa en bild eller en upplevelse som uppfyller dina behov. Använd ett tydligt och beskrivande språk för att ge så detaljerad information som möjligt:

- Använd ord som beskriver atmosfär, humör, färg, komposition och stil för **bilder**.
- Använd ord som beskriver målgrupp, syfte, beskrivningar av nya funktioner, exempel och åtgärder för **copy**.

Här följer ett exempel på en uppmaning som ger information om din avsikt, målgrupp och stil.

```bash
Write an email to motivate infrequent users of Photoshop to follow an in-app tutorial that teaches them to combine elements of two photos into a beautiful work of art. Highlight the generative AI capabilities of Photoshop and use references to natural imagery.
```

+++Se exempelresultat

![tre genererade e-postmeddelanden](/help/assets/sample-email.png)

+++

## Frågevillkor

I GenStudio for Performance Marketers [[!DNL Create]](/help/user-guide/create/overview.md) kan du använda **[!UICONTROL Prompt criteria]** ([_Parametrar_](/help/user-guide/create/overview.md#parameters) och en uppmaning) i promptområdet för att lägga till information genom markering för att förbättra AI-tolkningen.

Frågevillkoren för [e-post](/help/tutorials/create-email-experience.md) kan omfatta tillägg av [riktlinjer](/help/user-guide/guidelines/overview.md) i _parametrar_, överföring av en resurs som ska användas i e-postvarianterna samt en beskrivande uppmaning. För en [metaannons](/help/tutorials/create-meta-ad.md) kan frågevillkoren innehålla en varumärkesriktlinje i _Parametrar_, val eller överföring av en befintlig resurs, inställningar för bilder eller resurser som proportioner samt en fråga. Den verkliga kraften börjar med [att konfigurera riktlinjer](/help/user-guide/guidelines/add-guidelines.md).

>[!NOTE]
>
>Om riktlinjer läggs till i _Parametrar_ i promptområdet behöver du inte inkludera referenser till dem i prompten. GenStudio för Performance Marketers utnyttjar dessa [!DNL Brands], [!DNL Products] och [!DNL Personas] i innehållsgenereringen.

### Riktlinjer

Riktlinjerna för GenStudio for Performance Marketers hjälper den generativa AI att personalisera din resurskomposition. När du får ett frågevillkor kan du välja en [[!DNL Brand]](/help/user-guide/guidelines/brands.md), en [[!DNL Persona]](/help/user-guide/guidelines/personas.md) och en [[!DNL Product]](/help/user-guide/guidelines/products.md) bland dina konfigurerade riktlinjer.

>[!TIP]
>
>Du styr hur och när GenStudio for Performance Marketers använder dina [!DNL Brand]-riktlinjer. Se [Riktlinjer](/help/user-guide/guidelines/overview.md) om du vill veta mer om hur du konfigurerar och hanterar riktlinjer för varumärken.

### Strukturerade uppmaningar

För e-postmeddelanden med flera avsnitt kan du strukturera uppmaningar om att tillhandahålla avsnittsspecifika instruktioner för att generera varierande innehåll för varje avsnitt i ett e-postmeddelande. Strukturerade uppmaningar ska direkt referera till [avsnittsnamn i e-postmallen](/help/user-guide/content/email-template.md#multi-section-emails) så att det genererade innehållet kan infogas i motsvarande innehållsplatshållare.

Du kan till exempel instruera GenStudio for Performance Marketing att generera innehåll som marknadsför en ny produkt i det första avsnittet i ett e-postmeddelande och generera innehåll som detaljerar de kostnadsbesparande fördelarna med produkten i det andra e-postavsnittet.

Den strukturerade uppmaningen ska:

- Använd någon av följande referenser till avsnittsnamnet i e-postmallen:
   - Pod
   - Grupp
   - Avsnitt
   - Modul

  Om mallen till exempel använder `moduleA` eller `Group-3` som avsnittsnamn kan du referera till avsnittsnamnen i uppmaningen.

- Följ de rekommenderade reglerna/strukturen. Om promptstrukturen inte följer det angivna formatet gäller uppmaningen för *alla* e-postavsnitt och ändå underlättar det att generera innehåll.
- Använd avsnittsnamn som [definierat i din e-postmall](/help/user-guide/content/email-template.md#code-an-email-template). Frågereferenser måste matcha avsnittsnamnen som kodats i din e-postmall.
- Var inte skiftlägeskänslig. Du kan till exempel använda `Pod` eller `pod` i din e-postmall och strukturerade fråga.
- Referera till den generiska användarprompten först och sedan de avsnittsspecifika direktiven.
- Använd kolon, bindestreck, kommatecken eller annan avgränsning (`,:;#$!~|@=-%&*^_`) som en separation mellan avsnittsnamnreferensen och -direktivet. Du kan till exempel använda följande som ett avsnittsspecifikt promptdirektiv: `Pod1; Describe how to easily edit text and swap images.`

Följande är ett exempel på en fråga som redogör för den rekommenderade promptstrukturen och använder en e-postmall som använder den identifierande termen `Pod` som i `Pod1`, `Pod2` och `Pod3`.

```properties
Create an exciting multi-pod email focusing on Creative Cloud and its powerful generative AI capabilities.

Encourage customers to convert to Photoshop or use a free Photoshop trial. We want to better educate them about app features.

Pod1: Focus on Adobe Photoshop and its new generative AI tools that enable creators to bring images to life in minutes.

Pod2: Focus on Adobe Illustrator and its new generative AI tools, such as Generative Shape Fill, which allows you to quickly fill your vector outline and explore a variety of options that match the look and feel of your own artwork.

Pod3: Focus on Adobe Acrobat Pro. Make users aware that with Acrobat Pro they can edit images and text inside a PDF.
```

Se [Förbered en e-postmall](/help/user-guide/content/email-template.md#code-an-email-template).

## Försök igen

Att fråga är en iterativ process. Om resultaten inte uppfyller dina förväntningar kan du granska frågan och göra några ändringar eller lägga till mer information. Du kan även klistra in avsnitt från en kampanjrapport. Du kan till och med begära att GenStudio for Performance Marketers undviker vissa ord, element eller teman.

## God praxis

Några enkla metodtips för att skapa effektiva uppmaningar:

- Var tydlig och ange vad du ska göra och inte göra.
- Ange kontext med hjälp av externa referenser.
- Utnyttja riktlinjerna för GenStudio för Performance Marketers.
- Granska och justera riktlinjerna regelbundet.
- Iterera och förfina.
- Lär dig genom experiment.
