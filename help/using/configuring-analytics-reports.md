---
title: Konfigurera Adobe Analytics-rapporter
description: Lär dig hur du konfigurerar Adobe Analytics-rapporter i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
topic: Integrations, Development
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '1217'
ht-degree: 0%

---

# Konfigurera Adobe Analytics-rapporter{#configuring-adobe-analytics-reports}

Information om vilken information du vill ha i Adobe Analytics rapporter får du på skärmen Adobe Analytics Configuration. Efter dina konfigurationsrapporter visar den här skärmen en motsvarande Adobe Analytics-variabel och Adobe Dynamic Media Classic-variabel för varje visningsprogramhändelse som du vill ha information om. Dessa visningsprogramhändelser-Adobe Analytics variabelkombinationer av variabel och Adobe Dynamic Media Classic avgör vilken information som rapporteras.

Förutom att associera visningsprogramhändelser med variabler innehåller konfigurationsskärmen i Adobe Analytics verktyg för att aktivera, redigera och ta bort visningsprogramhändelser.

>[!NOTE]
>
>När du ändrar inställningarna för Adobe Analytics Report i Adobe Analytics måste du logga in på Adobe Analytics igen från Adobe Dynamic Media Classic, spara konfigurationsinställningarna för Adobe Analytics och sedan publicera igen.

