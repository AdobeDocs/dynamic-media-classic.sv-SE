---
title: Lägga till bildtexter i video
description: Lär dig hur du lägger till bildtexter i video
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Visningsprogram,Video
role: Business Practitioner
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
source-git-commit: 210c501f56f97b7fab08b71c263be1c03d3d0fac
workflow-type: tm+mt
source-wordcount: '887'
ht-degree: 1%

---

# Lägga till bildtexter i video{#adding-captions-to-video}

Du kan utöka räckvidden för dina videor till globala marknader genom att lägga till bildtexter till enskilda videor eller till adaptiva videouppsättningar. Genom att lägga till bildtext undviker du behovet av att duplicera ljudet, eller behovet av att använda inbyggda högtalare för att spela in ljudet igen för varje språk. Videon spelas upp på det språk den spelades in på. Undertexter på främmande språk visas så att personer på olika språk fortfarande kan förstå ljuddelen.

Bildtext ger också bättre tillgänglighet genom att använda undertexter för personer som är döva eller hörselskadade.

>[!NOTE]
>
>Den videospelare som används måste ha stöd för visning av bildtexter.

Så här konfigurerar du bildtexteffekten och redigerar själva bildtextmenyn, inklusive menytexten för någon av följande visningsprogram:

* `Universal_HTML5_Video` visningsprogram
* `Universal_HTML5_MixedMedia_dark` visningsprogram
* `Universal_HTML5_MixedMedia_light` visningsprogram

se [Lägga till eller redigera en förinställning för visningsprogram för video](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Se även [Lägga till och redigera visningsprogramförinställningar](application-setup.md#adding_and_editing_viewer_presets).

Dynamic Media Classic kan konvertera bildtextfiler till JSON-format (JavaScript™ Object Notation). Den här konverteringen innebär att du kan bädda in JSON-texten på en webbsida som en dold men fullständig utskrift av videon. Sökmotorerna kan sedan crawla och indexera innehållet så att videoklippen blir lättare att hitta och ge kunderna mer information om videoinnehållet.

Mer information om hur du använder JSON-funktionen i en URL finns i [Servera statiskt (icke-image) innehåll](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api) i *API-hjälpen för Adobe Image Serving*.

**Lägga till bildtexter i video**

1. Använd ett tredjepartsprogram utanför Dynamic Media Classic för att skapa videobeskrivningsfilen baserat på vilken typ av visningsprogram du använder.

   | Typ av visningsprogram | Bildtextfil |
   |--- |--- |
   | HTML5 | Om du använder ett HTML5-videovisningsprogram måste bildtextfilen som du skapar följa standarden WebVTT (Web Video Text Tracks). Bildtextens filnamnstillägg är .vtt. Du kan läsa mer om bildtextstandarden WebVTT.<br><br>[Se WebVTT](https://w3c.github.io/webvtt/): Textspårningsformatet för webbvideo. <br><br>Det finns både kostnadsfria och kostnadsfria verktyg och tjänster som du kan använda för att skapa bildtextfiler utanför Dynamic Media Classic. Om du till exempel vill skapa en enkel videobeskrivningsfil utan formatering kan du använda följande kostnadsfria redigerings- och redigeringsverktyg för bildtexter online: <br><br>[WebVTT Caption Maker](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>Använd verktyget i Internet Explorer 9 eller senare, Google Chrome eller Safari för bästa resultat. <br><br>I verktyget, i fältet  <b>Ange URL för </b> videofilen, klistrar du in URL-adressen för videofilen och klickar sedan på  <b>Läs in</b>. <br><br>Om du till exempel använder en Dynamic Media Classic-URL för videofilen dubbelklickar du på en enskild videoresurs (inte en adaptiv videouppsättning eller en Överordnad video) för att öppna den i detaljvyn. Expandera URL:er och Bädda in kod i den högra panelen i detaljvyn. Klicka sedan på Kopiera URL under gruppen Mobil till höger om Mobil (progressiv). Den här processen ger dig URL:en till själva videofilen som du sedan kan klistra in i fältet <b>Ange URL:en för videofilen</b>. Internet Explorer, Chrome och Safari kan sedan spela upp videon direkt. Följ nu instruktionerna på skärmen för att skapa och spara WebVTT-filen. När du är klar kopierar du bildtextfilens innehåll och klistrar in det i en vanlig textredigerare och sparar det med filnamnstillägget .vtt. <br><br><b>Obs!</b> För globalt stöd för videobeskrivningar på andra språk än engelska kräver WebVTT-standarden att du skapar separata .vtt-filer och anropar för varje språk som du vill ha stöd för. <br><br>I allmänhet vill du ge bildtexten ett namn som är detsamma som videofilen och bifoga den med bildtexter. Genom att göra det kan det hjälpa dig att automatisera genereringen av video-URL:er med ditt befintliga system för hantering av webbinnehåll. |

1. I Dynamic Media Classic överför du XML-bildtextfilen WebVTT, DFXP eller SMPTE.

   Se [Överföra filer](uploading-files.md#uploading_files).

1. Gå till resursmappen som innehåller den videofil som du vill associera med bildtextfilen som du överförde i panelen Resursbibliotek på vänster sida.
1. Välj en enskild videoresurs i panelen Resursbläddring och klicka sedan på **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** under miniatyrbilden för resursen.
1. I tabellen Viewer List kan du hitta HTML5-visningsprogrammet **Univeral_HTML5_Video**, **Universal_HTML5_MixedMedia_dark** eller **Universal_HTML5_MixedMedia_light** och sedan göra något av följande:

   * Klicka **[!UICONTROL Copy URL]** längst till höger om namnet om du vill visa ett videoklipp.

      Lägg till den kopierade URL:en för videon med följande syntax för att associera den med den kopierade URL:en till bildtextfilen:

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      Lägg märke till `,1` i slutet av bildtextens URL-sökväg. Omedelbart efter tillägget .vtt i sökvägen kan du aktivera eller inaktivera den stängda bildtextsknappen i videospelarfältet genom att ange `1` eller `0`.

   * Klicka **[!UICONTROL Embed Code]** längst till höger om namnet om du vill se en inbäddad videovisningsfunktion.

      Klicka på **[!UICONTROL Copy to Clipboard]** i dialogrutan Bädda in kod.

      För HTML5-visningsprogrammen `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark` eller `Universal_HTML5_MixedMedia_light` lägger du till den kopierade inbäddningskoden med följande:

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      Lägg märke till `,1` i slutet av URL-sökvägen. Direkt efter tillägget .vtt i URL-sökvägen kan du aktivera eller inaktivera bildtextknappen i videospelarfältet genom att ange `1` eller `0`.
