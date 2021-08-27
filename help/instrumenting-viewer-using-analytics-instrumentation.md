---
title: Instrumentera ett visningsprogram med Adobe Analytics Instrumentation Kit
description: Lär dig hur du instrumenterar ett visningsprogram med Adobe Analytics Instrumentation Kit i Dynamic Media Classic.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
source-git-commit: bb387446f294cf1e90d26ae1df4422879ad29db7
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Instrumentera ett visningsprogram med Adobe Analytics Instrumentation Kit{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Du kan använda Adobe Analytics Instrumentation Kit för att integrera ett HTML5-visningsprogram med Adobe Analytics.

Om du använder någon av de fördefinierade visningsförinställningarna för Dynamic Media Classic HTML5 innehåller de redan all implementeringskod som behövs för att skicka data till Adobe Analytics. ingen ytterligare instrumentering krävs av dig.

## Konfigurera Adobe Analytics tracking från Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

För alla HTML5-visningsprogram lägger du till följande JavaScript i HTML-behållaren, vanligtvis i elementet &lt;head>:

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

Där `Dynamic Media Classic Company ID` är inställt på företagsnamnet för Dynamic Media Classic. Och `&preset` är valfritt såvida inte företagets förinställningsnamn är `companypreset`. I sådana fall kan det vara `companypreset-1, companypreset-2` och så vidare. Den högre siffran är en nyare instans av förinställningen. Välj **[!UICONTROL Copy URL]** och leta sedan på parametern `preset=`för att hitta namnet på företagets förinställning för att ta reda på rätt namn på företagets förinställning.

Nu kan du lägga till en funktion som skickar visningsprogramhändelsen till spårningskoden för Adobe Analytics.

Lägg till funktionen `s7ComponentEvent()` i behållar-HTML (eller JSP, eller ASPX eller annan):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

Funktionsnamnet är skiftlägeskänsligt. Den enda parameter som skickas till `s7componentEvent`som är obligatorisk är den sista: `eventData`. Där `s7track()` definieras i s_code.jsp som finns ovan. Och `s7track` hanterar all spårning för varje händelse. (I det här området kan du anpassa data som skickas till Adobe Analytics ytterligare.)

## Aktivera HREF- och ITEM-händelser {#enabling-href-and-item-events}

Du kan aktivera HREF- (överrullning) och ITEM-händelser (musklick/pekhändelser) i visningsprogrammen genom redigering av bildschema. Definiera identifierarna för HREF och ITEM i den bildschema som är kopplad till visningsprograminnehållet. Lägg till en `&rolloverKey=`-parameter i HREF-värdet i bildschemat.
