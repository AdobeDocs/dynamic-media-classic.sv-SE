---
title: "Snabbstart: Video i Adobe Dynamic Media Classic"
description: En introduktion och snabbstart till Adobe Dynamic Media Classic Video som hjälper dig att komma igång snabbt.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
source-git-commit: 38d7f8d6e5888e1c5ba9260ada45b79fb16b338f
workflow-type: tm+mt
source-wordcount: '1760'
ht-degree: 0%

---

# Snabbstart: Video i Adobe Dynamic Media Classic{#quick-start-video}

Adobe Dynamic Media Classic Video är en totallösning som gör det enkelt att publicera högkvalitativ adaptiv video för direktuppspelning på flera skärmar, inklusive datorer, iOS, Android™, BlackBerry® och Windows®-mobilenheter. En adaptiv videouppsättning grupperar versioner av samma video som är kodade med olika bithastigheter och format som 400 kbit/s, 800 kbit/s och 1 000 kbit/s. Den stationära datorn eller mobila enheten känner av den tillgängliga bandbredden.

På en mobilenhet från iOS identifieras t.ex. en bandbredd som 3G, 4G eller Wi-Fi. Sedan väljs automatiskt rätt kodad video bland de olika videobithastigheterna i den adaptiva videouppsättningen. Videon strömmas till datorer, mobila enheter eller surfplattor.

Dessutom ändras videokvaliteten dynamiskt automatiskt om nätverksförhållandena ändras på datorn eller den mobila enheten. Om en kund går över till helskärmsläge på en stationär dator svarar den adaptiva videouppsättningen med en bättre upplösning, vilket förbättrar kundens tittarupplevelse. Med adaptiva videouppsättningar får du bästa möjliga uppspelning för kunder som spelar upp Adobe Dynamic Media Classic-video på flera skärmar och enheter.

Den logik som en videospelare använder för att avgöra vilken kodad video som ska spelas upp eller väljas under uppspelningen baseras på följande algoritm:

1. Videospelaren läser in det inledande videofragmentet baserat på den bithastighet som ligger närmast värdet som är inställt för&quot;inledande bithastighet&quot; i spelaren.
1. Videospelaren växlar baserat på ändringar av bandbreddshastigheten med följande kriterier:

   1. Spelaren väljer den högsta bandbreddsströmmen under eller lika med den beräknade bandbredden.
   1. Spelaren hanterar bara 80 % av den tillgängliga bandbredden. Men om den byter upp sig är det mer konservativt med bara 70 % för att undvika överskattning och omedelbart behöva byta tillbaka.

Se algoritmens logik på [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) för teknisk information om det.

För hantering av enstaka video och adaptiva videouppsättningar har Adobe Dynamic Media Classic stöd för följande:

* Överföra video från ett stort antal videoformat och ljudformat som stöds samt koda video till MP4 H.264-format för uppspelning på flera skärmar. Du kan använda fördefinierade videoförinställningar för Adobe Dynamic Media Classic, enskilda videokodningsförinställningar eller anpassa din egen kodning för att styra videons kvalitet och storlek.

