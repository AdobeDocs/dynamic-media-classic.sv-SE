---
title: Aktivera Adobe Analytics videorapporter
description: Lär dig hur du aktiverar Adobe Analytics videorapporter i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
topic: Development, Integrations
level: Experienced
source-git-commit: f054057d383b26e9088582f418f62504c3f327d8
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Aktivera Adobe Analytics videorapporter{#enabling-adobe-analytics-video-reports}

Med Adobe Analytics hjärttaktsbaserade videorapportering behöver du inte längre aktivera de fyra videovisningsprogramhändelserna (Play, Pause, Stop, Milestone) när du konfigurerar Adobe Analytics i Adobe Dynamic Media Classic. Videopulsslag fungerar med färdiga visningsprogram för Adobe Dynamic Media Classic HTML 5 och blandade media. Videospelaren genererar spårningsdata för visning i Adobe Analytics videorapporter.

* En introduktion till direktuppspelningsmedia och mätning av pulsslag finns på [Om Adobe Analytics per contenuti in streaming](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* Integreringen av Adobe Analytics videorapporter med Adobe Dynamic Media Classic har stöd för lösningsvariabler, men inte för anpassade variabler.

  Se [Parametrar för ljud och video](https://experienceleague.adobe.com/en/docs/media-analytics/using/implementation/variables/audio-video-parameters) för mer information om lösningsvariabler och anpassade variabler.

* Färdiga segment med 1-minutersintervall stöds. Anpassad segmentrapportering, t.ex. kunddefinierade milstolpar som baseras på tidsökningar, % milstolpar eller milstolpar för förskjutning, stöds inte.

  Mer information om krav och inställningar för direktuppspelningsmedia finns i [Mät strömmande media i Adobe Analytics](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* Mer information om anpassade variabler och lösningsvariabler finns i [Aktivera medierapporter](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-reports/media-reports-enable#media-reports).

>[!NOTE]
>
>Om din licensierade lösning av Adobe Analytics inte innehåller videopulsslag måste du fortsätta att använda stegen som beskrivs i detta kapitel för att tilldela Adobe Analytics-variabler till Adobe Dynamic Media Classic-visningsprogramhändelser och -variabler.
