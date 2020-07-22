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
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---


# Logga in på Adobe Analytics{#log-in-to-adobe-analytics}

Innan du loggar in för att konfigurera Adobe Analytics-rapporter och matcha rapportvariabler i Adobe Analytics med Dynamic Media Classic-händelser kontrollerar du att du har lagts till som medlem i gruppen Web Service Access i Adobe Analytics. Medlemmar i den här gruppen kan komma åt alla rapporter i de angivna rapportsviterna via Marketing Clouds webbtjänstAPI, oavsett vilka behörigheter som har angetts i gränssnittet. Om du vill lägga till en medlem i gruppen i Adobe Analytics klickar du på **Administratörsverktyg** > **Användarhantering** > **Redigera grupper**.

När du loggar in har du möjlighet att ange ditt Marketing Cloud Org ID för att använda den senaste videoanalysimplementeringen. Om du väljer att inte ange ditt ID fungerar ändå videorapportering. Det kan dock leda till att data inte integreras korrekt med andra data för klienten från externa Dynamic Media Classic.

**Logga in på Adobe Analytics**

1. Klicka på **Konfigurera** > **Programinställningar**.
1. Klicka på **Adobe Analytics** under Programinställningar i den vänstra rutan.
1. På skärmen Adobe Analytics Configuration klickar du på **Adobe Analytics Login**.
1. I dialogrutan Logga in anger du ditt företagsnamn, ditt företags-ID för Marketing Cloud (valfritt), användarnamn och lösenord.
1. Klicka på **Logga in**.
1. Välj en rapportsvit och klicka sedan på **OK**.

   >[!NOTE]
   >
   >Första gången du loggar in på Adobe Analytics är listrutan Report Suite tom. Du väljer ingen rapportsvit första gången du loggar in. När du loggat in första gången loggar du ut och återgår sedan till Adobe Analytics-skärmen. Logga in igen för att kunna välja en rapportsserie.

>[!MORELIKETHIS]
>
>* [Konfigurera Adobe Analytics-rapporter](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

