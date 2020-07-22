---
title: Programinställningar
seo-title: Programinställningar
description: Lär dig hur du ställer in programområdet för Dynamic Media Classic.
seo-description: Lär dig hur du ställer in programområdet för Dynamic Media Classic.
uuid: 3e2f1d30-8f33-4a9d-bbe4-e8c3dbc968f8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: ae2d1895-a437-4463-bfac-3960c8027551
translation-type: tm+mt
source-git-commit: 7c9b1976ced6ef5ad48b624b99aeeffed380168a
workflow-type: tm+mt
source-wordcount: '10977'
ht-degree: 3%

---


# Programinställningar{#application-setup}

Du kan använda sidorna Programinställningar för att ange allmänna inställningar, skapa bildförinställningar, förinställningar för videokodning, förinställningar för visningsprogram eller för att definiera standardvisningsprogram och metadata. Du kan också konfigurera gruppuppsättningsförinställningar för att automatisera genereringen av 2D-snurpuppsättningar (till exempel), publiceringsinställningar och video-SEO-inställningar.

>[!NOTE]
>
>Endast Dynamic Media Classic-administratörer kan ändra inställningarna på programinställningssidorna.

## Allmänna inställningar {#general-settings}

Om du vill öppna sidan Allmänna inställningar för programmet klickar du på i fältet Global navigering **[!UICONTROL Setup > Application Setup > General Settings]**.

### Servrar

När du skapar ett konto får du automatiskt de tilldelade servrarna för ditt företag i Dynamic Media Classic. De här servrarna används för att skapa URL-strängar för din webbplats och dina program. Dessa URL-anrop är specifika för ditt konto.

