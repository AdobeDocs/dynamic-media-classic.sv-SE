---
title: Aktivera Adobe Analytics videorapporter
description: Lär dig hur du aktiverar Adobe Analytics videorapporter.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Datatekniker, administratör, affärsansvarig
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# Aktivera Adobe Analytics videorapporter{#enabling-adobe-analytics-video-reports}

Med Adobe Analytics hjärttaktsbaserade videorapportering behöver du inte längre aktivera de fyra videovisningsprogramhändelserna (Play, Pause, Stop, Milestone) när du konfigurerar Adobe Analytics i Dynamic Media Classic. Videoberättelser fungerar med färdiga visningsprogram för Dynamic Media Classic HTML5 Video och MixedMedia. Videospelaren genererar spårningsdata för visning i Adobe Analytics videorapporter.

* En introduktion till direktuppspelningsmedia och&quot;hjärtslagsmätning&quot; finns i [Om Adobe Analytics for Streaming Media](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* Integreringen av Adobe Analytics videorapporter med Dynamic Media Classic stöder lösningsvariabler, men inte anpassade variabler.

   Se [Ljud- och videoparametrar](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) för mer information om lösningsvariabler och anpassade variabler.

* Färdiga segment med 1 minuters intervall stöds. Anpassad segmentrapportering, t.ex. kunddefinierade milstolpar som baseras på tidsökningar, milstolpar i % eller milstolpar för förskjutning, stöds inte.

   Mer information om krav och inställningar för direktuppspelningsmedia finns i [Mäta direktuppspelningsmedia i Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Mer information om anpassade variabler och lösningsvariabler finns i [Aktivera medierapporter](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>Om din licensierade lösning av Adobe Analytics inte innehåller videopulsslag måste du fortsätta att använda stegen som beskrivs i det här kapitlet för att tilldela Adobe Analytics-variabler till Dynamic Media Classic-visningsprogramhändelser och variabler.

