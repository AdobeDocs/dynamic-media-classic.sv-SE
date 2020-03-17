---
title: Konfigurera Adobe Analytics-rapporter
seo-title: Konfigurera Adobe Analytics-rapporter
description: 'null'
seo-description: Lär dig hur du konfigurerar Adobe Analytics-rapporter.
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Konfigurera Adobe Analytics-rapporter{#configuring-adobe-analytics-reports}

Om du vill berätta för Adobe Analytics vilken information du vill ha i Adobe Analytics-rapporter går du till konfigurationsskärmen för Adobe Analytics. När du har konfigurerat rapporter visas en motsvarande Adobe Analytics-variabel och Dynamic Media Classic-variabel för varje visningsprogramhändelse som du vill ha information om. Dessa visningsprogramhändelser - variabelkombinationerna Adobe Analytics - Dynamic Media Classic avgör vilken information som rapporteras.

Förutom att associera visningsprogramhändelser med variabler innehåller konfigurationsskärmen i Adobe Analytics verktyg för att aktivera, redigera och ta bort visningsprogramhändelser.

>[!NOTE]
>
>När du ändrar rapportinställningarna i Adobe Analytics måste du logga in på Adobe Analytics igen från Adobe Scene7 Publishing System, spara konfigurationsinställningarna för Adobe Analytics och sedan publicera på nytt.

Se [Logga in på Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Se [Publiceringskonfigurationsinformation](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Tilldela Adobe Analytics-variabler till Dynamic Media Classic-visningsprogramhändelser och variabler {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Använd konfigurationsskärmen i Adobe Analytics för att associera visningsprogramhändelser med Adobe Analytics-variabler och Dynamic Media Classic-variabler. För varje visningsprogramhändelse väljer du en Adobe Analytics-variabel och en Dynamic Media Classic-variabel. Instruktioner om hur du öppnar konfigurationsskärmen i Adobe Analytics finns i [Logga in på Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**Tilldela Adobe Analytics-variabler till Dynamic Media Classic-visningsprogramhändelser och variabler**

1. När du har loggat in på Adobe Analytics från Dynamic Media Classic och valt en rapportsvit aktiverar du en visningsprogramhändelse på sidan Adobe Analytics-konfiguration längst till höger i tabellen genom att klicka på **Aktivera**.
1. Visa variabelparsväljaren under kolumnen Variabler genom att klicka på pilknappen för önskad visningsprogramhändelse.

   Se [Viewer-händelser](configuring-analytics-reports.md#viewer_events).

1. Lägg till en Dynamic Media Classic-variabel.

   Se [Dynamic Media Classic-variabler](configuring-analytics-reports.md#scene7_variables).

1. Lägg till en Adobe Analytics-variabel.
1. (Valfritt) Om du vill lägga till ett till variabelpar klickar du på **Lägg till**.
1. Klicka på **Spara**.

   När du har klickat på Spara visas visningsprogramhändelsen, Adobe Analytics-variabeln och dess Dynamic Media Classic-variabel på konfigurationsskärmen i Adobe Analytics.

1. Klicka på **Stäng** i det nedre högra hörnet.
1. Klicka på **Publicera** > **Skicka publicering** för att köra en Image Serving-publicering.

   Publicering är nödvändigt för att informationen i visningsprogrammen ska vara tillgänglig på Dynamic Media Classic-servrar.

### Viewer-händelser {#viewer-events}

Visningshändelser beskriver åtgärder som användare utför med visningsprogram för Dynamic Media Classic. När en användare initierar en viss åtgärd, till exempel klickar på en miniatyrbild eller startar eller stoppar en video, &quot;sänder&quot; användaren en händelse till webbsidan tillsammans med data som är kopplade till händelsen.

I följande tabell beskrivs de visningsprogramhändelser som du kan lägga till i konfigurationsskärmen för Adobe Analytics.

| Viewer-händelse | Stöd för HTML5 Viewer Platform och visningsprogram | Beskrivning |
|--- |--- |--- |
| LADDA | **X** (eCatalog, Flyout, SpinSet, Video, Zoom) | När en användare startar visningsprogrammet. |
| SIDA | **X** (eCatalog) | I eCatalogs när en användare byter sida; i målvisningsprogram för zoomning när en användare klickar på ett annat mål eller en färgruta. |
| SWAP | **X** (eCatalog, Flyout, SpinSet, Video, Zoom) | När en användare klickar på en annan miniatyrbild för att visa en annan bild. |
| OBJEKT | **X** (eCatalog) | I visningsprogram som stöder bildscheman där överrullningar definieras, när en användare håller pekaren över en bildschema för att läsa överrullningstexten. |
| HREF | **X** (eCatalog) | I visningsprogram som stöder bildscheman klickar en användare på en URL i en bildschema. |
| MÅL |  | När en användare klickar på ett zoommål för att zooma till en del av en bild i målvisningsprogram. |
| SÖK |  | I e-kataloger, när en användare gör en ordsökning. |
| SPELA | **X** (video) | När en användare klickar på Spela upp i videovisningsprogram för att börja spela upp en video.<br><br>**Obs!**Om du använder Adobe Analytics-videorapportering för hjärtslag behöver du inte mappa några variabler till den här visningsprogramhändelsen när du konfigurerar Adobe Analytics i Dynamic Media Classic. Videopulser fungerar med färdiga Dynamic Media Classic HTML5 Video- och MixedMedia-visningsprogram. Videospelaren genererar spårningsdata för visning i Adobe Analytics-videorapporter. Se[Aktivera Adobe Analytics-videorapporter](enabling-analytics-video-reports.md). |
| PAUS | **X** (video) | I videovisningsprogram, när en användare klickar på Paus för att pausa en video.<br><br>**Obs!**Om du använder Adobe Analytics-videorapportering för hjärtslag behöver du inte mappa några variabler till den här visningsprogramhändelsen när du konfigurerar Adobe Analytics i Dynamic Media Classic. Videopulser fungerar med färdiga Dynamic Media Classic HTML5 Video- och MixedMedia-visningsprogram. Videospelaren genererar spårningsdata för visning i Adobe Analytics-videorapporter. Se[Aktivera Adobe Analytics-videorapporter](enabling-analytics-video-reports.md). |
| STOP | **X** (video) | I videovisningsprogram, när en användare klickar på Stoppa för att sluta spela upp en video.<br><br>**Obs!**Om du använder Adobe Analytics-videorapportering för hjärtslag behöver du inte mappa några variabler till den här visningsprogramhändelsen när du konfigurerar Adobe Analytics i Dynamic Media Classic. Videopulser fungerar med färdiga Dynamic Media Classic HTML5 Video- och MixedMedia-visningsprogram. Videospelaren genererar spårningsdata för visning i Adobe Analytics-videorapporter. Se[Aktivera Adobe Analytics-videorapporter](enabling-analytics-video-reports.md). |
| MILESTON | **X** (video) | I videovisningsprogram genereras milstolpehändelser när användaren tittar på 0, 25, 50, 75 eller 100 procent av videon.<br><br>**Obs!**Om du använder Adobe Analytics-videorapportering för hjärtslag behöver du inte mappa några variabler till den här visningsprogramhändelsen när du konfigurerar Adobe Analytics i Dynamic Media Classic. Videopulser fungerar med färdiga Dynamic Media Classic HTML5 Video- och MixedMedia-visningsprogram. Videospelaren genererar spårningsdata för visning i Adobe Analytics-videorapporter. Se[Aktivera Adobe Analytics-videorapporter](enabling-analytics-video-reports.md). |
| FÄRGRUTA | X (utfällbar, zoom) | Den här visningsprogramhändelsen mappas till PAGE-visningsprogramhändelsen i Scene7 Publishing System. |
| ZOOMA | **X** (eCatalog, SpinSet, Zoom) | Spåras inte av Adobe Analytics.<br> |
| PAN | **X** (eCatalog, SpinSet, Zoom) | Spåras inte av Adobe Analytics.<br> |
| SPIN | **X** (SpinSet) | Spåras inte av Adobe Analytics.<br> |


### Dynamic Media Classic-variabler {#scene-variables}

För varje visningsprogramhändelse på konfigurationsskärmen i Adobe Analytics väljer du en Adobe Analytics-variabel och en *Dynamic Media Classic-variabel*. Dynamiska Media Classic-variabler representerar data som du kan hämta för en rapport. Variabeln visar till exempel nyckelord som används i eCatalog-sökningar `searchTerm` .

I följande tabell beskrivs Dynamic Media Classic-variabler.

| Dynamic Media Classic-variabel | Beskrivning |
|--- |:--- |
| resurs | Scene7 Publishing System-resurs-ID eller videosökvägsfil. |
| viewerId | Ett godtyckligt nummer som tilldelas varje enskild visningsprogramtyp. |
| pageLabel | I eCatalogs är den sida som visas i ett visningsprogram. |
| label | Etikettvärdet (en sträng). |
| frame | Sidan eller sidreferensen i en bilduppsättning. |
| rollover_keyRaw | Hela HREF-värdet, inte bara bearbetade delar av det. |
| rollover_keyProc | ID:t för ett objekt som refereras i en bildschema (giltigt för href- och artikelhändelser). |
| searchTerm | En term som används i eCatalog-sökning. |
| timeStamp | Spela upp, Stoppa och Pausa i videovisningsprogram. |
| progress | Procentandel av en milstolpehändelse som är slutförd. |
| targetId | ID-värdet (ett tal). |

## Aktivera, redigera och ta bort visningsprogramhändelser {#activating-editing-and-deleting-viewer-events}

På skärmen Adobe Analytics Configuration kan du aktivera, redigera och ta bort visningsprogramhändelser:

* **Aktivera** Klicka **[!UICONTROL Enable]** för att aktivera eller **[!UICONTROL Disable]** inaktivera en vald visningsprogramhändelse.

* **Redigera** Välj en visningsprogramhändelse och klicka på den **[!UICONTROL View/Edit]** grå knappen Variabler. I listrutorna Dynamic Media Classic Variable och Adobe Analytics Variable väljer du en annan variabel i respektive lista. Mer information finns i Tilldela Adobe Analytics-variabler till Dynamic Media Classic-visningsprogramhändelser och variabler.

* **Ta bort** Välj en visningsprogramhändelse och klicka på den **[!UICONTROL View/Edit]** grå knappen Variabler. Klicka på **[!UICONTROL Delete]**.