---
title: Logga in på Adobe Analytics
seo-title: Logga in på Adobe Analytics
description: 'null'
seo-description: Lär dig hur du loggar in på Adobe Analytics.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---


# Logga in på Adobe Analytics{#log-in-to-adobe-analytics}

Innan du loggar in för att konfigurera Adobe Analytics-rapporter och matcha Adobe Analytics rapportvariabler med Dynamic Media Classic-händelser, kontrollerar du att du har lagts till som medlem i webbtjänståtkomstgruppen i Adobe Analytics. Medlemmar i den här gruppen kan få åtkomst till alla rapporter i de angivna rapportsviterna via Marketing Cloud’s Web Services API oavsett vilka behörigheter som har angetts i gränssnittet. Om du vill lägga till en medlem i gruppen i Adobe Analytics klickar du på **Administratörsverktyg** > **Användarhantering** > **Redigera grupper**.

När du loggar in kan du ange ditt Marketing Cloud-Org-ID för att använda den senaste videoanalysimplementeringen. Om du väljer att inte ange ditt ID fungerar ändå videorapportering. Det kan dock leda till att data inte integreras korrekt med andra data för klienten utanför Dynamic Media Classic.

>[!NOTE]
>
>Om ditt Adobe Analytics-konto har migrerats till Adobe IMS-baserad autentisering (Identity Management System) för inloggning fungerar inte det att ange direkta autentiseringsuppgifter.

**Logga in på Adobe Analytics**

1. Tryck på i det övre högra hörnet av sidan Dynamic Media Classic **[!UICONTROL Setup > Application Setup]**.
1. I den vänstra rutan, under **[!UICONTROL Application Setup]**, trycker du **[!UICONTROL Adobe Analytics]**.
1. Tryck på Adobe Analytics Configuration **[!UICONTROL Adobe Analytics Login]**.
1. I **[!UICONTROL Adobe Analytics Login]** dialogrutan anger du företagsnamn, Marketing Cloud Org ID (valfritt), användarnamn och den *delade hemliga* nyckeln i **[!UICONTROL Password]** textfältet.

   Du kan hämta den *delade hemliga* nyckeln från administratörskonsolen för Analytics. Se [Hämta API-autentiseringsuppgifter för användarkonton](https://helpx.adobe.com/analytics/kb/how-to-get-api-credentials-for-user-accounts-.html).

1. Klicka på **[!UICONTROL Login]**.
1. Välj en rapportsvit på den **[!UICONTROL Report Suite]** nedrullningsbara menyn och klicka sedan på **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >Första gången du loggar in på Adobe Analytics är listrutan Report Suite tom. Du väljer ingen rapportsvit första gången du loggar in. När du har loggat in första gången loggar du ut och återgår sedan till Adobe Analytics-skärmen. Logga in igen för att kunna välja en rapportsserie.

>[!MORELIKETHIS]
>
>* [Konfigurera Adobe Analytics-rapporter](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

