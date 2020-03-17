---
title: '"Snabbstart: Integrera Dynamic Media Classic och Adobe Analytics'
seo-title: '"Snabbstart: Integrera Dynamic Media Classic och Adobe Analytics'
description: 'null'
seo-description: En introduktion och snabbstart för att integrera Dynamic Media Classic och Adobe Analytics så att du snabbt kommer igång.
uuid: 3f9e2c91-15d4-4b53-8220-9b1ca57c0b1d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: abec9a85-013c-4030-b129-bf27a89cb464
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Snabbstart: Integrera Dynamic Media Classic och Adobe Analytics {#quick-start-integrating-scene-and-adobe-analytics}

Adobe Analytics är den branschledande produkten som ger marknadsförarna en plats där de kan mäta, analysera och optimera integrerade data från alla onlineinitiativ över flera marknadsföringskanaler.

När du har integrerat Adobe Analytics med Scene7 Publishing System kan du få rapporter om webbplatsbesökarnas beteende med hjälp av Dynamic Media Classic-visningsprogram på webbplatsen. När en besökare på en webbplats till exempel klickar på ett zoommål i en Dynamic Media Classic Zoom Viewer registrerar Adobe Analytics den här åtgärden. Adobe Analytics-rapporter kan samla in kumulativ information om användaraktivitet i Dynamic Media Classic-visningsprogram.

Med hjälp av Adobe Analytics-rapporter kan ni få en tydlig bild av kundernas aktivitet på er webbplats. Du kan avgöra vilka produktpresentationer som leder till konvertering och vilka som inte drar nytta av kundernas intresse.

Se även [Mäta video i Adobe Analytics](https://marketing.adobe.com/resources/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>Ett giltigt Adobe Analytics-konto krävs för att integrera Analytics med Scene7 Publishing System och generera analysrapporter.

**Snabbstart**

Den här snabbstarten är utformad för att du snabbt ska komma igång med Adobe Analytics Instrumentation Kit.

**1. Logga in på Adobe Analytics med Dynamic Media Classic och hämta rapportvariabler för Adobe Analytics**

>[!NOTE]
>
>Innan du kan konfigurera Adobe Analytics-rapporter och matcha Adobe Analytics-rapportvariabler med Dynamic Media Classic-händelser måste du kontrollera att du har lagts till som medlem i gruppen Web Service Access i Adobe Analytics. Medlemmar i den här gruppen kan komma åt alla rapporter i de angivna rapportsviterna via Marketing Clouds webbtjänstAPI, oavsett vilka behörigheter som har angetts i gränssnittet. Om du vill lägga till en medlem i gruppen går du till Adobe Analytics och klickar på **Administratörsverktyg** > **Användarhantering** > **Redigera grupper**.

När du har verifierat att du är medlem i webbtjänståtkomstgruppen klickar du i Dynamic Media Classic på **Inställningar** > **Programkonfiguration** > **Adobe Analytics**. På sidan Adobe Analytics Configuration klickar du på **Adobe Analytics-inloggning**.

Se [Logga in på Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

I dialogrutan Adobe Analytics-inloggning skriver du ditt Marketing Cloud-organisations-ID (valfritt) och dina fullständiga inloggningsuppgifter. Klicka sedan på **Logga in**. I listrutan Report Suite väljer du namnet på den rapportserie som du vill använda.

**2. Tilldela rapportvariabler för Adobe Analytics till Dynamic Media Classic-visningsprogramhändelser och Dynamic Media Classic-variabler**

På sidan Adobe Analytics-konfiguration anger du den information du vill ha i Adobe Analytics-rapporter. För varje Dynamic Media Classic-visningsprogramhändelse som du vill ha information om väljer du en Adobe Analytics-variabel (från rapportsviten) och en Dynamic Media Classic-variabel.

* Visningsprogramhändelser beskriver den användaraktivitet som du vill mäta i rapporter.
* Dynamiska Media Classic-variabler beskriver data om användarhändelser som du vill att rapporterna ska leverera.

Adobe Analytics Configuration innehåller även verktyg för att aktivera, redigera och ta bort visningsprogramhändelser.

När du har klickat på Spara i Adobe Analytics Configuration-skärmen infogas en anpassad spårningskod för att mäta användaraktivitet i Dynamic Media Classic-visningsprogram. Med den här funktionen kan du spåra användaraktivitet i Adobe Analytics-rapporter.

Se [Konfigurera Adobe Analytics-rapporter](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

**3. Publicera dina Dynamic Media Classic-visningsprogram**

Publicera dina Dynamic Media Classic-visningsprogram så att visningsprogrammen (med kod för att spåra användaraktivitet i Adobe Analytics-rapporter) läses in på Dynamic Media Classic-servrar. Efter publiceringen inkluderas den här informationen i visningsprogram och kan användas för analyser av Adobe Analytics.

Se [Publiceringskonfigurationsinformation](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

**4. Placera Dynamic Media Classic-visningsprogram på webbplatsen**

Placera Dynamic Media Classic-tittarna med Adobe Analytics-spårningskod på er webbplats.

**5. Testa Adobe Analytics-integreringen genom att visa en Adobe Analytics-rapport**

Om du vill visa Adobe Analytics-rapporter går du till Adobe Analytics-webbplatsen. På rapportsidan kan du visa data och generera diagram för att mäta användaraktivitet med olika visningsprogram.

Se [Testa Adobe Analytics-integreringen genom att visa en Adobe Analytics-rapport](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
