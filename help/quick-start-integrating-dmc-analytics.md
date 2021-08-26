---
title: '"Snabbstart: Integrera Adobe Dynamic Media Classic och Adobe Analytics"'
description: En introduktion och snabbstart för att integrera Adobe Dynamic Media Classic och Adobe Analytics så att du snabbt kommer igång.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Snabbstart: Integrera Adobe Dynamic Media Classic och Adobe Analytics {#quick-start-integrating-dmc-analytics}

Adobe Analytics är den branschledande produkten som ger marknadsförarna en plats där de kan mäta, analysera och optimera integrerade data från alla onlineinitiativ i flera marknadsföringskanaler.

När du har integrerat Adobe Analytics med Adobe Dynamic Media Classic kan du få rapporter om hur besökare beter sig med Adobe Dynamic Media Classic-visningsprogram på din webbplats. När en besökare på en webbplats till exempel klickar på ett zoommål i zoomningsvisningsprogrammet för Adobe Dynamic Media Classic, registrerar Adobe Analytics den här åtgärden. Adobe Analytics-rapporter kan samla in kumulativ information om användaraktivitet i visningsprogram för Adobe Dynamic Media Classic.

Med Adobe Analytics rapporter kan du få en tydlig bild av kundernas aktivitet på din webbplats. Du kan avgöra vilka produktpresentationer som leder till konvertering och vilka som inte drar till sig kundernas intresse.

Se även [Mäta video i Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

>[!NOTE]
>
>Ett giltigt Adobe Analytics-konto krävs för att integrera Analytics med Adobe Dynamic Media Classic och för att generera analysrapporter.

Den här snabbstarten är utformad för att du snabbt ska komma igång med Adobe Analytics Instrumentation Kit.

## 1. Logga in på Adobe Analytics med Adobe Dynamic Media Classic och hämta Adobe Analytics rapportvariabler

>[!NOTE]
>
>Innan du kan konfigurera Adobe Analytics-rapporter och matcha Adobe Analytics-rapportvariabler med Adobe Dynamic Media Classic-händelser måste du kontrollera att du har lagts till som medlem i webbtjänståtkomstgruppen i Adobe Analytics. Medlemmar i den här gruppen kan få åtkomst till alla rapporter i de angivna rapportsviterna via Marketing Cloud’s Web Services API oavsett vilka behörigheter som har angetts i gränssnittet. Om du vill lägga till en medlem i gruppen i Adobe Analytics klickar du på **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** > **[!UICONTROL Edit Groups]**.

När du har verifierat att du är medlem i webbtjänståtkomstgruppen klickar du i Adobe Dynamic Media Classic på **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Adobe Analytics]**. Klicka på **[!UICONTROL Adobe Analytics Login]** på konfigurationssidan för Adobe Analytics.

Se [Logga in på Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

I dialogrutan Adobe Analytics-inloggning skriver du ditt Marketing Cloud Org-ID (valfritt) och fullständig inloggningsinformation och klickar sedan på **[!UICONTROL Login]**. I listrutan Report Suite väljer du namnet på den rapportserie som du vill använda.

## 2. Tilldela Adobe Analytics rapportvariabler till visningsprogramhändelser i Adobe Dynamic Media Classic och Adobe Dynamic Media Classic-variabler

På Adobe Analytics konfigurationssida anger du den information du vill ha i Adobe Analytics-rapporter. För varje visningsprogramhändelse för Adobe Dynamic Media Classic som du vill ha information om väljer du en Adobe Analytics-variabel (från rapportsviten) och en Adobe Dynamic Media Classic-variabel.

* Visningsprogramhändelser beskriver den användaraktivitet som du vill mäta i rapporter.
* Adobe Dynamic Media Classic-variabler beskriver data om användarhändelser som du vill att rapporterna ska leverera.

I Adobe Analytics Configuration finns även verktyg för att aktivera, redigera och ta bort visningsprogramhändelser.

När du har klickat på **[!UICONTROL Save]** på Adobe Analytics konfigurationssida infogas en anpassad spårningskod för att mäta användaraktivitet i visningsprogram för Adobe Dynamic Media Classic. Med den här funktionen kan du spåra användaraktivitet i Adobe Analytics-rapporter.

Se [Konfigurera Adobe Analytics-rapporter](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

## 3. Publicera dina visningsprogram för Adobe Dynamic Media Classic

Publicera dina visningsprogram för Adobe Dynamic Media Classic så att de (med kod för att spåra användaraktiviteter i Adobe Analytics-rapporter) läses in på Adobe Dynamic Media Classic-servrar. När du har publicerat den här informationen ingår den i visningsprogrammen och kan användas för analyser av Adobe Analytics.

Se [Publicera konfigurationsinformation](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## 4. Placera Adobe Dynamic Media Classic-visningsprogram på din webbplats

Placera Adobe i Dynamic Media Classic-visningsprogrammen med Adobe Analytics spårningskod på webbplatsen.

## 5. Testa Adobe Analytics-integrationen genom att visa en Adobe Analytics-rapport

Om du vill visa Adobe Analytics-rapporter går du till Adobe Analytics webbplats. På rapportsidan kan du visa data och generera diagram för att mäta användaraktivitet med olika visningsprogram.

Se [Testa Adobe Analytics-integrationen genom att visa en Adobe Analytics-rapport](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
