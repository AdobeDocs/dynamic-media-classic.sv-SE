---
title: Logga in på Adobe Analytics
description: Lär dig hur du loggar in på Adobe Analytics från Adobe Dynamic Media Classic.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: 876b4c61167b28f7d5e50a656564eafcbe5b9eab
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# Logga in på Adobe Analytics{#log-in-to-adobe-analytics}

Innan du loggar in för att konfigurera Adobe Analytics-rapporter och matcha Adobe Analytics rapportvariabler med Adobe Dynamic Media Classic-händelser kontrollerar du att du är medlem i gruppen Web Service Access i Adobe Analytics. Medlemmar i den här gruppen kan få åtkomst till alla rapporter i de angivna rapportsviterna via Experience Cloud’s Web Services API oavsett vilka behörigheter som har angetts i gränssnittet. Om du vill lägga till en medlem i gruppen går du till Adobe Analytics **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** > **[!UICONTROL Edit Groups]**.

När du loggar in kan du ange ditt Experience Cloud-Org-ID för att använda den senaste videoanalysimplementeringen. Om du väljer att inte ange ditt ID fungerar ändå videorapportering. Det kan dock leda till att data inte integreras korrekt med andra data för klienten från andra Adobe Dynamic Media Classic.

>[!NOTE]
>
>Om ditt Adobe Analytics-konto har migrerats till Adobe IMS-baserad autentisering (Identity Management System) för inloggning fungerar inte det att ange direkta autentiseringsuppgifter.

**Så här loggar du in på Adobe Analytics från Adobe Dynamic Media Classic:**

Börja med att integrera Dynamic Media Classic med Adobe Analytics OAuth. Adobe Analytics OAuth-integrering med Dynamic Media Classic görs vanligtvis bara en gång per användare.

1. Åtkomst [Adobe Developer Console](https://developer.adobe.com/console). Se till att ditt konto har administratörsbehörighet för organisationen som integreringen krävs för.
1. I den nedrullningsbara listan i det övre högra hörnet av hemsidan väljer du önskat företag. (Skärmbilden nedan är endast avsedd för information. det faktiska företagsnamnet du väljer kan variera.)

   ![Skapa ett nytt projekt](assets/analytics-oauth1.png)

1. Gör något av följande:

   * Överst på sidan, från **[!UICONTROL Home]** flik, välja **[!UICONTROL Create new project]**.
   * Överst på sidan, från **[!UICONTROL Projects]** -fliken. I närheten av sidans högra hörn väljer du **[!UICONTROL Create new project]**.

1. Välj **[!UICONTROL Add API]**.
1. På **[!UICONTROL Add an API]** sida, markera **[!UICONTROL Adobe Analytics]**.
1. I det nedre högra hörnet av sidan väljer du **[!UICONTROL Next]**.

   ![Lägg till ett API](assets/analytics-oauth2.png)

1. På **[!UICONTROL Configure API]** sida, markera **[!UICONTROL USER AUTHENTICATION OAuth]**.
1. I det nedre högra hörnet av sidan väljer du **[!UICONTROL Next]**.
1. På **[!UICONTROL Configure API]** sida, markera **[!UICONTROL OAUTH 2.0 Web]**.
1. I **[!UICONTROL Default redirect URI]** anger du följande sökväg exakt som den visas i textfältet:

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. I **[!UICONTROL Redirect URI pattern]** anger du följande sökväg exakt som den visas i textfältet:

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. Välj **[!UICONTROL Save configured API]**.
1. På navigeringspanelen till vänster på Adobe Analytics-sidan, under **[!UICONTROL Credentials]**, markera **[!UICONTROL OAuth Web]**.
1. Under **[!UICONTROL Credential details]** gör du följande:
   * Under **[!UICONTROL Client ID]**, markera **[!UICONTROL Copy]** för att kopiera värdet. Du behöver det här värdet för den efterföljande Analytics-konfigurationen i Dynamic Media Classic-datorprogrammet som ska följas.
   * Under **[!UICONTROL Client Secret]**, markera **[!UICONTROL Retrieve client secret]** för att visa det associerade värdet. Välj **[!UICONTROL Copy]** för att kopiera värdet. Du behöver det här värdet för den efterföljande Adobe Analytics-konfigurationen i Dynamic Media Classic-skrivbordsprogram som ska följas.

**Konfigurera Adobe Analytics i Dynamic Media Classic datorprogram**

>[!NOTE]
>
>När du har konfigurerat Adobe Analytics i Dynamic Media Classic första gången behöver du bara göra om konfigurationen i följande fall:
>
>* En ny rapport läggs till i Analytics och användaren vill börja skicka data till den nya rapporten.
>* Spårningsservern uppdateras i Adobe Analytics.
>* En ny spårningsvariabel introduceras i en rapport och du vill länka en specifik visningsprogramvariabel i Dynamic Media Classic-användargränssnittet till den nya Analytics-variabeln.

>


1. Nära det övre högra hörnet av Adobe Dynamic Media Classic-programmet går du till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]**.
1. I den vänstra panelen, under **[!UICONTROL Application Setup]**, markera **[!UICONTROL Adobe Analytics]**.
1. På **[!UICONTROL Adobe Analytics Configuration]** sida, markera **[!UICONTROL Adobe Analytics Login]**.
1. I **[!UICONTROL Adobe Analytics Login]** i **[!UICONTROL CLIENT ID]** fält och **[!UICONTROL CLIENT SECRET]** klistrar du in respektive värden som du kopierade tidigare.
1. I dialogrutans nedre högra hörn väljer du Logga in och utför inloggningen till Adobe IMS (Identity Management Services).

   När du har loggat in visas inloggningsdialogrutan för Adobe Analytics igen tillsammans med **[!UICONTROL COMPANIES]** nedrullningsbar lista, initierad av de företag som är tillgängliga för dig.

1. Från **[!UICONTROL COMPANIES]** väljer du ett företag.

   När du har valt ett företag visas **[!UICONTROL SUITES]** den nedrullningsbara listan, som initieras av de rapportsviter som är tillgängliga för det valda företaget, visas.

1. Från **[!UICONTROL SUITES]** väljer du en rapportsvit.

   >[!NOTE]
   >
   >Som standard måste användaren vara medveten om att båda **[!UICONTROL COMPANIES]** och **[!UICONTROL SUITES]** listrutorna är tomma. Användaren måste därför välja ett värde i varje lista.

1. Välj **[!UICONTROL OK]** så att du kan spara konfigurationen.

   >[!NOTE]
   >
   >The **[!UICONTROL Adobe Analytics Server]** fältet fylls i med en föreslagen tredjepartsspårningsserver som matchar ditt analysnamnutrymme när du väljer **[!UICONTROL OK]**. Om du använder en annan spårningsserver bör du uppdatera den i det här fältet för att undvika dataförlust.

1. I det nedre vänstra hörnet på Adobe Analytics konfigurationssida väljer du **[!UICONTROL Save]** för att säkerställa att din Adobe Analytics-kontokonfiguration uppdateras.

>[!MORELIKETHIS]
>
>* [Konfigurera Adobe Analytics-rapporter](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