Se [Aktivera eller inaktivera anpassade videoförinställningar](/help/using/application-setup.md#activating-or-deactivating-adaptive-video-presets)

Se även [Videoförinställningar](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) utbildningsvideo.

När en adaptiv videouppsättning genereras innehåller den MP4-videor.

>[!NOTE]
>
>Primära videoklipp/källvideoklipp och annan video i källformat är *not* läggs till i en adaptiv videouppsättning.

* Bildtext för video i vyerna Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark och Universal_HTML5_MixedMedia_light samt kapitelnavigering i visningsprogrammen Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark och Universal_HTML5_MixedMedia_light.

   Se [Lägga till bildtexter i video](adding-captions-video.md).

   Se [Lägga till kapitelmarkörer i video](adding-chapter-markers-video.md).

* Ordna, bläddra bland och sök videoklipp med fullt stöd för metadata för effektiv hantering av videomaterial.
* Leverera adaptiva videouppsättningar till webben, datorer och mobila enheter som iPhone, iPad, Android™, BlackBerry® och Windows®.

   Adaptiv videoströmning stöds på olika iOS-plattformar.

   Se den senaste supporten i [Referenshandbok för Adobe-visningsprogram](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html).

   Adobe Dynamic Media Classic har stöd för videouppspelning i mobiler för MP4 H.264-video. Du kan hitta BlackBerry®-enheter som stöder det här videoformatet på följande webbplats:

   Se [Videoformat som stöds på BlackBerry®](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482).

   Följande Windows®-enheter har stöd för det här videoformatet:

   Se [Videoformat som stöds på Windows® Phone](https://docs.microsoft.com/en-us/).

* Spela upp videon med Adobe Dynamic Media Classic Viewer Presets, inklusive följande:

   * Enstaka videovisningsprogram.
   * Visningsprogram för blandade media som kombinerar både video- och bildinnehåll.

* Konfigurera videospelare för att tillgodose era varumärkesbehov.
* Integrera video på webbplatsen, mobilsajten eller mobilapplikationen med en enkel URL eller inbäddningskod.

Se följande utbildningsvideor:
* [MP4 - videoöversikt](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/563_MP4%20Video%20Overview_converted%20renamed_eVideos-AVS)

* [Förhandsgranskning av MP4-video](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/564_MP4%20Video%20Preview_converted%20renamed_eVideos-AVS)

* [MP4-videouppladdning](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/565_MP4%20Video%20Upload_converted%20renamed_eVideos-AVS)

* [Översikt över direktuppspelning](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/567_Streaming%20Overview_master_eVideos_converted%20renamed_eVideos-AVS)

**Snabbstart**

Följande steg-för-steg-beskrivning av arbetsflödet hjälper dig att komma igång snabbt med anpassningsbara videouppsättningar i Adobe Dynamic Media Classic. Efter varje steg finns det en korsreferens till en ämnesrubrik där du kan hitta mer information.

## 1. Överföra och koda videoklipp

Överför och generera adaptiva videouppsättningar i något av följande två scenarier:

* **Överför förkodade videoklipp** - Om dina videoklipp redan har kodats utanför Adobe Dynamic Media Classic väljer du **[!UICONTROL Upload]** för att bläddra bland och ladda upp MP4-videofiler direkt till Adobe Dynamic Media Classic. Gå sedan till **[!UICONTROL Build]** > **[!UICONTROL Adaptive Video Sets]**. Bläddra till videofilerna. Dra och släpp de videofiler du vill ha i tabellen Adaptiv videouppsättning och spara sedan uppsättningen.
* **Överför primära källvideor** - Om videoklippen inte är kodade väljer du **[!UICONTROL Upload]** för att överföra primära videokällfiler (ej MP4). Adobe Dynamic Media Classic kodar dem till MP4-filer åt dig. I **[!UICONTROL Upload Job Options]** dialogruta, under **[!UICONTROL EVideo Options]**, markera **[!UICONTROL Adaptive Video]**.

   Med det här önskade alternativet kan du skapa en adaptiv videouppsättning som automatiskt tillämpar rätt kodningsförinställning på videon, oavsett om den är 16:9 eller 4:3, för att matcha dimensionerna för videon som du överförde. När du skickar ditt överföringsjobb skapas automatiskt en adaptiv videouppsättning som innehåller tre videoinställningar med rätt proportioner.

   Eller i samma **[!UICONTROL Job Options]** dialogruta, under **[!UICONTROL EVideo Options]**, expandera **[!UICONTROL Single Encoding Presets]**. Välj enskilda förinställningar för videokodning som du vill använda **Skrivbord**, **Mobil (iPhone, iPad, Android™)** och **Surfplatta (iPad, Android™)** så att du kan skapa MP4-filer.

* Du kan också bearbeta om en primär video med **[!UICONTROL Reprocess]** -funktion. De nykodade videoklippen läggs till i den befintliga adaptiva videouppsättningen.

Se [Överföra och koda videoklipp](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Valfritt**

Adobe Dynamic Media Classic har många fördefinierade videokodningsförinställningar. Dessa fördefinierade förinställningar återspeglar de vanligaste videokodningsinställningarna som används idag och är optimerade för uppspelning på målsidor.

Om ytterligare anpassningar behövs kan dock administratörerna skapa videoförinställningar för att anpassa storleken och uppspelningen av videoklipp för slutanvändarna. Administratörer kan lägga till och hantera videoförinställningar från sidan Videoförinställningar som finns under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]** > **[!UICONTROL Single Encoding Presets]**. På sidan Videoförinställningar finns alternativ för att lägga till, redigera, ta bort och aktivera videoförinställningar.

Se [Arbeta med förinställningar för videokodning](uploading-encoding-videos.md#working_with_video_encoding_presets).

## 2. Förhandsgranska videoklipp i ett videovisningsprogram

Om du vill se hur en video spelas upp för slutanvändare på en dator, på din webbplats eller på en mobil enhet väljer du videon i panelen Bläddra och sedan väljer du **[!UICONTROL Preview]**.

Se [Förhandsgranska videoklipp i ett videovisningsprogram](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

Du kan spela upp videon på förhandsgranskningssidan. Du kan också välja olika videovisningsprogram för att ta reda på hur videon visas i olika spelare. Det bästa sättet är att använda videospelaren HTML5 för uppspelning på datorer, surfplattor och mobila enheter.

**Valfritt**

Anpassning av visningsförinställningar - Adobe Dynamic Media Classic har fördefinierade visningsförinställningar för videoutgång. Dessa förinställningar avgör hur visningsprogrammet ser ut och hur uppspelningskontrollerna fungerar. Administratörer kan lägga till och hantera visningsförinställningar från sidan Förinställningar för visningsprogram för att anpassa visningsprogrammet. Om du vill öppna den här sidan går du till **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**. På sidan Förinställningar för visningsprogram finns kommandon för att lägga till, redigera, ta bort och aktivera visningsförinställningar.

Se [Arbeta med förinställningar för visningsprogram för video](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

Se även [Videoförinställningar](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) utbildningsvideo.

## 3. Distribuera videor till webbplatser och mobilsajter

Om du vill integrera video på webbplatsen kan du göra något av följande:

* Visa videon i ett eget popup-fönster eller modalt fönster, i vilket fall använder du **[!UICONTROL Copy URL]** -funktion.

   Om du vill hämta URL-adressen för en video markerar du den i stödrastervyn eller listvyn på panelen Bläddra. Välj **[!UICONTROL Preview]** och sedan markera **[!UICONTROL Copy URL]** till höger om `Universal_HTML5_Viewer`.

   När du väljer **[!UICONTROL Copy URL]**, kopieras URL-adressen till Urklipp. Placera den här koden HTML på din webbplats, mobilwebbplats eller i ditt program.

   >[!NOTE]
   >
   >URL-adresser aktiveras först när du har publicerat videon eller den adaptiva videouppsättningen.

* Visa videon som är inbäddad på webbsidan. I så fall använder du **[!UICONTROL Embed Code]** -funktion.

   Om du vill hämta inbäddningskoden för en video väljer du videon i Stödrastervisning eller Listvy på panelen Bläddra. Gå till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**. Under kolumnen Åtgärder i tabellen väljer du **[!UICONTROL Embed Code]** till höger om `Universal_HTML5_Video`. Det är inte tillåtet att redigera koden.

   Välj **[!UICONTROL Close]** och klistra in inbäddningskoden på dina webbsidor.

   >[!NOTE]
   >
   >Inbäddningskoden aktiveras bara när du har publicerat videon eller den adaptiva videouppsättningen.

Se [Distribuera video till webbplatser och mobilsajter](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Bästa tillvägagångssätt för videokodning](uploading-encoding-videos.md#best_practices_for_video_encoding)

