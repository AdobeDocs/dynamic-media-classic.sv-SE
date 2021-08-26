---
title: Aktivera Adobe Analytics videorapporter
description: Lär dig hur du aktiverar Adobe Analytics videorapporter i Adobe Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Aktivera Adobe Analytics videorapporter{#enabling-adobe-analytics-video-reports}

Om du använder Adobe Analytics hjärttaktsbaserad videorapportering behöver du inte längre aktivera de fyra videovisningsprogramhändelserna (Play, Pause, Stop, Milestone) när du konfigurerar Adobe Analytics i Adobe Dynamic Media Classic. Videopulsslag fungerar med färdiga visningsprogram för Adobe Dynamic Media Classic HTML5 Video och Mixed Media. Videospelaren genererar spårningsdata för visning i Adobe Analytics videorapporter.

* En introduktion till direktuppspelningsmedia och&quot;hjärtslagsmätning&quot; finns i [Om Adobe Analytics for Streaming Media](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* Integreringen av Adobe Analytics videorapporter med Adobe Dynamic Media Classic stöder lösningsvariabler, men inte anpassade variabler.

   Se [Ljud- och videoparametrar](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) för mer information om lösningsvariabler och anpassade variabler.

* Färdiga segment med 1-minutersintervall stöds. Anpassad segmentrapportering, t.ex. kunddefinierade milstolpar som baseras på tidsökningar, milstolpar i % eller milstolpar för förskjutning, stöds inte.

   Mer information om krav och konfiguration för direktuppspelningsmedia finns i [Mät direktuppspelningsmedia i Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Mer information om anpassade variabler och lösningsvariabler finns i [Aktivera medierapporter](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>Om din licensierade lösning av Adobe Analytics inte innehåller videopulsslag måste du fortsätta att använda stegen som beskrivs i det här kapitlet för att tilldela Adobe Analytics-variabler till visningsprogramhändelser och variabler för Adobe Dynamic Media Classic.
