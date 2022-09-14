---
title: Konfigurera Adobe Analytics-rapporter
description: Lär dig hur du konfigurerar Adobe Analytics-rapporter i Adobe Dynamic Media Classic.
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1214'
ht-degree: 0%

---

# Konfigurera Adobe Analytics-rapporter{#configuring-adobe-analytics-reports}

Information om vilken information du vill ha i Adobe Analytics rapporter får du på skärmen Adobe Analytics Configuration. När du har konfigurerat rapporter visas en motsvarande Adobe Analytics-variabel och Adobe Dynamic Media Classic-variabel för varje visningsprogramhändelse som du vill ha information om. Dessa visningsprogramhändelser-Adobe Analytics variabelkombinationer av variabel och Adobe Dynamic Media Classic avgör vilken information som rapporteras.

Förutom att associera visningsprogramhändelser med variabler innehåller konfigurationsskärmen i Adobe Analytics verktyg för att aktivera, redigera och ta bort visningsprogramhändelser.

>[!NOTE]
>
>När du ändrar inställningarna för Adobe Analytics Report i Adobe Analytics måste du logga in på Adobe Analytics igen från Adobe Dynamic Media Classic, spara konfigurationsinställningarna för Adobe Analytics och sedan publicera igen.

Se [Logga in på Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Se [Publicera konfigurationsinformation](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Tilldela Adobe Analytics-variabler till Adobe Dynamic Media Classic Viewer-händelser och -variabler {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Använd Adobe Analytics konfigurationsskärm för att associera visningsprogramhändelser med Adobe Analytics-variabler och Adobe Dynamic Media Classic-variabler. För varje visningsprogramhändelse väljer du en Adobe Analytics-variabel och en Adobe Dynamic Media Classic-variabel. Instruktioner om hur du öppnar skärmen Adobe Analytics Configuration finns i [Logga in på Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**Så här tilldelar du Adobe Analytics-variabler till Adobe Dynamic Media Classic Viewer-händelser och -variabler:**

1. När du har loggat in på Adobe Analytics från Adobe Dynamic Media Classic och valt en rapportsvit aktiverar du en visningsprogramhändelse på konfigurationssidan för Adobe Analytics i den högra tabellkolumnen genom att välja **[!UICONTROL Enable]**.
1. Visa variabelparsväljaren under kolumnen Variabler genom att markera pilknappen för önskad visningsprogramhändelse.

   Se [Viewer-händelser](configuring-analytics-reports.md#viewer_events).

1. Lägg till en Adobe Dynamic Media Classic-variabel.

   Se [Adobe Dynamic Media Classic-variabler](configuring-analytics-reports.md#scene7_variables).

1. Lägg till en Adobe Analytics-variabel.
1. (Valfritt) Om du vill lägga till ytterligare ett variabelpar väljer du **[!UICONTROL Add]**.
1. Välj **[!UICONTROL Save]**.

   När du har valt **[!UICONTROL Save]**, visningsprogramhändelsen, dess Adobe Analytics-variabel och dess Adobe Dynamic Media Classic-variabel visas på skärmen för Adobe Analytics Configuration.

1. I det nedre högra hörnet väljer du **[!UICONTROL Close]**.
1. Gå till **[!UICONTROL Publish]** > **[!UICONTROL Submit Publish]** för att köra en Image Serving-publicering.

   Publicering är nödvändigt för att informationen i visningsprogrammen ska vara tillgänglig på Adobe Dynamic Media Classic-servrar.

### Viewer-händelser {#viewer-events}

Viewer-händelser beskriver åtgärder som användare utför med Adobe Dynamic Media Classic-visningsprogram. När en användare initierar en viss åtgärd, till exempel väljer en miniatyrbild eller startar eller stoppar en video, &quot;sänder&quot; användaren en händelse till webbsidan tillsammans med data som är kopplade till händelsen.

I följande tabell beskrivs de visningsprogramhändelser som du kan lägga till på skärmen Adobe Analytics Configuration.

| Viewer-händelse | Stöd för och visningsprogram för HTML5 Viewer Platform | Beskrivning |
| --- | --- | --- |
| LADDA | **X** (eCatalog, Flyout, SpinSet, Video, Zoom) | När en användare startar ett visningsprogram |
| SIDA | **X**  (eCatalog) | I eCatalogs när en användare byter sida; i målvisningsprogram för zoomning när en användare väljer ett annat mål eller en färgruta. |
| SWAP | **X**  (eCatalog, Flyout, SpinSet, Video, Zoom) | När en användare väljer en annan miniatyrbild för att visa en annan bild. |
| OBJEKT | **X**  (eCatalog) | I visningsprogram som stöder bildscheman där överrullningar definieras, när en användare håller pekaren över en bildschema för att läsa överrullningstexten. |
| HREF | **X**  (eCatalog) | I visningsprogram som stöder bildscheman väljer en användare en URL i en bildschema. |
| MÅL |  | När en användare väljer ett zoommål för att zooma in en del av en bild i målvisningsprogram. |
| SÖK |  | I e-kataloger, när en användare gör en ordsökning. |
| SPELA | **X**  (Video) | När en användare väljer Spela upp för att börja spela upp en video i videovisningsprogram.<br><br>**Obs!** Om du använder Adobe Analytics pulsslagsbaserade videorapportering behöver du inte mappa några variabler till den här visningsprogramhändelsen när du konfigurerar Adobe Analytics i Adobe Dynamic Media Classic. Videopulsslag fungerar med färdiga visningsprogram för Adobe Dynamic Media Classic HTML5 och MixedMedia. Videospelaren genererar spårningsdata för visning i Adobe Analytics videorapporter. Se [Aktivera Adobe Analytics videorapporter](enabling-analytics-video-reports.md). |
| PAUS | **X** (Video) | I videovisningsprogram, när en användare väljer **[!UICONTROL Pause]** för att frysa en video.<br><br>**Obs!** Om du använder Adobe Analytics pulsslagsbaserade videorapportering behöver du inte mappa några variabler till den här visningsprogramhändelsen när du konfigurerar Adobe Analytics i Adobe Dynamic Media Classic. Videopulsslag fungerar med färdiga visningsprogram för Adobe Dynamic Media Classic HTML5 och MixedMedia. Videospelaren genererar spårningsdata för visning i Adobe Analytics videorapporter. Se [Aktivera Adobe Analytics videorapporter](enabling-analytics-video-reports.md). |
| STOP | **X** (Video) | I videovisningsprogram, när en användare väljer **[!UICONTROL Stop]** om du vill sluta spela upp en video.<br><br>**Obs!** Om du använder Adobe Analytics pulsslagsbaserade videorapportering behöver du inte mappa några variabler till den här visningsprogramhändelsen när du konfigurerar Adobe Analytics i Adobe Dynamic Media Classic. Videopulsslag fungerar med färdiga visningsprogram för Adobe Dynamic Media Classic HTML5 och MixedMedia. Videospelaren genererar spårningsdata för visning i Adobe Analytics videorapporter. Se [Aktivera Adobe Analytics videorapporter](enabling-analytics-video-reports.md). |
| MILESTON | **X**  (Video) | I videovisningsprogram genereras milstolpehändelser när användaren tittar på 0, 25, 50, 75 eller 100 procent av videon.<br><br>**Obs!** Om du använder Adobe Analytics pulsslagsbaserade videorapportering behöver du inte mappa några variabler till den här visningsprogramhändelsen när du konfigurerar Adobe Analytics i Adobe Dynamic Media Classic. Videopulsslag fungerar med färdiga visningsprogram för Adobe Dynamic Media Classic HTML5 och MixedMedia. Videospelaren genererar spårningsdata för visning i Adobe Analytics videorapporter. Se [Aktivera Adobe Analytics videorapporter](enabling-analytics-video-reports.md). |
| FÄRGRUTA | **X** (Utfällbar, Zooma) | Den här visningsprogramhändelsen mappas till PAGE-visningsprogramhändelsen i Adobe Dynamic Media Classic. |
| ZOOMA | **X** (eCatalog, SpinSet, Zoom) | Inte spårad av Adobe Analytics. |
| PAN | **X** (eCatalog, SpinSet, Zoom) | Inte spårad av Adobe Analytics. |
| SPIN | **X** (SpinSet) | Inte spårad av Adobe Analytics. |

### Adobe Dynamic Media Classic-variabler {#scene-variables}

För varje visningsprogramhändelse på skärmen Adobe Analytics Configuration väljer du en Adobe Analytics-variabel och en *Adobe Dynamic Media Classic-variabel*. Adobe Dynamic Media Classic-variabler representerar data som du kan hämta för en rapport. Till exempel `searchTerm` variabellistor nyckelord som används i eCatalog-sökningar.

I följande tabell beskrivs Adobe Dynamic Media Classic-variabler:

| Adobe Dynamic Media Classic-variabel | Beskrivning |
| --- | --- |
| resurs | Adobe Dynamic Media Classic resurs-ID eller videosökvägsfil. |
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

* **Aktivera** - Välj **[!UICONTROL Enable]** för att aktivera eller **[!UICONTROL Disable]** för att inaktivera en vald visningsprogramhändelse.

* **Redigera** - Välj en visningsprogramhändelse och välj **[!UICONTROL View/Edit]** Grå variabelknapp. I listrutorna Adobe Dynamic Media Classic-variabel och Adobe Analytics-variabel väljer du en annan variabel i varje lista. Mer information finns i [Tilldela Adobe Analytics-variabler till Adobe Dynamic Media Classic Viewer-händelser och -variabler](#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables).

* **Ta bort** - Välj en visningsprogramhändelse och välj **[!UICONTROL View/Edit]** Grå variabelknapp. Välj **[!UICONTROL Delete]**.
