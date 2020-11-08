---
title: Instrumentera ett visningsprogram med Adobe Analytics Instrumentation Kit
seo-title: Instrumentera ett visningsprogram med Adobe Analytics Instrumentation Kit
description: 'null'
seo-description: Lär dig hur du instrumenterar ett visningsprogram med Adobe Analytics Instrumentation Kit.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---


# Instrumentera ett visningsprogram med Adobe Analytics Instrumentation Kit{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Du kan använda Adobe Analytics Instrumentation Kit för att integrera ett HTML5-visningsprogram med Adobe Analytics.

Om du använder någon av de fördefinierade visningsinställningarna för Dynamic Media Classic HTML5 bör du vara medveten om att de redan innehåller all implementeringskod som behövs för att skicka data till Adobe Analytics. Du behöver inte använda någon ytterligare instrumentering.

## Konfigurera Adobe Analytics tracking från Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

För alla HTML5-visningsprogram lägger du till följande JavaScript i HTML-behållaren, vanligtvis i elementet &lt;head>:

```as3
<!-- ***** Site Catalyst Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

`Company` är inställt på Dynamic Media Classic-företagsnamnet. `&preset` är valfritt om inte namnet på företagets förinställning inte är `companypreset`. I sådana fall kan det vara `companypreset-1, companypreset-2`så vidare. Den högre siffran är en nyare instans av förinställningen. Om du vill ta reda på rätt namn på företagets förinställda värde klickar du på **Kopiera URL** och söker sedan efter namnet på företagets förinställning i `preset=`parametern.

Du kommer nu att lägga till en funktion som överför visningsprogramhändelsen till spårningskoden för Adobe Analytics.

Lägg till `s7ComponentEvent()` funktionen i behållar-HTML (eller JSP, eller ASPX eller någon annan):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

Funktionsnamnet är skiftlägeskänsligt. Den enda parameter `s7componentEvent`som skickas till som krävs är den sista: `eventData`. `s7track()` definieras i s_code.jsp som ingår ovan. `s7track` hanterar all spårning per händelse. (I det här området kan du anpassa data som skickas till Adobe Analytics ytterligare.)

## Aktivera HREF- och ITEM-händelser {#enabling-href-and-item-events}

Du kan aktivera HREF- (överrullning) och ITEM-händelser (musklick/pekhändelser) i visningsprogrammen genom redigering av bildschema. Definiera identifierarna för HREF och ITEM i den bildschema som är kopplad till visningsprograminnehållet. Lägg till en `&rolloverKey=` parameter till HREF-värdet i bildschemat.
