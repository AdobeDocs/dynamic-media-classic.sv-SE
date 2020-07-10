---
title: '"Snabbstart: Integrera Dynamic Media Classic och Adobe Analytics "'
seo-title: '"Snabbstart: Integrera Dynamic Media Classic och Adobe Analytics "'
description: 'null'
seo-description: En introduktion och snabbstart för att integrera Dynamic Media Classic och Adobe Analytics så att du snabbt kommer igång.
uuid: 3f9e2c91-15d4-4b53-8220-9b1ca57c0b1d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: abec9a85-013c-4030-b129-bf27a89cb464
translation-type: tm+mt
source-git-commit: 2fb7e34b734dba1e0bd1d150580d7d6c74ee1b79
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 0%

---


# Snabbstart: Integrera Dynamic Media Classic och Adobe Analytics {#quick-start-integrating-scene-and-adobe-analytics}

Adobe Analytics är den branschledande produkten som ger marknadsförarna en plats där de kan mäta, analysera och optimera integrerade data från alla onlineinitiativ i flera marknadsföringskanaler.

När du har integrerat Adobe Analytics med Scene7 Publishing System kan du få rapporter om hur besökare beter sig med Dynamic Media Classic-visningsprogram på din webbplats. När en besökare på en webbplats till exempel klickar på ett zoommål i ett zoomningsvisningsprogram för Dynamic Media Classic, registrerar Adobe Analytics den här åtgärden. Adobe Analytics-rapporter kan samla in kumulativ information om användaraktivitet i visningsprogram för Dynamic Media Classic.

Med hjälp av rapporter från Adobe Analytics kan du få en tydlig bild av kundernas aktivitet på din webbplats. Du kan avgöra vilka produktpresentationer som leder till konvertering och vilka som inte drar nytta av kundernas intresse.

Se även [Mäta video i Adobe Analytics](https://docs.adobe.com/content/help/en/media-analytics/using/media-overview.html).

>[!NOTE]
>
>Ett giltigt Adobe Analytics-konto krävs för att integrera Analytics med Scene7 Publishing System och generera Analytics-rapporter.

**Snabbstart**

Den här snabbstarten är utformad för att du snabbt ska komma igång med Adobe Analytics Instrumentation Kit.

**1. Logga in på Adobe Analytics med Dynamic Media Classic och hämta rapportvariabler för Adobe Analytics**

>[!NOTE]
>
>Innan du kan konfigurera Adobe Analytics-rapporter och matcha rapportvariabler i Adobe Analytics med Dynamic Media Classic-händelser måste du kontrollera att du har lagts till som medlem i gruppen Web Service Access i Adobe Analytics. Medlemmar i den här gruppen kan komma åt alla rapporter i de angivna rapportsviterna via Marketing Clouds webbtjänstAPI, oavsett vilka behörigheter som har angetts i gränssnittet. Om du vill lägga till en medlem i gruppen i Adobe Analytics klickar du på **Administratörsverktyg** > **Användarhantering** > **Redigera grupper**.

När du har verifierat att du är medlem i webbtjänståtkomstgruppen klickar du i Dynamic Media Classic på **Konfigurera** > **Programinställningar** > **Adobe Analytics**. På sidan Adobe Analytics Configuration klickar du på **Adobe Analytics Login**.

Se [Logga in på Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

I dialogrutan Adobe Analytics-inloggning skriver du ditt Marketing Cloud-organisations-ID (valfritt) och dina fullständiga inloggningsuppgifter. Klicka sedan på **Logga in**. I listrutan Report Suite väljer du namnet på den rapportserie som du vill använda.

**2. Tilldela rapportvariabler för Adobe Analytics till visningsprogramhändelser för Dynamic Media Classic och Dynamic Media Classic-variabler**

På konfigurationssidan för Adobe Analytics anger du den information du vill ha i Adobe Analytics-rapporter. För varje visningsprogramhändelse för Dynamic Media Classic som du vill ha information om väljer du en Adobe Analytics-variabel (från rapportsviten) och en Dynamic Media Classic-variabel.

* Visningsprogramhändelser beskriver den användaraktivitet som du vill mäta i rapporter.
* Dynamic Media Classic-variabler beskriver de data om användarhändelser som du vill att rapporterna ska leverera.

Adobe Analytics Configuration innehåller även verktyg för att aktivera, redigera och ta bort visningsprogramhändelser.

När du har klickat på Spara i Adobe Analytics Configuration-skärmen infogas en anpassad spårningskod för att mäta användaraktivitet i visningsprogram för Dynamic Media Classic. Med den här funktionen kan du spåra användaraktivitet i Adobe Analytics-rapporter.

Se [Konfigurera rapporter](configuring-analytics-reports.md#configuring_adobe_analytics_reports)om Adobe Analytics.

**3. Publicera dina visningsprogram för Dynamic Media Classic**

Publicera dina Dynamic Media Classic-visningsprogram så att visningsprogrammen (med kod för att spåra användaraktiviteter i Adobe Analytics-rapporter) läses in på Dynamic Media Classic-servrar. När du har publicerat den här informationen ingår den i visningsprogrammen och kan användas för analyser av Adobe Analytics.

Se [Publiceringskonfigurationsinformation](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

**4. Placera Dynamic Media Classic-visningsprogram på webbplatsen**

Placera Dynamic Media Classic-visningsprogrammen med Adobe Analytics spårningskod på webbplatsen.

**5. Testa integrationen med Adobe Analytics genom att visa en Adobe Analytics-rapport**

Om du vill se rapporter om Adobe Analytics går du till Adobe Analytics webbplats. På rapportsidan kan du visa data och generera diagram för att mäta användaraktivitet med olika visningsprogram.

Se [Testa integrationen med Adobe Analytics genom att visa en Adobe Analytics-rapport](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
