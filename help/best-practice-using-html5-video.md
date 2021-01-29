---
title: Bästa sättet att använda HTML5 Video Viewer
description: Lär dig mer om de bästa sätten att använda HTML5-videovisningsprogrammet.
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---


# Bästa tillvägagångssätt för att använda HTML5 Video Viewer{#best-practice-using-the-html-video-viewer}

Förinställningarna för visningsprogrammet för Dynamic Media Classic HTML5-video är robusta videospelare. På designsidan av spelaren kan du skapa alla videospelarens funktioner med standardverktyg för webbutveckling. Du kan till exempel utforma knappar, kontroller och anpassad förhandsgranskningsbildbakgrund med HTML5 och CSS så att du kan nå dina kunder med ett anpassat utseende.

På visningsprogrammets uppspelningssida identifieras webbläsarens videokapacitet automatiskt. Sedan visas videon med HLS (adaptive video streaming). Om leveransmetoden inte finns används HTML5 Progressiv i stället.

Genom att i en enda spelare kombinera möjligheten att utforma uppspelningskomponenterna med HTML5 och CSS, ha inbäddad uppspelning och använda adaptiv och progressiv strömning beroende på webbläsarens kapacitet, kan du utöka räckvidden för ditt multimedieinnehåll till både dator- och mobilanvändare och säkerställa en smidig videoupplevelse.

Se även [Om HTML5-visningsprogram](https://docs.adobe.com/content/help/en/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html) i referenshandboken för Adobe-visningsprogram.

## Uppspelning av video på stationära datorer och mobila enheter med Dynamic Media Classic Video Viewer {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

För strömning av anpassningsbara video för datorer och mobilenheter baseras de videor som används för växling av bithastighet på alla MP4-videor i den adaptiva videouppsättningen.

Videouppspelning sker med HLS eller progressiv video. HLS (HTTP Live Streaming) är en Apple-standard för adaptiv videoströmning som automatiskt justerar uppspelningen baserat på nätverkets bandbreddskapacitet. Man kan också &quot;söka&quot; till valfri punkt i videon utan att behöva vänta på att resten av videon ska laddas ned. Se även [HTTP-direktuppspelning](https://developer.apple.com/streaming/). Progressiv video levereras genom att videon hämtas och lagras lokalt på en användares datorskärm eller mobila enhet.

I följande tabell beskrivs enheten, webbläsaren och uppspelningsmetoden för videoklipp på stationära datorer och mobila enheter med Dynamic Media Classic Video Viewer.

| Enhet | Webbläsare | Videouppspelningsläge |
|--- |--- |--- |
| Stationär | Internet Explorer 9 och 10 | Progressiv nedladdning. |
| Skrivbord | Internet Explorer 11+ | HLS-videoströmning. |
| Skrivbord | Firefox 23-44 | Progressiv nedladdning. |
| Skrivbord | Firefox 45 eller senare | HLS-videoströmning. |
| Skrivbord | Krom | HLS-videoströmning. |
| Skrivbord | Safari (Mac) | HLS-videoströmning. |
| Mobil | Chrome (Android 6 eller tidigare) | Progressiv nedladdning. |
| Mobil | Chrome (Android 7 eller senare) | HLS-videoströmning. |
| Mobil | Android (standardwebbläsare) | Progressiv nedladdning. |
| Mobil | Safari (iOS) | HLS-videoströmning. |
| Mobil | Chrome (iOS) | HLS-videoströmning. |
| Mobil | Blackberry | HLS-videoströmning. |
