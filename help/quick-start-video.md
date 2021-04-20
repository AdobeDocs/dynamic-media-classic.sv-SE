---
title: '"Snabbstart: Video"'
description: En introduktion och snabbstart till Adobe Dynamic Media Classic Video som hjälper dig att komma igång snabbt.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '1448'
ht-degree: 0%

---


# Snabbstart: Video{#quick-start-video}

Adobe Dynamic Media Classic Video är en totallösning som gör det enkelt att publicera högkvalitativ adaptiv video för direktuppspelning på flera skärmar, inklusive datorer, iOS, Android, Blackberry och Windows-enheter. En adaptiv videouppsättning grupperar versioner av samma video som är kodade med olika bithastigheter och format som 400 kbit/s, 800 kbit/s och 1 000 kbit/s. Den stationära datorn eller mobila enheten känner av den tillgängliga bandbredden.

På en iOS-mobil enhet upptäcker den till exempel en bandbredd som 3G, 4G eller Wi-Fi. Sedan väljs automatiskt rätt kodad video bland de olika videobithastigheterna i den adaptiva videouppsättningen. Videon strömmas till datorer, mobila enheter eller surfplattor.

Dessutom ändras videokvaliteten dynamiskt automatiskt om nätverksförhållandena ändras på datorn eller den mobila enheten. Om en kund går över till helskärmsläge på en stationär dator svarar den adaptiva videouppsättningen med en bättre upplösning, vilket förbättrar kundens tittarupplevelse. Med adaptiva videouppsättningar får du bästa möjliga uppspelning för kunder som spelar upp Dynamic Media Classic-video på flera skärmar och enheter.

Den logik som en videospelare använder för att avgöra vilken kodad video som ska spelas upp eller väljas under uppspelningen baseras på följande algoritm:

1. Videospelaren läser in det inledande videofragmentet baserat på den bithastighet som ligger närmast värdet som är inställt för&quot;inledande bithastighet&quot; i spelaren.
1. Videospelaren växlar baserat på ändringar av bandbreddshastigheten med följande kriterier:

   1. Spelaren väljer den högsta bandbreddsströmmen under eller lika med den beräknade bandbredden.
   1. Spelaren hanterar bara 80 % av den tillgängliga bandbredden. Men om den byter upp sig är det mer konverteringsfullt, bara 70 %, för att undvika överskattning och omedelbart behöva byta tillbaka.

Se algoritmens logik på [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) för teknisk information om den.

För hantering av enstaka video och adaptiva videouppsättningar har Dynamic Media Classic stöd för följande:

* Överföra video från ett antal videoformat och ljudformat som stöds och koda video till MP4 H.264-format för uppspelning på flera skärmar. Du kan använda fördefinierade förinställningar för adaptiv video i Dynamic Media Classic, enskilda förinställningar för videokodning eller anpassa din egen kodning för att styra videons kvalitet och storlek.

   När en adaptiv videouppsättning genereras innehåller den MP4-videor.

   `**Note:**` Överordnad videoklipp, källvideoklipp och andra videofilmer i källformat läggs  ** inte till i en adaptiv videouppsättning.

* Bildtext för video i vyerna Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark och Universal_HTML5_MixedMedia_light samt kapitelnavigering i Univeral_HTML5_Video, Universal_HTML5_MixedMedia_dark och Universal_HTML5_MixedMedia_light.

   Se [Lägga till bildtexter i videon](adding-captions-video.md).

   Se [Lägga till kapitelmarkörer i video](adding-chapter-markers-video.md).