Se [Logga in på Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Se [Konfigurationsinformation för Publish](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Tilldela Adobe Analytics-variabler till Adobe Dynamic Media Classic Viewer-händelser och -variabler {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Använd Adobe Analytics konfigurationsskärm för att associera visningsprogramhändelser med Adobe Analytics-variabler och Adobe Dynamic Media Classic-variabler. För varje visningsprogramhändelse väljer du en Adobe Analytics-variabel och en Adobe Dynamic Media Classic-variabel. Instruktioner om hur du öppnar skärmen Adobe Analytics Configuration finns i [Logga in på Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**Så här tilldelar du Adobe Analytics-variabler till Adobe Dynamic Media Classic-visningsprogramhändelser och -variabler:**

1. När du har loggat in på Adobe Analytics inifrån Dynamic Media Classic och valt en rapportsvit aktiverar du en visningsprogramhändelse på konfigurationssidan för Adobe Analytics i den högra tabellkolumnen genom att välja **[!UICONTROL Enable]**.
1. Under kolumnen Variabler visar du variabelparet genom att markera pilknappen för önskad visningsprogramhändelse.

   Se [Viewer-händelser](configuring-analytics-reports.md#viewer_events).

1. Lägg till en Adobe Dynamic Media Classic-variabel.

   Se [Adobe Dynamic Media Classic-variabler](configuring-analytics-reports.md#scene7_variables).

1. Lägg till en Adobe Analytics-variabel.
1. (Valfritt) Om du vill lägga till ett till variabelpar väljer du **[!UICONTROL Add]**.
1. Välj **[!UICONTROL Save]**.

   När du har valt **[!UICONTROL Save]** visas visningsprogramhändelsen, dess Adobe Analytics-variabel och dess Adobe Dynamic Media Classic-variabel på skärmen Konfigurera i Adobe Analytics.

1. Välj **[!UICONTROL Close]** i det nedre högra hörnet.
1. Gå till **[!UICONTROL Publish]** > **[!UICONTROL Submit Publish]** om du vill köra en Image Serving-publicering.

   Publicering är nödvändigt för att informationen i visningsprogrammen ska vara tillgänglig på Adobe Dynamic Media Classic-servrar.

### Viewer-händelser {#viewer-events}

Viewer-händelser beskriver åtgärder som användare utför med Dynamic Media Classic-visningsprogram. När en användare initierar en åtgärd, till exempel väljer en miniatyrbild eller startar eller stoppar en video, sänder användaren en händelse till webbsidan. Data som är associerade med den händelsen skickas också.

I följande tabell beskrivs de visningsprogramhändelser som du kan lägga till på skärmen Adobe Analytics Configuration.

| Viewer-händelse | Stöd för och visningsprogram för HTML5 Viewer Platform | Beskrivning |
| --- | --- | --- |
| LADDA | **X** (eCatalog, Flyout, SpinSet, Video, Zoom) | När en användare startar ett visningsprogram |
| SIDA | **X** (eCatalog) | I eCatalogs, när en användare byter sida, i målvisningsprogram för zoomning när en användare väljer ett annat mål eller en färgruta. |
| SWAP | **X** (eCatalog, Flyout, SpinSet, Video, Zoom) | När en användare väljer en annan miniatyrbild för att visa en annan bild. |
| OBJEKT | **X** (eCatalog) | I visningsprogram som stöder bildscheman där överrullningar definieras, när en användare håller pekaren över en bildschema för att läsa överrullningstexten. |
| HREF | **X** (eCatalog) | I visningsprogram som stöder bildscheman väljer en användare en URL i en bildschema. |
| MÅL | | När en användare väljer ett zoommål för att zooma in en del av en bild i målvisningsprogram. |
| SÖK | | I eCatalogs, när en användare gör en ordsökning. |
| SPELA | **X** (video) | När en användare väljer Spela upp för att börja spela upp en video i videovisningsprogram.<br><br>**Obs!** Om du använder Adobe Analytics pulsslagsbaserade videorapportering behöver du inte mappa några variabler till den här visningsprogramhändelsen när du konfigurerar Adobe Analytics i Adobe Dynamic Media Classic. Videopulsslag fungerar med färdiga visningsprogram för Adobe Dynamic Media Classic HTML5 och MixedMedia. Videospelaren genererar spårningsdata för visning i Adobe Analytics videorapporter. Se [Aktivera Adobe Analytics-videorapporter](enabling-analytics-video-reports.md). |
| PAUS | **X** (video) | I videovisningsprogram när en användare väljer **[!UICONTROL Pause]** för att frysa en video.<br><br>**Obs!** Om du använder Adobe Analytics pulsslagsbaserade videorapportering behöver du inte mappa några variabler till den här visningsprogramhändelsen när du konfigurerar Adobe Analytics i Adobe Dynamic Media Classic. Videopulsslag fungerar med färdiga visningsprogram för Adobe Dynamic Media Classic HTML5 och MixedMedia. Videospelaren genererar spårningsdata för visning i Adobe Analytics videorapporter. Se [Aktivera Adobe Analytics-videorapporter](enabling-analytics-video-reports.md). |
| STOP | **X** (video) | I videovisningsprogram när en användare väljer **[!UICONTROL Stop]** för att sluta spela upp en video.<br><br>**Obs!** Om du använder Adobe Analytics pulsslagsbaserade videorapportering behöver du inte mappa några variabler till den här visningsprogramhändelsen när du konfigurerar Adobe Analytics i Adobe Dynamic Media Classic. Videopulsslag fungerar med färdiga visningsprogram för Adobe Dynamic Media Classic HTML5 och MixedMedia. Videospelaren genererar spårningsdata för visning i Adobe Analytics videorapporter. Se [Aktivera Adobe Analytics-videorapporter](enabling-analytics-video-reports.md). |
| MILESTON | **X** (video) | I videovisningsprogram genereras milstolpehändelser när användaren tittar på 0, 25, 50, 75 eller 100 procent av videon.<br><br>**Obs!** Om du använder Adobe Analytics pulsslagsbaserade videorapportering behöver du inte mappa några variabler till den här visningsprogramhändelsen när du konfigurerar Adobe Analytics i Adobe Dynamic Media Classic. Videopulsslag fungerar med färdiga visningsprogram för Adobe Dynamic Media Classic HTML5 och MixedMedia. Videospelaren genererar spårningsdata för visning i Adobe Analytics videorapporter. Se [Aktivera Adobe Analytics-videorapporter](enabling-analytics-video-reports.md). |
| FÄRGRUTA | **X** (utfällbar, zoomad) | Den här visningsprogramhändelsen mappas till PAGE-visningsprogramhändelsen i Adobe Dynamic Media Classic. |
| ZOOMA | **X** (eCatalog, SpinSet, Zoom) | Inte spårad av Adobe Analytics. |
| PAN | **X** (eCatalog, SpinSet, Zoom) | Inte spårad av Adobe Analytics. |
| SPIN | **X** (SpinSet) | Inte spårad av Adobe Analytics. |

### Adobe Dynamic Media Classic-variabler {#scene-variables}

För varje visningsprogramhändelse på konfigurationsskärmen i Adobe Analytics väljer du en Adobe Analytics-variabel och en *Adobe Dynamic Media Classic-variabel* . Adobe Dynamic Media Classic-variabler representerar data som du kan hämta för en rapport. Variabeln `searchTerm` visar till exempel nyckelord som används i eCatalog-sökningar.

I följande tabell beskrivs Adobe Dynamic Media Classic-variabler:

| Adobe Dynamic Media Classic-variabel | Beskrivning |
| --- | --- |
| resurs | Adobe Dynamic Media Classic resurs-ID eller videosökvägsfil. |
| viewerId | Ett godtyckligt nummer som tilldelas varje enskild visningsprogramtyp. |
| pageLabel | I eCatalogs är den sida som visas i ett visningsprogram. |
| label | Etikettvärdet (en sträng). |
| frame | Sidan eller sidreferensen i en bilduppsättning. |
| rollover_keyRaw | Hela HREF-värdet, inte bara en bearbetad del av det. |
| rollover_keyProc | ID för ett objekt som refereras i en bildschema (giltigt för href- och artikelhändelser). |
| searchTerm | En term som används i eCatalog-sökning. |
| timeStamp | Spela upp, Stoppa och Pausa som valts i videovisningsprogram. |
| progress | Procentandel av en milstolpehändelse som är slutförd. |
| targetId | ID-värdet (ett tal). |

## Aktivera, redigera och ta bort visningsprogramhändelser {#activating-editing-and-deleting-viewer-events}

På skärmen Adobe Analytics Configuration kan du aktivera, redigera och ta bort visningsprogramhändelser:

* **Aktivera**: Välj **[!UICONTROL Enable]** om du vill aktivera eller **[!UICONTROL Disable]** om du vill inaktivera en vald visningsprogramhändelse.

* **Redigera**: Markera en visningsprogramhändelse och välj den grå knappen **[!UICONTROL View/Edit]** Variabler. I listrutorna Adobe Dynamic Media Classic-variabel och Adobe Analytics-variabel väljer du en annan variabel i respektive lista. Mer information finns i [Tilldela Adobe Analytics-variabler till Adobe Dynamic Media Classic Viewer-händelser och variabler](#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables).

* **Ta bort**: Markera en visningsprogramhändelse och välj den grå knappen **[!UICONTROL View/Edit]** Variabler. Välj **[!UICONTROL Delete]**.
