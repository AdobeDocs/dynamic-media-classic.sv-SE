---
title: '"Snabbstart: Integrera Dynamic Media Classic och Adobe Analytics"'
description: En introduktion och snabbstart för att integrera Dynamic Media Classic och Adobe Analytics så att du snabbt kommer igång.
uuid: 3f9e2c91-15d4-4b53-8220-9b1ca57c0b1d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: abec9a85-013c-4030-b129-bf27a89cb464
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---


# Snabbstart: Integrera Dynamic Media Classic och Adobe Analytics {#quick-start-integrating-dmc-analytics}

Adobe Analytics är den branschledande produkten som ger marknadsförarna en plats där de kan mäta, analysera och optimera integrerade data från alla onlineinitiativ i flera marknadsföringskanaler.

När du har integrerat Adobe Analytics med Dynamic Media Classic kan du få rapporter om hur besökare beter sig med Dynamic Media Classic-visningsprogram på din webbplats. När en besökare på en webbplats till exempel klickar på ett zoommål i ett zoomningsvisningsprogram för Dynamic Media Classic, registreras den här åtgärden i Adobe Analytics. Adobe Analytics-rapporter kan samla in kumulativ information om användaraktivitet i Dynamic Media Classic-visningsprogram.

Med Adobe Analytics rapporter kan du få en tydlig bild av kundernas aktivitet på din webbplats. Du kan avgöra vilka produktpresentationer som leder till konvertering och vilka som inte drar nytta av kundernas intresse.

Se även [Mäta video i Adobe Analytics](https://docs.adobe.com/content/help/en/media-analytics/using/media-overview.html).

>[!NOTE]
>
>Ett giltigt Adobe Analytics-konto krävs för att integrera Analytics med Dynamic Media Classic och för att generera analysrapporter.

**Snabbstart**

Den här snabbstarten är utformad för att du snabbt ska komma igång med Adobe Analytics Instrumentation Kit.

**1. Logga in på Adobe Analytics med Dynamic Media Classic och hämta Adobe Analytics rapportvariabler**

>[!NOTE]
>
>Innan du kan konfigurera Adobe Analytics-rapporter och matcha Adobe Analytics-rapportvariabler med Dynamic Media Classic-händelser måste du kontrollera att du har lagts till som medlem i gruppen Web Service Access i Adobe Analytics. Medlemmar i den här gruppen kan få åtkomst till alla rapporter i de angivna rapportsviterna via Marketing Cloud’s Web Services API oavsett vilka behörigheter som har angetts i gränssnittet. Om du vill lägga till en medlem i gruppen i Adobe Analytics klickar du på **Admin Tools** > **Användarhantering** > **Redigera grupper**.

När du har verifierat att du är medlem i webbtjänståtkomstgruppen klickar du i Dynamic Media Classic på **Inställningar** > **Programinstallation** > **Adobe Analytics**. Klicka på **Adobe Analytics-inloggning** på konfigurationssidan för Adobe Analytics.

Se [Logga in på Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

I dialogrutan Adobe Analytics-inloggning skriver du ditt Marketing Cloud Org-ID (valfritt) och dina fullständiga inloggningsuppgifter. Klicka sedan på **Logga in**. I listrutan Report Suite väljer du namnet på den rapportserie som du vill använda.

**2. Tilldela Adobe Analytics rapportvariabler till Dynamic Media Classic-visningsprogramhändelser och Dynamic Media Classic-variabler**

På Adobe Analytics konfigurationssida anger du den information du vill ha i Adobe Analytics-rapporter. För varje Dynamic Media Classic-visningsprogramhändelse som du vill ha information om väljer du en Adobe Analytics-variabel (från rapportsviten) och en Dynamic Media Classic-variabel.

* Visningsprogramhändelser beskriver den användaraktivitet som du vill mäta i rapporter.
* Dynamic Media Classic-variabler beskriver de data om användarhändelser som du vill att rapporterna ska leverera.

I Adobe Analytics Configuration finns även verktyg för att aktivera, redigera och ta bort visningsprogramhändelser.

När du har klickat på Spara på skärmen Adobe Analytics Configuration infogas en anpassad spårningskod för att mäta användaraktivitet i visningsprogram för Dynamic Media Classic. Med den här funktionen kan du spåra användaraktivitet i Adobe Analytics-rapporter.

Se [Konfigurera Adobe Analytics-rapporter](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

**3. Publicera dina Dynamic Media Classic-visningsprogram**

Publicera dina Dynamic Media Classic-visningsprogram så att visningsprogrammen (med kod för att spåra användaraktiviteter i Adobe Analytics-rapporter) läses in på Dynamic Media Classic-servrar. När du har publicerat den här informationen ingår den i visningsprogrammen och kan användas för analyser av Adobe Analytics.

Se [Publicera konfigurationsinformation](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

**4. Placera Dynamic Media Classic-visningsprogram på din webbplats**

Placera Dynamic Media Classic-läsarna med Adobe Analytics spårningskod på webbplatsen.

**5. Testa Adobe Analytics-integrationen genom att visa en Adobe Analytics-rapport**

Om du vill visa Adobe Analytics-rapporter går du till Adobe Analytics webbplats. På rapportsidan kan du visa data och generera diagram för att mäta användaraktivitet med olika visningsprogram.

Se [Testa Adobe Analytics-integrationen genom att visa en Adobe Analytics-rapport](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
