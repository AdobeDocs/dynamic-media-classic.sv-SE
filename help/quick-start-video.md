---
title: '"Snabbstart: Video"'
seo-title: '"Snabbstart: Video"'
description: 'null'
seo-description: En introduktion och Snabbstart till video som hjälper dig att komma igång snabbt.
uuid: bf0ecf87-a1f2-4e83-8041-df5192dd26a1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 6cef541b-e9df-48eb-9a16-ca3e1f07238e
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

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

Information om algoritmens logik finns på [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) .

Dynamic Media Classic kan hantera enstaka videoklipp och adaptiva videouppsättningar på följande sätt:

* Överföra video från ett antal videoformat och ljudformat som stöds och koda video till MP4 H.264-format för uppspelning på flera skärmar. Du kan använda fördefinierade dynamiska Media Classic-anpassade videoförinställningar, enskilda videokodningsförinställningar eller anpassa din egen kodning för att styra videons kvalitet och storlek.

   När en adaptiv videouppsättning genereras innehåller den MP4-videor.

   `**Note:**` Huvud-/källvideor och andra videofilmer i källformat läggs *inte* till i en adaptiv videouppsättning.

* Bildtext för video i vyerna Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark och Universal_HTML5_MixedMedia_light samt kapitelnavigering i Univeral_HTML5_Video, Universal_HTML5_MixedMedia_dark och Universal_HTML5_MixedMedia_light.

   Se [Lägga till bildtexter till video](adding-captions-video.md).

   Se [Lägga till kapitelmarkörer i video](adding-chapter-markers-video.md).

* Ordna, bläddra bland och sök videoklipp med fullt stöd för metadata för effektiv hantering av videomaterial.
* Leverera adaptiva videouppsättningar till webben, datorer och mobila enheter som iPhone, iPad, Android™, Blackberry och Windows Phone.

   Adaptiv videoströmning stöds på flera olika iOS-plattformar.

   Se det senaste stödet i [Adobe Viewer Reference Guide](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/).

   Dynamic Media Classic har stöd för videouppspelning på mobiler för MP4 H.264-video. Blackberry-enheter som stöder det här videoformatet finns på följande webbplats:

   Se [Videoformat som stöds på Blackberry](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482).

   Windows-enheter som stöder det här videoformatet finns på följande plats:

   Se [Videoformat som stöds på Windows Phone](https://msdn.microsoft.com/en-us/library/ff462087(v=vs.92).aspx).

* Spela upp videon med Dynamic Media Classic Viewer Presets, bland annat följande:

   * Enstaka videovisningsprogram.
   * Visningsprogram för blandade media som kombinerar både video- och bildinnehåll.

* Konfigurera videospelare för att tillgodose era varumärkesbehov.
* Integrera video på webbplatsen, mobilsajten eller mobilapplikationen med en enkel URL eller inbäddningskod.

**Snabbstart**

Följande steg-för-steg-beskrivning av arbetsflödet hjälper dig att komma igång snabbt med adaptiva videouppsättningar i Dynamic Media Classic. Efter varje steg finns en korsreferens till en ämnesrubrik där du kan hitta mer information.

**1. Överföra och koda videofilmer**

Överför och generera adaptiva videouppsättningar i något av följande två scenarier:

* **Ladda upp förkodade videor** Om dina videor redan har kodats utanför Dynamic Media Classic klickar du på **Överför** i det globala navigeringsfältet för att bläddra och överföra MP4-videofiler direkt till Scene7 Publishing System. Klicka sedan på **Skapa > Adaptiva videouppsättningar**. Bläddra till videofilerna. Dra och släpp de videofiler du vill ha i tabellen Adaptiv videouppsättning och spara sedan uppsättningen.
* **Överför huvudkällvideor** Om videoklippen inte är kodade klickar du på **Överför** i fältet Global Navigation (Global Navigation) för att överföra huvudvideokällfiler (ej MP4) och låta Scene7 Publishing System koda dem till MP4-filer. Välj **Adaptiv video** under EVideo-alternativ i dialogrutan Alternativ för överföringsjobb.

   Med det här önskade alternativet kan du skapa en adaptiv videouppsättning som automatiskt tillämpar rätt kodningsförinställning på videon, oavsett om den är 16:9 eller 4:3, för att matcha dimensionerna för videon som du överförde. När du skickar ditt överföringsjobb skapas automatiskt en adaptiv videouppsättning som innehåller tre videokoder i rätt proportioner.

   Du kan också utöka **Encoding Presets** i dialogrutan Jobbalternativ under EVideo-alternativ och välja enskilda förinställningar för videokodning som du vill ha från **Skrivbord**, **Mobil (iPhone, iPad, Android)** och **Surfplatta (iPad, Android)** så att du kan skapa MP4-filer.

* Du kan också bearbeta en huvudvideo på nytt med hjälp av funktionen Bearbeta igen. De nykodade videoklippen läggs till i den befintliga adaptiva videouppsättningen.

Se [Överföra och koda videofilmer](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Valfritt**

Dynamic Media Classic har många fördefinierade förinställningar för videokodning. Dessa fördefinierade förinställningar återspeglar de vanligaste videokodningsinställningarna som används idag och är optimerade för uppspelning på målskärmar.

Om ytterligare anpassningar behövs kan dock administratörerna skapa videoförinställningar för att anpassa storleken och uppspelningen av videoklipp för slutanvändarna. Administratörer kan lägga till och hantera videoförinställningar från sidan Videoförinställningar som finns under Konfigurera > Programinställningar > Videoförinställningar > Enkla kodningsförinställningar. På sidan Videoförinställningar finns alternativ för att lägga till, redigera, ta bort och aktivera videoförinställningar.

Se [Arbeta med förinställningar](uploading-encoding-videos.md#working_with_video_encoding_presets)för videokodning.

**2. Förhandsgranska videoklipp i ett videovisningsprogram**

Om du vill se hur en video spelas upp för slutanvändare på en dator, på din webbplats eller på en mobil enhet väljer du videon i panelen Bläddra och klickar sedan på **Förhandsgranska**.

Se [Förhandsgranska videoklipp i ett videovisningsprogram](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

Du kan spela upp videon på förhandsgranskningsskärmen. Du kan också välja olika videovisningsprogram för att ta reda på hur videon ser ut i olika spelare. Det bästa sättet är att använda HTML5-videospelaren för uppspelning på datorer, surfplattor och mobila enheter.

**Valfritt**

Anpassning av visningsförinställningar - Dynamic Media Classic erbjuder fördefinierade visningsförinställningar för videouppspelning. Dessa förinställningar avgör hur visningsprogrammet ser ut och hur uppspelningskontrollerna fungerar. Administratörer kan lägga till och hantera visningsförinställningar från sidan Förinställningar för visningsprogram för att anpassa visningsprogrammet. Om du vill öppna den här sidan klickar du på Inställningar > Visningsförinställningar i det övre högra hörnet av Scene7 Publishing System. På sidan Förinställningar för visningsprogram finns kommandon för att lägga till, redigera, ta bort och aktivera visningsförinställningar.

Se [Arbeta med förinställningar](previewing-videos-video-viewer.md#working_with_video_viewer_presets)för visningsprogram för video.

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

