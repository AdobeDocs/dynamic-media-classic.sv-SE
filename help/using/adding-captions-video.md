---
title: Lägga till bildtexter i video
description: Lär dig hur du lägger till bildtexter i videofilmer i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 0%

---

# Lägga till bildtexter i video {#add-captions-to-video}

Nå ut till globala marknader med dina videor. Du kan göra det genom att lägga till bildtext till enskilda videoklipp eller adaptiva videouppsättningar. Genom att lägga till bildtext undviker du behovet av att duplicera ljudet, eller behovet av att använda inbyggda högtalare för att spela in ljudet igen för varje språk. Videon spelas upp på det språk den spelades in på. Undertexter på främmande språk visas så att personer på olika språk fortfarande kan förstå ljuddelen.

Bildtext ger också bättre tillgänglighet genom att använda undertexter för personer som är döva eller hörselskadade.

>[!NOTE]
>
>Den videospelare som används måste ha stöd för visning av bildtexter.

Så här konfigurerar du bildtexteffekten och redigerar själva bildtextmenyn, inklusive menytexten för någon av följande visningsprogram:

* `Universal_HTML5_Video` visningsprogram
* `Universal_HTML5_MixedMedia_dark` visningsprogram
* `Universal_HTML5_MixedMedia_light` visningsprogram

Se [Lägga till eller redigera en förinställning för visningsprogrammet för video](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Se även [Lägga till och redigera visningsprogramförinställningar](application-setup.md#adding_and_editing_viewer_presets).

Adobe Dynamic Media Classic kan konvertera bildtextfiler till JSON-format (JavaScript Object Notation). Den här konverteringen innebär att du kan bädda in JSON-texten på en webbsida som en dold men fullständig utskrift av videon. Sökmotorerna kan sedan crawla och indexera innehållet så att videoklippen blir lättare att hitta och ge kunderna mer information om videoinnehållet.

Se [Hantera statiskt innehåll (inte bildinnehåll)](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents#image-serving-api) in om du vill ha mer information om hur du använder JSON-funktionen i en URL.

**Så här lägger du till beskrivningar i en video:**

1. Använd ett tredjepartsprogram utanför Adobe Dynamic Media Classic för att skapa videobeskrivningsfilen baserat på vilken typ av visningsprogram du använder.

   | Typ av visningsprogram | Bildtextfil |
   |--- |--- |
   | HTML5 | Om du använder ett HTML5-videovisningsprogram måste bildtextfilen som du skapar följa standarden WebVTT (Web Video Text Tracks). Bildtextens filnamnstillägg är `.VTT`. Du kan läsa mer om bildtextstandarden WebVTT.<br><br>[Se WebVTT](https://w3c.github.io/webvtt/): Textspårningsformatet för webbvideo. <br><br>Det finns många webbplatser som innehåller både kostnadsfria och kostnadsfria verktyg och tjänster som du kan använda för att skapa WebVTT-bildtextfiler. <br><br>Följ instruktionerna på skärmen för att skapa och spara WebVTT-filen. När du är klar kopierar du bildtextfilens innehåll och klistrar in det i en vanlig textredigerare och sparar det med filnamnstillägget VTT. <br><br><b>Obs!</b> För globalt stöd för videobeskrivningar på andra språk än engelska krävs att du skapar separata `.VTT` filer och samtal för varje språk som du vill ha stöd för. <br><br>I allmänhet vill du ge bildtexten ett namn som är detsamma som videofilen och bifoga den med bildtexter. Genom att göra det kan det hjälpa dig att automatisera genereringen av video-URL:er med ditt befintliga system för hantering av webbinnehåll. |

1. I Adobe Dynamic Media Classic överför du bildtextfilen WebVTT, DFXP eller SMPTE XML.

   Se [Överför filer](uploading-files.md#uploading_files).

1. Gå till resursmappen som innehåller den videofil som ska associeras med den bildtextfil som du överförde i panelen Resursbibliotek på vänster sida.
1. Välj en enskild videoresurs i panelen Resursbläddring och välj sedan under miniatyrbilden för resursen **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
1. I tabellen Viewer List kan du hitta visningsprogrammet HTML 5 med namnet **Univeral_HTML5_Video**, **Universal_HTML5_MixedMedia_dark**, eller **Universal_HTML5_MixedMedia_light** gör du något av följande:

   * Om du vill visa en popup-video väljer du **[!UICONTROL Copy URL]** till höger om namnet.

     Lägg till den kopierade URL:en för videon med följande syntax så att du kan koppla den till den kopierade URL:en till bildtextfilen:

     `&caption=<full Copy URL path to the caption file .vtt>,1`

     Anteckna `,1` i slutet av bildtextens URL-sökväg. Omedelbart efter filnamnstillägget VTT i sökvägen kan du aktivera eller inaktivera knappen för undertexter i videospelarfältet genom att ställa in på `1` eller `0`, respektive

   * Om du vill visa en inbäddad video väljer du **[!UICONTROL Embed Code]** till höger om namnet.

     Välj i dialogrutan Bädda in kod **[!UICONTROL Copy to Clipboard]**.

     För HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark`, eller `Universal_HTML5_MixedMedia_light` visningsprogram, lägga till den kopierade inbäddningskoden med följande:

     `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1"`

     Anteckna `,1` i slutet av URL-sökvägen. Omedelbart efter filnamnstillägget VTT i URL-sökvägen kan du aktivera eller inaktivera bildtextknappen i videospelarfältet genom att ställa in på `1` eller `0`, respektive