* Ordna, bläddra bland och sök videoklipp med fullt stöd för metadata för effektiv hantering av videomaterial.
* Leverera adaptiva videouppsättningar till webben, datorer och mobila enheter som iPhone, iPad, Android™, Blackberry och Windows Phone.

   Adaptiv videoströmning stöds på flera olika iOS-plattformar.

   Se det senaste stödet i [referenshandboken för visningsprogram för Adobe](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/home.html).

   Dynamic Media Classic har stöd för videouppspelning i mobiler för MP4 H.264-video. Blackberry-enheter som stöder det här videoformatet finns på följande webbplats:

   Se [Videoformat som stöds på Blackberry](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482).

   Windows-enheter som stöder det här videoformatet finns på följande plats:

   Se [Videoformat som stöds på Windows Phone](https://msdn.microsoft.com/en-us/library/ff462087(v=vs.92).aspx).

* Spela upp videon med Dynamic Media Classic Viewer Presets, inklusive följande:

   * Enstaka videovisningsprogram.
   * Visningsprogram för blandade media som kombinerar både video- och bildinnehåll.

* Konfigurera videospelare för att tillgodose era varumärkesbehov.
* Integrera video på webbplatsen, mobilsajten eller mobilapplikationen med en enkel URL eller inbäddningskod.

**Snabbstart**

Följande steg-för-steg-beskrivning av arbetsflödet hjälper dig att komma igång snabbt med anpassningsbara videouppsättningar i Dynamic Media Classic. Efter varje steg finns en korsreferens till en ämnesrubrik där du kan hitta mer information.

**1. Överföra och koda videofilmer**

Överför och generera adaptiva videouppsättningar i något av följande två scenarier:

* **Överför förkodade**
videoklippOm dina videoklipp redan har kodats utanför Dynamic Media Classic klickar du på 
**Ladda** upp på Global Navigation Bar för att bläddra bland och ladda upp MP4-videofiler direkt till Dynamic Media Classic. Klicka sedan på **Skapa > Adaptiva videouppsättningar**. Bläddra till videofilerna. Dra och släpp de videofiler du vill ha i tabellen Adaptiv videouppsättning och spara sedan uppsättningen.
* **Överför**
videoklipp med överordnad källkodOm dina videoklipp inte är kodade klickar du på 
**Ladda** upp på Global Navigation Bar för att ladda upp överordnad videokällfiler (ej MP4) och låt Dynamic Media Classic koda dem till MP4-filer. Välj **Adaptiv video** under EVideo-alternativ i dialogrutan Alternativ för överföringsjobb.

   Med det här önskade alternativet kan du skapa en adaptiv videouppsättning som automatiskt tillämpar rätt kodningsförinställning på videon, oavsett om den är 16:9 eller 4:3, för att matcha dimensionerna för videon som du överförde. När du skickar ditt överföringsjobb skapas automatiskt en adaptiv videouppsättning som innehåller tre videokoder i rätt proportioner.

   Du kan också utöka **Encoding Presets** under EVideo-alternativ i samma dialogruta för jobbalternativ och välja enskilda förinställningar för videokodning som du vill ha från **Skrivbord**, **Mobil (iPhone, iPad, Android)** och **Surfplatta (iPad, Android)** så att du kan skapa MP4-filer.

* Du kan också bearbeta om en överordnad video med hjälp av funktionen Bearbeta om. De nykodade videoklippen läggs till i den befintliga adaptiva videouppsättningen.

Se [Överföra och koda videofilmer](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Valfritt**

Dynamic Media Classic har flera fördefinierade videokodningsförinställningar. Dessa fördefinierade förinställningar återspeglar de vanligaste videokodningsinställningarna som används idag och är optimerade för uppspelning på målskärmar.

Om ytterligare anpassningar behövs kan dock administratörerna skapa videoförinställningar för att anpassa storleken och uppspelningen av videoklipp för slutanvändarna. Administratörer kan lägga till och hantera videoförinställningar från sidan Videoförinställningar som finns under Konfigurera > Programinställningar > Videoförinställningar > Enkla kodningsförinställningar. På sidan Videoförinställningar finns alternativ för att lägga till, redigera, ta bort och aktivera videoförinställningar.

Se [Arbeta med förinställningar för videokodning](uploading-encoding-videos.md#working_with_video_encoding_presets).

**2. Förhandsgranska videoklipp i ett videovisningsprogram**

Om du vill se hur en video spelas upp för slutanvändare på en dator, på webbplatsen eller på en mobil enhet väljer du videon i panelen Bläddra och klickar sedan på **Förhandsgranska**.

Se [Förhandsgranska videoklipp i ett videovisningsprogram](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

Du kan spela upp videon på förhandsgranskningsskärmen. Du kan också välja olika videovisningsprogram för att ta reda på hur videon ser ut i olika spelare. Det bästa sättet är att använda HTML5-videospelaren för uppspelning på datorer, surfplattor och mobila enheter.

**Valfritt**

Anpassning av visningsförinställningar - Dynamic Media Classic innehåller fördefinierade visningsförinställningar för video. Dessa förinställningar avgör hur visningsprogrammet ser ut och hur uppspelningskontrollerna fungerar. Administratörer kan lägga till och hantera visningsförinställningar från sidan Förinställningar för visningsprogram för att anpassa visningsprogrammet. Du öppnar den här sidan genom att klicka på Konfigurera > Visningsförinställningar i det övre högra hörnet av Dynamic Media Classic. På sidan Förinställningar för visningsprogram finns kommandon för att lägga till, redigera, ta bort och aktivera visningsförinställningar.

Se [Arbeta med förinställningar för visningsprogram för video](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

**3. Distribuera videor till webbplatser och mobilsajter**

Om du vill integrera video på webbplatsen kan du göra något av följande:

* Visa videon i ett eget popup-fönster eller modalt fönster. I så fall bör du använda funktionen Kopiera URL.

   Om du vill hämta URL-adressen för en video markerar du den i stödrastervyn eller listvyn på panelen Bläddra. Klicka på Förhandsgranska och sedan på Kopiera URL till höger om `Universal_HTML5_Viewer`.

   När du klickar på Kopiera URL kopieras URL-adressen till Urklipp. Placera den här koden i HTML-koden för webbplatsen, mobilwebbplatsen eller programmet.

   >[!NOTE]
   >
   >URL-adresser aktiveras först när du har publicerat videon eller den adaptiva videouppsättningen.

* Visa videon som är inbäddad på webbsidan. I så fall bör du använda funktionen Bädda in kod.

   Om du vill hämta inbäddningskoden för en video väljer du videon i Stödrastervisning eller Listvy på panelen Bläddra. Klicka på Förhandsgranska > Visningsprogramlista. Under åtgärdskolumnen i tabellen klickar du på Bädda in kod till höger om `Universal_HTML5_Video`. Det är inte tillåtet att redigera koden.

   Klicka på Stäng och klistra in inbäddningskoden på dina webbsidor.

   >[!NOTE]
   >
   >Inbäddningskoden aktiveras bara när du har publicerat videon eller den adaptiva videouppsättningen.

Se [Distribuera video till webbplatser och mobilsajter](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Bästa tillvägagångssätt för videokodning](uploading-encoding-videos.md#best_practices_for_video_encoding)

