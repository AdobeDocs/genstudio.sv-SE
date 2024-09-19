---
title: Ansluta till en AEM Assets Content Hub-databas
description: Lär dig koppla GenStudio för Performance Marketers till en Adobe Experience Manager (AEM) Content Hub-databas och utnyttja befintligt godkänt innehåll.
level: Experienced
feature: Assets, Content
source-git-commit: dc438085cfe7c93b20dc7fb0d5919d2dc8b3dcde
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Anslut till en [!DNL AEM Assets Content Hub]-databas

Om du har resurser i Adobe Experience Manager (AEM) kan du följa de här stegen för att göra dem tillgängliga i GenStudio för Performance Marketers.

>[!BEGINSHADEBOX]

**Förutsättningar**:

Följande steg kräver administratörsbehörighet för Admin Console och AEM Assets as a Cloud Service.

>[!ENDSHADEBOX]

## Steg 1: Aktivera [!DNL AEM Assets Content Hub]

Följ självbetjäningsprocessen **Distribuera Content Hub** för att aktivera [!DNL Content Hub] för din befintliga AEM Assets i Cloud Manager. Se [Distribuera [!DNL Content Hub]](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub) i _AEM as a Cloud Service_ -dokumentationen.

När du har aktiverat [!DNL AEM Assets Content Hub] har du en ny instans med suffixet `contenthub` i [!DNL AEM Assets as a Cloud Service] på Admin Console.

## Steg 2: Införliva GenStudio-användare

I [!DNL Admin Console] lägger du till GenStudio-användare eller användargrupper i produktprofilerna för [!DNL AEM Assets Content Hub]. [!DNL AEM Assets Content Hub] användare kan visa resurser, men inte lägga till resurser eller ändra befintliga resurser.

- [Inbyggt [!DNL Content Hub] administratör](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-administrator)
- [Anlita [!DNL Content Hub] användare](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-users)

## Steg 3: Godkänn tillgångar

Godkänn resurser som ska användas i [!DNL AEM Assets Content Hub], vilket gör dem tillgängliga i GenStudio för Performance Marketers. Se [Godkänn resurser i Experience Manager](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/approve-assets) i _AEM as a Cloud Service_ -dokumentationen.

## Steg 4: Konfigurera synlighet för resurser

Granska varje uppsättning konfigurationsalternativ i konfigurationsalternativen för filter, resursinformation, sökning och branding i _[!DNL AEM Assets Content Hub]_. Se [Konfigurera Content Hub-användargränssnitt](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/configure-content-hub-ui-options) i dokumentationen för_ AEM as a Cloud Service _.

## Steg 5: Verifiera anslutningen

I GenStudio för Performance Marketers-innehåll är listan _[!UICONTROL Location]_tillgänglig ovanför galleriet till höger. Listan är inte tillgänglig om du inte har åtkomst eller om din organisation inte har distribuerat och anslutit en [!DNL AEM Assets Content Hub]-databas.