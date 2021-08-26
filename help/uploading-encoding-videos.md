---
title: Överföra och koda videofilmer
seo-title: Uploading and encoding videos
description: Lär dig hur du överför och kodar videofilmer.
seo-description: Learn how to upload and encode videos.
uuid: 9a7d6513-b10c-40b0-aebb-18a795c2b8d1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: a0941823-850c-4373-9e37-f32032de3805
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 93ad91d7-f3dd-484b-b62c-633fcb864bbf
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '3789'
ht-degree: 1%

---

# Överföra och koda videofilmer{#uploading-and-encoding-videos}

Om du vill skapa en enda video eller adaptiva videouppsättningar för webben eller mobila enheter måste du först överföra dina överordnad videofiler till Adobe Dynamic Media Classic. Adobe Dynamic Media Classic kodar videoklipp till MP4-format och publicerar videoklipp i följande filformat:

* **MP4** - Adobe Dynamic Media Classic rekommenderar MP4 som det videofilformat du föredrar. Använd MP4-filer för följande:

   * HTTP Dynamic Streaming på stationära datorer.
   * HTTP Live Streaming (Apples direktuppspelningsprotokoll).
   * Progressiv leverans av video till mobila enheter med Android™, BlackBerry® och Windows®

   Adobe Dynamic Media Classic har två arbetsflöden för att överföra videofiler:

* **Förkodade videoklipp**  - Du kan överföra MP4-filer direkt till Adobe Dynamic Media Classic. Med det här arbetsflödet kodas inte filer när du överför dem. Filerna är förkodade för att kunna skickas till datorn och till mobila enheter.

