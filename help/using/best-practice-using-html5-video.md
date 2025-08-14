---
title: Bästa tillvägagångssätt för att använda videovisningsprogrammet för HTML5
description: Lär dig mer om de bästa sätten att använda videovisningsprogrammet för HTML5.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---

# Bästa tillvägagångssätt för att använda videovisningsprogrammet för HTML5{#best-practice-using-the-html-video-viewer}

Förinställningarna för videovisning i Adobe Dynamic Media Classic HTML5 är robusta videospelare. På designsidan av spelaren kan du skapa hela videouppspelarens funktionalitet med standardverktyg för webbutveckling. Du kan till exempel utforma knapparna, kontrollerna och den anpassade bakgrunden för förhandsvisningsbilder med HTML5 och CSS så att du kan nå dina kunder med ett anpassat utseende.

På visningsprogrammets uppspelningssida identifieras webbläsarens videokapacitet automatiskt. Sedan skickas videon via HLS (HTTP Live Streaming), som också kallas för adaptiv videoströmning. Om leveransmetoden inte finns används progressiv i HTML5 i stället.

Genom att kombinera följande funktioner i en enda spelare:

* Uppspelningskomponenter som utformats med HTML5 och CSS
* Inbäddad uppspelning
* Användning av adaptiv och progressiv strömning baserat på webbläsarens kapacitet

Du kan göra multimediematerialet tillgängligt för både dator- och mobilanvändare. Du får också en smidig videoupplevelse.

Se även [Om HTML5-visningsprogram](https://experienceleague.adobe.com/sv/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only) i referenshandboken för Adobe-visningsprogram.

Se även utbildningsvideon [Visningsförinställningar](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS).

## Spela upp video på stationära datorer och mobila enheter med Adobe Dynamic Media Classic Video Viewer {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

För strömning av anpassningsbara video för datorer och mobilenheter baseras de videor som används för växling av bithastighet på alla MP4-videor i den adaptiva videouppsättningen.

Videouppspelning sker med antingen HLS eller progressiv video. HLS (HTTP Live Streaming) är en Apple-standard för strömning av adaptiv video som automatiskt justerar uppspelningen baserat på nätverkets bandbreddskapacitet. Man kan också &quot;söka&quot; till valfri punkt i videon utan att behöva vänta på att resten av videon ska laddas ned. Se även [HTTP Live Streaming](https://developer.apple.com/streaming/). Progressiv video levereras genom att videon hämtas och lagras lokalt på en användares datorskärm eller mobila enhet.

I följande tabell beskrivs enheten, webbläsaren och uppspelningsmetoden för videofilmer på stationära datorer och mobila enheter med Adobe Dynamic Media Classic Video Viewer.

| Enhet | Webbläsare | Videouppspelningsläge |
|--- |--- |--- |
| Skrivbord | Internet Explorer 9 och 10 | Progressiv hämtning. |
| Skrivbord | Internet Explorer 11+ | HLS videoströmning. |
| Skrivbord | Firefox 23-44 | Progressiv hämtning. |
| Skrivbord | Firefox 45 eller senare | HLS videoströmning. |
| Skrivbord | Chrome | HLS videoströmning. |
| Skrivbord | Safari (Mac) | HLS videoströmning. |
| Mobil | Chrome (Android™ 6 eller tidigare) | Progressiv hämtning. |
| Mobil | Chrome (Android™ 7 eller senare) | HLS videoströmning. |
| Mobil | Android™ (standardwebbläsare) | Progressiv hämtning. |
| Mobil | Safari (iOS) | HLS videoströmning. |
| Mobil | Chrome (iOS) | HLS videoströmning. |
| Mobil | BlackBerry® | HLS videoströmning. |