Se även [Testa tjänsten](testing-assets-making-them-public.md#testing_the_secure_testing_service)Secure Testing.

* **Publicerat servernamn** - Den här servern är den CDN-live-server som används i alla systemgenererade URL-anrop som är specifika för ditt konto. Ändra inte det här servernamnet om du inte har fått instruktioner om att göra det av en Dynamic Media Classic-supporttekniker.

* **Ursprungligt servernamn** - Den här servern används endast för kvalitetstestning. Ändra inte det här servernamnet om du inte har fått instruktioner om att göra det av en Dynamic Media Classic-supporttekniker.

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by a Dynamic Media Classic support technician. -->

* **Test&amp;Target Server Name** - Your Test&amp;Target URL, up to and including .com. Instruktioner om hur du hämtar den här URL:en finns i Integrera [!DNL Dynamic Media Classic] med [!DNL Target Standard/Premium].

<!-- **Test Publish Context Server Name** -->

* **Namn på** iOS-direktuppspelningsserver - URL:en till din [!DNL Dynamic Media Classic] iOS-direktuppspelningsserver. Den här servern levererar direktuppspelad video till iOS-baserade enheter med HTTP-protokoll.

* **Progressivt namn på** videoserver - URL:en till din [!DNL Dynamic Media Classic] progressiva videoserver. Den här servern levererar progressiv video med HTTP-protokoll.

* **Visa URL för opublicerade resurser** - Välj det här alternativet om du vill [!DNL Dynamic Media Classic] visa en URL när du förhandsgranskar en resurs, oavsett om den är publicerad eller inte. Om resursen inte publiceras fungerar inte URL:en. Du kan dock använda URL-adressen för planering eller organisering.

<!-- **Allow AIR install** Select this option to allow users to download Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the web version of Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Dynamic Media Classic AIR. Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **CDN-mall** för invalidering - Anger den mall som används för att ogiltigförklara CDN-cachen (Content Delivery Network).

   Anta till exempel att du anger en bild-URL (inklusive bildförinställningar eller modifierare) som refererar `<ID>`i stället för ett specifikt bild-ID, som i följande exempel:

   `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

   Om mallen bara innehåller `<ID>`fylls Dynamic Media Classic i `https://<server>/is/image`, där `<server>` är namnet på publiceringsservern som definieras i Allmänna inställningar.

   Om du ställer in mallen för invalidering av CDN, markerar en bild med namnet Backpack_B och sedan klickar på **Arkiv** > **Invalidera CDN** , skapas följande genererade URL i CDN-gränssnittet:

   `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

   I listrutan URL klickar du på **Fortsätt** för att rensa cachen för det specifika bild-URL-anropet. Observera att du även kan lägga till URL-adresser genom att skriva eller klistra in dem i URL-listrutan; du inte behöver ange mallen i förväg.

   När du har valt en mall för CDN-validering och gjort en begäran om ogiltig CDN visas en indikator i användargränssnittet som ger dig en uppskattning av hur lång tid det tar att rensa cachen.

   Om flera bilder är markerade i Dynamic Media Classic när du klickar på **Arkiv** > **Invalidera CDN**, refereras varje bild till i den sparade mall-URL:en. Därför kan du definiera en mall för Ovalidering av CDN som refererar till varje URL som finns på webbplatsen (t.ex. produktinformation, sökresultat osv.). När du sedan väljer en eller flera bilder som ska ogiltigförklaras från cachen fylls gränssnittet automatiskt i med URL:erna.

   Se [Cachelagring](dmc-platform-overview.md#content_caching)av innehåll.

   Se [Återpublicerade resurser och CDN-fördröjningar](publishing-files.md#republished_assets_and_cdn_delays).

### Bläddra

* **Visa projekt** - Avgör om projekt är tillgängliga som ett sätt att ordna dina Dynamic Media Classic-resurser. Se Ordna ditt arbete med projekt.

* **Visa exempel på eVideo-innehåll** - Aktivera eller inaktivera visning av exempelinnehåll för eVideo.

* **Visa genererat innehåll** - I mappar visas innehåll som genererats från en resurs. När en PDF-fil till exempel rastreras när den överförs skapas en bild för varje sida i den ursprungliga PDF-filen i Dynamic Media Classic. Om Visa genererat innehåll är markerat visas varje bild som genereras när den ursprungliga PDF-filen överfördes tillsammans med PDF-filen i den mapp som PDF-filen överfördes till.

* **Visa kodade videoklipp** - avmarkerat (av) som standard.

   Om du snabbt vill söka efter och bläddra efter videofilmer i Dynamic Media Classic utan att behöva navigera bland flera kodade derivat av samma videofil låter du det här alternativet vara avmarkerat (standard). Endast miniatyrbilden för huvudvideon, som är den källvideo som du överfört och använt för att skapa alla derivat, och bara miniatyrbilden för den överordnade adaptiva videouppsättningen, som innehåller alla underordnade derivat för den kodade videouppsättningen, visas i användargränssnittet.

   Du kan dock fortfarande komma åt enskilda kodade videoklipp från den Överordnad videon eller den adaptiva videouppsättningen. Om du vill göra det dubbelklickar du på miniatyrbilden för videon för att öppna detaljvyn. Klicka sedan på **Kodade videoklipp** i den högra panelen för att komma åt alla underordnade videoklipp.

   Du kan också använda **Arkiv > Bearbeta** om du vill skapa mer kodade underordnade videor direkt från en adaptiv videouppsättning. Dynamic Media Classic hittar automatiskt den&quot;överordnade&quot; Överordnad videon i den adaptiva videouppsättningen och använder den som källvideo för omkodning. När du sparar de nya enskilda kodade videofilmerna visas de dock inte när du söker efter eller bläddrar. De är dock fortfarande tillgängliga på fliken Kodade videoklipp i detaljvyn.

   Se [Överföra och koda video](uploading-encoding-videos.md#uploading_and_encoding_videos).

   Om du vill ha fortsatt åtkomst till alla kodade videoderivat när du söker och bläddrar väljer du **Visa kodade videoklipp**.

   Det finns vissa åtgärder på menyn Skapa som bara fungerar, eller eventuellt fungerar, med enskilda videor. Den här funktionen gör det nödvändigt att visa alla kodade videoderivat som du kan välja mellan, oavsett hur du ställer in **Visa kodade videoklipp**. De Build-åtgärder som åsidosätter inställningen **Visa kodade videoklipp** är bland annat **Adaptiva videouppsättningar** och **e-kataloger**.

   >[Anteckning]
   >
   >Om du inte använde Dynamic Media Classic för att överföra och koda videoresurser visas alla dina enskilda kodade videofilmer i Dynamic Media Classic, även om det här alternativet är avmarkerat.

* **Knappen** Visa Uppdatera undermappar - Aktivera eller inaktivera visning av knappen Uppdatera för undermappar.

### Dynamic Media Classic FTP-konto

* **Server** - Visar en lista över din FTP-kontoserver.

* **Användarnamn** - Visar användarnamnet för ditt FTP-konto.

### Överför till program

* **Skriv över bilder** - två filer kan inte ha samma namn i Dynamic Media Classic. Varje objekts Dynamic Media Classic-ID (bildnamnet minus filnamnstillägget) måste vara unikt. På grund av den här regeln har dialogrutan Överför ett överskrivningsalternativ. Den exakta effekten av det här alternativet beror på det angivna alternativet Skriv över bilder. De här alternativen anger hur ersättningsbilder överförs: om de ersätter originalbilderna eller blir dubblettbilder. Duplicerade bilder får ett nytt namn med namnet&quot;-1&quot; (till exempel heter stol.tif stol-1.tif). De här alternativen påverkar bilder som har överförts till en annan mapp än den ursprungliga eller bilder med ett annat filnamnstillägg än den ursprungliga (till exempel JPG, TIF eller PNG). (Se Använda alternativet Skriv över bilder.)

   * **Skriv över i den aktuella mappen, samma basbildnamn/tillägg** - Det här alternativet är den striktaste regeln för ersättning. Det kräver att du överför ersättningsbilden till samma mapp som originalbilden och att ersättningsbilden har samma filnamnstillägg som originalbilden. Om dessa krav inte uppfylls skapas en dubblett.

   * **Skriv över i den aktuella mappen, samma basresursnamn oavsett tillägg** - Kräver att du överför ersättningsbilden till samma mapp som originalet, men filnamnstillägget kan skilja sig från originalet. Till exempel ersätter stol.tif stol.jpg.

   * **Skriv över i valfri mapp, samma basresursnamn/filnamnstillägg** - Kräver att ersättningsbilden har samma filnamnstillägg som den ursprungliga bilden (till exempel måste stol.jpg ersätta stol.jpg, inte stol.tif). Du kan dock överföra ersättningsbilden till en annan mapp än den ursprungliga. Den uppdaterade bilden finns i den nya mappen; filen inte längre kan hittas på sin ursprungliga plats

   * **Skriv över i valfri mapp, samma basresursnamn oavsett tillägg** - Det här alternativet är den mest omfattande ersättningsregeln. Du kan överföra en ersättningsbild till en annan mapp än den ursprungliga, överföra en fil med ett annat filnamnstillägg och ersätta den ursprungliga filen. Om originalfilen finns i en annan mapp finns ersättningsbilden i den nya mappen som den överfördes till.

* **Behåll publicering** - Anger om en ersättningsbild som överförts till Dynamic Media Classic ska behålla inställningen Klart för publicering för den bild som ersätts, eller om inställningen anges vid överföring.

* **Standardfärgprofiler** - Anger de färgprofiler som används som en del av alternativen för standardfärgprofil när du lägger till CMYK-bilder.

* **Standardalternativ** för överföring - Öppnar dialogrutan Alternativ för överföringsjobb, där du kan ange standardalternativ för överföring. Mer information om de här alternativen finns i Överföringsalternativ.

### Image Map Editor, to Application

* **Standardbildmappning HREF** - Definierar den standard-URL som används för bildmappningens href-kolumn. Den här URL:en är den standardadress du ser när du skapar nya bildscheman.

* **Standardmall** för bildmappning - Definierar JavaScript-standardvärdet för bildmappningens href-mall. Du kan ange att egen kod ska köras här när du klickar på ett bildschema.

### Andra inställningar, till program

* **Papperskorgen kan rensa upp varningar** - resurser i papperskorgen tas automatiskt bort inom sju dagar. Välj&quot;Skicka e-postmeddelanden innan papperskorgen tas bort automatiskt&quot; om du vill att meddelanden ska skickas till företagsadministratörer när resurser i papperskorgen inte tas bort permanent om fyra dagar. Se Hantera papperskorgen.

## Använda alternativet Skriv över bilder {#using-the-overwrite-images-option}

Två filer kan inte ha samma namn i Dynamic Media Classic. Varje objekts Dynamic Media Classic-ID (bildnamnet minus filnamnstillägget) måste vara unikt. På grund av den här regeln innehåller dialogrutan Överför alternativ för Skriv över bilder. Den exakta effekten av det här alternativet beror på en inställning för varje företags interna Dynamic Media Classic-inställningar.

Om du tidigare överförde bilder och sedan ändrade originalfilerna (eller ersatt dem), anger det valda alternativet Skriv över hur Dynamic Media Classic ersätter bilderna. Ingen information om bilden ändras, men den nya bilden ersätter den gamla. Om mappen även innehåller bilder som inte redan finns i Dynamic Media Classic läggs dessa bilder till.

Använd det här alternativet om de överförda bilderna har ändrats på något sätt (bilden har ändrats) men referensen till bilden är densamma. Skriv över är också användbart när du överför och rippar Adobe® PDF-filer. Om du vill finjustera hur bilden *rips* med Dynamic Media Classic justerar du ICC-färgprofilalternativen i dialogrutan Överför och överför igen med hjälp av funktionen Skriv över.

De Dynamic Media Classic-ID:n som används för att komma åt bilder från produktionsservrarna härleds från bildens filnamn. Det är viktigt att du använder versaler och gemener i filnamnet, både för att ersätta befintliga filer och för de Dynamic Media Classic ID som används för att få åtkomst till bilden. Se till att versaler och gemener i filnamn används korrekt innan du överför till Dynamic Media Classic för att undvika Dynamic Media Classic-ID:n som bara skiljer sig åt för samma bild.

Om du avmarkerar det här alternativet behandlas alla bilder med samma filnamn som befintliga bilder som dubbletter och läggs inte till.

## Bildförinställningar {#image-presets}

Skärmen Bildförinställningar används för att skapa och redigera bildförinställningar. Med bildförinställningar kan du med Dynamic Media Classic leverera bilder dynamiskt i olika storlekar från samma överordnad bild. Varje bildförinställning representerar en fördefinierad samling kommandon för storleksändring och formatering för visning av bilder. När du skapar en bildförinställning väljer du en storlek för bildleverans. Du kan också välja formateringskommandon så att bildens utseende optimeras när bilden levereras för visning.

Administratörer kan skapa förinställningar för att exportera resurser. Användarna kan välja en förinställning när de exporterar bilder, vilket även innebär att bilderna formateras om till de specifikationer som administratören anger.

Du öppnar skärmen Bildförinställning genom att klicka på **Inställningar** > **Bildförinställningar** i fältet Global navigering.

Se [Smart bildbehandling](https://helpx.adobe.com/experience-manager/6-3/assets/using/imaging-faq.html).

### Skapa och redigera bildförinställningar {#creating-and-editing-image-presets}

1. Klicka på **Konfigurera** > **Bildförinställningar**.
1. Skapa en ny förinställning eller börja från en befintlig:
   * **Skapa en bildförinställning** - klicka på **Lägg till**.
   * **Skapa en bildförinställning från en befintlig förinställning** - Välj den bildförinställning som är mest lik den du vill skapa och klicka sedan på Redigera.

1. Ange ett namn för förinställningen på skärmen Lägg till (eller Redigera) förinställning.
1. Ange de förinställningsalternativ som du vill använda.

   Se Alternativ för [bildförinställningar](application-setup.md#image_preset_options).

1. Klicka på **Spara** eller, om du har startat från en befintlig förinställning, klicka på **Spara som**.
1. Om du vill förhandsvisa förinställningen med en egen bild klickar du på **Bläddra** och väljer sedan en bild. Om du vill förhandsvisa med standardbilden klickar du på **Återställ**.

Du kan redigera en bildförinställning genom att markera namnet på skärmen Bildförinställningar och sedan klicka på Redigera. Om du vill ta bort en bildförinställning markerar du den och klickar sedan på Ta bort.

### Alternativ för bildförinställning {#image-preset-options}

Skärmarna Lägg till förinställning och Redigera förinställning innehåller följande alternativ för att skapa och redigera bildförinställningar:

**Förinställningsnamn** Ange ett beskrivande namn utan blanksteg. Inkludera bildstorleksspecifikationen i namnet så att användarna lättare kan identifiera den här bildförinställningen.

**Bredd och Höjd** Ange bildens storlek i pixlar.

**Format** Välj ett format på menyn. Om du väljer formaten GIF, JPEG, PDF eller TIFF visas ytterligare alternativ:

* Alternativ för GIF-färgkvantifiering

   **Typ**

   Välj Adaptiv (standard), Webb eller Macintosh. Om du väljer GIF med alfa är Macintosh®-alternativet inte tillgängligt.

   **Gitter**

   Välj Diffusera eller Av.

   **Antal färger**

   Dra skjutreglaget för att ange 2-255.

   **Färglista**

   Ange en kommaavgränsad lista. För vitt, grått och svart anger du 00000,888888,ffff.

* JPEG-alternativ

   **Kvalitet**

   Styr JPEG-komprimeringsnivån. Den här inställningen påverkar både filstorlek och bildkvalitet. JPEG-kvalitetsskalan är 1-100.

   **Aktivera JPG-krominanshämtning**

   Eftersom ögat är mindre känsligt för högfrekvent färginformation än högfrekvent luminans delas bildinformationen i JPEG-bilder in i luminans och färgkomponenter. När en JPEG-bild komprimeras lämnas luminanskomponenten i full upplösning, medan färgkomponenterna nedsamplas genom att medelvärdet av grupper av pixlar ökas. Nedsampling minskar datavolymen med en halv eller en tredjedel utan att det påverkar den upplevda kvaliteten. Nedsampling kan inte användas för gråskalebilder. Den här tekniken minskar mängden komprimering som är användbar för bilder med hög kontrast (till exempel bilder med överlagrad text).

* Alternativ för PDF och TIFF

   **Komprimering**

   Välj en komprimeringsalgoritm.

**Färgrymd** Välj en färgrymd.

**Skärpa** Välj alternativet Aktivera enkel skärpa om du vill använda ett grundläggande skärpefilter på bilden när all skalning har gjorts. Skärpa kan kompensera för oskärpa som kan uppstå när du visar en bild i en annan storlek.

Mer information om skärpa, omsamplingslägen och oskarp maskning finns i [Skärpa i en bild](sharpening-image.md#sharpening_an_image).

**Omsamplingsläge** Välj ett alternativ för omsamplingsläge. Dessa alternativ gör bilden skarpare när den nedsamplas:

**B-Linjär** den snabbaste omsamplingsmetoden. vissa aliaseringsartefakter är märkbara.

**Bi-Cubic** Ökar processoranvändningen på bildservern men ger skarpare bilder med mindre framträdande aliasing-artefakter.

**Sharp2** Kan ge något skarpare resultat än alternativet Bi-Cubic, men till ännu högre processorkostnad på Image Server.

**Tri-Linear** Använder både högre och lägre upplösningar, om sådana finns. rekommenderas bara när alias är ett problem. Den här metoden minskar JPEG-storleken på grund av reducerade högfrekventa data.

**Oskarp mask** Välj följande alternativ för att finjustera skärpan:

**Mängd** Styr mängden kontrast som används på kantpixlar. Standardvärdet är 1.0. För högupplösta bilder kan du öka den till upp till 5.0. Tänk på Mängd som ett mått på filterintensiteten.

**Radie** Anger antalet pixlar runt kantpixlarna som påverkar skärpan. För högupplösta bilder anger du 1 till 2. Med ett lågt värde ökas endast kantpixlarna skärpan. ett högt värde ökar skärpan i ett större antal pixlar. Vilket värde som är korrekt beror på bildens storlek.

**Tröskelvärde** bestämmer vilket kontrastintervall som ska ignoreras när filtret för oskarp mask används. Med andra ord, det här alternativet avgör hur olika de pixlar som ska göras skarpare måste vara från det omgivande området innan de betraktas som kantpixlar och blir skarpare. Experimentera med värden mellan 0,02 och 0,2 för att undvika brus. Standardvärdet 6 innebär att skärpan ökas för alla pixlar i bilden.

**Färgrymd** Anger om bilden ska använda det utrymme som bilden skapades i, vanligen RGB (original) eller luminansutrymme (intensitet).

**Färg** Välj följande alternativ:

**Utdatafärgprofil** Välj Använd standard eller någon av de ICC-färgprofiler som är tillgängliga i Dynamic Media Classic.

Se även [ICC-profiler](icc-profiles.md#icc_profiles).

**Återgivningsmetod** Välj ett alternativ om du vill åsidosätta färgprofilens standardåtergivningsmetod. Använd det här alternativet när en av ICC-standardprofilerna är målfärgrymden för en färgkonvertering, en utdataenhet (skrivare eller bildskärm) karakteriseras av den här profilen och den angivna återgivningsmetoden är giltig för den här profilen.

**Bädda in profil** Välj det här alternativet så att den här profilen används om du öppnar bilden i Adobe® Photoshop®.

**Utskriftsupplösning** Välj en upplösning för utskrift av den här bilden; 72 pixlar är standard.

**URL-modifierare** Om du föredrar att ange URL-modifierare som definierar bildförinställningen, i stället för inställningarna, anger du modifieringarna här.

**Exempelbild-URL** Visar den &quot;raw&quot;-URL-sträng som Dynamic Media Image Server använder för att leverera bilder med den bildförinställning som du lägger till eller redigerar. Den här URL-strängen kodar alla formatinställningar som du väljer på skärmen Lägg till förinställning eller Redigera förinställning.

### Redigera, ta bort eller inaktivera en bildförinställning {#editing-removing-or-deactivating-an-image-preset}

1. Klicka på **Konfigurera** > **Bildförinställningar**.
1. Välj en förinställning i tabellen på skärmen Bildförinställningar och gör sedan något av följande:

   * Klicka på **Redigera** och ange sedan nya alternativ i dialogrutan Redigera förinställning.
   * Klicka på **Ta bort** för att ta bort förinställningen från listan.
   * Avmarkera kryssrutan Aktiv bredvid ett förinställningsnamn om du vill ta bort den från hela Dynamic Media Classic-användargränssnittet för MediaPortal-användare.

## Aktivera eller inaktivera anpassade videoförinställningar {#activating-or-deactivating-adaptive-video-presets}

I Dynamic Media Classic finns förinställningar för adaptiv videokodning. Det är en överordnad lista med förinställningar som kombinerar både 16:9-förinställningar för adaptiv video och 4:3-förinställningar för adaptiv video till en grupp. Dessa fördefinierade förinställningar återspeglar de vanligaste kodningsinställningarna och är optimerade för uppspelning på mobila målenheter, surfplattor och datorer.

Endast kodningsförinställningar för adaptiv video aktiveras (aktiverat eller aktiverat) som standard. Du kan avaktivera den om du vill. Inaktiva förinställningar för adaptiv video visas inte som ett valbart alternativ i delen eVideo i dialogrutan Alternativ för överföringsjobb.

Se [Överföra och koda videofilmer](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Aktivera eller inaktivera anpassade videoförinställningar**

1. I det övre högra hörnet av Dynamic Media Classic klickar du på **Inställningar** > **Programinställningar** > **Videoförinställningar** > **Adaptiva videoförinställningar**.
1. På sidan Adaptiva videoförinställningar avmarkerar du kryssrutan bredvid ett förinställningsnamn för att ta bort förinställningen från listan eVideo-alternativ i dialogrutan Alternativ för överföringsjobb.
1. Klicka på **Stäng**.

## Videoförinställningar för kodning av videofiler {#video-presets-for-encoding-video-files}

Om du vill välja en kodningsförinställning klickar du på Jobbalternativ i det nedre högra hörnet på sidan Överför. Expandera eVideo-alternativ i dialogrutan Alternativ för överföringsjobb och välj de förinställningar för videokodning som du vill använda.

>[!NOTE]
>
>Med undantag för Adaptiv video, som är aktiverat som standard, kanske du inte ser alla andra adaptiva video- eller enstaka videokodningsförinställningar i dialogrutan Alternativ för överföringsjobb. Dynamic Media Classic-administratörer avgör vilka förinställningar för videokodning som visas i dialogrutan Alternativ för överföringsjobb.

* Välj mellan följande adaptiva videokodningsförinställningar eller enskilda kodningsförinställningar:

   **16:9 Adaptiv video**

   Skapa videor med 16:9-proportioner för leverans till datorer, mobiler (iPhone, iPad, Android) och surfplattor (iPad, Android), optimerade med den upplösning och bithastighet som bäst matchar tittarens anslutningshastighet.

   **4:3 Adaptiv video**

   Skapa videor med 4:3-proportioner för leverans till datorer, mobiler (iPhone, iPad, Android) och surfplattor (iPad, Android), optimerade med den upplösning och bithastighet som bäst matchar tittarens anslutningshastighet.

   **Adaptiv video**

   En enda förinställning för kodning som fungerar med alla proportioner för att skapa videor som ska skickas till mobilen, surfplattan och datorn. Överförda källvideor som är kodade med den här förinställningen har en fast höjd. Bredden skalas dock automatiskt så att videons proportioner bevaras.

   Den här flexibiliteten med automatisk skalförändring är också tillgänglig som standard när du skapar en egen förinställning för videokodning.

   Se [Lägga till eller redigera en förinställning](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset)för videokodning.

   **Adaptiv videokodning (16:9 eller 4:3)**

   Skapa videor med både 16:9- och 4:3-proportioner för leverans till datorer, mobilenheter (iPhone, iPad, Android) och surfplattor (iPad, Android), optimerade med den upplösning och bithastighet som bäst matchar tittarens anslutningshastighet.

   Se [Videoförinställningar](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets)för adaptiv videokodning (16:9 eller 4:3).

   **Förinställningar för enskild kodning**

   >[ANMÄRKNING]
   >
   >Om du vill leverera video till iPad kan du välja en Mobile-kodningsförinställning eller en kodningsförinställning för Tablet. Förinställningar för surfplattor är särskilt utformade för iPad, vanligtvis med högre upplösning och kvalitet för att dra nytta av den större skärmstorleken och bandbreddsanslutningen. För att kunna leverera videofiler som är kodade med en Tablet-förinställning måste du inkludera enhetsidentifieringskod på din mobila webbplats eller i ditt mobila program. Den här koden växlar mellan en iPhone- eller iPad-videoupplevelse, beroende på uppspelningsenheten. Att välja en Mobile-förinställning för att leverera videofiler till iPad är ett enklare arbetsflöde. Orsaken är att du kan använda samma videofil för både iPhone och iPad. Kvaliteten standardiseras emellertid med iPhone-upplevelsen med lägre upplösning.

   * I gruppen Kodningsförinställningar väljer du Namn eller Storlek i listrutan Sortera kodningsförinställningar om du vill sortera förinställningar efter namn eller upplösning.
   * Välj en kodningsförinställning baserat på upplösningsstorleken och bandbredden som du vill spela upp videon med.
   * Du kan välja Adaptiv videokodning och en eller flera kodningsförinställningar per video. Du kan till exempel koda en fil för både dator och mobil i ett överföringsjobb.

När du klickar på **Starta överföring**&#x200B;överförs den ursprungliga överordnad videofilen och kodade filer genereras från den överordnad filen.

### Om alternativ för kodningsförinställningar {#about-encoding-preset-options}

Parametrarna för de förinställda alternativen för kodning är följande:

**Target anslutningshastighet** Slutanvändarens internetanslutning.

**Kodat filsuffix** Det suffix som är kopplat till den kodade videofilen i identifieringssyfte.

**Videobithastighet (datahastighet)** Den datamängd som kodas för att skapa en enda sekund av videouppspelning (i kB per sekund).

**Pixelbredd/höjd** Skärmbildens bredddimension i pixlar. skärmbildens höjddimension (i pixlar).

**Bildruta per sekund (fps)** Antalet bildrutor, eller stillbilder, för varje sekund i videon. I USA och Japan spelas de flesta videoklipp in med 29,97 fps. i Europa och Asien (utom Japan) spelas de flesta videoklipp in med 25 bildrutor per sekund. Film filmas med 24 fps.

**Ljudbithastighet** Den mängd data som kodas för att skapa en enda sekund av ljuduppspelning, i kilobit per sekund.

I följande tabeller visas de bästa sätten att välja videoförinställningar och de namnkonventioner som används för att ange kodade filer.

### Adaptiv video (standard) {#adaptive-video-default}

En förinställning för kodning som fungerar med alla proportioner så att du kan skapa videor för leverans till mobilen, surfplattan och datorn. Överförda källvideofilmer som är kodade med den här förinställningen (standard och bästa praxis) ställs in på en fast höjd medan bredden automatiskt skalas för att bevara videons proportioner.

**Adaptiv video (standard)**

|  | Kodningsförinställningsnamn/knappbeskrivningstext | Kodat filsuffix | Videodatahastighet (kbit/s) | Bredd/höjd (pixlar) | Fps | Bithastighet för ljud (kbit/s) | Rekommendationer |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | Auto x 360, 800 kbit/s | _Mobile_Autox360p_800K | 800 | Autox360 | Samma som källan | 64 | För mobiler (iPhone, iPad, Android) |
| 2 | Auto x 480, 1 400 kbit/s | _Tablet_Autox480p_1400K | 1400 | Autox480 | Samma som källan | 96 | För surfplattor (iPad, Android) |
| 3 | Auto x 720, 2 600 kbit/s | _Desktop_Autox720p_2600K | 2600 | Autox720 | Samma som källan | 128 | För datorer |

### Videoförinställningar för Adaptiv videokodning (16:9 eller 4:3) {#adaptive-video-encoding-or-video-presets}

Dessa adaptiva videokodningsförinställningar kombinerar en serie individuella kodningsförinställningar som väljs automatiskt utifrån proportionerna för den video du överförde. Om du till exempel överför en 4:3-video kodas den automatiskt med alla fem 4:3-förinställningar som finns i den överordnad förinställningslistan i alternativet **Adaptiv videokodning (16:9 eller 4:3)** .

Mer information om parametrar för kodningsalternativ finns i [Om alternativ](application-setup.md#about_encoding_preset_options)för kodningsförinställningar.

**Förinställningar för adaptiv videokodning (16:9 eller 4:3)**

|  | Kodningsförinställningsnamn/knappbeskrivningstext | Target anslutningshastighet (kbit/s) | Kodat filsuffix | Videodatahastighet (kbit/s) | Bredd/höjd (pixlar) | Fps | Bithastighet för ljud (kbit/s) | Rekommendationer |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512x288, Mobil (iPhone, iPad, Android), (400 kbit/s) | 500 | _Mobile_512x288_400K | 400 | 512x288 | Samma som källan | 64 | Låg upplösning, 3G |
| 2 | 4:3, 384x288px, Mobil (iPhone, iPad, Android), (400 kbit/s) | 500 | _Mobile_384x288_400K | 400 | 384x288 | Samma som källan | 64 | Låg upplösning, 3G |
| 3 | 16:9, 512x288, Mobil (iPhone, iPad, Android), (600 kbit/s) | 700 | _Mobile_512x288_600K | 600 | 512x288 | Samma som källan | 64 | Medelhög upplösning, 3G |
| 4 | 4:3, 384x288, Mobil (iPhone, iPad, Android), (600 kbit/s) | 700 | _Mobile_384x288_600 | 600 | 384x288 | Samma som källan | 64 | Medelhög upplösning, 3G |
| 5 | 16:9, 640x360, surfplatta (iPad, Android), (800 kbit/s) | 900 | _iPad_640x360_800K | 800 | 640x360 | Samma som källan | 80 | Medelhög upplösning, WiFi |
| 6 | 4:3, 640x480, surfplatta (iPad, Android), (800 kbit/s) | 900 | _iPad_640x480_800K | 800 | 640x480 | Samma som källan | 80 | Medelhög upplösning, WiFi |
| 7 | 16:9, 768x432, surfplatta (iPad, Android), (1 200 kbit/s) | 1,5 Mbit/s | _iPad_768x432_1200K | 1200 | 768x432 | Samma som källan | 96 | Hög upplösning, WiFi |
| 8 | 4:3, 768x576, surfplatta (iPad, Android), (1 200 kbit/s) | 1,5 Mbit/s | _iPad_768x576_1200K | 1200 | 768x576 | Samma som källan | 96 | Hög upplösning, WiFi |
| 9 | 16:9, 1280x720, stationär dator, (2000 kbit/s) | 3,0 Mbit/s | _1280x720_2000K | 2000 | 1280x720 | Samma som källan | 128 | HD, widescreen |
| 10 | 4:3, 1 280 x 960, stationär dator (2 000 kbit/s) | 3,0 Mbit/s | _1280x960_2000K | 2000 kbit/s | 1280x960 | Samma som källan | 128 | HD |

### Videokodningsförinställningar för datorer {#desktop-video-encoding-presets}

Videokodningsförinställningar för MP4 och OGV på stationära datorer.

Mer information om parametrar för kodningsalternativ finns i [Om alternativen](application-setup.md#about_encoding_preset_options)för kodningsförinställningar.

**H264 Main 3.2 - Audio AAC, MP4-filtillägg**

|  | Kodningsförinställningsnamn/knappbeskrivningstext | Target anslutningshastighet (kbit/s) | Kodat filsuffix | Videodatahastighet (kbit/s) | Bredd/höjd (pixlar) | Fps | Bithastighet för ljud (kbit/s) | Rekommendationer |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480x270 (400 kbit/s) | 500 | _480x270_400K | 400 | 480x270 | Samma som källan | 64 | Låg widescreen-upplösning |
| 2 | 16:9, 640x360 (800 kbit/s) | 900 | _640x360_800K | 800 | 640x360 | Samma som källan | 80 | Medelstor widescreen-upplösning |
| 3 | 16:9, 800x450 (1 200 kbit/s) | 1,5 Mbit/s | _800x450_1200K | 1200 | 800x450 | Samma som källan | 96 | Medelhög upplösning |
| 4 | 16:9, 1 280 x 720 (2 000 kbit/s) | 3,0 Mbit/s | _1280x720_2000K | 2000 | 1280x720 | Samma som källan | 128 | HD, widescreen |
| 5 | 4:3, 320x240 (400 kbit/s) | 500 | _320x240_400K | 400 | 320x240 | Samma som källan | 64 | Låg upplösning |
| 6 | 4:3, 480x360 (800 kbit/s) | 900 | _480x360_800K | 800 | 480x360 | Samma som källan | 80 | Medelhög upplösning |
| 7 | 4:3, 640x480 (1 200 kbit/s) | 1,5 Mbit/s | _640x480_1200K | 1200 | 640x480 | Samma som källan | 96 | Medelhög upplösning |
| 8 | 4:3, 1 280 x 960 (2 000 kbit/s) | 3,0 Mbit/s | _1280x960_2000K | 2000 | 1280x960 | Samma som källan | 128 | Hög definition |

**OGG Theora Vorbis - OGV-filtillägg**

|  | Kodningsförinställningsnamn/knappbeskrivningstext | Target anslutningshastighet (kbit/s) | Kodat filsuffix | Videodatahastighet (kbit/s) | Bredd/höjd (pixlar) | Fps | Bithastighet för ljud (kbit/s) | Rekommendationer |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480x270 (400 kbit/s), OGG | 500 | _OGG_480x270_400K | 400 | 480x270 | Samma som källan | 64 | Låg widescreen-upplösning |
| 2 | 16:9, 640x360 (800 kbit/s), OGG | 900 | _OGG_640x360_800K | 800 | 640x360 | Samma som källan | 80 | Medelstor widescreen-upplösning |
| 3 | 16:9, 800x450 (1 200 kbit/s), OGG | 1,5 Mbit/s | _OGG_800x450_1200K | 1200 | 800x450 | Samma som källan | 96 | Medelhög upplösning |
| 4 | 16:9, 1 280 x 720 (2 000 kbit/s), OGG | 3,0 Mbit/s | _OGG_1280x720_2000K | 2000 | 1280x720 | Samma som källan | 128 | HD, widescreen |
| 5 | 4:3, 320x240 (400 kbit/s), OGG | 500 | _OGG_320X240_400K | 400 | 320x240 | Samma som källan | 64 | Låg upplösning |
| 6 | 4:3, 480x360 (800 kbit/s), OGG | 900 | _OGG_480x360_800K | 800 | 480x360 | Samma som källan | 80 | Medelhög upplösning |
| 7 | 4:3, 640x480 (1 200 kbit/s), OGG | 1,5 Mbit/s | _OGG_640x480_1200K | 1200 | 640x480 | Samma som källan | 96 | Medelhög upplösning |
| 8 | 4:3, 1 280 x 960 (2 000 kbit/s), OGG | 3,0 Mbit/s | _OGG_1280x960_2000K | 2000 | 1280x960 | Samma som källan | 128 | Hög definition |

### Förinställningar för kodning av mobilvideo {#mobile-video-encoding-presets}

Samma som käll-fps. Videokodningsförinställningar för iPhone-, iPad- och Android-mobilenheter.

Mer information om parametrar för kodningsalternativ finns i [Om alternativen](application-setup.md#about_encoding_preset_options)för kodningsförinställningar.

**H264 Originalplan 2.1 - Ljud-AAC, MP4-filtillägg**

|  | Kodningsförinställningsnamn/knappbeskrivningstext | Target-anslutningshastighet (kbit/s) | Kodat filsuffix | Videobithastighet (kbit/s) | Pixelbredd/höjd | Fps | Bithastighet för ljud (kbit/s) | Rekommendationer |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512x288, mobil (400 kbit/s) | 500 | _Mobile_512x288_400K | 400 | 512x288 | Samma som källan | 64 | Låg upplösning, 3G |
| 2 | 16:9, 512x288, mobil (600 kbit/s) | 700 | _Mobile_512x288_600K | 600 | 512x288 | Samma som källan | 64 | Medelhög upplösning, 3G |
| 3 | 16:9, 512x288, mobil (800 kbit/s) | 900 | _Mobile_512x288_800K | 800 | 512x288 | Samma som källan | 80 | Medelhög upplösning, Wi-Fi |
| 4 | 16:9, 512x288, mobil (1 000 kbit/s) | 1,2 Mbit/s | _Mobile_512x288_1000K | 1000 | 512x288 | Samma som källan | 80 | Hög upplösning, Wi-Fi |
| 5 | 16:9, 512x288, mobil (1 200 kbit/s) | 1,5 Mbit/s | _Mobile_512x288_1200K | 1200 | 512x288 | Samma som källan | 96 | Hög upplösning, Wi-Fi |
| 6 | 4:3, 384x288, mobil (400 kbit/s) | 500 | _Mobile_384x288_400K | 400 | 384x288 | Samma som källan | 64 | Låg upplösning, 3G |
| 7 | 4:3, 384x288, mobil (600 kbit/s) | 700 | _Mobile_384x288_600K | 600 | 384x288 | Samma som källan | 64 | Medelhög upplösning, 3G |
| 8 | 4:3, 448x336, mobil (800 kbit/s) | 900 | _Mobile_448x336_800K | 800 | 448x336 | Samma som källan | 80 | Medelhög upplösning, Wi-Fi |
| 9 | 4:3, 448x336, mobil (1 000 kbit/s) | 1,2 Mbit/s | _Mobile_448x336_1000K | 1000 | 448x336 | Samma som källan | 80 | Hög upplösning, Wi-Fi |
| 10 | 4:3, 448x336, mobil (1 200 kbit/s) | 1,5 Mbit/s | _Mobile_448x336_1200K | 1200 | 448x336 | Samma som källan | 96 | Hög upplösning, Wi-Fi |

## Förinställningar för visningsprogram {#viewer-presets}

>[!NOTE]
>
>**Meddelande** om att Flash-visningsprogrammet upphör att gälla - Från och med den 31 januari 2017 upphörde Adobe Dynamic Media Classic officiellt med stödet för Flash-visningsprogramplattformen. Mer information om den här viktiga ändringen finns på följande webbplats med vanliga frågor och svar: [https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html](https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html).

En *visningsförinställning* är en samling inställningar som bestämmer hur användare visar mediefiler på datorskärmar och mobila enheter. Som administratör kan du skapa visningsförinställningar. Inställningarna är tillgängliga för en array med visningskonfigurationsalternativ. Du kan till exempel ändra visningsprogrammets visningsstorlek, zoombeteende, färgscheman, kanter och teckensnitt.

Det bästa sättet att göra det är att använda videovisningsprogram i Dynamic Media Classic HTML5. De förinställningar som används i HTML5 Video-visningsprogram är robusta videospelare. Genom att i en enda spelare kombinera möjligheten att utforma uppspelningskomponenterna med HTML5 och CSS, ha inbäddad uppspelning och använda adaptiv och progressiv strömning beroende på webbläsarens kapacitet, kan du utöka räckvidden för ditt multimedieinnehåll till datorer, surfplattor och mobilanvändare och få en smidig videoupplevelse.

Se [Om HTML5-visningsprogram](hhttps://docs.adobe.com/content/help/en/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html) i referenshandboken för Adobe-visningsprogram.

Se Kompatibilitetsmatris för [Dynamic Media Classic Viewer Preset](application-setup.md#scene7_viewer_preset_compatibility_matrix).

Se [Bästa praxis: Använda HTML5 Video Viewer](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer).

Beroende på visningsprogrammet kan du lägga till communityfunktioner. Community-funktionerna är bland annat knappen Bädda in, knappen E-post, knappen Länk och knappen Besök webbplats. Med de här knapparna kan personer som använder visningsprogrammen dela visningsprogrammet med andra eller öppna Dynamic Media Classic-webbplatsen.

Se även [Adobe Viewer Reference Library-exempel](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

### Stöd för visningsprogram för responsiva webbsidor {#viewer-support-for-responsive-designed-web-pages}

Olika webbsidor har olika behov. Ibland kanske du vill ha en webbsida som innehåller en länk som öppnar HTML5 Viewer i ett separat webbläsarfönster. I andra fall kan det vara nödvändigt att bädda in HTML5 Viewer direkt på värdsidan. I det senare fallet kan webbsidan ha en statisk layout. Det kan också vara&quot;responsivt&quot; och visas på olika enheter eller för olika webbläsarfönsterstorlekar. För att tillgodose dessa behov har HTML5-visningsprogrammen som medföljer Dynamic Media Classic stöd för både statiska webbsidor och responsiva designade webbsidor.

Mer information om hur du bäddar in responsiva visningsprogram på dina webbsidor finns i [Responsive Static Image](https://marketing.adobe.com.com/resources/help/en_US/s7/is_ir_api/is_api/c_about_responsive_static_image_library.html)libraries i hjälpen *för* Adobe Image Serving API.

### Förinställningstyper för visningsprogram {#viewer-preset-types}

Administratörer kan skapa och anpassa följande typer av visningsförinställningar:

**eCatalog Viewer** Simulerar upplevelsen av att läsa en utskriven katalog. Du kan gå från sida till sida, zooma in och ut från objekt på en sida, använda bildscheman för att visa mer information om objekt på sidan eller söka i katalogen. Du kan även inkludera en informationspanel för att visa detaljerad information och ett bildschemat objekt om mappningsområdet har ett giltigt rollover_key-attribut. Om du vill ta med en informationspanel anger du en URL för informationsservern på panelen Info-inställningar i fönstret för visningsförinställningar för eCatalog.

**Färgruta Ställ in visningsprogram** Visar en bild i en annan färg, material, struktur, finish eller struktur. Användarna klickar på en miniatyrbild för att se variationerna i bilden.

**Visningsprogram för blandad medieuppsättning** Visar olika typer av media i ett visningsprogram. Du kan inkludera färgruteuppsättningar, snurruppsättningar, bilder och videoklipp. Du kan ställa in flikar så att de innehåller olika typer av innehåll, till exempel en flik för bilduppsättningar och en flik för videoklipp. Videofilmer som spelas upp från en blandad medieuppsättning använder ett standardvisningsprogram för video med en tidslinje och videokontroller, till exempel Stop, Pause, Rewind och Play. När du ställer in en förinställning för visningsprogrammet för blandad medieuppsättning anger du vilka visningsprogram du vill använda för de olika resurstyperna i din uppsättning med blandade media. Du kan också använda stödrastervisningsprogrammet eller Carousel Viewer för att visa en blandad medieuppsättning.

**Snurra Ställ in visningsprogram** Tillhandahåller flera vyer av en bild så att användare kan vrida objektet för att undersöka olika sidor och vinklar.

**Video Viewer** Visar videor med källfilens upplösningsdimensioner eller en anpassad storlek. Dynamic Media Classic innehåller många fördefinierade visningsförinställningar för uppspelning av video, och om du är administratör kan du skapa anpassade förinställningar för visningsprogrammet för video. Det finns mer än ett dussin olika inställningar för att konfigurera Video Viewer. Du kan konfigurera dess storlek, för- och bakgrundsfärg, video- och ljudkontroller, förloppsindikator, användargränssnittets skal, sociala funktioner och hjälp.

**Zoomvisningsprogram** erbjuder tre typer av zoomningsvisningsprogram:

**Zooma visningsprogram** Används för att zooma in i området genom att klicka på det. De kan klicka på kontroller för att zooma in, zooma ut och återställa bilden till standardstorleken.

**Zoomvisningsprogram: Flyg ut** Visar en andra bild av det zoomade området bredvid originalbilden. Det finns inga kontroller att använda. Användarna flyttar bara markeringen över det område som de vill visa.

När du fastställer den fullständiga bandbreddsanvändningen för det här visningsprogrammet bör du tänka på att både huvudbilden och den utfällbara bilden visas i visningsprogrammet. Huvudbildens storlek (scenens bredd och höjd) och zoomfaktorn bestämmer den utfällbara bildens storlek. Om du vill förhindra att den utfällbara filstorleken blir för stor ska du balansera dessa två värden: om du har en stor huvudbildstorlek, sänker du zoomfaktorn. (Utfällbar bredd och Utfällbar höjd bestämmer storleken på det utfällbara fönstret, men inte storleken på den utfällbara bild som visas i visningsprogrammet.)

Om huvudbildens storlek till exempel är 350 x 350 pixlar, med zoomfaktorn 3, blir den utfällbara bilden 1 050 x 1 050 pixlar. Om huvudbildstorleken är 300 x 300 pixlar, med zoomfaktorn 4, är den utfällbara bilden 1 200 x 1 200 pixlar. Beroende på kvalitetsinställningen för JPEG (rekommenderade inställningar är mellan 80 och 90) kan du minska filstorleken avsevärt. Rekommenderade zoomningsfaktorer är 2,5 till 4, beroende på storleken på huvudbilden.

### Kompatibilitetsmatris för Dynamic Media Classic Viewer-förinställning {#scene-viewer-preset-compatibility-matrix}

**Meddelande** om att Flash-visningsprogrammet upphör att gälla: Från och med den 31 januari 2017 upphör stödet för Flash-visningsprogramplattformen officiellt i Adobe Dynamic Media Classic.

Mer information om den här viktiga ändringen finns på följande webbplats med vanliga frågor och svar: [https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html](https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html).

Följande tabell visar vilka förinställningar för Dynamic Media Classic Viewer som är tillgängliga. Tabellen anger också visningsprogrammets kompatibilitet med datorer och mobila enheter samt vilken teknik som används för varje visningsprogram.

Se även [Adobe Viewer Reference Library-exempel](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

Information om vilka webbläsare och operativsystemversioner som stöds för visningsprogram finns i Viewer Release Notes.

Se Versionsinformation om [Adobe Viewer Reference](https://docs.adobe.com/content/help/en/dynamic-media-developer-resources/library/home.html).

|  | Viewer Technology | Skrivbord | Apple iPhone | Apple iPad | Android Smartphone | Android-surfplatta |
|--- |--- |--- |--- |--- |--- |--- |
| Zooma visningsprogram |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | Viewer Technology | Skrivbord | Apple iPhone | Apple iPad | Android Smartphone | Android-surfplatta |
|--- |--- |--- |--- |--- |--- |--- |
| Bilduppsättningsvisningsprogram |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | Viewer Technology | Skrivbord | Apple iPhone | Apple iPad | Android Smartphone | Android-surfplatta |
|--- |--- |--- |--- |--- |--- |--- |
| Visningsprogram för färgruteuppsättning |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | Viewer Technology | Skrivbord | Apple iPhone | Apple iPad | Android Smartphone | Android-surfplatta |
|--- |--- |--- |--- |--- |--- |--- |
| eCatalog Viewers |  |  |  |  |  |  |
| Universal_HTML5_eCatalog_Adv(Innehåller stöd för sociala medier och katalogsökning.) | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog(Innehåller stöd för sociala medier och katalogsökning.) | HTML5 | X | X | X | X | X |

|  | Viewer Technology | Skrivbord | Apple iPhone | Apple iPad | Android Smartphone | Android-surfplatta |
|--- |--- |--- |--- |--- |--- |--- |
| Snurra visningsprogram |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**eVideo Viewers**

Dynamic Media Classic har stöd för videouppspelning i mobiler för MP4 H.264-video.

* Du kan hitta Blackberry-enheter som stöder det här videoformatet på följande sätt: [Videoformat som stöds på Blackberry](https://developer.blackberry.com/devzone/develop/supported_media/bb10_media_support.html)
* Du kan även hitta Windows-enheter som stöder det här videoformatet på följande:Videoformat som[stöds på Windows Phone](https://docs.microsoft.com/en-us/previous-versions/windows/apps/ff462087(v=vs.105)?redirectedfrom=MSDN)

|  | Viewer Technology | Skrivbord | Apple iPhone | Apple iPad | Android Smartphone | Android-surfplatta | Blackberry Smartphone | Windows Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video(Innehåller stöd för undertextning.) Se [Bästa praxis: Använda det universella HTML5 Video Viewer.](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social(Innehåller stöd för undertexter och sociala medier.) | HTML5 | X | X | X | X | X | X | X |

|  | Viewer Technology | Skrivbord | Apple iPhone | Apple iPad | Android Smartphone | Android-surfplatta |
|--- |--- |--- |--- |--- |--- |--- |
| Visningsprogram för blandad medieuppsättning |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### Matris för gester för mobilvisningsprogram som stöds {#supported-mobile-viewers-gestures-matrix}

Följande tabell visar vilka mobilvisningsgester som stöds på iOS-, Android 2.x- och Android 3.x-enheter.

|  | Viewer Technology | Skrivbord | Apple iPhone | Apple iPad | Android Smartphone | Android-surfplatta |
|--- |--- |--- |--- |--- |--- |--- |
| Bilduppsättningsvisningsprogram |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### Om skärmen med visningsförinställningar {#about-the-viewer-preset-screen}

Skapa och hantera visningsförinställningar på skärmen Förinställningar för visningsprogram. Om du vill öppna den här skärmen klickar du på **Inställningar** > **Visningsförinställningar**.

Skärmen Förinställningar för visningsprogram innehåller verktyg för följande åtgärder:

**Lägga till en förinställning** Klicka på Lägg till och gör önskade inställningar i dialogrutan Lägg till visningsförinställning.

Se [Lägga till och redigera visningsprogramförinställningar](application-setup.md#adding_and_editing_viewer_presets).

**Redigera en förinställning** Välj en förinställning och klicka sedan på **Redigera**.

Se [Lägga till och redigera visningsprogramförinställningar](application-setup.md#adding_and_editing_viewer_presets).

**Ta bort en förinställning** Välj en förinställning och klicka sedan på **Ta bort**.

**Exportera en förinställning** Välj en förinställning för HTML5-visningsprogrammet och klicka sedan på Exportera för att hämta visningsskalet så att du kan använda det som grund för att skapa och lägga till en ny visningsförinställning.

Se [Exportera en HTML5 Viewer-förinställning](application-setup.md#exporting_an_html5_viewer_preset).

**Filtrera listan** med visningsförinställningar Använd dessa verktyg för att filtrera listan:

* Öppna listrutan **Aktiv/Inaktiv** och välj ett alternativ för att visa aktiva förinställningar, inaktiva förinställningar eller alla förinställningar.
* Öppna listrutan **Visningsprogram** och välj ett alternativ för att endast visa visningsprogram av en viss typ. Välj **Alla visningsprogram** om du vill visa alla visningsprogram.

**Sortera förinställningar** Klicka på en kolumnrubrik (Aktiv, Typ, Förinställning eller Platform) för att sortera listan i en kolumn. Klicka på en kolumnrubrik en andra gång om du vill sortera listan i fallande (eller stigande) ordning.

**Aktivera och inaktivera förinställningar** Välj en förinställning och klicka på alternativet Aktiv för att aktivera eller inaktivera den.

Se [Aktivera eller inaktivera visningsprogramförinställningar](application-setup.md#activating_or_deactivating_viewer_presets).

>[!NOTE]
>
>Klicka på Förhandsvisa till höger på skärmen Förinställningar för visningsprogram för att se hur en resurs ser ut i den valda visningsförinställningen. Om du vill visa en annan resurs kan du klicka på Bläddra på skärmen Förinställningar för visningsprogram och välja en annan resurs i dialogrutan Välj förhandsgranskning av resurs.

### Lägga till och redigera visningsprogramförinställningar {#adding-and-editing-viewer-presets}

Förutom att lägga till förinställningar för visningsprogram med Lägg till i användargränssnittet kan du också använda Exportera för att lägga till en förinställning för visningsprogrammet. Du exporterar bara en befintlig förinställning för HTML5-visningsprogrammet och använder den som bas för den nya förinställningen.

Se [Exportera en HTML5 Viewer-förinställning](application-setup.md#exporting_an_html5_viewer_preset).

**Lägga till och redigera visningsprogramförinställningar**

1. I det övre högra hörnet av Dynamic Media Classic klickar du på **Inställningar** > **Visningsförinställningar**.

   Du kan filtrera i listan med förinställningar. Om du till exempel bara vill visa förinställningar för videovisningsprogram väljer du Videovisningsprogram i listrutan Visare i verktygsfältet direkt ovanför tabellen.

1. Lägg till eller redigera visningsförinställningen på skärmen Förinställningar för visningsprogram.

   **Lägg till** Klicka på Lägg till i verktygsfältet. I dialogrutan Lägg till visningsförinställning väljer du en plattform och väljer en medieresurstyp.

   Klicka på **Spara som** när du har skapat visningsförinställningen.

   **Lägg till genom att starta från en befintlig visningsförinställning** i tabellen, markera en förinställning för visningsprogrammet för video och klicka sedan på Redigera i verktygsfältet.

   När du har konfigurerat om videovisningsprogrammet klickar du på **Spara som** för att spara förinställningen med ett annat namn i textfältet Förinställningsnamn.

   **Redigera** Välj en befintlig visningsförinställning och klicka sedan på **Redigera**.

1. Ange eller redigera förinställningsnamnet i fältet Förinställningsnamn på skärmen Konfigurera visningsprogram.
1. Ange de återstående alternativen som du vill ha.

   >[ANMÄRKNING]
   >
   >Välj Samma som källa om du automatiskt vill ändra storlek på videovisningsprogrammet till upplösningsstorleken för den kodade videon. Om du väljer det här alternativet kan du inte ange scenens bredd och höjd. I stället kommer dessa alternativ från själva videon. Om du väljer Samma som källa anger du alternativet Marginalstorlek för att visa skalets dimensioner utanför videouppspelningsområdet. Marginalstorleken är pixelhöjden och bredden på videokontrollerna. Du kan använda följande bild för att avgöra vilka marginalstorlekar du vill använda.*

   ![](assets/vs_video_viewer_configure_margin.png)

1. Gör något av följande:

   * Klicka på **Spara som** om du har lagt till en visningsförinställning genom att starta från en befintlig förinställning.
   * Klicka på **Spara** om du har lagt till eller redigerat en visningsförinställning.

### Exportera en HTML5-visningsförinställning {#exporting-an-html-viewer-preset}

Du kan exportera en befintlig HTML5 Viewer-förinställning som du kan använda som grund för att skapa en ny HTML5 Viewer-förinställning. Det här exportalternativet är användbart eftersom du inte behöver skapa visningsprogrammet från grunden. I stället exporterar du en förinställning som ser ut och beter sig ungefär som du vill ha den, och sedan kan du använda den som utgångspunkt för att göra designjusteringar.

Observera att alla standardförinställda CSS-filer för visningsprogram i Dynamic Media Classic använder relativa bildvisningssökvägar som pekar på resurser som finns på `Scene7SharedAssets`. Följande är en relativ sökväg till en bildresurs i en CSS-fil för visningsförinställning som finns på `Scene7SharedAsset`: `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`Om du däremot har CSS-filer för visningsprogram på din egen plats, måste du lösa den relativa sökvägen genom att använda en explicit sökväg till bildservern i din egen miljö. I illustrationssyfte, om du skulle uppdatera den relativa sökvägen ovan till en explicit sökväg, kan den se ut så här, där `https://s7d1.scene7.com` är den direkta sökvägen till bildservern: `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**Exportera en HTML5-visningsförinställning**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. Klicka på **Inställningar** > **Visningsförinställningar**.
1. Välj **HTML5** i den andra listrutan till vänster i verktygsfältet Visningsförinställningar.
1. I den tredje listrutan till vänster väljer du **Alla visningsprogram**.
1. Välj den visningsförinställning som du vill använda som bas för en ny visningsförinställning för HTML5.
1. Klicka på **Exportera** i verktygsfältet.
1. Klicka på **Skicka export** i dialogrutan Exportera markerade resurser.

   Efter exporten får du en CSS-fil. Ladda ned och zippa upp filen.

1. Öppna CSS-filen i en CSS-redigerare, gör ändringarna och spara sedan filen.
1. Överför CSS-filen till Dynamic Media Classic.

   Se [Överföra filer](uploading-files.md#uploading_files).

1. Publicera CSS-filen på Dynamic Media Image Server.

   Se [Publicera filer](publishing-files.md#publishing_files).

1. Lägg till den nya visningsförinställningen som vanligt. Välj CSS-filen för visningsprogrammet som du överförde.

   Se [Lägga till och redigera visningsprogramförinställningar](application-setup.md#adding_and_editing_viewer_presets).

### Aktivera eller inaktivera visningsprogramförinställningar {#activating-or-deactivating-viewer-presets}

Om du vill skapa en URL för att visa resurser öppnar användarna listrutan Förinställningar i dialogrutan Förhandsvisa, väljer en visningsförinställning och klickar på Kopiera URL (se [Kopiera URL för en visningsförinställning](application-setup.md#copying_the_url_of_a_viewer_preset)). Den här förinställningslistan innehåller förinställningar för visningsprogram som administratörer kan lägga till och hantera på skärmen Förinställningar för visningsprogram. Alla aktiva förinställningar för eCatalog Viewer visas till exempel i listrutan Förinställningar i dialogrutan Förhandsvisa när en användare förhandsgranskar en e-katalog.

Om du inte inaktiverar visningsförinställningar på skärmen Förinställningar för visningsprogram kan listrutan Förinställningar i dialogrutan Förhandsvisa bli full.

**Aktivera eller inaktivera visningsförinställningar**

1. Välj **Inställningar** > **Förinställningar** för visningsprogram för att öppna skärmen Förinställningar för visningsprogram.
1. Markera eller avmarkera Aktiva alternativ om du vill aktivera eller inaktivera visningsförinställningar.

### Kopiera URL:en för en visningsförinställning {#copying-the-url-of-a-viewer-preset}

När du har publicerat en resurs kan du kopiera en URL för att visa resursen med inställningarna från en visningsförinställning.

URL:en kopieras till Urklipp. Du kan använda den vid behov i HTML-koden för webbsidan, den mobila enheten eller programmet.

**Så här kopierar du URL:en för en visningsförinställning**

1. Markera resursen på panelen Bläddra.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Klicka på **Stödrastervisning**. Dubbelklicka på en enskild resurs på panelen Resursbläddring för att öppna den i detaljvyn. Klicka på **Kopiera URL** till höger om det visningsprogram du vill använda i panelen URL:er och Bädda in kod till höger.
   * Klicka på **Stödrastervisning**. Markera en enskild resurs på panelen Resursbläddring och klicka sedan under miniatyrbilden på **Förhandsvisa** > **Visningsprogramlista**.

   Klicka på **Kopiera URL** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Klicka på **Listvy**. Markera en enskild resurs på panelen Resursbläddring och klicka sedan på **Förhandsvisa** > **Visningslista** till höger om miniatyrbilden.

   Klicka på **Kopiera URL** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Klicka på **Stödrastervisning**, **Listvy** eller **Detaljvy**. Klicka på **Förhandsgranska** > **Visningsprogramlista** i samma verktygsfält.

   Klicka på **Kopiera URL** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

### Kopiera inbäddningskoden för en visningsförinställning {#copying-the-embed-code-of-a-viewer-preset}

Med funktionen Bädda in kod kan du granska visningsprogramkoden för den valda visningsförinställningen. Du kan också kopiera koden till Urklipp så att du kan klistra in den på dina webbsidor för att distribuera visningsprogrammet.

Det är inte tillåtet att redigera koden i dialogrutan Bädda in kod.

**Så här kopierar du inbäddningskoden för en visningsförinställning**

1. Markera resursen på resurspanelen.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Klicka på **Stödrastervisning**. Dubbelklicka på en enskild resurs på panelen Resursbläddring för att öppna den i detaljvyn. Klicka på **Bädda in kod** på panelen URL:er till höger.
   * Klicka på **Stödrastervisning**. Markera en enskild resurs på panelen Resursbläddring och klicka sedan under miniatyrbilden på **Förhandsvisa** > **Visningsprogramlista**.

   Klicka på **Bädda in kod** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Klicka på **Listvy**. Markera en enskild resurs på panelen Resursbläddring och klicka sedan på **Förhandsvisa** > **Visningslista** till höger om miniatyrbilden.

   Klicka på **Bädda in kod** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Klicka på **Stödrastervisning**, **Listvy** eller **Detaljvy**. Klicka på **Förhandsgranska** > **Visningsprogramlista** i samma verktygsfält.

   Klicka på **Bädda in kod** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

1. I dialogrutan Bädda in kod klickar du på **Kopiera till Urklipp**.
1. Klicka på **Stäng**.

## Konfigurera standardvisningsprogram {#configuring-default-viewers}

Du kan använda standardvisningsprogram för att konfigurera standardvisningsprogrammet som är associerat med en resurs när du använder Förhandsvisa i Dynamic Media Classic. Du kan ställa in standardförhandsvisningen för följande resurstyper:

* Bild
* Video
* SpinSet
* Katalog
* ImageSet
* SwatchSet
* MediaSet

**Konfigurera standardvisningsprogram**

1. Klicka på **Programinställningar** i listrutan Inställningar.
1. Expandera **Programinställningar** > **Visare i det vänstra fönstret**
1. Klicka på **Standardvisningsprogram**.
1. Välj det visningsprogram som du vill associera med resursens förhandsgranskning i listrutan för varje resurstyp i fönstret Standardvisningsprogram.
1. Klicka på **Spara inställningar** i det nedre högra hörnet av fönstret Standardvisningsprogram.
1. Klicka på **Stäng** i det nedre högra hörnet av inställningsfönstret för att återgå till fönstret Resurser.

## Metadatavyer {#metadata-views}

*Metadata* är standardiserad information om en resurs. Du kan använda metadata för att effektivisera arbetsflödet, ordna dina resurser och förbättra sökningen. Dynamic Media Classic stöder standarderna IPTC (International Press Telecommunications Council) och XMP (extensible metadata platform). Innan användarna visar eller anger metadata om en resurs i detaljvyn kan de öppna menyn Metadatavyer och välja den uppsättning metadatafält som de vill visa eller använda för att beskriva resursen.

Dynamic Media Classic innehåller fördefinierade metadatavyer och administratörer kan skapa egna metadatavyer som användarna kan välja när de anger metadata.

### Skapa en metadatavy {#creating-a-metadata-view}

1. Klicka på **Konfigurera** > **Programinställningar** > **Metadata** > **Metadatavyer**.
1. Klicka på **Lägg till**.
1. Ange ett namn för vyn i textfältet Förinställningsnamn.
1. (Valfritt) Markera **Gör till standard** om du vill att den här vyn ska vara den som visas för användarna när de öppnar panelen Metadata i detaljvyn.
1. (Valfritt) Markera **Inkludera UDF** om du vill inkludera användardefinierade fält i vyn. Användardefinierade fält visas högst upp på panelen Metadata i detaljvyn.
1. Markera de fält som du vill visa (klicka på **Markera alla** för att markera alla fält).
1. Klicka på **Spara**.

   De markerade kategorierna och fälten för vyn visas på panelen Förhandsgranska.

### Hantera metadatavyer {#managing-metadata-views}

1. Klicka på **Konfigurera** > **Programinställningar** > **Metadata** > **Metadatavyer**.
1. Gör något av följande:

   * Om du vill förhandsgranska en vy markerar du den. Fälten i vyn visas på förhandsvisningspanelen.
   * Om du vill redigera en vy markerar du den och klickar sedan på **Redigera**. Markera eller avmarkera sedan fältnamn på panelen Förhandsgranska och markera eller avmarkera alternativet **Inkludera användardefinierat** fält.
   * Om du vill ta bort en vy markerar du den och klickar sedan på **Ta bort**.
   * Om du vill göra en vy till standardvy markerar du den och klickar sedan på **Använd som standard**. Standardvyn är den vy som användarna ser när de öppnar en resurs i detaljvyn och går till panelen Metadata.

## Metadataförinställningar {#metadata-presets}

Med metadataförinställningar kan administratörer styra och reglera metadata som tilldelas resurser. I vyn Detalj kan en användare ange metadata om en resurs i fält som tillhandahålls för det ändamålet. En användare kan till exempel ange ett ägarnamn, en copyrightbeskrivning och en adress. Om du vill vara säker på att användarna anger den här informationen korrekt och fullständigt kan du skapa metadataförinställningar. Om du väljer en metadataförinställning i vyn Detalj fylls metadatafält med fördefinierade värden. Exempel: Ägarnamn, copyrightbeskrivning och adress anges automatiskt.

Skapa en metadataförinställning för varje uppsättning metadatavärden som du vill att användarna ska kunna ange automatiskt i vyn Detalj för att beskriva en resurs.

### Skapa eller redigera en metadataförinställning {#creating-or-editing-a-metadata-preset}

1. Klicka på **Konfigurera** > **Programinställningar** > **Metadata** > **Metadataförinställningar** .
1. Gör något av följande på skärmen Metadataförinställningar:

   * Om du vill skapa en förinställning klickar du på **Lägg till**. I textfältet Namn på metadatamall skriver du ett namn för förinställningen, klickar på **Metadatavyer** och väljer en vy i listrutan (se [Metadatavyer](application-setup.md#metadata_views)).
   * Om du vill redigera en befintlig förinställning markerar du förinställningen i listan Metadataförinställningar och klickar sedan på **Redigera**.

1. Expandera rubriker som du vill ta med i förinställningen och ange värden i de olika fält som du vill ta med i förinställningen.
1. Klicka på **Spara**.

   De valda kategorierna och fälten för förinställningen visas på panelen Förhandsgranska.

### Hantera metadataförinställningar {#managing-metadata-presets}

1. Klicka på **Konfigurera** > **Programinställningar** > **Metadata** > **Metadataförinställningar**.
1. Gör något av följande:

   * Om du vill förhandsgranska en förinställning markerar du den förinställning som du vill förhandsgranska. Förinställningsinformationen (kategorier och fält) visas på förhandsgranskningsskärmen.
   * Om du vill ta bort en förinställning markerar du förinställningen och klickar sedan på **Ta bort**.

## Användardefinierade fält {#user-defined-fields}

En Media Portal-administratör eller en företagsadministratör kan skapa anpassade, användardefinierade metadatafält. Med anpassade fält kan du ordna resurser i Dynamic Media Classic. Du kan markera fälten som aktiva, efter behov. När du aktiverar det här alternativet visas namnen på dessa anpassade metadatafält på panelen Metadata i detaljvyn. Användare kan ange information i användardefinierade metadatafält för att beskriva resurser. Användarna kan också göra ett användardefinierat metadatafält till ett villkor i sökningar.

Ett effektivt sätt att använda användardefinierade metadatafält är att fördröja aktiveringstiden för en mediefil för en viss start eller försäljning. Du definierar ett aktiveringsfält baserat på typen *Datum*. Sedan kan du ange när resursen ska aktiveras med panelen **Metadata** i vyn **Detalj** eller **Arkiv** > **Redigera information**. Dynamic Media Classic kontrollerar publiceringsstatusen för en resurs och publiceringshistoriken. Om det inte är inom aktiveringstiden visas publiceringsstatusen som Inte publicerad.

>[!NOTE]
>
>Om du vill att användardefinierade fält ska visas på panelen Metadata i vyn Detalj, inkluderar du användardefinierade fält i metadatavyer. Markera alternativet Inkludera användardefinierat fält (Inkludera användardefinierat fält) på skärmen Metadatavyer. Mer information finns i [Metadatavyer](application-setup.md#metadata_views).

>[!NOTE]
>
>Om du vill söka efter resurser med anpassade, användardefinierade fält klickar du på **Inställningar** > **Personliga inställningar** och väljer sedan **Inkludera användardefinierat fält i sökningen**. Se [Personliga inställningar](personal-setup.md#personal_setup).

### Skapa ett användardefinierat metadatafält {#creating-a-user-defined-metadata-field}

1. Klicka på **Konfigurera** > **Programinställningar** > **Metadata** > **Användardefinierade fält**.
1. Klicka på **Lägg till**
1. Ange önskade alternativ i dialogrutan Anpassat fält.

   **Namn** Ange ett namn för metadatafältet.

   **Skriv** Välj ett alternativ som definierar vilken typ av information som användare kan ange i metadatafältet:

   **Sträng** En textsträng.

   **Int** ett heltal.

   **Flyttal** Ett flyttal.

   **Ja/Nej** A ja/nej booleskt värde.

   **Datum** ett datum. Formatet MM/DD/ÅÅÅÅ accepteras.

   **Filnamn** Namnet på en fil.

   **Färg** Namnet på en färg.

   **Dimension** Resursens bredd och höjd.

   **Typlös** för bakåtkompatibilitet. Markera inte det här alternativet.

   **Standardvärde** . Du kan också ange det värde som användarna mest sannolikt anger i fältet. Värdet som du anger blir standardvärdet för fältet som du skapar.

   **Tillämpas på** (valfritt), välj en resurstyp om du vill att metadatafältet endast ska gälla för en viss typ av resurs.

   ***Obs**! Välj ett **Tillämpa på** -alternativ noggrant eftersom du inte kan ändra alternativet **Tillämpa på** när du har skapat ett användardefinierat fält. I Dynamic Media Classic kan du redigera namn, typ och standardvärde för ett användardefinierat fält, men inte för inställningen **Gäller** . *

1. Klicka på **Spara** när du har skapat metadatafältet.

### Hantera användardefinierade fält {#manage-user-defined-fields}

Skärmen Användardefinierade fält innehåller kommandon för att hantera anpassade, användardefinierade metadatafält.

Endast en Media Portal-administratör eller en företagsadministratör kan hantera användardefinierade fält.

Om du vill öppna den här skärmen klickar du på **Inställningar** > **Programinställningar** > **Metadata** > **Användardefinierade fält**.

**Redigera ett fält** Markera fältet och klicka sedan på **Redigera**.

**Ta bort ett fält** Markera fältet och klicka sedan på **Ta bort**.

**Aktivera fält** Klicka för att markera eller avmarkera alternativet Aktiv bredvid namnet på ett fält. Om du har en företagsadministrationsroll kanske det här alternativet inte visas. Eftersom det här alternativet är relaterat till MediaPortal måste du markera (aktivera) Visa MediaPortal-funktioner i Personliga inställningar för att se aktiveringsfälten.

## Optimera filer {#optimize-files}

När du överför filer till Dynamic Media Classic optimeras de för lagring och publicering. Om överföringen avbryts kan vissa bilder inte optimeras. I det här fallet visas meddelandet &quot;Bilden är inte optimerad ännu&quot;. Du kan dock optimera dessa filer om du är administratör.

Dynamic Media Classic söker igenom dina filer och optimerar bara de bilder som inte har optimerats fullständigt tidigare.

1. Välj **Konfigurera** > **Programinställningar** och sedan **Optimera filer**.
1. Ange information för optimeringsjobbet och klicka på **Skicka**.

   Om du arbetar med mer än ett företag optimerar du filer som tillhör olika företag separat.

## Förinställningar för gruppuppsättning {#batch-set-presets}

Använd förinställningarna för gruppuppsättningar för att automatiskt skapa bilduppsättningar eller snurruppsättningar när ett jobb körs för att överföra resurser till Dynamic Media Classic.

Företagsadministratörer definierar först namnkonventioner för de resurser som de vill gruppera tillsammans i en uppsättning. Du kan sedan skapa en förinställning för batchuppsättning som refererar till dessa bilder. Varje förinställning är en unik, självständig uppsättning instruktioner som definierar hur uppsättningen ska skapas med bilder som matchar de definierade namnkonventionerna i förinställningsreceptet.

Alla aktiva gruppuppsättningsförinställningar för ett företag visas i dialogrutan Alternativ för överföring av jobb, så att du kan ange vilken förinställning du vill använda under varje överföringssession. Företagsadministratörer ser alla aktiva och inaktiva förinställningar för gruppuppsättningar. När du överför filer skapar Dynamic Media Classic automatiskt en uppsättning med alla filer som matchar den definierade namnkonventionen i de aktiva förinställningarna.

### Standardnamn {#default-naming}

Företagsadministratören skapar en standardnamnkonvention som används i alla förinställda gruppuppsättningar. Den standardnamnkonvention som valts i förinställningsdefinitionen för gruppuppsättning kan vara allt ditt företag behöver för att gruppgenerera uppsättningar för alla webbplatser. En gruppuppsättningsförinställning skapas för att använda den standardnamnkonvention som du definierar. Du kan skapa så många gruppuppsättningsförinställningar med alternativa, anpassade namnkonventioner som behövs för en viss uppsättning innehåll om det finns ett undantag från den företagsdefinierade standardnamngivningen.

När det inte krävs någon standardnamnkonvention för att använda funktionen för gruppuppsättningsförinställningar rekommenderar vi att du använder standardnamnkonventionen för att definiera så många element i namnkonventionen som du vill gruppera i en uppsättning för att effektivisera skapandet av gruppuppsättningar.

1. Klicka på **Konfigurera** > **Programinställningar** > **Gruppera inställda** inställningar > **Standardnamn**.
1. Select **View Form** or **View Code** to specify how you want to view and enter information about each element.

   Du kan markera kryssrutan Visa kod om du vill visa värdeuppbyggnaden för reguljära uttryck tillsammans med dina formulärval. Du kan ange eller ändra dessa värden för att underlätta definitionen av elementen i namnkonventionen, om formulärvyn begränsar dig av någon anledning. Om dina värden inte kan tolkas i formulärvyn blir formulärfälten inaktiva.

   >[!NOTE]
   Inaktiverade formulärfält indikerar inte ett ogiltigt reguljärt uttryck. Det finns ingen validering av att dina reguljära uttryck är korrekta. Resultaten av det reguljära uttryck som du skapar för varje element visas efter resultatraden. Det fullständiga reguljära uttrycket visas längst ned på sidan.

1. Expandera varje element efter behov och ange de namnkonventioner som du vill använda.
1. Om det behövs klickar du på **Lägg till** för att lägga till en annan namnkonvention för ett element. Du kan också klicka på **Ta bort** för att ta bort en namnkonvention för ett element.
1. Klicka på **Spara som** och skriv ett namn för förinställningen. Du kan också klicka på **Spara** om du redigerar en befintlig förinställning.

Du kan också använda Visa kod utan några formulärfält. I den här vyn skapar du namnkonventionens definitioner helt med hjälp av reguljära uttryck.

Det finns två element för definition, Matcha och Basnamn. Med dessa fält kan du definiera alla element i en namnkonvention och identifiera den del av konventionen som används för att namnge den uppsättning i vilken de finns. Ett företags personliga namnkonvention kan använda en eller flera definitionsrader för vart och ett av dessa element. Du kan använda så många rader för din unika definition och gruppera dem i distinkta element, t.ex. för Huvudbild, Färgelement, Alternativa vyer och Färgruteelement.

### Skapa en gruppuppsättningsförinställning {#creating-a-batch-set-preset}

I Dynamic Media Classic används gruppuppsättningsförinställningar för att ordna resurser som delar viss vanlig information eller innehåll i uppsättningar med bilder som ska visas i visningsprogram. Förinställningsrecepten för gruppuppsättningar körs automatiskt tillsammans med de resursimporteringsjobb som du schemalägger i Dynamic Media Classic.

Använd Förinställning för gruppuppsättning för att skapa, redigera och hantera dina gruppuppsättningsförinställningar. Du kan skapa så många batchuppsättningsförinställningar som behövs för att täcka alla tillgångsimportjobb som du behöver. Det finns två former av förinställda gruppuppsättningsdefinitioner: en för en standardnamnkonvention som du kan ha konfigurerat och en för anpassade namnkonventioner som du skapar direkt.

Du kan antingen använda formulärfältsmetoden för att definiera en gruppuppsättningsförinställning eller kodmetoden, som gör att du kan använda reguljära uttryck. Som i Standardnamngivning kan du välja kodvyn samtidigt som du definierar i formulärvyn och använda reguljära uttryck för att skapa definitioner. Du kan också avmarkera en vy om du vill använda den ena eller den andra enbart.

Se även [Skapa en förinställning för batchuppsättning för automatisk generering av en 2D-snurra uppsättning](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

**Skapa en gruppuppsättningsförinställning**

1. Klicka på **Konfigurera** > **Programinställningar** > **Gruppera förinställningar** > **Gruppera inställningsförinställning**. **Vyformulär**, som det anges i det övre högra hörnet på detaljsidan, är standardvyn.
1. Klicka på **Lägg** till på panelen Förinställningslista för att aktivera definitionsfälten på panelen Detaljer till höger på skärmen.
1. Skriv ett namn på förinställningen i fältet Förinställningsnamn på panelen Detaljer.
1. Välj en förinställningstyp i listrutan Gruppuppsättningstyp.

   Om du vill generera en tvådimensionell snurrsuppsättning automatiskt väljer du **Flera axelsnurruppsättningar** i listrutan Gruppuppsättningstyp.

1. Gör något av följande:

   * If you are using a default naming convention that you previously set up under Application Setup > Batch Set Presets > Default Naming, expand **Asset Naming Conventions**, and then in the File Naming drop-down list, click **Default**.
   * To define a naming convention as you set up the preset, expand **Asset Naming Conventions**, and then in the File Naming drop-down list, click **Custom**.

1. I Sekvensordning definierar du ordningen för bilderna när uppsättningen har grupperats tillsammans i Dynamic Media Classic. Som standard sorteras dina resurser alfanumeriskt. Du kan dock använda en kommaavgränsad lista med reguljära uttryck för att definiera ordningen.
1. Ange suffixet eller prefixet till basnamnet som du definierade i konventionen om namngivning av tillgångar för Ange namngivning och skapande. Ange också var bilduppsättningen ska skapas i mappstrukturen för Dynamic Media Classic.

   Om du definierar ett stort antal bilduppsättningar kanske du föredrar att hålla dessa åtskilda från de mappar som innehåller själva resurserna. Många kunder skapar en mapp för bilduppsättningar och dirigerar om programmet för att placera gruppuppsättningar som genererats här.

1. Klicka på **Spara** på panelen Detaljer.

### Skapa en gruppuppsättningsförinställning för automatisk generering av en 2D-snurpuppsättning {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

Du kan använda **multiaxelrotationsuppsättningen** för gruppuppsättningstyp för att skapa ett recept som automatiserar genereringen av tvådimensionella snurruppsättningar. Vid gruppering av bilder används reguljära uttryck för rad och kolumn så att bildresurserna justeras korrekt på motsvarande plats i den flerdimensionella arrayen.

Se även [Skapa en förinställning](application-setup.md#creating_a_batch_set_preset)för gruppuppsättning.

Det finns inget minsta eller högsta antal rader eller kolumner som du måste ha i en rotationsuppsättning med flera axlar.

Anta till exempel att du vill skapa en fleraxelsnurra med namnet *spin-2dspin*. Du har en uppsättning bilder med snurra uppsättningar som innehåller tre rader, med 12 bilder per rad. Bilderna får följande namn:

```as3
spin-01-01
spin-01-02
… 
spin-01-12
spin-02-01
… 
spin-03-12
```

Med den här informationen kan ditt recept för gruppuppsättningstyp skapas på följande sätt:

![](assets/se_batch_set_recipe.png)

Gruppering för den delade resursnamnsdelen av rotationsuppsättningen läggs till i fältet **Matcha** (markerat). Variabeldelen av resursnamnet som innehåller raden och kolumnen läggs till i fälten **Rad** och **Kolumn**.

När rotationsuppsättningen har överförts och publicerats aktiverar du namnet på det 2D-rotationsuppsättningsrecept som visas under **Förinställningar för gruppuppsättning** i dialogrutan **Alternativ för överföringsjobb**.

**Skapa en gruppuppsättningsförinställning för automatisk generering av en 2D-snurpuppsättning**

1. Välj **Konfigurera** > **Programinställningar** > **Gruppera inställningsförinställningar** > **Gruppera inställningsförinställning**. **Vyformulär**, som det anges i det övre högra hörnet på detaljsidan, är standardvyn.
1. Klicka på **Lägg** till på panelen Förinställningslista för att aktivera definitionsfälten på panelen Detaljer till höger på skärmen.
1. Skriv ett namn på förinställningen i fältet Förinställningsnamn på panelen Detaljer.
1. In the Batch Set Type drop-down menu, select **Asset Set**.
1. I listrutan Undertyp väljer du **Mångaxelsnurra uppsättning**.
1. Expandera **Konventioner** för namngivning av resurser och klicka sedan på **Anpassad** i listrutan Namnge fil.
1. Use the **Match** and, optionally, **Base Name** attributes to define a regular expression for the naming of image assets that make up the grouping.

   Det reguljära uttrycket för literal Match kan till exempel se ut så här:

   `(\w+)-\w+-\w+`

1. Expandera **Radkolumnposition** och definiera sedan namnformatet för bildresursens position i 2D-rotationsmatrisen.

   Använd parentesen för att omsluta rad- eller kolumnpositionen i filnamnet.

   För en rad med ett reguljärt uttryck kan det se ut så här:

   `\w+-R([0-9]+)-\w+`

   eller

   `\w+-(\d+)-\w+`

   För det reguljära uttrycket i kolumnen kan det se ut så här:

   `\w+-\w+-C([0-9]+)`

   eller

   `\w+-\w+-C(\d+)`

   Kom ihåg att detta bara är exempel. Du kan skapa det reguljära uttrycket hur du vill.

   >[!NOTE]
   Om kombinationen av reguljära uttryck för rader och kolumner inte kan avgöra positionen för resursen i den flerdimensionella spinset-arrayen, läggs resursen inte till i uppsättningen och ett fel loggas.

1. Ange suffixet eller prefixet till basnamnet som du definierade i konventionen om namngivning av tillgångar för Ange namngivning och skapande. Ange också var bilduppsättningen ska skapas i mappstrukturen för Dynamic Media Classic.

   Om du definierar ett stort antal bilduppsättningar kanske du föredrar att hålla dessa åtskilda från de mappar som innehåller själva resurserna. Många kunder skapar en mapp för bilduppsättningar och dirigerar om programmet för att placera gruppuppsättningar som genererats här.

1. Klicka på **Spara** på panelen Detaljer.
1. Ladda upp och publicera din snurruppsättning som vanligt och se till att du aktiverar namnet på din 2D-snurruppsättning i dialogrutan Alternativ för jobbinläsning under Gruppera förinställningar.

>[!MORELIKETHIS]
* [Förhandsgranska en resurs](previewing-asset.md#previewing_an_asset)
* [Konfigurera bildförinställningar](setting-image-presets.md#setting_up_image_presets)
* [Visa, lägga till och exportera metadata](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
* [Kontrollerar jobbfiler](checking-job-files.md#checking_job_files)

