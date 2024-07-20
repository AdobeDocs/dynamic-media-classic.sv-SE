---
title: Instrumentera ett visningsprogram med Adobe Analytics Instrumentation Kit
description: Lär dig hur du instrumenterar ett visningsprogram med Adobe Analytics Instrumentation Kit i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
topic: Integrations, Development
level: Experienced
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Instrumentera ett visningsprogram med Adobe Analytics Instrumentation Kit{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Du kan använda Adobe Analytics Instrumentation Kit för att integrera ett HTML5-visningsprogram med Adobe Analytics.

Om du använder någon av de fördefinierade Adobe Dynamic Media Classic HTML5-visningsförinställningarna innehåller de redan all implementeringskod som skickas data till Adobe Analytics. Du behöver inte lägga till fler instrument.

## Ställ in Adobe Analytics tracking från Adobe Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

För alla visningsprogram för HTML5 lägger du till följande JavaScript i behållaren HTML, vanligtvis i elementet &lt;head>:

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

Där `Adobe Dynamic Media Classic Company ID` är inställt på Adobe Dynamic Media Classic företagsnamn. Och `&preset` är valfritt. Om företagets förinställningsnamn inte är `companypreset` är det inte valfritt. I sådana fall kan det vara `companypreset-1, companypreset-2` och så vidare. Den högre siffran är en nyare instans av förinställningen. Om du vill ta reda på rätt namn på företagets förinställningsvärde väljer du **[!UICONTROL Copy URL]** och söker sedan efter namnet på företagets förinställning i parametern `preset=`.

Nu kan du lägga till en funktion som skickar visningsprogramhändelsen till spårningskoden för Adobe Analytics.

Lägg till funktionen `s7ComponentEvent()` i behållaren HTML (eller JSP, eller ASPX eller någon annan):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

Funktionsnamnet är skiftlägeskänsligt. Den enda parameter som skickas till `s7componentEvent` som krävs är den sista: `eventData`. Där `s7track()` definieras i s_code.jsp som ingår ovan. Och `s7track` hanterar all spårning per händelse. (Du kan anpassa data som skickas till Adobe Analytics ytterligare i det här området.)

## Aktivera HREF- och ITEM-händelser {#enabling-href-and-item-events}

Du kan aktivera HREF- (överrullning) och ITEM-händelser (musklick/pekhändelser) i visningsprogrammen genom redigering av bildschema. Definiera identifierarna för HREF och ITEM i den bildschema som är kopplad till visningsprograminnehållet. Lägg till en `&rolloverKey=`-parameter i HREF-värdet i bildschemat.
