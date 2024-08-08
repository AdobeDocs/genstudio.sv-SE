---
title: Varumärkesvalidering i GenStudio
description: Läs om hur det inbyggda varumärkesvalideringssystemet fungerar i GenStudio.
feature: Brands Service, Guidelines
source-git-commit: 12af1741c368666a56ff8663b8b3dfe2087d7e54
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 0%

---


# Varumärkesvalidering

I GenStudio är varumärkesvalidering en viktig komponent som fungerar i samarbete med de generativa AI-funktionerna och -riktlinjerna -[[!DNL Brands]](/help/user-guide/guidelines/brands.md), [[!DNL Products]](/help/user-guide/guidelines/products.md) och [[!DNL Personas]](/help/user-guide/guidelines/personas.md). Det ser till att allt innehåll är anpassat till er varumärkesidentitet.

GenStudio genomför varumärkesvalidering av olika aspekter, bland annat:

* Varumärkesspecifika riktlinjer för varje kund
* Kopiera riktlinjer för olika kanalplattformar
* Etiska överväganden som rör kön, etnicitet, ras, funktionshinder och ålder i AI-genererat innehåll

## Kontroll av varumärkesriktlinjer

En sammanfattning av varumärkesverifieringsinformation för varje genererad innehållsvariant finns tillgänglig via ikonen _Varumärkeskontroll_ bredvid varje variant på arbetsytan.

Kontrollen _Varumärkesriktlinjer_ visar procentandelen kompatibilitet med ditt [varumärke](brands.md). Procentandelen beräknas som antalet [riktlinjer](overview.md) som godkändes vid validering jämfört med antalet testade riktlinjer.

Klicka på ikonen för att se vilka riktlinjer som är kompatibla med ert varumärke och vilka som behöver granskas.

Se [Förbättra varumärkesjusteringen](#improve-brand-alignment).

## Panelen Varumärkesvalidering

Panelen _Varumärkesvalidering_ innehåller detaljerad varumärkesverifieringsinformation och visar på möjligheter till förbättring för varje variantfragment.

På _varumärkesvalideringspanelen_ visas information om:

* **E-post**:
   * Ämnesradfragment
   * Förrubriksfragment
   * Rubrikfragment
   * Kroppsfragment
   * CTA (call to action) fragment
   * Riktlinjer för varumärkesröst
* **Metaannons**:
   * Rubrikfragment
   * Body copy fragment
   * CTA (call to action) fragment
   * Textfragment i bild

Se [Förbättra varumärkesjusteringen](#improve-brand-alignment).

### Filter

På _varumärkesvalideringspanelen_ kan du filtrera de riktlinjer som visas. Klicka på filterikonen längst upp på panelen för att visa:

* **Misslyckade riktlinjer**—_Visa felaktiga riktlinjer_ visar endast riktlinjer som inte godkänts i varumärkesverifieringen.
* **Alla riktlinjer**—_Visa felaktiga och godkända riktlinjer_ visar alla riktlinjer som varianterna mäts mot.
* **Godkända riktlinjer**—_Visa godkända riktlinjer_ visar endast riktlinjer som godkänts vid varumärkesvalidering.

<!-- The _Brand Validation panel_ has different areas of focus for each content channel:

* Email - brand voice and channel compliance
* Images - application photography restrictions and other considerations -->

## Förbättra varumärkesanpassningen

Använd kontrollen _Varumärkesriktlinjer_ och panelen _Varumärkesvalidering_ om du vill maximera effekten av genererat innehåll och behålla en konsekvent varumärkesidentitet. Du kan ändra specifika fragment manuellt för att anpassa dem efter [varumärkesriktlinjerna](brands.md).

**Så här förbättrar du varumärkesjusteringen för genererade innehållsvarianter**:

1. Klicka på ikonen **[!UICONTROL [!DNL Brand] guidelines check]** för en enskild variant.

   Se en sammanfattning av hur den specifika varianten fungerar - riktlinjer som godkänns vid varumärkesvalidering och riktlinjer som behöver granskas - när de kontrolleras mot ert varumärke.

1. Klicka **[!UICONTROL Review]** _eller_ på ikonen för validering av varumärke i den övre menyraden för att visa information om de fragment och riktlinjer som behöver förbättras, så att _panelen för validering av varumärke_ visas.

   Se alla fragment och varumärkesriktlinjer som behöver er uppmärksamhet. Det fragment som är markerat på panelen motsvarar det fragment som är markerat i den genererade varianten på arbetsytan.

   >[!NOTE]
   >
   > Riktlinjen _Varumärkesröst_ som beskrivs på _Varumärkesvalideringspanelen_ gäller för hela varianten, inte för ett enskilt fragment. Hela innehållsvarianten markeras för föreslagna förbättringar.

1. Manuellt revidera variantfragment för att få den starkaste justeringen till ert varumärke.

1. När du har gjort nödvändiga ändringar klickar du på **[!UICONTROL Re-check]** för att validera dina ändringar och se till att de är bättre anpassade till din varumärkesidentitet.

   Varumärkesvalideringsprocessen kommer att köras igen. Om fragment/riktlinje godkänns i valideringen visas en grön bockmarkering för det fragmentet på _varumärkesvalideringspanelen_. Procentandelen i ikonen _Varumärkesstödlinje_ för den reviderade varianten visar också förloppet.

1. Fortsätt att ändra fragment för att säkerställa att hela varianten godkänns i varumärkesvalideringen.

   Navigera mellan riktlinjer på _varumärkesvalideringspanelen_ med knapparna **[!UICONTROL Next]** och **[!UICONTROL Previous]** .

1. Överst på _varumärkesvalideringspanelen_ navigerar du genom varje variant med hjälp av pilarna (använd till exempel pilen för att gå från `Email 1` till `Email 2`) och fortsätter att ändra fragmenten så att de passar ert varumärke bättre.

   Mer information om aktuella riktlinjer finns i [Riktlinjer för varumärkesröst](/help/user-guide/guidelines/brands.md#brand-voice-guidelines).
