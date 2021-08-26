---
title: Logga in på Adobe Analytics
description: Läs om hur du loggar in på Adobe Analytics från Adobe Dynamic Media Classic.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Logga in på Adobe Analytics{#log-in-to-adobe-analytics}

Innan du loggar in för att konfigurera Adobe Analytics-rapporter och matcha Adobe Analytics-rapportvariabler med Adobe Dynamic Media Classic-händelser måste du kontrollera att du är medlem i webbtjänståtkomstgruppen i Adobe Analytics. Medlemmar i den här gruppen kan få åtkomst till alla rapporter i de angivna rapportsviterna via Experience Cloud’s Web Services API oavsett vilka behörigheter som har angetts i gränssnittet. Om du vill lägga till en medlem i gruppen går du till **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** > **[!UICONTROL Edit Groups]** i Adobe Analytics.

När du loggar in kan du ange ditt Experience Cloud-Org-ID för att använda den senaste videoanalysimplementeringen. Om du väljer att inte ange ditt ID fungerar ändå videorapportering. Det kan dock leda till att data inte integreras korrekt med andra data för den klienten från utsidan av Adobe Dynamic Media Classic.

>[!NOTE]
>
>Om ditt Adobe Analytics-konto har migrerats till Adobe IMS-baserad autentisering (Identity Management System) för inloggning fungerar inte det att ange direkta autentiseringsuppgifter.

**Så här loggar du in på Adobe Analytics:**

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** nära det övre högra hörnet på Adobe-Dynamic Media Classic-sidan.
1. I den vänstra rutan, under **[!UICONTROL Application Setup]**, trycker du på **[!UICONTROL Adobe Analytics]**.
1. Tryck på **[!UICONTROL Adobe Analytics Login]** på konfigurationssidan för Adobe Analytics.
1. I dialogrutan **[!UICONTROL Adobe Analytics Login]** anger du ditt företagsnamn, Experience Cloud Org ID (valfritt), användarnamn och *delad hemlighet* i textfältet **[!UICONTROL Password]**.

   Du kan hämta *nyckeln för delad hemlighet* från Analytics-Admin Console. Se [Hämta API-autentiseringsuppgifter för användarkonton](https://github.com/AdobeDocs/analytics-2.0-apis/blob/master/create-oauth-client.md).

1. Välj **[!UICONTROL Login]**.
1. I listrutan **[!UICONTROL Report Suite]** väljer du en rapportserie och sedan **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >Första gången du loggar in på Adobe Analytics är listrutan Report Suite tom. Du väljer ingen rapportsvit första gången du loggar in. När du har loggat in första gången loggar du ut och återgår sedan till Adobe Analytics-skärmen. Logga in igen för att kunna välja en rapportsserie.

>[!MORELIKETHIS]
>
>* [Konfigurera Adobe Analytics-rapporter](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

