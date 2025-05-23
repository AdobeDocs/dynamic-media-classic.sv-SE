---
title: 'Snabbstart: Video i Adobe Dynamic Media Classic'
description: En introduktion och snabbstart till Adobe Dynamic Media Classic Video som hjälper dig att komma igång snabbt.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
topic: Content Management
level: Beginner
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1395'
ht-degree: 0%

---

# Snabbstart: Video i Adobe Dynamic Media Classic{#quick-start-video}

Adobe Dynamic Media Classic Video är en totallösning som gör det enkelt att publicera högkvalitativ adaptiv video för direktuppspelning på flera skärmar, inklusive datorer, iOS, Android™, BlackBerry® och Windows®-mobilenheter. En adaptiv videouppsättning grupperar versioner av samma video som är kodade med olika bithastigheter och format som 400 kbit/s, 800 kbit/s och 1 000 kbit/s. Datorns eller mobilenhetens tillgängliga bandbredd identifieras.

På en mobilenhet från iOS identifieras t.ex. en bandbredd som 3G, 4G eller Wi-Fi. Sedan väljs automatiskt rätt kodad video bland de olika videobithastigheterna i den adaptiva videouppsättningen. Videon strömmas till datorer, mobila enheter eller surfplattor.

Dessutom ändras videokvaliteten dynamiskt automatiskt om nätverksförhållandena ändras på datorn eller den mobila enheten. Om en kund går över till helskärmsläge på en stationär dator svarar den adaptiva videouppsättningen med en bättre upplösning, vilket förbättrar kundens tittarupplevelse. Med adaptiva videouppsättningar får du bästa möjliga uppspelning. Det passar bäst för kunder som spelar Adobe Dynamic Media Classic Video på olika skärmar och enheter.

Den logik som en videospelare använder för att avgöra vilken kodad video som ska spelas upp eller väljas under uppspelningen baseras på följande algoritm:

1. Videospelaren läser in det inledande videofragmentet baserat på den bithastighet som ligger närmast värdet som är inställt för&quot;inledande bithastighet&quot; i själva spelaren.
1. Videospelaren växlar baserat på ändringar av bandbreddshastigheten med följande kriterier:

   1. Spelaren väljer den högsta bandbreddsströmmen under eller lika med den beräknade bandbredden.
   1. Spelaren hanterar bara 80 % av den tillgängliga bandbredden. Men om den byter upp sig är det mer försiktigt med bara 70 % för att undvika överskattning och omedelbart byta tillbaka.

Information om algoritmens logik finns på [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp).

För hantering av enstaka videor och adaptiva videouppsättningar har Adobe Dynamic Media Classic stöd för följande:

* Överföra video från flera videoformat som stöds. Och ladda upp ljudformat och koda video till MP4 H.264-format för uppspelning på flera skärmar. Du kan använda fördefinierade Adobe Dynamic Media Classic Adaptive Video-förinställningar, enskilda videokodningsförinställningar eller anpassa din egen kodning för att styra videons kvalitet och storlek.

