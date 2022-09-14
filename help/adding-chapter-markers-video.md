---
title: Lägga till kapitelmarkörer i video
description: Lär dig hur du lägger till kapitelmarkörer i en videofilm i Adobe Dynamic Media Classic.
uuid: 4e1e6daf-afc6-49d9-ac90-183fe2a903b2
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 8bc5e552-2abb-41f0-89d2-bdf3ae5d96c2
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 0%

---

# Lägga till kapitelmarkörer i video {#adding-chapter-markers-to-video}

Du kan göra det enklare att titta på och navigera i videoklipp med långa formulär genom att lägga till kapitelmarkörer i enstaka videor eller i adaptiva videouppsättningar. När en användare spelar upp videon kan han/hon välja kapitelmarkörer på tidslinjen (kallas även videobandskrubber). På så sätt kan de enkelt navigera till sin intressepunkt eller direkt gå till nytt innehåll, demonstrationer, självstudiekurser och så vidare.

>[!NOTE]
>
>Den videospelare som används måste ha stöd för kapitelmarkörer.

Se [Lägga till eller redigera en förinställning för visningsprogram för video](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) om du vill konfigurera kapitelnavigeringsreferenspunkter och kapiteltitelns popup-text för `Universal_HTML5_Video` visningsprogram (HTML5).

Se även [Lägga till och redigera visningsprogramförinställningar](application-setup.md#adding_and_editing_viewer_presets).

Du skapar en kapitellista för videon på ungefär samma sätt som du skapar bildtexter. Det innebär att du skapar en WebVTT-fil. Observera dock att den här filen måste vara separat från alla WebVTT-beskrivningsfiler som du också använder. du kan inte kombinera bildtexter och kapitel i en WebVTT-fil.

Du kan använda följande exempel som exempel på det format du använder för att skapa en WebVTT-fil med kapitelnavigering:

```as3
WEBVTT 
Chapter 1 
00:00.000 --> 01:04.364 
The bicycle store behind it all. 
Chapter 2 
01:04.364 --> 02:00.944 
Creative Cloud. 
Chapter 3 
02:00.944 --> 03:02.937 
Ease of management for a working solution. 
Chapter 4 
03:02.937 --> 03:35.000 
Cost-efficient access to rapidly evolving technology.
```

I exemplet ovan `Chapter 1` är referensidentifieraren och är valfri. Referenstiden för `00:00:000 --> 01:04:364` anger kapitlets starttid och sluttid, i 00:00:000-format. De sista tre siffrorna är millisekunder och kan lämnas som 000 om du vill. Kapiteltiteln för `The bicycle store behind it all` är den faktiska beskrivningen av kapitlets innehåll. Referensidentifieraren, startreferenstiden och kapiteltiteln visas alla i ett popup-fönster i videospelaren när pekaren placeras över en visuell referenspunkt i videons tidslinje.

Eftersom du använder ett HTML5-videovisningsprogram bör du kontrollera att den kapitelfil du skapar följer standarden WebVTT (Web Video Text Tracks). Kapitelfilnamnstillägget är .VTT. Du kan läsa mer om bildtextstandarden WebVTT.

Se [WebVTT: Textspårningsformat för webbvideo](https://w3c.github.io/webvtt/).

**Så här lägger du till kapitelmarkörer i video:**

1. Skapa en videokapitelfil med en enkel textredigerare utanför Adobe Dynamic Media Classic.

   >[!NOTE]
   >
   >För globalt stöd för videokapitel på andra språk än engelska kräver WebVTT-standarden att du skapar separata VTT-filer och anropar varje språk som du vill ha stöd för.

1. Spara VTT-filen i UTF8-kodning så att du slipper problem med teckenåtergivning i kapiteltiteltexten.

   Vanligtvis vill du ge den kapitelbaserade VTT-filen samma namn som videofilen och lägga till den med `chapters`. Genom att göra det kan det hjälpa dig att automatisera genereringen av video-URL:er med ditt befintliga system för hantering av webbinnehåll.

1. Överför din WebVTT-kapitelfil till Adobe Dynamic Media Classic.

   Se [Överför filer](uploading-files.md#uploading_files).

1. Navigera till resursmappen som innehåller den videofil som du vill associera med den överförda kapitelfilen i panelen Resursbibliotek på vänster sida.
1. Välj en enskild videoresurs i panelen Resursbläddring och välj sedan under miniatyrbilden för resursen **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
1. I tabellen Viewer List kan du hitta visningsprogrammet HTML 5 med namnet **Univeral_HTML5_Video** och gör sedan något av följande:

   * Om du vill visa en popup-video väljer du **[!UICONTROL Copy URL]** till höger om namnet.

      Lägg till den kopierade URL:en för videon med följande syntax så att du kan koppla den till den kopierade URL:en till bildtextfilen:

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Om du vill visa en inbäddad video väljer du **[!UICONTROL Embed Code]** till höger om namnet.

      I dialogrutan Bädda in kod väljer du **[!UICONTROL Copy to Clipboard]**.

      För HTML5 `Universal_HTML5_Video` visningsprogrammet lägger du till den kopierade inbäddningskoden med följande:

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`
