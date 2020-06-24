---
title: Lägga till bildtexter i video
seo-title: Lägga till bildtexter i video
description: 'null'
seo-description: Lär dig hur du lägger till bildtexter i video
uuid: 4cc64469-4369-44a9-83db-63bad51aba8a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
translation-type: tm+mt
source-git-commit: 74238f90f45f0fb9a4566915a20a1d41dfb69fe1
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 1%

---


# Lägga till bildtexter i video{#adding-captions-to-video}

Du kan utöka räckvidden för dina videor till globala marknader genom att lägga till bildtexter till enskilda videor eller till adaptiva videouppsättningar. Genom att lägga till bildtext undviker du behovet av att duplicera ljudet, eller behovet av att använda inbyggda högtalare för att spela in ljudet igen för varje språk. Videon spelas upp på det språk den spelades in på. Undertexter på främmande språk visas så att personer på olika språk fortfarande kan förstå ljuddelen.

Bildtext ger också bättre tillgänglighet genom att använda undertexter för personer som är döva eller hörselskadade.

>[!NOTE]
>
>Den videospelare som används måste ha stöd för visning av bildtexter.

Se [Lägga till eller redigera en förinställning](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) för visningsprogram för video för att konfigurera bildtexteffekten och för att redigera själva bildtextmenyn, inklusive menytexten för någon av följande visningsprogram:

* `Universal_HTML5_Video` visningsprogram.
* `Universal_HTML5_MixedMedia_dark` visningsprogram.
* `Universal_HTML5_MixedMedia_light` visningsprogram.

Se även [Lägga till och redigera visningsprogramförinställningar](application-setup.md#adding_and_editing_viewer_presets).

I Dynamic Media Classic kan du konvertera bildtextfiler till JSON-format (JavaScript Object Notation). Den här konverteringen innebär att du kan bädda in JSON-texten på en webbsida som en dold men fullständig utskrift av videon. Sökmotorerna kan sedan crawla och indexera innehållet så att videoklippen blir lättare att hitta och ge kunderna ytterligare information om videoinnehållet.

Mer information om hur du använder JSON-funktionen i en URL finns i [Servera statiskt (icke-bildinnehåll](https://docs.adobe.com/content/help/en/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html) ) i API-hjälpen *för* Adobe Image Serving.

**Lägga till bildtexter i video**

1. Använd ett tredjepartsprogram utanför Scene7 Publishing System och skapa en videobildtextfil utifrån den typ av visningsprogram som du använder.

   | Typ av visningsprogram | Bildtextfil |
   |--- |--- |
   | HTML5 | Om du använder ett HTML5-videovisningsprogram måste bildtextfilen som du skapar följa standarden WebVTT (Web Video Text Tracks). Bildtextens filnamnstillägg är .vtt. Du kan läsa mer om bildtextstandarden WebVTT.<br><br>[Se WebVTT](https://dev.w3.org/html5/webvtt/): Textspårningsformatet för webbvideo. <br><br>Det finns både kostnadsfria och kostnadsfria verktyg och tjänster som du kan använda för att skapa bildtextfiler utanför Scene7 Publishing System. Om du till exempel vill skapa en enkel videobeskrivningsfil utan formatering kan du använda följande kostnadsfria redigerings- och redigeringsverktyg för bildtexter online: <br><br>[WebVTT Caption Maker](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>För bästa resultat bör du använda verktyget i Internet Explorer 9 eller senare, Google Chrome eller Safari. <br><br>I verktyget, i fältet <b>Ange URL för videofilen</b> , klistrar du in URL-adressen för videofilen och klickar sedan på <b>Läs in</b>. <br><br>Om du till exempel använder en Dynamic Media Classic-URL för videofilen dubbelklickar du i SPS på en enskild videoresurs (inte en adaptiv videouppsättning eller en huvudvideo) för att öppna den i detaljvyn. Expandera URL:er och Bädda in kod i den högra panelen i detaljvyn. Klicka sedan på Kopiera URL under gruppen Mobil till höger om Mobil (progressiv). Den här processen ger dig webbadressen till själva videofilen som du sedan kan klistra in i fältet <b>Ange webbadress för videofilen</b> . Internet Explorer, Chrome och Safari kan sedan spela upp videon direkt. Följ nu instruktionerna på skärmen för att skapa och spara WebVTT-filen. När du är klar kopierar du bildtextfilens innehåll och klistrar in det i en vanlig textredigerare och sparar det med filnamnstillägget .vtt. <br><br><b>Obs!</b> Om du vill ha globalt stöd för videobeskrivningar på andra språk än engelska måste du tänka på att WebVTT-standarden kräver att du skapar separata VTT-filer och anropar varje språk som du vill ha stöd för. <br><br>I allmänhet vill du ge bildtexten ett namn som är detsamma som videofilen och bifoga den med bildtexter. Genom att göra det kan det hjälpa dig att automatisera genereringen av video-URL:er med ditt befintliga system för hantering av webbinnehåll. |

1. I Scene7 Publishing System överför du XML-bildtextfilen WebVTT, DFXP eller SMPTE.

   Se [Överföra filer](uploading-files.md#uploading_files).

1. Gå till resursmappen som innehåller den videofil som du vill associera med bildtextfilen som du överförde i panelen Resursbibliotek på vänster sida.
1. Markera en enskild videoresurs på panelen Resursbläddring och klicka sedan på **Förhandsvisa** > **Visningslista** nedanför miniatyrbilden av resursen.
1. I tabellen Viewer List kan du hitta HTML5-visningsprogrammet med namnet **Univeral_HTML5_Video**, **Universal_HTML5_MixedMedia_dark** eller **Universal_HTML5_MixedMedia_light** och sedan göra något av följande:

   * Om du vill visa en popup-video klickar du på **Kopiera URL** längst till höger om namnet.

      Lägg till den kopierade URL:en för videon med följande syntax för att associera den med den kopierade URL:en till bildtextfilen:

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      Anteckna `,1` i slutet av bildtextens URL-sökväg. Omedelbart efter tillägget .vtt i sökvägen kan du aktivera eller inaktivera den stängda bildtextknappen i videospelarfältet genom att ställa in på `1` respektive `0`.

   * Om du vill visa en inbäddad video klickar du på **Bädda in kod** längst till höger om namnet.

      I dialogrutan Bädda in kod klickar du på **Kopiera till Urklipp**.

      För HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark`eller `Universal_HTML5_MixedMedia_light` visningsprogram, lägger du till den kopierade inbäddningskoden med följande:

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      Lägg märke till `,1` slutet av URL-sökvägen. Omedelbart efter tillägget .vtt i URL-sökvägen kan du aktivera eller inaktivera bildtextknappen i videospelarfältet genom att ställa in på `1` respektive `0`.