Se [Aktivera eller inaktivera anpassade videoförinställningar](/help/using/application-setup.md#activating-or-deactivating-adaptive-video-presets)

Se även utbildningsvideon [Videoförinställningar](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS).

När en adaptiv videouppsättning genereras innehåller den MP4-videor.

>[!NOTE]
>
>Primära videoklipp/källvideoklipp och andra videofilmer i källformat läggs *inte* till i en adaptiv videouppsättning.

* Bildtext för video i vyerna Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark och Universal_HTML5_MixedMedia_light samt kapitelnavigering i visningsprogrammen Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark och Universal_HTML5_MixedMedia_light.

  Se [Lägga till bildtexter i en video](adding-captions-video.md).

  Se [Lägga till kapitelmarkörer i en video](adding-chapter-markers-video.md).

* Ordna, bläddra bland och sök videoklipp med fullt stöd för metadata för effektiv hantering av videomaterial.
* Leverera adaptiva videouppsättningar till webben, datorer och mobila enheter som iPhone, iPad, Android™, BlackBerry® och Windows®.

  Adaptiv videoströmning stöds på olika iOS-plattformar.

  Se det senaste stödet i [referenshandboken för visningsprogram för Adobe](https://experienceleague.adobe.com/sv/docs/dynamic-media-developer-resources).

  Adobe Dynamic Media Classic har stöd för videouppspelning i mobiler för MP4 H.264-video. <!-- LINK IS 404; NO SUITABLE REPLACEMENT WAS FOUND You can find BlackBerry&reg; devices that support this video format at the following website: -->

  <!-- See [Supported video formats on BlackBerry&reg;](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482). -->

  Följande Windows®-enheter har stöd för det här videoformatet:

  [Videoformat som stöds på Windows® Phone](https://learn.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs).

* Spela upp videon med Adobe Dynamic Media Classic Viewer Presets, inklusive följande:

   * Enstaka videoredigeringsprogram.
   * Visningsprogram för blandade media som kombinerar både video- och bildinnehåll.

* Konfigurera videospelare för att tillgodose era varumärkesbehov.
* Integrera video på en webbplats, mobilsajt eller mobilapplikation med en enkel URL eller Embed Code.

Se följande utbildningsvideor:
* [MP4 - videoöversikt](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/563_MP4%20Video%20Overview_converted%20renamed_eVideos-AVS)

* [Förhandsgranskning av MP4-video](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/564_MP4%20Video%20Preview_converted%20renamed_eVideos-AVS)

* [MP4-videoöverföring](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/565_MP4%20Video%20Upload_converted%20renamed_eVideos-AVS)

* [Översikt över direktuppspelning](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/567_Streaming%20Overview_master_eVideos_converted%20renamed_eVideos-AVS)

**Snabbstart**

Följande steg-för-steg-beskrivning av arbetsflödet hjälper dig att komma igång snabbt med adaptiva videouppsättningar i Adobe Dynamic Media Classic. Efter varje steg finns det en korsreferens till en ämnesrubrik där du kan hitta mer information.

## 1. Överför och koda videoklipp

Överför och generera adaptiva videouppsättningar i något av följande två scenarier:

* **Överför förkodade videoklipp**: Om dina videoklipp redan har kodats externt från Adobe Dynamic Media Classic väljer du **[!UICONTROL Upload]** i det globala navigeringsfältet. Bläddra och ladda upp MP4-videofiler direkt till Adobe Dynamic Media Classic. Gå sedan till **[!UICONTROL Build]** > **[!UICONTROL Adaptive Video Sets]**. Bläddra till dina videofiler. Dra och släpp de videofiler du vill ha i tabellen Adaptiv videouppsättning och spara sedan uppsättningen.
* **Överför primära källvideoklipp**: Om dina videoklipp inte är kodade väljer du **[!UICONTROL Upload]** i fältet Global navigering för att överföra primära videokällfiler (inte MP4). Adobe Dynamic Media Classic kodar dem till MP4-filer åt dig. Välj **[!UICONTROL Adaptive Video]** under **[!UICONTROL EVideo Options]** i dialogrutan **[!UICONTROL Upload Job Options]**.

  Med det här alternativet kan du skapa adaptiva videouppsättningar. Den korrekta kodningsförinställningen används automatiskt på videon, oavsett om den är 16:9 eller 4:3, för att matcha dimensionerna för den video som du överförde. När du skickar ditt överföringsjobb skapas automatiskt en adaptiv videouppsättning som innehåller tre videoinställningar med rätt proportioner.

  Eller expandera **[!UICONTROL Single Encoding Presets]** under **[!UICONTROL EVideo Options]** i samma **[!UICONTROL Job Options]**-dialogruta. Välj de enskilda förinställningar för videokodning som du vill använda. Du kan välja **Skrivbord**, **Mobil (iPhone, iPad, Android™)** och **Surfplatta (iPad, Android™)** om du vill skapa MP4-filer.

* Du kan också bearbeta om en primär video med funktionen **[!UICONTROL Reprocessing]**. De nykodade videoklippen läggs till i den befintliga adaptiva videouppsättningen.

Se [Överför och koda videoklipp](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Valfritt**

Adobe Dynamic Media Classic har många fördefinierade videokodningsförinställningar. Dessa fördefinierade förinställningar återspeglar de vanligaste videokodningsinställningarna som används idag och är optimerade för uppspelning på målsidor.

Om ytterligare anpassningar behövs kan dock administratörerna skapa videoförinställningar för att anpassa storleken och uppspelningen av videoklipp för slutanvändarna. Administratörer kan lägga till och hantera videoförinställningar från sidan Videoförinställningar som finns under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]** > **[!UICONTROL Single Encoding Presets]**. På sidan Videoförinställningar finns alternativ för att lägga till, redigera, ta bort och aktivera videoförinställningar.

Se [Arbeta med förinställningar för videokodning](uploading-encoding-videos.md#working_with_video_encoding_presets).

## 2. Förhandsgranska videoklipp i ett videovisningsprogram

Om du vill se hur en video spelas upp för slutanvändare på en dator, på din webbplats eller på en mobil enhet väljer du videon på panelen Bläddra. Välj sedan **[!UICONTROL Preview]**.

Se [Förhandsgranska videoklipp i ett videovisningsprogram](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

Du kan spela upp videon på förhandsgranskningssidan. Du kan också välja olika videovisningsprogram för att ta reda på hur videon visas i olika spelare. Det bästa sättet är att använda videospelaren HTML5 för uppspelning på datorer, surfplattor och mobila enheter.

**Valfritt**

Anpassning av visningsförinställningar: Adobe Dynamic Media Classic har fördefinierade visningsförinställningar för videoutgång. Dessa förinställningar avgör hur visningsprogrammet ser ut och hur uppspelningskontrollerna fungerar. Administratörer kan lägga till och hantera visningsförinställningar från sidan Förinställningar för visningsprogram för att anpassa visningsprogrammet. Om du vill öppna den här sidan går du till **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]** i det övre högra hörnet av Adobe Dynamic Media Classic. På sidan Förinställningar för visningsprogram finns kommandon för att lägga till, redigera, ta bort och aktivera visningsförinställningar.

Se [Arbeta med förinställningar för visningsprogram för video](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

Se även utbildningsvideon [Videoförinställningar](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS).

## 3. Lägg ut videor på webbplatser och mobilsajter

Om du vill integrera video på webbplatsen kan du göra något av följande:

* Visa videon i ett eget popup-fönster eller modalt fönster. I så fall använder du funktionen **[!UICONTROL Copy URL]**.

  Om du vill hämta URL-adressen för en video markerar du den i stödrastervyn eller listvyn på panelen Bläddra. Välj **[!UICONTROL Preview]** och välj sedan **[!UICONTROL Copy URL]** till höger om `Universal_HTML5_Viewer`.

  När du väljer **[!UICONTROL Copy URL]** kopieras URL:en till Urklipp. Placera den här koden HTML på din webbplats, mobilwebbplats eller i ditt program.

  >[!NOTE]
  >
  >URL-adresser aktiveras först när du har publicerat videon eller den adaptiva videouppsättningen.

* Visa videon som är inbäddad på webbsidan. I så fall använder du funktionen **[!UICONTROL Embed Code]**.

  Om du vill hämta inbäddningskoden för en video väljer du videon i Stödrastervisning eller Listvy på panelen Bläddra. Gå till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**. Under åtgärdskolumnen i tabellen väljer du **[!UICONTROL Embed Code]** till höger om `Universal_HTML5_Video`. Det är inte tillåtet att redigera koden.

  Markera **[!UICONTROL Close]** och klistra in den inbäddade koden på en eller flera av dina webbsidor.

  >[!NOTE]
  >
  >Inbäddningskoden aktiveras först när du har publicerat videon eller den adaptiva videouppsättningen.

Se [Distribuera video till webbplatser och mobilwebbplatser](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Bästa tillvägagångssätt för videokodning](uploading-encoding-videos.md#best_practices_for_video_encoding)
