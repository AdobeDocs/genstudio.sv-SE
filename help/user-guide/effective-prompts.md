---
title: Skriv effektiva uppmaningar
description: Lär dig skriva effektiva uppmaningar för GenStudio.
feature: Prompt, Generative AI, Brands Service, Personas Service, Products Service, Guidelines
source-git-commit: d7de679ce310dcdcec4a1b5ea814b2ca8b1fc413
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---


# Skriv effektiva uppmaningar

För att kunna arbeta effektivt i GenStudio är det viktigt att kommunicera med den generativa AI-miljön.

GenStudio ger en generativ AI-fråga varje gång det finns möjlighet att skapa eller ändra en resurs. Komponenterna i en effektiv prompt ska innehålla beskrivande språk, exempel och information som inte tillhandahålls via dina konfigurerade riktlinjer.

Som en god praxis är det att förse GenStudio med din varumärkesinformation med [riktlinjer](/help/user-guide/guidelines/overview.md), så kan du till fullo utnyttja den generativa AI:n för att skapa varumärkesanpassat innehåll.

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

I GenStudio [[!DNL Create]](/help/user-guide/create/overview.md) kan du använda **[!UICONTROL Prompt criteria]** ([_Parametrar_](/help/user-guide/create/overview.md#parameters) och en uppmaning) i promptområdet för att lägga till information genom markeringen för att förbättra AI-tolkningen.

Frågevillkoren för [e-post](/help/tutorials/create-email-experience.md) kan omfatta tillägg av [riktlinjer](/help/user-guide/guidelines/overview.md) i _parametrar_, överföring av en resurs som ska användas i e-postvarianterna samt en beskrivande uppmaning. För en [metaannons](/help/tutorials/create-meta-ad.md) kan frågevillkoren innehålla en varumärkesriktlinje i _Parametrar_, val eller överföring av en befintlig resurs, inställningar för bilder eller resurser som proportioner samt en fråga. Den verkliga kraften börjar med [att konfigurera GenStudio-riktlinjer](/help/user-guide/guidelines/add-guidelines.md).

>[!NOTE]
>
>Om riktlinjer läggs till i _Parametrar_ i promptområdet behöver du inte inkludera referenser till dem i prompten. GenStudio utnyttjar dessa [!DNL Brands], [!DNL Products] och [!DNL Personas] när det gäller innehållsgenerering.

### Riktlinjer

GenStudio riktlinjer hjälper den generativa AI-funktionen att personalisera din GenStudio-komposition. När du får ett frågevillkor kan du välja en [[!DNL Brand]](/help/user-guide/guidelines/brands.md), en [[!DNL Persona]](/help/user-guide/guidelines/personas.md) och en [[!DNL Product]](/help/user-guide/guidelines/products.md) bland dina konfigurerade riktlinjer.

>[!TIP]
>
>Du styr hur och när GenStudio ska använda dina [!DNL Brand]-riktlinjer. Se [Riktlinjer](/help/user-guide/guidelines/overview.md) om du vill veta mer om hur du konfigurerar och hanterar riktlinjer för varumärken.

## Försök igen

Att fråga är en iterativ process. Om resultaten inte uppfyller dina förväntningar kan du granska frågan och göra några ändringar eller lägga till mer information. Du kan förfina uppmaningen genom att ange en URL som exempel eller en källa för mer information.

```bash
Write an email to motivate infrequent users of Photoshop to follow an in-app tutorial that teaches them to combine elements of two photos into a beautiful work of art. Highlight the generative AI capabilities of Photoshop and use references to natural imagery.

Use information from https://www.adobe.com/products/photoshop.html to inspire users with the latest features.
```

Du kan även klistra in avsnitt från en kampanjrapport. Du kan också begära att GenStudio undviker vissa ord, element eller teman.

## God praxis

Några enkla tips för att skapa effektiva uppmaningar i GenStudio:

- Var tydlig och ange vad du ska göra och inte göra.
- Ange kontext med hjälp av externa referenser.
- Utnyttja GenStudio riktlinjer.
- Granska och justera riktlinjerna regelbundet.
- Iterera och förfina.
- Lär dig genom experiment.