* **Överordnad källvideor**  - Ladda upp överordnad källvideofiler och koda dessa filer till MP4-filer när de överförs. Kodade videor får etiketten&quot;Video&quot; i panelen Bläddra. Adobe Dynamic Media Classic har stöd för kodning av videofiler i många format.

   * Kontrollera att de överordnad källvideofiler som du vill koda stöds.

      Se [Videofiltyper som stöds för kodning](uploading-encoding-videos.md#supported-video-file-types-for-encoding).

   * Välj en förinställning för videokodning.

      Se [Videoförinställningar för kodning av videofiler](application-setup.md#video-presets-for-encoding-video-files).

      Se [Bästa tillvägagångssätt för videokodning](uploading-encoding-videos.md#best-practices-for-video-encoding).

Adobe Dynamic Media Classic genererar även videominiatyrer. Du kan lära dig mer om videominiatyrbilder, hur du hämtar deras URL-adresser och ändrar affischramar.

Se [Arbeta med videominiatyrer](deploying-video-websites-mobile-sites.md#working-with-video-thumbnails).

**Så här överför och kodar du videoklipp:**

Gör något av följande.

*Om dina videoklipp redan är kodade*

1. Klicka på **[!UICONTROL Upload]** i fältet Global navigering.
1. Klicka på fliken **[!UICONTROL From Desktop]** på sidan Överför.
1. På sidan Överför klickar du på **[!UICONTROL Select Files for Upload]** på panelen **[!UICONTROL Browse]**, navigerar till en MP4-videofil och klickar sedan på **[!UICONTROL Open]**.
1. Välj en mapp för den överförda filen på panelen **[!UICONTROL Choose Folder Destination]**.
1. Kontrollera att **[!UICONTROL Publish After Uploading]** är markerat på sidan Överför.
1. Klicka på **[!UICONTROL Submit Upload]**.

*Om du vill koda videofilmer med Adobe Dynamic Media Classic*

1. Klicka på **[!UICONTROL Upload]** i fältet Global navigering.
1. Klicka på fliken **[!UICONTROL From Desktop]** på sidan Överför.
1. I panelen **[!UICONTROL Select Files to Upload]** klickar du på **[!UICONTROL Browse]**, navigerar till en överordnad källvideofil och klickar sedan på **[!UICONTROL Open]**.
1. Välj en mapp för den överförda filen på panelen **[!UICONTROL Choose Folder Destination]**.
1. I sidans nedre högra hörn klickar du på **[!UICONTROL Job Options]**,
1. Expandera **[!UICONTROL EVideo Options]** i dialogrutan Alternativ för överföringsjobb och gör sedan något av följande:

   * Det bästa sättet är att välja **[!UICONTROL Adaptive Video Encoding]**. Se [Adaptiv video (standard)](application-setup.md#adaptive-video-default).
   * Valfritt. Om du vill använda enskilda kodningsinställningar expanderar du **[!UICONTROL Single Encoding Presets]** och väljer sedan de kodningsalternativ du vill använda för Skrivbord, Mobil och Surfplatta.
Se [Förinställningar för videokodning för datorer](application-setup.md#desktop-video-encoding-presets), [Förinställningar för videokodning för mobiler](application-setup.md#mobile-video-encoding-presets), [Videokodningsförinställningar för surfplattor](application-setup.md#tablet-video-encoding-presets).
1. Klicka på **[!UICONTROL Save]** i dialogrutan Alternativ för överföringsjobb.
1. Kontrollera att **[!UICONTROL Publish After Uploading]** är markerat på sidan Överför.
1. Klicka på **[!UICONTROL Submit Upload]** längst ned till höger på sidan Överför.

*Om du vill koda om en videofil som du överfört tidigare*

1. I Adobe Dynamic Media Classic navigerar du till videon i panelen Bläddra och markerar den.
1. Klicka på **[!UICONTROL File]** > **[!UICONTROL Reprocess]**.
1. Expandera **[!UICONTROL EVideo Options]** i dialogrutan Bearbeta resurser och gör sedan något av följande:
   * Det bästa sättet är att använda följande metod. Välj **Adaptiv video**.
Se [Adaptiv video (standard)](application-setup.md#adaptive-video-default).
   * Valfritt. Om du vill använda enskilda kodningsinställningar expanderar du ****[!UICONTROL Single Encoding Presets]**** och väljer sedan de kodningsalternativ du vill använda för Skrivbord, Mobil och Surfplatta.
Se [Förinställningar för videokodning för datorer](application-setup.md#desktop-video-encoding-presets), [Förinställningar för videokodning för mobiler](application-setup.md#mobile-video-encoding-presets), [Videokodningsförinställningar för surfplattor](application-setup.md#tablet-video-encoding-presets).
1. Klicka på **[!UICONTROL Submit]** i dialogrutan Bearbeta resurser.

När du använder förinställningen Adaptiv videokodning eller använder flera kodningsförinställningar blir resultatet en adaptiv videouppsättning som automatiskt skapas med flera videokodningar. Du kan också skapa en adaptiv videouppsättning manuellt genom att markera enskilda videoklipp.

Endast MP4- och M4V-filtyper skapas när du genererar en adaptiv videouppsättning automatiskt eller manuellt.

## Videofiltyper som stöds för kodning {#supported-video-file-types-for-encoding}

I följande tabell visas videofiltyper (med tillåtna videokodekar) som du kan koda till MP4- eller OGV-format när du överför filer. I tabellen visas filformat och kodekar:

* **Videofilformat**  - På samma sätt som en ZIP-fil avgör videofilformatet hur filerna finns i videofilen. En videofil innehåller vanligtvis flera spår - ett videospår (utan ljud) och ett eller flera ljudspår (utan video) - som är sammankopplade och synkroniserade. Videofilformatet avgör hur dessa olika dataspår och metadata ordnas.

* **Videokodekar**  - En videokodek beskriver den algoritm som en video kodas med. En videospelare avkodar videon enligt dess kodek och visar sedan en serie bilder, eller bildrutor, på skärmen. Kodekar minimerar mängden information som videofiler behöver för att kunna lagra videon. I stället för information om varje enskild bildruta sparas bara information om skillnaderna mellan en bildruta och nästa. Eftersom de flesta videoklipp inte ändras så mycket från en bildruta till nästa, kan du använda codecenheter för hög komprimeringshastighet, vilket ger mindre filstorlekar.

   | Videofilformat | Videokodekar |
   |:--- |:--- |
   | 3GP | H.263, H.264 |
   | AVI | DivX, DV |
   | M2P | MPEG-2 PS |
   | M2T | MPEG-2 TS |
   | M2TS | MPEG-2 TS |
   | M2V | MPEG-2 ES |
   | M4V | H.264 |
   | MOV | DV, DVCPro 50, H.261, H.263, H.264, Sorenson Video 1 |
   | MP4 | H.264/MPEG-4 AVC |
   | MPEG | MPEG-2 SS |
   | MPG | MPEG-2 SS |
   | MTS | MPEG-2 |
   | ProRes | APCN, APCS, APCO, APCH, AP4H |
   | TS | DVCPro 50 |
   | VOB | MPEG-2 |
   | WMV/ASF | VC-1, Windows® Media Video 7, Windows® Media Video 8 |

   >[!NOTE]
   >
   >På jobbskärmen visas ett varningsmeddelande om du överför och försöker koda en videofil, men filen avvisas eftersom den innehåller en inkompatibel kodek eller filbehållare. Mer information finns i [Kontrollera jobbfiler](checking-job-files.md).

## Bästa tillvägagångssätt för videokodning {#best-practices-for-video-encoding}

Nedan följer några tips om hur du kodar källvideofiler i Adobe Dynamic Media Classic.

<!-- THE FOLLOWINGS LINKS APPEAR TO BE DEAD AND THE CONTENT COMPLETELY LOST. THE GO URL DOESN'T EVEN WORK ANYMORE.
For advice about video encoding, see the following:

* Article: [Streaming 101: The Basics — Codecs, Bandwidth, Data Rate, and Resolution][www.adobe.com/go/learn_s7_streaming101_en](https://www.adobe.com/go/learn_s7_streaming101_en). THIS MATERIAL WAS FOUND ON A THIRD PARTY WEBSITE HERE: https://streaminglearningcenter.com/articles/streaming-101-the-basics-codecs-bandwidth-data-rate-and-resolution.html MATERIAL IS GOOD BUT DO NOT LINK TO IT
* Video: [Video Encoding Basics][www.adobe.com/go/learn_s7_encoding_en](https://www.adobe.com/go/learn_s7_encoding_en). -->

### Källvideofiler {#source-video-files}

När du kodar en videofil ska du använda en källvideofil med högsta möjliga kvalitet. Undvik att använda tidigare kodade videofiler eftersom dessa filer redan är komprimerade, och ytterligare kodning skapar en video med delkvalitet.

I följande tabell beskrivs rekommenderad storlek, proportioner och lägsta bithastighet som källvideofilerna måste ha när du kodar dem:

| Storlek | Proportioner | Minsta bithastighet |
|--- |--- |--- |
| 1024 x 768 | 4:3 | 4 500 kbit/s för de flesta videoklipp. |
| 1280 x 720 | 16:9 | 3 000 - 6 000 kbit/s, beroende på mängden rörelse i videon. |
| 1920 x 1080 | 16:9 | 6000 - 8 000 kbit/s, beroende på mängden rörelse i videon. |

### Hämta metadata för en fil {#obtaining-a-file-s-metadata}

Du kan hämta metadata för en fil genom att visa dess metadata i Adobe Dynamic Media Classic, med ett videoredigeringsverktyg eller med ett program som utformats för att hämta metadata. Nedan följer instruktioner om hur du använder MediaInfo, ett tredjepartsprogram, för att hämta videofilens metadata:

1. Gå till den här webbsidan: [https://mediainfo.sourceforge.net/en/Download](https://mediainfo.sourceforge.net/en/Download).
1. Välj och hämta installationsprogrammet för den grafiska användargränssnittsversionen och följ installationsanvisningarna.
1. Efter installationen högerklickar du på videofilen (endast Windows®) och väljer MediaInfo, eller så öppnar du MediaInfo och drar videofilen till programmet. Alla metadata som är associerade med videofilen, inklusive bredd, höjd och fps, visas.

### Proportioner {#aspect-ratio}

När du väljer eller skapar en förinställning för videokodning för den överordnad videofilen måste du se till att förinställningen har samma proportioner som den överordnad videofilen. *proportionen* är proportionerna mellan bredden och höjden på videon.

Om du vill ta reda på videofilens proportioner hämtar du filens metadata och noterar filens bredd och höjd (se [Hämta filens metadata](uploading-encoding-videos.md#obtaining_a_file_s_metadata)). Använd sedan den här formeln för att bestämma proportionerna:

width/height = aspect ratio

I följande tabell beskrivs hur formelresultaten översätts till vanliga alternativ för proportioner:

| Formelresultat | Proportioner |
|--- |--- |
| 1,33 | 4:3 |
| 0,75 | 3:4 |
| 1,78 | 16:9 |
| 0,56 | 9:16 |

En video som till exempel är 1440 bredd x 1080 höjd har proportionerna 1440/1080 eller 1,33. I det här fallet väljer du en förinställning för videokodning med 4:3-proportioner för att koda videofilen.

### Datahastighet {#data-rate}

Datahastigheten ** (kallas även *bithastighet*) är den datahastighet som kodas för att skapa en enda sekund av videouppspelning. Datahastigheten mäts i kilobit per sekund (kbit/s).

>[!NOTE]
>
>Eftersom förlustgivande komprimering används för alla kodekar är datahastigheten den viktigaste faktorn i videokvaliteten. Ju mer du komprimerar en videofil desto sämre blir kvaliteten. Därför är alla andra egenskaper lika (upplösning, bildrutefrekvens och kodek), ju lägre datahastighet, desto lägre kvalitet får den komprimerade filen.

När du väljer en förinställning för videokodning måste du tänka på att ta hänsyn till målanvändarens anslutningshastighet. Välj en förinställning med en datahastighet som är 80 % av den hastigheten. Om målanvändarens anslutningshastighet till exempel är 1 000 kbit/s är den bästa förinställningen en med en videodatahastighet på 800 kbit/s.

I den här tabellen beskrivs datahastigheten för typiska anslutningshastigheter.

| Hastighet (kbit/s) | Anslutningstyp |
|--- |--- |
| 256 | Uppringd anslutning. |
| 800 | Vanlig mobilanslutning. För den här anslutningen anger du en datahastighet mellan 400 och maximalt 800 för 3G-upplevelser som mål. |
| 2000 | Vanlig anslutning till stationär bredbandsuppkoppling. För den här anslutningen anger du en datahastighet i intervallet 800-2000 kbit/s med de flesta mål som är i genomsnitt 1200-1500 kbit/s. |
| 5000 | Vanlig bredbandsanslutning. Kodning i det här övre intervallet rekommenderas inte eftersom videoleverans i den här hastigheten inte är tillgänglig för de flesta konsumenter. |

### Upplösning {#resolution}

*Upplösning* beskriver videofilens höjd och bredd i pixlar. Den mesta källvideon lagras med hög upplösning (till exempel 1 920 x 1 080). Vid direktuppspelning komprimeras källvideo till en lägre upplösning (640 x 480 eller lägre).

Upplösning och datahastighet är två sammankopplade faktorer som avgör videokvaliteten. Om du vill behålla samma videokvalitet måste datahastigheten vara högre ju fler pixlar en videofil har (ju högre upplösning). Ta till exempel antalet pixlar per bildruta i en 320 x 240-upplösning och en 640 x 480-upplösningsvideofil:

| Upplösning | Pixlar per bildruta |
|--- |--- |
| 320 x 240 | 76 800 |
| 640 x 480 | 307 200 |

Filen på 640 x 480 har fyra gånger fler pixlar per bildruta. För att uppnå samma datahastighet för dessa två exempelupplösningar tillämpar du fyra gånger komprimeringen på 640 x 480-filen, vilket kan minska videons kvalitet. En videodatahastighet på 250 kbit/s ger därför en högkvalitativ bild med upplösningen 320 x 240, men inte med upplösningen 640 x 480.

>[!NOTE]
>
>I allmänhet gäller att ju högre datahastighet du använder, desto bättre visas videon och ju högre upplösning du använder, desto högre datahastighet måste du behålla visningskvaliteten (jämfört med lägre upplösningar).

Eftersom upplösning och datahastighet är länkade finns det två alternativ när du kodar video:

* Välj en datahastighet och koda sedan med den högsta upplösningen som ser bäst ut med den datahastighet du väljer.
* Välj en upplösning och koda sedan med den datahastighet som krävs för att få en video med hög kvalitet med den upplösning du väljer.

När du väljer (eller skapar) en videokodningsförinställning för den överordnad videofilen använder du den här tabellen för att ange rätt upplösning:

| Upplösning | Höjd (pixlar) | Skärmstorlek |
|--- |--- |--- |
| 240p | 240 | Liten skärm |
| 300p | 300 | Liten skärm för mobila enheter |
| 360p | 360 | Liten skärm |
| 480p | 480 | Medelstor skärm |
| 720p | 720 | Stor skärm |
| 1080p | 1080 | Stor HD-skärm |

### Fps (bildrutor per sekund) {#fps-frames-per-second}

I USA och Japan spelas de flesta videoklipp in med 29,97 bildrutor per sekund (fps). i Europa spelas de flesta videoklipp in med 25 bildrutor per sekund. Film filmas med 24 fps.

Välj en förinställning för videokodning som matchar fps-hastigheten för den överordnad videofilen. Om den överordnad videon till exempel är 25 fps väljer du en kodningsförinställning med 25 fps. Som standard används den överordnad videofilens fps för all anpassad kodning. Därför behöver du inte uttryckligen ange fps-inställningen när du skapar en förinställning för videokodning.

### Videokodningsdimensioner {#video-encoding-dimensions}

För bästa resultat väljer du kodningsdimensioner så att källvideon är en hel multipel av alla dina kodade videor.

Om du vill beräkna förhållandet dividerar du källbredden med den kodade bredden för att få breddförhållandet. Sedan dividerar du källhöjden med kodad höjd för att få höjdförhållandet.

Om förhållandet är ett heltal betyder det att videon är optimalt skalad. Om den resulterande kvoten inte är ett heltal påverkas videokvaliteten genom att kvarvarande pixelartefakter lämnas kvar på skärmen. Effekten märks mest när videon innehåller text.

Anta till exempel att källvideon är 1 920 x 1 080. I följande tabell ger de tre kodade videoklippen de optimala kodningsinställningarna som kan användas.

| Videotyp | Bredd x höjd | Breddförhållande | Höjdförhållande |
|--- |--- |--- |--- |
| Källa | 1920 x 1080 | 3 | 1 |
| Kodad | 960 x 540 | 2 | 2 |
| Kodad | 640 x 360 | 3 | 3 |
| Kodad | 480 x 270 | 4 | 4 |

### Kodat videofilformat {#encoded-video-file-format}

Adobe Dynamic Media Classic rekommenderar att du använder MP4 H.264-videokodningsförinställningar. Eftersom MP4-filer använder H.264-videokodeken ger den video med hög kvalitet men i en komprimerad filstorlek.

## Arbeta med förinställningar för videokodning {#working-with-video-encoding-presets}

Överordnad videofiler som skapats med videoproduktionsutrustning och videoredigeringsprogram är ofta för stora och har inte rätt format för leverans till onlinedestinationer. Om du vill konvertera digital video till rätt format och specifikationer för uppspelning på olika skärmar kan du *koda* videofiler (en process som också kallas *kodning*). Under kodningen komprimeras videon till en mindre, effektiv filstorlek för optimal distribution till webben och mobila enheter.

Se [Överföra och koda videofilmer](uploading-encoding-videos.md#uploading-and-encoding-videos).

Adobe Dynamic Media Classic innehåller ett bibliotek med fördefinierade videokodningsförinställningar som återspeglar de vanligaste kodningsinställningarna som används idag. Dessa kodningsförinställningar är optimerade för uppspelning på målskärmar. Dessutom kan administratörer skapa egna videokodningsförinställningar för att anpassa storleken och uppspelningskvaliteten på videoklipp för slutanvändarna. Alla förinställningar för videokodning, oavsett om de är färdiga från Adobe Dynamic Media Classic eller skräddarsydda utdata för video i MP4-format.

På skärmen Videoförinställningar kan administratörer konfigurera och hantera videokodning. De kan göra följande:

* Aktivera och inaktivera förinställningar för videokodning.
* Skapa en förinställning för videokodning.
* Redigera förinställningar för videokodning.
* Ta bort videoförinställningar.

Alla videofilmer som du överför till Adobe Dynamic Media Classic eller kodar i Adobe Dynamic Media Classic behandlas som&quot;videofilmer&quot;. Med andra ord innebär den här resursklassificeringen att du kan leverera videon för uppspelning på datorer, mobila enheter eller båda. Du kan till exempel förhandsgranska den här typen av videofilmer i Adobe Dynamic Media Classic. Du kan också generera URL:er (med funktionen Kopiera URL) och kod som du kan bädda in (med funktionen Bädda in kod) för användning med videospelare, på webbplatser och så vidare.

Se [Förhandsgranska videoklipp i ett videovisningsprogram](previewing-videos-video-viewer.md#previewing-videos-in-a-video-viewer).

Se [Länka en video-URL till en mobilwebbplats eller en webbplats](deploying-video-websites-mobile-sites.md#linking-a-video-url-to-a-mobile-site-or-a-website).

Se [Bädda in visningsprogrammet på en webbsida](deploying-video-websites-mobile-sites.md#embedding-the-video-viewer-on-a-web-page).

För videomaterial som du överför och kodar i Adobe Dynamic Media Classic levereras videon i följande filformat:

**MP4 H.264** Använd MP4-filer för följande:

* HTTP Dynamic Streaming på stationära datorer.
* HLS (HTTP Live Streaming, Apples direktuppspelningsprotokoll).
* Progressiv leverans av video till mobila Android™-, BlackBerry®- och Windows®-enheter.

Alla andra videoformat och kodekar behandlas som&quot;Överordnad Video&quot;. Den här resursklassificeringen innebär att videon är en videokällfil och inte kan användas för uppspelning på datorer eller mobila enheter. Du kan till exempel inte förhandsgranska den här typen av videofilmer i Adobe Dynamic Media Classic. Du kan inte heller generera Kopiera URL:er eller Bädda in kod för användning i videospelare, på webbplatser och så vidare.

### Filtrera listan med förinställningar för videokodning {#filtering-the-list-of-video-encoding-presets}

Sidan Videoförinställningar och sidan Adaptiva videoförinställningar består av en tabell som visar aktiv status, förinställningsnamn, avsedd uppspelningsenhet, videomängd och datahastighet för varje videoförinställning.

Du kan förfina listan genom att välja att filtrera på både Aktiv och Inaktiv om du vill se alla videoförinställningar eller begränsa listan till förinställningar som är aktiva eller inaktiva.

Du kan också filtrera baserat på ett uppspelningsenhetsalternativ om du vill begränsa listan till videoförinställningar som är utformade för att spela upp videofilmer på alla enheter, datorer, mobiler och surfplattor.

**Så här filtrerar du listan med förinställningar för videokodning:**

1. I Adobe Dynamic Media Classic klickar du på **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]** > **[!UICONTROL Adaptive Video Presets]** eller **[!UICONTROL Single Encoding Presets]** i fältet Global Navigation.

   Sidorna för adaptiva videoförinställningar och Förinställningar för enskild kodning innehåller en tabell med information om aktiv status, förinställningens namn, avsedd uppspelningsenhet, videodimensioner och datahastighet för varje videoförinställning.

1. Använd de två listrutorna i verktygsfältet Videoförinställningar på sidan Förinställningar för enskild kodning, som heter Videoförinställningar, för att förfina listan med förinställningar i tabellen baserat på Aktiv-status och uppspelningsenhet.

   * I den första smalare listrutan väljer du **[!UICONTROL Both]** om du vill se alla videoförinställningar, eller väljer **[!UICONTROL Active]** eller **[!UICONTROL Inactive]** eller begränsar listan till förinställningar som är aktiva eller inaktiva.
   * I den andra, bredare listrutan väljer du en uppspelningsenhet för att begränsa listan till videoförinställningar som är utformade för att spela upp video på stationära datorer. eller för att spela upp videor på mobiler eller surfplattor.

### Aktivera eller inaktivera förinställningar för videokodning {#activating-or-deactivating-video-encoding-presets}

De aktiverade videoförinställningarna visas i dialogrutan Alternativ för överföringsjobb. Dialogrutan visas när en användare överför videofiler under överföringen. De kan välja från en lista med alla aktiverade kodningsförinställningar.

1. I Adobe Dynamic Media Classic klickar du på **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]** i fältet Global Navigation.
1. Gör något av följande:

   * Klicka på **[!UICONTROL Adaptive Video Presets]**.
   * Klicka på **[!UICONTROL Single Encoding Presets]**.

1. Gör något av följande:

   * Om du vill aktivera en videoförinställning markerar du rutan bredvid ett förinställningsnamn under kolumnen Aktiv på sidan med förinställningar.
   * Om du vill inaktivera en videoförinställning avmarkerar du rutan bredvid de videoförinställningar som du vill göra inaktiva.

      >[!NOTE]
      >
      >Inaktiva videoförinställningar visas inte i dialogrutan Alternativ för överföringsjobb.

1. Klicka på **[!UICONTROL Close]** längst ned till höger på sidan.

### Lägga till eller redigera en förinställning för videokodning {#adding-or-editing-a-video-encoding-preset}

Du kan skapa egna videoförinställningar för enskild kodning och lägga till dem i tabellen Videoförinställningar. Du kan också ändra alla fördefinierade videoförinställningar för enskild kodning som medföljer Adobe Dynamic Media Classic, förutsatt att du sparar den redigerade förinställningen med ett nytt namn.

Adobe Dynamic Media Classic har angett maxgränser för måldatahastighet, upplösningshöjd och upplösningsbredd för att säkerställa en korrekt uppspelningsupplevelse. Varningsmeddelanden visas om du överskrider följande gränser:

* För datoruppspelning är gränserna: (Bredd/16) * (Höjd/16) &lt; 8192.
* För mobiluppspelning är gränserna: (Bredd/16) * (Höjd/16) &lt; 660; måldatahastighet &lt; 4000.
* För uppspelning på surfplattor är gränserna: (Bredd/16) * (Höjd/16) &lt; 3 600.

**Så här lägger du till eller redigerar en förinställning för videokodning:**

1. I Adobe Dynamic Media Classic klickar du på **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]** i fältet Global Navigation.
1. Klicka på **[!UICONTROL Single Encoding Presets]**.
1. Gör något av följande på sidan Videoförinställningar:

   * Klicka på **[!UICONTROL Add]** i verktygsfältet Videoförinställningar så att du kan lägga till en videoförinställning.
   * Välj en videoförinställning. Klicka på **[!UICONTROL Edit]** i verktygsfältet.

      Du kan inte redigera fördefinierade Adobe Dynamic Media Classic-förinställningar; Du kan bara skapa en förinställning från en befintlig genom att välja **[!UICONTROL Save As]**.

1. På sidan Lägg till videoförinställning eller på sidan Redigera videoförinställning anger du önskade alternativ för videoförinställning.

   Mer information om rekommenderade inställningar finns i [Bästa tillvägagångssätt för videokodning](uploading-encoding-videos.md#best-practices-for-video-encoding).

   | Videoförinställning, alternativ | Beskrivning |
   |--- |--- |
   | Förinställningsnamn | Ange ett beskrivande namn för videoförinställningen. Det namn du anger visas i dialogrutan Alternativ för överföringsjobb, där användarna väljer alternativ för omkodning. |
   | Beskrivning | Beskriv videoförinställningen. Det du anger visas som ett verktygstips när du flyttar pekaren över namnet på förinställningen i dialogrutan Alternativ för överföringsjobb där användarna väljer omkodningsalternativ. |
   | Uppspelningsenhet | Välj den enhet som videon ska spelas upp på. Alternativen är Dator (stationära datorer), Mobil (iPhone, iPad, Android™). eller Tablet (endast iPad). Den här inställningen avgör automatiskt vilken video- och ljudkodek som används vid kodningen. |
   | Måldatahastighet | Ange den genomsnittliga internetanslutningshastigheten (i kilobit per sekund) för målslutanvändaren. Du kan ange hastigheten eller dra reglaget för att ange den. I spektrumet för användaranslutningshastighet visas typiska hastigheter för bredband, DSL, mobiler och fjärranslutningar. Den här inställningen bestämmer automatiskt den kombinerade video- och ljuddatahastigheten. Med andra ord den datamängd som kodas för att utgöra en sekund av videouppspelningen. Ju högre datahastighet, desto bättre kvalitet får videon. För höga datahastigheter resulterar dock i stora filstorlekar som skapar en underordnad visningsupplevelse för användare med låg bandbredd. Det bästa sättet är att hitta en balans mellan höga och låga datahastigheter. Rikta in dig på att skapa en bra uppspelningsupplevelse utan att ge alienera användare med smala bandbredder. |
   | Proportioner | Proportionerna är proportionerna mellan videons bredd och höjd. De två första proportionerna som anges nedan används ofta för att visa video vågrätt:<ul><li> 4:3 - Används för nästan allt tv-sändningsinnehåll med standarddefinition.</li><li>16:9 - Används för nästan allt bredbildsformat, HD-TV-innehåll (HDTV) och filmer.</li><li>Skala automatiskt - (standard) En enda kodningsförinställning som fungerar med alla proportioner för att skapa videor som ska skickas till mobiler, surfplattor och datorer. Överförda källvideor som är kodade med den här förinställningen har en fast höjd. Bredden skalas dock automatiskt så att videons proportioner (bredd-/höjdförhållande) bevaras.</li><li>Anpassad - Används när du vill definiera en videostorlek som inte är standard.</li><li>De proportioner du väljer avgör inställningarna för bredd och höjd för upplösningsstorleken. värdet för bredd och höjd automatiskt skalas till rätt proportioner.</li></ul> |
   | Upplösningsstorlek | Upplösningsstorleken, uttryckt som antalet pixlar breda och antalet pixlar höga, avgör storleken. Ange ett bredd- och höjdvärde i pixlar eller dra reglaget för att ange dessa värden. I upplösningsspektrumet visas vanliga upplösningsstorlekar. Bredd- och höjdvärdena följer automatiskt de proportioner som du har valt. Om du till exempel väljer 4:3 som proportioner och anger 400 som bredd, anges 300 automatiskt som höjd. Om du valde Skala automatiskt för inställningen Proportioner, ställs värdet för Bredd för upplösningsstorleken automatiskt in på Auto. Klicka på Förhandsgranska så att du kan öppna ett webbläsarfönster och se dina upplösningsalternativ där. |
   | Koda filsuffix | Ange ett suffix. Det här suffixet läggs till i den resulterande kodade videofilen. Du kan skriva ett bindestreck och ett understreck i namnet; blanksteg och specialtecken tillåts inte. |
   | Andra inställningar | Adobe Dynamic Media Classic fastställer automatiskt alla andra kodningsinställningar enligt riktlinjerna för bästa praxis-kodning. |

1. Gör något av följande:

   * Klicka på **[!UICONTROL Save]** om du har lagt till eller redigerat en videoförinställning.
   * Klicka på **[!UICONTROL Save As]** om du har lagt till en videoförinställning genom att starta från en befintlig förinställning.

### Ta bort en förinställning för videokodning {#deleting-a-video-encoding-preset}

Administratörer kan ta bort anpassade videoförinställningar. Videoförinställningar som medföljer Adobe Dynamic Media Classic kan inte tas bort.

1. I Adobe Dynamic Media Classic klickar du på **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]** i fältet Global Navigation.
1. Klicka på **[!UICONTROL Single Encoding Presets]**.
1. På sidan Videoförinställningar väljer du en videoförinställning i tabellen som du inte längre vill ha eller behöver.
1. Klicka på **[!UICONTROL Delete]** i verktygsfältet Videoförinställningar.
1. Klicka på **[!UICONTROL Delete]** i dialogrutan Ta bort förinställning.

>[!MORELIKETHIS]
>
>* [Snabbstart: Video](quick-start-video.md#quick-start-video)
>* [Överföra och koda videofilmer](uploading-encoding-videos.md#uploading-and-encoding-videos)
>* [Arbeta med förinställningar för visningsprogram för video](previewing-videos-video-viewer.md#working-with-video-viewer-presets)

