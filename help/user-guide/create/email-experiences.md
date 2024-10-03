---
title: E-postupplevelser
description: Läs om e-postupplevelser i Adobe GenStudio for Performance Marketing.
feature: Experiences, Content Generation, Create, Generative AI, Variant Generation
role: User
level: Beginner
source-git-commit: 67a3fe86facf0fef12f1fd63d8cf79132b0f42b0
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 0%

---


# E-postupplevelser

Med Adobe GenStudio for Performance Marketing kan du använda generativ AI för att effektivisera [skapandet av effektiva e-postupplevelser](/help/tutorials/create-email-experience.md).

Med [!DNL Create] kan moderna marknadsförare använda [riktlinjer](/help/user-guide/guidelines/overview.md), bildresurser och en [välskapad uppmaning](/help/user-guide/effective-prompts.md) för att snabbt [skapa varumärkesanpassade e-postupplevelser](/help/tutorials/create-email-experience.md).

Redigerbara avsnitt i en e-postupplevelse omfattar:

* Förrubrik
* Headline
* Brödtext
* Call-to-action (CTA)
* Bild
* Varumärkeslogotyp

Se [Mallelement](/help/user-guide/content/use-templates.md#template-elements).

<!-- ## Email capabilities

Content creators and marketers can produce brand-consistent email experiences in GenStudio for Performance Marketing. -->

## E-post med flera avsnitt

E-postupplevelser kan innehålla flera avsnitt, vilket möjliggör fullständig anpassning för att passa ert varumärke och era mål. [Välj [!DNL Products] och visuella resurser för varje avsnitt](/help/tutorials/create-email-experience.md#add-parameters) och använd [strukturerade uppmaningar](/help/user-guide/effective-prompts.md#structured-prompts) för att skapa unikt innehåll. Varje avsnitt har stöd för en visuell resurs.

Läs [Förbered en e-postmall](/help/user-guide/content/email-template.md) om du vill veta mer om hur du skapar en mall för flera avsnitt.

## Progressiv inläsning

När innehållsgenereringsprocessen startar läses varje avsnitt av genererat innehåll i e-postvarianter in progressivt på arbetsytan. Erfarenheter, resurser, fält och avsnitt i upplevelser visas individuellt på arbetsytan när de skapas.

När du klickar på **[!UICONTROL Generate]** visas en inläsningsindikator längst ned på arbetsytan som uppdaterar dig när du genererar.

Varje fält och avsnitt i e-postupplevelsen läses in stegvis i den här sekvensen:

1. Variantnamn
1. Ärenderader för alla variationer
1. Förhuvuden
1. Headlines, email body (for single section emails), and call-to-action
1. E-postbrödtext för efterföljande avsnitt (för e-post med flera avsnitt)
1. Varumärkesvalideringsprocessen inträffar och kontrollen [_Varumärkesriktlinjer_](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) fylls i för varje variant.
