---
title: 'Snabbstart: Integrera Adobe Dynamic Media Classic och Adobe Analytics'
description: En introduktion och snabbstart om hur du integrerar Adobe Dynamic Media Classic och Adobe Analytics.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Snabbstart: Integrera Adobe Dynamic Media Classic och Adobe Analytics {#quick-start-integrating-dmc-analytics}

Adobe Analytics är den branschledande produkten som ger marknadsförarna en plats där de kan mäta, analysera och optimera integrerade data från alla onlineinitiativ i flera marknadsföringskanaler.

När du har integrerat Adobe Analytics med Adobe Dynamic Media Classic kan du få rapporter om webbplatsbesökarnas beteende med Adobe Dynamic Media Classic-visningsprogram på din webbplats. När en besökare på en webbplats väljer ett zoommål i en Adobe Dynamic Media Classic Zoom Viewer registrerar Adobe Analytics den här åtgärden. Adobe Analytics-rapporter kan samla in kumulativ information om användaraktivitet i Adobe Dynamic Media Classic-visningsprogram.

Med Adobe Analytics rapporter kan du få en tydlig bild av kundernas aktivitet på din webbplats. Du kan avgöra vilka produktpresentationer som leder till konvertering och vilka som inte drar till sig kundernas intresse.

Se även [Mäta video i Adobe Analytics](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

>[!NOTE]
>
>Det krävs ett giltigt Adobe Analytics-konto för att integrera Analytics med Adobe Dynamic Media Classic och generera Analytics-rapporter.

Snabbstarten är utformad för att du snabbt ska komma igång med Adobe Analytics Instrumentation Kit.

## 1. Logga in på Adobe Analytics med Adobe Dynamic Media Classic och hämta Adobe Analytics rapportvariabler

>[!NOTE]
>
>Kontrollera att du har lagts till som medlem i webbtjänståtkomstgruppen i Adobe Analytics. Verifiera innan du konfigurerar Adobe Analytics-rapporter. Och innan du matchar Adobe Analytics rapportvariabler med Adobe Dynamic Media Classic-händelser. Medlemmar i den här gruppen kan komma åt alla rapporter i de angivna rapportsviterna. Du kan göra det med Experience Cloud Web Services API oavsett vilka behörigheter som anges i gränssnittet. Om du vill lägga till en medlem i gruppen går du till **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** > **[!UICONTROL Edit Groups]** i Adobe Analytics.

När du har verifierat att du är medlem i webbtjänståtkomstgruppen går du till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Adobe Analytics]** i Adobe Dynamic Media Classic. På konfigurationssidan för Adobe Analytics väljer du **[!UICONTROL Adobe Analytics Login]**.

Se [Logga in på Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

I dialogrutan Adobe Analytics-inloggning skriver du ditt Experience Cloud Org-ID (valfritt) och dina fullständiga inloggningsuppgifter och väljer sedan **[!UICONTROL Login]**. I listrutan Report Suite väljer du namnet på den rapportserie som du vill använda.

## 2. Tilldela Adobe Analytics rapportvariabler till Adobe Dynamic Media Classic viewer-händelser och Adobe Dynamic Media Classic-variabler

På Adobe Analytics konfigurationssida anger du den information du vill ha i Adobe Analytics-rapporter. För varje Adobe Dynamic Media Classic-visningsprogramhändelse som du vill ha information om väljer du en Adobe Analytics-variabel (från rapportsviten) och en Adobe Dynamic Media Classic-variabel.

* Visningsprogramhändelser beskriver den användaraktivitet som du vill mäta i rapporter.
* Adobe Dynamic Media Classic-variabler beskriver de data om användarhändelser som du vill att rapporterna ska leverera.

I Adobe Analytics Configuration finns även verktyg för att aktivera, redigera och ta bort visningsprogramhändelser.

När du har valt **[!UICONTROL Save]** på Adobe Analytics konfigurationssida infogas en anpassad spårningskod för att mäta användaraktivitet i Adobe Dynamic Media Classic-visningsprogram. Med den här funktionen kan du spåra användaraktivitet i Adobe Analytics-rapporter.

Se [Konfigurera Adobe Analytics-rapporter](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

## 3. Publish dina Adobe Dynamic Media Classic-tittare

Publish dina Adobe Dynamic Media Classic-visningsprogram så att de som tittar på dem (med kod för att spåra användaraktivitet i Adobe Analytics-rapporter) läses in på Adobe Dynamic Media Classic-servrar. När du har publicerat inkluderas den här informationen i visningsprogrammen. Använd den för analys hos Adobe Analytics.

Se [Konfigurationsinformation för Publish](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## 4. Lägg Adobe Dynamic Media Classic-tittare på er webbplats

Placera Adobe Dynamic Media Classic-tittarna med Adobe Analytics spårningskod på er webbplats.

## 5. Testa Adobe Analytics-integrationen genom att visa en Adobe Analytics-rapport

Om du vill visa Adobe Analytics-rapporter går du till Adobe Analytics webbplats. På rapportsidan kan du visa data och generera diagram för att mäta användaraktivitet med olika visningsprogram.

Se [Testa Adobe Analytics-integrationen genom att visa en Adobe Analytics-rapport](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
