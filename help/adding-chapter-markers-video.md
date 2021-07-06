---
title: Lägga till kapitelmarkörer i video
description: Lär dig hur du lägger till kapitelmarkörer i en video.
uuid: 4e1e6daf-afc6-49d9-ac90-183fe2a903b2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 8bc5e552-2abb-41f0-89d2-bdf3ae5d96c2
feature: Dynamic Media Classic,Visningsprogram,Video
role: User
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---

# Lägga till kapitelmarkörer i video{#adding-chapter-markers-to-video}

Du kan göra det enklare att titta på och navigera i videoklipp med långa formulär genom att lägga till kapitelmarkörer i enstaka videor eller i adaptiva videouppsättningar. När en användare spelar upp videon kan han/hon klicka på kapitelmarkörerna på tidslinjen (kallas även videoscubbaren) för att enkelt navigera till sin intressanta punkt eller omedelbart hoppa till nytt innehåll, demonstrationer, självstudiekurser och så vidare.

>[!NOTE]
>
>Den videospelare som används måste ha stöd för kapitelmarkörer.

Se [Lägga till eller redigera en förinställning för visningsprogram för video](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) för att konfigurera kapitelnavigeringsreferenspunkter och kapiteltitelns popup-text för visningsprogrammet `Universal_HTML5_Video` (HTML5).

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

I exemplet ovan är `Chapter 1` referensidentifieraren och valfri. Referenstiden på `00:00:000 --> 01:04:364` anger kapitlets start- och sluttid i formatet 00:00:000. De sista tre siffrorna är millisekunder och kan lämnas som 000 om du vill. Kapiteltiteln för `The bicycle store behind it all` är den faktiska beskrivningen av kapitlets innehåll. Referensidentifieraren, startreferenstiden och kapiteltiteln visas alla i ett popup-fönster i videospelaren när en användare håller muspekaren över en visuell referenspunkt i videons tidslinje.

Eftersom du använder ett HTML5-videovisningsprogram bör du kontrollera att den kapitelfil du skapar följer standarden WebVTT (Web Video Text Tracks). Kapitelfilnamnstillägget är .vtt. Du kan läsa mer om bildtextstandarden WebVTT.

Se [WebVTT: Textspårningsformatet för webbvideo](https://dev.w3.org/html5/webvtt/).

**Lägga till kapitelmarkörer i video**

1. Skapa videokapitelfilen med en enkel textredigerare utanför Dynamic Media Classic.

   >[!NOTE]
   >
   >Om du vill ha globalt stöd för videokapitel på andra språk än engelska måste du tänka på att WebVTT-standarden kräver att du skapar separata .vtt-filer och anropar varje språk som du vill ha stöd för.

1. Spara VTT-filen i UTF8-kodning för att undvika problem med teckenåtergivning i kapiteltiteltexten.

   Vanligtvis vill du ge den kapitelbaserade VTT-filen samma namn som videofilen och lägga till den med `chapters`. Genom att göra det kan det hjälpa dig att automatisera genereringen av video-URL:er med ditt befintliga system för hantering av webbinnehåll.

1. Överför din WebVTT-kapitelfil till Dynamic Media Classic.

   Se [Överföra filer](uploading-files.md#uploading_files).

1. Navigera till resursmappen som innehåller den videofil som du vill associera med den överförda kapitelfilen i panelen Resursbibliotek på vänster sida.
1. Välj en enskild videoresurs i panelen Resursbläddring och klicka sedan på **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** under miniatyrbilden för resursen.
1. Leta reda på HTML5-visningsprogrammet **Univeral_HTML5_Video** i tabellen Visningsprogramlista och gör sedan något av följande:

   * Klicka **[!UICONTROL Copy URL]** längst till höger om namnet om du vill visa ett videoklipp.

      Lägg till den kopierade URL:en för videon med följande syntax för att associera den med den kopierade URL:en till bildtextfilen:

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Klicka **[!UICONTROL Embed Code]** längst till höger om namnet om du vill se en inbäddad videovisningsfunktion.

      Klicka på **[!UICONTROL Copy to Clipboard]** i dialogrutan Bädda in kod.

      För HTML5 `Universal_HTML5_Video`-visningsprogrammet lägger du till den kopierade inbäddningskoden med följande:

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`
