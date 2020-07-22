---
title: Aktivera videorapporter för Adobe Analytics
seo-title: Aktivera videorapporter för Adobe Analytics
description: 'null'
seo-description: Lär dig hur du aktiverar Adobe Analytics videorapporter.
uuid: 078594b2-7d53-4714-8128-ff3b5c3a5e36
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 18644a53-92da-40ab-b961-318d8332c54d
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 0%

---


# Aktivera videorapporter för Adobe Analytics{#enabling-adobe-analytics-video-reports}

Med Adobe Analytics hjärttaktsbaserad videorapportering behöver du inte längre aktivera de fyra videovisningsprogramhändelserna (Play, Pause, Stop, Milestone) när du konfigurerar Adobe Analytics i Dynamic Media Classic. Videopulser fungerar med färdiga visningsprogram för Dynamic Media Classic HTML5 Video och MixedMedia. Videospelaren genererar spårningsdata för visning i Adobe Analytics videorapporter.

* Integreringen av Adobe Analytics videorapporter med Dynamic Media Classic stöder lösningsvariabler, men inte anpassade variabler.

   Mer information om lösningsvariabler och anpassade variabler finns i [Konfigurera Analytics Video Reporting](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html) .

* Färdiga segment med 1 minuters intervall stöds. Anpassad segmentrapportering, t.ex. kunddefinierade milstolpar som baseras på tidsökningar, milstolpar i % eller milstolpar för förskjutning, stöds inte.

Mer information om krav och inställningar för videopulsslag finns i [Mäta video i Adobe Analytics med Videopulsslag](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>Om din licensierade lösning av Adobe Analytics inte innehåller videouppslag måste du fortsätta att använda stegen som beskrivs i det här kapitlet för att tilldela Adobe Analytics-variabler till visningsprogramhändelser och variabler i Dynamic Media Classic.

