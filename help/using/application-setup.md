---
title: Programinställningar
description: Lär dig hur du konfigurerar programområdet i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: 3f96606e-ef5c-4c01-aa0f-3148f14e28be
topic: Administration
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '10351'
ht-degree: 1%

---

# Programinställningar{#application-setup}

Du kan använda programinställningssidorna för att ange allmänna inställningar, skapa bildförinställningar, förinställningar för videokodning, förinställningar för visningsprogram eller för att definiera standardvisningsprogram och metadata. Du kan konfigurera gruppuppsättningsförinställningar så att de automatiserar genereringen av 2D-snurpuppsättningar (till exempel), publiceringsinställningar och video-SEO-inställningar.

>[!NOTE]
>
>Endast Adobe Dynamic Media Classic-administratörer kan ändra inställningarna i Programinställningar.

## Allmänna inställningar {#general-settings}

Öppna sidan Allmänna inställningar för programmet genom att gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** i fältet Global navigering.

### Servrar

När du skapar ett konto tillhandahåller Adobe Dynamic Media Classic automatiskt de tilldelade servrarna för ditt företag. De här servrarna används för att skapa URL-strängar för din webbplats och dina program. Dessa URL-anrop är specifika för ditt konto.

Se även [Testa tjänsten Secure Testing](testing-assets-making-them-public.md#testing_the_secure_testing_service).

* **[!UICONTROL Published Server Name]**: Den här servern är den aktiva CDN-servern (Content Deliver Network) som används i alla systemgenererade URL-anrop som är specifika för ditt konto. Ändra bara det här servernamnet om du har instruerats att göra det av en Adobe Dynamic Media Classic supporttekniker.

* **[!UICONTROL Origin Server Name]**: Den här servern används endast för kvalitetstestning. Ändra bara det här servernamnet om du har instruerats att göra det av en Adobe Dynamic Media Classic supporttekniker.

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by an Adobe DynamicMedia Classic support technician. -->

* **[!UICONTROL Test&Target Server Name]**: Test&amp;Target-URL, inklusive `.com`. Instruktioner om hur du hämtar den här URL:en finns i Integrera [!DNL Adobe Dynamic Media Classic] med [!DNL Adobe Target Standard/Premium].

<!-- **Test Publish Context Server Name** -->

* **[!UICONTROL iOS Streaming Server Name]**: URL:en till din [!DNL Adobe Dynamic Media Classic] iOS-direktuppspelningsserver. Den här servern levererar direktuppspelad video till iOS-baserade enheter med HTTP-protokollet.

* **[!UICONTROL Progressive Video Server Name]**: URL:en till den [!DNL Adobe Dynamic Media Classic] progressiva videoservern. Den här servern levererar progressiv video med HTTP-protokollet.

* **[!UICONTROL Show URL for unpublished assets]**: Välj det här alternativet om du vill att [!DNL Adobe Dynamic Media Classic] ska visa en URL när du förhandsgranskar en resurs, publicerad eller inte. Om resursen inte publiceras fungerar inte URL:en. Du kan dock använda URL-adressen för planering eller organisering.

<!-- **Allow AIR install** Select this option to allow users to download Adobe Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the Web version of Adobe Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Adobe Dynamic Media Classic AIR. Adobe Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **[!UICONTROL CDN Invalidation Template]**: Anger den mall som används för att ogiltigförklara CDN-cachen (Content Delivery Network).

  Anta till exempel att du anger en bild-URL (inklusive bildförinställningar eller modifierare) som refererar till `<ID>`, i stället för ett specifikt bild-ID som i följande exempel:

  `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

  Om mallen bara innehåller `<ID>` fyller Adobe Dynamic Media Classic i `https://<server>/is/image`, där `<server>` är det publiceringsservernamn som definieras i Allmänna inställningar.

  Om du ställer in mallen för invalidering av CDN markerar du en bild med namnet Backpack_B och går sedan till **[!UICONTROL File]** > **[!UICONTROL Invalidate CDN]** så skapas följande genererade URL i gränssnittet för CDN-invalidering:

  `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

  I listrutan URL väljer du **[!UICONTROL Continue]** för att rensa cachen för det specifika bild-URL-anropet. Du kan också lägga till URL-adresser genom att skriva eller klistra in dem i listrutan URL. Du behöver inte ställa in mallen i förväg.

  När du har valt en mall för CDN-validering och gjort en begäran om ogiltig CDN visas en indikator i användargränssnittet. Du får en uppskattning av hur lång tid det tar att rensa cachen.

  När du klickar på **[!UICONTROL File]** > **[!UICONTROL Invalidate CDN]** refereras varje bild till i den sparade mall-URL:en om flera bilder är markerade i Dynamic Media Classic. Därför kan du definiera en mall för Ovalidering av CDN som refererar till varje URL som finns på webbplatsen (t.ex. produktinformation och sökresultat). När du sedan markerar en eller flera bilder som ska ogiltigförklaras från cachen fyller URL-adresserna automatiskt i gränssnittet.

  Se [Cachelagring av innehåll](dmc-platform-overview.md#content_caching).

  Se [Återpublicerade resurser och CDN-fördröjningar](publishing-files.md#republished_assets_and_cdn_delays).

### Bläddra

* **[!UICONTROL Show Projects]**: Avgör om projekt är tillgängliga som ett sätt att ordna dina Adobe Dynamic Media Classic-resurser. Se [Organisera ditt arbete med projekt](/help/using/organizing-projects.md).

* **[!UICONTROL Show Sample eVideo Content]**: Aktivera eller inaktivera visning av exempelinnehåll för eVideo.

* **[!UICONTROL Show Generated Content]**: I mappar visas innehåll som genererats från en resurs. När en PDF-fil till exempel rastreras när den överförs, skapas en bild för varje sida i den ursprungliga PDF. Om Visa genererat innehåll är markerat visas varje genererad bild när den ursprungliga PDF överförs. Det visas tillsammans med PDF i den mapp som PDF överfördes till.

* **[!UICONTROL Show Encoded Videos]**: Avmarkerat (av) som standard.

  Du kan snabbt söka efter och bläddra bland videofilmer i Adobe Dynamic Media Classic utan att behöva navigera i ett antal kodade derivat av samma videofil. Låt alternativet vara avmarkerat (standard). Endast den primära videominiatyrbilden (den källvideo som du överförde och använde för att skapa derivat) och den överordnade miniatyrbilden för den anpassade videouppsättningen (som innehåller de underordnade derivaten för den kodade videouppsättningen) visas.

  Du kan dock fortfarande komma åt enskilda kodade videoklipp från den primära videon eller den adaptiva videouppsättningen. Om du vill göra det dubbelklickar du på miniatyrbilden för videon för att öppna detaljvyn. Välj sedan **[!UICONTROL Encoded Videos]** i den högra panelen så att du kan komma åt alla underordnade videor.

  Du kan också gå till **[!UICONTROL File]** > **[!UICONTROL Reprocess]** för att skapa mer kodade underordnade videor direkt från en adaptiv videouppsättning. Adobe Dynamic Media Classic hittar automatiskt den&quot;överordnade&quot; primära videon i den adaptiva videouppsättningen och använder den som källvideo för transkodning. När du sparar de nya enskilda kodade videofilmerna visas de dock inte när du söker efter eller bläddrar. De är dock fortfarande tillgängliga på fliken Kodade videoklipp i detaljvyn.

  Se [Överför och koda om videor](uploading-encoding-videos.md#uploading_and_encoding_videos).

  Välj **[!UICONTROL Show Encoded Videos]** om du vill ha fortsatt åtkomst till alla dina kodade videoderivat när du söker och bläddrar.

  Det finns vissa åtgärder på menyn Skapa som bara fungerar, eller eventuellt fungerar, med enskilda videor. Den här funktionen gör det nödvändigt att visa alla kodade videoderivat som du kan välja mellan, oavsett hur du anger **[!UICONTROL Show Encoded Videos]**. De Build-åtgärder som åsidosätter inställningen **[!UICONTROL Show Encoded Videos]** omfattar **[!UICONTROL Adaptive Video Sets]** och **[!UICONTROL eCatalogs]**.

  >[!NOTE]
  >
  >Om du inte använde Adobe Dynamic Media Classic för att överföra och koda videoresurser visar Adobe Dynamic Media Classic alla dina enskilda kodade videor, även om det här alternativet är avmarkerat.

* **[!UICONTROL Show Refresh Subfolders Button]**: Aktivera eller inaktivera visning av knappen Uppdatera för undermappar.

### ADOBE DYNAMIC MEDIA CLASSIC FTP

* **[!UICONTROL Server]**: Visar din FTP-kontoserver.

* **[!UICONTROL User Name]**: Visar användarnamnet för ditt FTP-konto.

### Överför till program

Se även [Alternativ för överföringsjobb](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/569_Default%20Job%20Options_converted%20renamed_Getting%20Started-AVS) utbildningsvideo.

* **[!UICONTROL Overwrite Images]**: Adobe Dynamic Media Classic tillåter inte att två filer har samma namn. Varje objekts Adobe Dynamic Media Classic-ID (bildnamnet minus filnamnstillägget) måste vara unikt. På grund av den här regeln har dialogrutan Överför ett överskrivningsalternativ. Den exakta effekten av det här alternativet beror på det angivna alternativet Skriv över bilder. Dessa alternativ anger hur ersättningsbilder överförs: om de ersätter originalbilderna eller blir dubblettbilder. Duplicerade bilder får ett nytt namn med namnet&quot;-1&quot; (till exempel heter stol.tif stol-1.tif). De här alternativen påverkar bilder som har överförts till en annan mapp än den ursprungliga eller bilder med ett annat filnamnstillägg än den ursprungliga (till exempel JPG, TIF eller PNG). Se [Använda alternativet Skriv över bilder](#using-the-overwrite-images-option).

   * **[!UICONTROL Overwrite in current folder, same base image name or extension]**: Det här alternativet är den striktaste regeln för ersättning. Det kräver att du överför ersättningsbilden till samma mapp som originalbilden och att ersättningsbilden har samma filnamnstillägg som originalbilden. Om dessa krav inte uppfylls skapas en dubblett.

   * **[!UICONTROL Overwrite in current folder, same base asset name regardless of extension]**: Du måste överföra ersättningsbilden till samma mapp som originalet, men filnamnstillägget kan skilja sig från originalet. Till exempel ersätter stol.tif stol.jpg.

   * **[!UICONTROL Overwrite in any folder, same base asset name or extension]**: Kräver att ersättningsbilden har samma filnamnstillägg som den ursprungliga bilden. Till exempel måste stol.jpg ersätta stol.jpg, inte stol.tif). Du kan dock överföra ersättningsbilden till en annan mapp än den ursprungliga. Den uppdaterade bilden finns i den nya mappen. Det går inte längre att hitta filen på den ursprungliga platsen

   * **[!UICONTROL Overwrite in any folder, same base asset name regardless of extension]**: Det här alternativet är den mest omfattande ersättningsregeln. Du kan överföra en ersättningsbild till en annan mapp än den ursprungliga, överföra en fil med ett annat filnamnstillägg och ersätta den ursprungliga filen. Om originalfilen finns i en annan mapp finns ersättningsbilden i den nya mappen som den överfördes till.

* **[!UICONTROL Retain Publish]**: Anger om en ersättningsbild som överförs till Adobe Dynamic Media Classic ska behålla inställningen Ready to Publish för den bild den ersätter. Eller så anges inställningen vid överföring.

* **[!UICONTROL Default Color Profiles]**: Anger de färgprofiler som används som en del av alternativen för standardfärgprofil när CMYK-bilder läggs till.

* **[!UICONTROL Default Upload Options]**: Öppnar dialogrutan Alternativ för överföring av jobb, där du kan ange standardalternativ för överföring. Mer information om de här alternativen finns i [Överföringsalternativ](/help/using/uploading-files.md#upload_options).

### Redigerare för bildschema (till program)

* **[!UICONTROL Default Image Mapping HREF]**: Definierar den standard-URL som används för HREF-kolumnen i bildmappningen. Den här URL:en är den standardadress som visas när du skapar bildscheman.

* **[!UICONTROL Default Image Mapping Template]**: Definierar JavaScript som standard för HREF-mallen i bildmappningen. Du kan ange att en anpassad kod ska köras när du väljer en bildschema här.

### Andra inställningar (till program)

* **[!UICONTROL Trash Can Clean Up Warnings]**: Assets i papperskorgen tas bort automatiskt inom sju dagar. Välj&quot;Skicka e-post innan papperskorgen tas bort automatiskt&quot; om du vill att meddelanden ska skickas till företagsadministratörer när resurser i papperskorgen inte tas bort permanent om fyra dagar. Se [Hantera papperskorgen](/help/using/trash-folder.md).

## Använda alternativet Skriv över bilder {#using-the-overwrite-images-option}

Adobe Dynamic Media Classic tillåter inte att två filer har samma namn. Varje objekts Adobe Dynamic Media Classic-ID (bildnamnet minus filnamnstillägget) måste vara unikt. På grund av den här regeln innehåller dialogrutan Överför alternativ för Skriv över bilder. Den exakta effekten av det här alternativet beror på en inställning för varje företags Adobe Dynamic Media Classic Internal Settings.

Om du tidigare överförde bilder och sedan ändrade originalfilerna (eller ersatt dem) anger det valda alternativet Skriv över hur Adobe Dynamic Media Classic ska ersätta bilderna. Ingen information om bilden ändras, men den nya bilden ersätter den gamla. Om mappen även innehåller bilder som inte redan finns i Adobe Dynamic Media Classic läggs dessa bilder till.

Använd det här alternativet om överförda bilder har ändrats på något sätt (bilden har ändrats) men referensen till bilden är densamma. Skriv över är också användbart när du överför och rippar Adobe® PDF. Du kan finjustera hur Adobe Dynamic Media Classic *rippar* bilden. Du kan också justera ICC-färgprofilalternativen i dialogrutan Överför och överföra igen med hjälp av överskrivningsfunktionen.

De Adobe Dynamic Media Classic-ID:n som används för att få åtkomst till bilder från produktionsservrarna härleds från bildens filnamn. Det är viktigt att du använder versaler och gemener i filnamnet, både när du ersätter befintliga filer och när du ersätter de Adobe Dynamic Media Classic-id:n som används för att komma åt bilden. Det är korrekt att använda filnamn med versaler och gemener innan du överför dem till Adobe Dynamic Media Classic för att undvika Adobe Dynamic Media Classic-ID:n som bara skiljer sig åt för samma bild.

Om du avmarkerar det här alternativet behandlas alla bilder med samma filnamn som befintliga bilder som dubbletter och läggs inte till.

## Bildförinställningar {#image-presets}

Skärmen Bildförinställningar används för att skapa och redigera bildförinställningar. Med bildförinställningar kan Adobe Dynamic Media Classic leverera bilder dynamiskt i olika storlekar från samma primära bild. Varje bildförinställning representerar en fördefinierad samling kommandon för storleksändring och formatering för visning av bilder. När du skapar en bildförinställning väljer du en storlek för bildleverans. Du kan också välja formateringskommandon så att bildens utseende optimeras när bilden levereras för visning.

Administratörer kan skapa förinställningar för att exportera resurser. Användarna kan välja en förinställning när de exporterar bilder, vilket även innebär att bilderna formateras om enligt de specifikationer som administratören anger.

Du öppnar skärmen Bildförinställning i fältet Global navigering genom att gå till **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**.

Se [Smart bildbehandling](https://experienceleague.adobe.com/sv/docs/experience-manager-65/content/assets/dynamic/imaging-faq).

### Skapa och redigera bildförinställningar {#creating-and-editing-image-presets}

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**.
1. Skapa en förinställning eller börja från en befintlig:

   * **Skapa en bildförinställning**: Välj **[!UICONTROL Add]**.
   * **Skapa en bildförinställning från en befintlig förinställning**: Markera den bildförinställning som är mest lik den du vill skapa och välj sedan **[!UICONTROL Edit]**.

1. Ange ett namn för förinställningen på sidan Lägg till (eller Redigera) förinställning.
1. Ange de förinställningsalternativ som du vill använda.

   Se [Alternativ för bildförinställning](application-setup.md#image_preset_options).

1. Välj **[!UICONTROL Save]**, eller om du började från en befintlig förinställning, välj **[!UICONTROL Save As]**.
1. Om du vill förhandsvisa förinställningen med din egen bild väljer du **[!UICONTROL Browse]** och sedan en bild. Om du vill förhandsvisa med standardbilden väljer du **[!UICONTROL Reset]**.

Du kan redigera en bildförinställning genom att markera namnet på skärmen Bildförinställningar och sedan välja **[!UICONTROL Edit]**. Om du vill ta bort en bildförinställning markerar du den och väljer sedan **[!UICONTROL Delete]**.

### Alternativ för bildförinställning {#image-preset-options}

Skärmarna Lägg till förinställning och Redigera förinställning innehåller följande alternativ för att skapa och redigera bildförinställningar:

* **[!UICONTROL Preset Name]**: Ange ett beskrivande namn utan blanksteg. Om du vill hjälpa användare att identifiera den här bildförinställningen tar du med bildstorleksspecifikationen i namnet.

* **[!UICONTROL Width and Height]**: Ange storleken som bilden levereras med i pixlar.

* **[!UICONTROL Format]**: Välj ett format på menyn. Om du väljer formatet GIF, JPEG, PDF eller TIFF får du fler alternativ:

   * Alternativ för färgkvantifiering i GIF

      * **[!UICONTROL Type]**: Välj Adaptiv (standard), Webb eller Mac. Om du väljer **[!UICONTROL GIF With Alpha]** är alternativet Mac inte tillgängligt.

      * **[!UICONTROL Dither]**: Välj Diffusera eller Av.

      * **[!UICONTROL Number Of Colors]**: Dra skjutreglaget för att ange 2-255.

      * **[!UICONTROL Color List]**: Ange en kommaavgränsad lista. Ange till exempel `000000,888888,ffffff` för vitt, grått och svart.

   * Alternativ för JPEG

      * **[!UICONTROL Quality]**: Styr komprimeringsnivån JPEG. Den här inställningen påverkar både filstorlek och bildkvalitet. Kvalitetsskalan JPEG är 1-100.

      * **[!UICONTROL Enable JPG Chrominance Downsampling]**: Eftersom ögat är mindre känsligt för högfrekvent färginformation än högfrekvent luminans, delas bildinformation in i luminans och färgkomponenter i JPEG-bilder. När en JPEG-bild komprimeras lämnas luminanskomponenten i full upplösning, medan färgkomponenterna nedsamplas genom att medelvärdet av alla pixelgrupper ökas. Nedsampling minskar datavolymen med en halv eller en tredjedel utan att det påverkar den upplevda kvaliteten. Nedsampling kan inte användas för gråskalebilder. Den här tekniken minskar mängden komprimering som är användbar för bilder med hög kontrast (till exempel bilder med överlagrad text).

   * Alternativ för PDF och TIFF

      * **[!UICONTROL Compression]**: Välj en komprimeringsalgoritm.

* **[!UICONTROL Colorspace]**: Välj en färgrymd.

* **[!UICONTROL Sharpening]**: Välj alternativet Aktivera enkel skärpa om du vill använda ett grundläggande skärpefilter på bilden när all skalning har gjorts. Skärpa kan kompensera för oskärpa som kan uppstå när du visar en bild i en annan storlek.

  Mer information om skärpa, omsamplingslägen och oskarp maskning finns i [Öka skärpan i en bild](sharpening-image.md#sharpening_an_image). Se även utbildningsvideon [Skärpa](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS).

* **[!UICONTROL Resample Mode]**: Välj ett alternativ för omsamplingsläge. Dessa alternativ gör bilden skarpare när den nedsamplas:

* **[!UICONTROL B-Linear]**: Den snabbaste omsamplingsmetoden. Vissa aliasing-artefakter är märkbara.

* **[!UICONTROL Bi-Cubic]**: Ökar processoranvändningen på bildservern, men ger skarpare bilder med mindre märkbara aliaseringsartefakter.

* **[!UICONTROL `Sharp 2`]**: Kan ge något skarpare resultat än alternativet Bi-Cubic, men till ännu högre processorkostnad på Image Server.

* **[!UICONTROL Tri-Linear]**: Använder både högre och lägre upplösningar, om sådana finns. Rekommenderas bara när alias är ett problem. Den här metoden minskar storleken på JPEG på grund av reducerade högfrekventa data.

* **[!UICONTROL Unsharp Masking]**: Välj följande alternativ för att finjustera skärpan:

* **[!UICONTROL Amount]**: Styr mängden kontrast som används på kantpixlar. Standardvärdet är 1.0. För högupplösta bilder kan du öka den till upp till 5.0. Tänk på Mängd som ett mått på filterintensiteten.

* **[!UICONTROL Radius]**: Anger antalet pixlar runt kantpixlarna som påverkar skärpan. För högupplösta bilder anger du 1 till 2. Med ett lågt värde ökas skärpan endast för kantpixlarna. Med ett högt värde ökas skärpan för ett bredare intervall av pixlar. Vilket värde som är korrekt beror på bildens storlek.

* **[!UICONTROL Threshold]**: Anger det kontrastintervall som ska ignoreras när det oskarpa maskfiltret används. Det innebär att det kan hjälpa till att lösa hur olika de pixlar som skärps måste vara från det omgivande området innan de betraktas som kantpixlar och skärpa. Experimentera med värden mellan `.02` och `0.2` för att undvika att införa brus. Standardvärdet 6 innebär att skärpan ökas för alla pixlar i bilden.

* **[!UICONTROL Color Space]**: Avgör om bilden använder det utrymme som bilden skapades i, vanligtvis RGB (original) eller ett luminansutrymme (intensitet).

* **[!UICONTROL Color]** Välj följande alternativ:

* **[!UICONTROL Output Color Profile]**: Välj **[!UICONTROL Use Default]** eller någon av de ICC-färgprofiler som är tillgängliga på Adobe Dynamic Media Classic.

  Se även [ICC-profiler](icc-profiles.md#icc_profiles).

* **[!UICONTROL Rendering Intent]**: Välj ett alternativ om du vill åsidosätta färgprofilens standardåtergivningsmetod. Använd det här alternativet när en av ICC-standardprofilerna är målfärgrymden för en färgkonvertering. Eller så karakteriserar den här profilen utdataenheten (skrivaren eller bildskärmen) och den angivna återgivningsmetoden är giltig för den här profilen.

* **[!UICONTROL Embed Profile]**: Välj det här alternativet så att den här profilen används om du öppnar bilden i Adobe® Photoshop®.

* **[!UICONTROL Print Resolution]**: Välj en upplösning för utskrift av den här bilden. 72 pixlar är standardvärdet.

* **[!UICONTROL URL Modifiers]**: Om du föredrar att ange URL-modifierare som definierar bildförinställningen, i stället för inställningarna, anger du modifieringarna här.

* **[!UICONTROL Sample Image URL]**: Visar den &quot;raw&quot;-URL-sträng som Dynamic Media Image Server använder för att leverera bilder med den bildförinställning som du lägger till eller redigerar. Den här URL-strängen kodar alla formatinställningar som du väljer på skärmen Lägg till förinställning eller Redigera förinställning.

### Redigera, ta bort eller inaktivera en bildförinställning {#editing-removing-or-deactivating-an-image-preset}

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**.
1. Välj en förinställning i tabellen på skärmen Bildförinställningar och gör sedan något av följande:

   * Välj **[!UICONTROL Edit]** och ange sedan nya alternativ i dialogrutan Redigera förinställning.
   * Välj **[!UICONTROL Delete]** om du vill ta bort förinställningen från listan.
   * Avmarkera kryssrutan **[!UICONTROL Active]** bredvid ett förinställningsnamn om du vill ta bort den från hela Adobe Dynamic Media Classic-användargränssnittet för MediaPortal-användare.

## Aktivera eller inaktivera adaptiva videoförinställningar {#activating-or-deactivating-adaptive-video-presets}

Adobe Dynamic Media Classic har förinställningar för adaptiv videokodning. Det är en primär lista med förinställningar som kombinerar både 16:9 adaptiva videoförinställningar och 4:3 adaptiva videoförinställningar i en grupp. Dessa fördefinierade förinställningar återspeglar de vanligaste kodningsinställningarna och är optimerade för uppspelning på mobila målenheter, surfplattor och datorer.

Endast kodningsförinställningar för adaptiv video aktiveras (aktiverat eller aktiverat) som standard. Du kan avaktivera den om du vill. Inaktiva adaptiva videoförinställningar visas inte som ett valbart alternativ i delen eVideo i dialogrutan Alternativ för överföringsjobb.

Se [Överför och koda videoklipp](uploading-encoding-videos.md#uploading_and_encoding_videos).

Se även utbildningsvideon [Videoförinställningar](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS).

**Så här aktiverar eller inaktiverar du anpassade videoförinställningar:**

1. I Adobe Dynamic Media Classic övre högra hörn går du till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]** > **[!UICONTROL Adaptive Video Presets]**.
1. På sidan Adaptiva videoförinställningar avmarkerar du kryssrutan bredvid ett förinställningsnamn för att ta bort förinställningen från listan eVideo-alternativ i dialogrutan Alternativ för överföringsjobb.
1. Välj **[!UICONTROL Close]**.

## Videoförinställningar för kodning av videofiler {#video-presets-for-encoding-video-files}

Om du vill välja en kodningsförinställning väljer du **[!UICONTROL Job Options]** längst ned till höger på sidan Överför. Expandera eVideo-alternativ i dialogrutan Alternativ för överföring av jobb och välj önskade förinställningar för videokodning.

>[!NOTE]
>
>Förutom &quot;Adaptiv video&quot;, som är aktiverat som standard, kan du inte se alla andra adaptiva video- eller enstaka videokodningsförinställningar i dialogrutan Alternativ för överföringsjobb. Adobe Dynamic Media Classic-administratörer avgör vilka förinställningar för videokodning som visas i dialogrutan Alternativ för överföringsjobb.

* Välj bland följande adaptiva videokodningsförinställningar eller enkodningsförinställningar:

   * **[!UICONTROL 16:9 Adaptive Video]**: Skapa videor med 16:9-proportioner för leverans till datorer, mobiler (iPhone, iPad, Android™) och surfplattor (iPad, Android™), optimerade med den upplösning och bithastighet som bäst matchar tittarens anslutningshastighet.

   * **[!UICONTROL 4:3 Adaptive Video]**: Skapa videor med 4:3-proportioner för leverans till datorer, mobiler (iPhone, iPad, Android™) och surfplattor (iPad, Android™), optimerade med den upplösning och bithastighet som bäst matchar tittarens anslutningshastighet.

   * **[!UICONTROL Adaptive Video]**: En förinställning för enskild kodning som fungerar med alla proportioner för att skapa videor för leverans till mobilen, surfplattan och datorn. Överförda källvideor som är kodade med den här förinställningen har en fast höjd. Bredden skalas dock automatiskt så att videons proportioner bevaras.

     Den här flexibiliteten med automatisk skalförändring är också tillgänglig som standard när du skapar en egen förinställning för videokodning.

     Se [Lägga till eller redigera en förinställning för videokodning](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset).

   * **[!UICONTROL Adaptive Video Encoding (16:9 or 4:3)]**: Skapa videor med 16:9- och 4:3-proportioner för datorer, mobiler (iPhone, iPad, Android™) och surfplattor (iPad, Android™). Alla optimerade med den upplösning och bithastighet som bäst matchar tittarens anslutningshastighet.

     Se [Videoförinställningar för adaptiv videokodning (16:9 eller 4:3)](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets).

   * **[!UICONTROL Single Encoding Presets]**

     >[!NOTE]
     >
     >Om du vill leverera video till iPad kan du välja en Mobile-kodningsförinställning eller en kodningsförinställning för Tablet. Förinställningar för surfplattor är särskilt utformade för iPad, vanligtvis med högre upplösning och kvalitet för att dra nytta av den större skärmstorleken och bandbreddsanslutningen. För att kunna leverera videofiler som är kodade med en Tablet-förinställning måste du inkludera enhetsidentifieringskod på din mobila webbplats eller i ditt mobila program. Den här koden växlar mellan en iPhone- eller iPad-videoupplevelse, beroende på uppspelningsenheten. Att välja en Mobile-förinställning för att leverera videofiler till iPad är ett enklare arbetsflöde. Orsaken är att du kan använda samma videofil för både iPhone och iPad. Kvaliteten standardiseras dock med iPhone med lägre upplösning.

      * I gruppen Kodningsförinställningar väljer du Namn eller Storlek i listrutan Sortera kodningsförinställningar om du vill sortera förinställningar efter namn eller upplösning.
      * Välj en kodningsförinställning baserat på upplösningsstorleken och bandbredden som du vill spela upp videon med.
      * Du kan välja Adaptiv videokodning och en eller flera kodningsförinställningar per video. Du kan till exempel koda en fil för både dator och mobil i ett överföringsjobb.

När du har valt **[!UICONTROL Start Upload]** överförs den ursprungliga primära videofilen och kodade filer genereras från den primära filen.

### Om alternativ för kodningsförinställningar {#about-encoding-preset-options}

Parametrarna för de förinställda alternativen för kodning är följande:

* **[!UICONTROL Target connection speed]**: Slutanvändarens internetanslutning.

* **[!UICONTROL Encoded file suffix]**: Det suffix som är kopplat till den kodade videofilen i identifieringssyfte.

* **[!UICONTROL Video bit rate (data rate)]**: Den datamängd som kodas för att skapa en enda sekund av videouppspelning (i kilobit per sekund).

* **[!UICONTROL Pixel Width/Height]**: Skärmbildens bredddimension i pixlar; skärmbildens höjddimension (i pixlar).

* **[!UICONTROL Frame per second (fps)]**: Antalet bildrutor, eller stillbilder, för varje sekund i videon. I USA och Japan spelas de flesta videoklipp in med 29,97 fps. I Europa och Asien (utom Japan) spelas de flesta videoklipp in med 25 fps. Filmen filmas med 24 fps.

* **[!UICONTROL Audio bit rate]**: Den datamängd som kodas för att skapa en enda sekund av ljuduppspelning, i kilobit per sekund.

I följande tabeller visas de bästa sätten att välja videoförinställningar och de namnkonventioner som används för att ange kodade filer.

### Adaptiv video (standard) {#adaptive-video-default}

En förinställning för kodning som fungerar med alla proportioner så att du kan skapa videor för leverans till mobilen, surfplattan och datorn. Överförda källvideor som är kodade med den här förinställningen (standard och bästa praxis) är inställda på en fast höjd, medan bredden automatiskt skalas för att bevara videons proportioner.

**Adaptiv video (standard)**

|  | Kodningsförinställningsnamn/knappbeskrivningstext | Kodat filsuffix | Videodatahastighet (kbit/s) | Bredd/höjd (pixlar) | FPS | Bithastighet för ljud (kbit/s) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | Auto × 360, 800 kbit/s | _Mobile_Auto×360p_800K | 800 | Auto×360 | Samma som källan | 64 | För mobiler (iPhone, iPad, Android™) |
| 2 | Auto × 480, 1 400 kbit/s | _Tablet_Auto×480p_1400K | 1400 | Auto×480 | Samma som källan | 96 | För surfplattor (iPad, Android™) |
| 3 | Auto × 720, 2 600 kbit/s | _Desktop_Auto×720p_2600K | 2600 | Auto×720 | Samma som källan | 128 | För datorer |

### Förinställningar för adaptiv videokodning (16:9 eller 4:3) {#adaptive-video-encoding-or-video-presets}

Dessa förinställningar för adaptiv videokodning kombinerar en serie individuella kodningsförinställningar som automatiskt väljs åt dig baserat på proportionerna för den video som du överförde. Om du till exempel överför en 4:3-video kodas den automatiskt med alla fem 4:3-förinställningar som finns i den primära förinställningslistan i alternativet **Adaptiv videokodning (16:9 eller 4:3)** .

Mer information om parametrar för kodningsalternativ finns i [Om alternativ för kodningsförinställningar](application-setup.md#about_encoding_preset_options).

**Förinställningar för adaptiv videokodning (16:9 eller 4:3)**

|  | Kodningsförinställningsnamn/knappbeskrivningstext | Målanslutningshastighet (kbit/s) | Kodat filsuffix | Videodatahastighet (kbit/s) | Bredd/höjd (pixlar) | FPS | Bithastighet för ljud (kbit/s) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | `16:9, 512x288, Mobile (iPhone, iPad, Android&trade;), (400 Kbps)` | 500 | _Mobile_512x288_400K | 400 | 512x288 | Samma som källan | 64 | Låg upplösning, 3G |
| 2 | `4:3, 384x288px, Mobile (iPhone, iPad, Android&trade;), (400 Kbps)` | 500 | _Mobile_384x288_400K | 400 | 384x288 | Samma som källan | 64 | Låg upplösning, 3G |
| 3 | `16:9, 512x288, Mobile (iPhone, iPad, Android&trade;), (600 Kbps)` | 700 | _Mobile_512x288_600K | 600 | 512x288 | Samma som källan | 64 | Medium upplösning, 3G |
| 4 | `4:3, 384x288, Mobile (iPhone, iPad, Android&trade;), (600 Kbps)` | 700 | _Mobile_384x288_600 | 600 | 384x288 | Samma som källan | 64 | Medium upplösning, 3G |
| 5 | `16:9, 640x360, Tablet (iPad, Android&trade;), (800 Kbps)` | 900 | _iPad_640x360_800K | 800 | 640x360 | Samma som källan | 80 | Medium upplösning, WiFi |
| 6 | `4:3, 640x480, Tablet (iPad, Android&trade;), (800 Kbps)` | 900 | _iPad_640x480_800K | 800 | 640x480 | Samma som källan | 80 | Medium upplösning, WiFi |
| 7 | `16:9, 768x432, Tablet (iPad, Android&trade;), (1200 Kbps)` | 1,5 Mbit/s | _iPad_768x432_1200K | 1200 | 768x432 | Samma som källan | 96 | Hög upplösning, WiFi |
| 8 | `4:3, 768x576, Tablet (iPad, Android&trade;), (1200 Kbps)` | 1,5 Mbit/s | _iPad_768x576_1200K | 1200 | 768x576 | Samma som källan | 96 | Hög upplösning, WiFi |
| 9 | `16:9, 1280x720, Desktop, (2000 Kbps)` | 3,0 Mbit/s | _1280x720_2000K | 2000 | 1280x720 | Samma som källan | 128 | HD, widescreen |
| 10 | `4:3, 1280x960, Desktop, (2000 Kbps)` | 3,0 Mbit/s | _1280x960_2000K | 2000 kbit/s | 1280x960 | Samma som källan | 128 | HD |

### Videokodningsförinställningar för datorer {#desktop-video-encoding-presets}

Videokodningsförinställningar för MP4 och OGV på stationära datorer.

Mer information om parametrar för kodningsalternativ finns i [Om alternativen för kodningsförinställningar](application-setup.md#about_encoding_preset_options).

**H264 Main 3.2: Audio AAC, MP4 file extension**

|  | Kodningsförinställningsnamn/knappbeskrivningstext | Målanslutningshastighet (kbit/s) | Kodat filsuffix | Videodatahastighet (kbit/s) | Bredd/höjd (pixlar) | FPS | Bithastighet för ljud (kbit/s) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480x270 (400 kbit/s) | 500 | _480x270_400K | 400 | 480x270 | Samma som källan | 64 | Låg widescreen-upplösning |
| 2 | 16:9, 640x360 (800 kbit/s) | 900 | _640x360_800K | 800 | 640x360 | Samma som källan | 80 | Medium widescreen-upplösning |
| 3 | 16:9, 800x450 (1 200 kbit/s) | 1,5 Mbit/s | _800x450_1200K | 1200 | 800x450 | Samma som källan | 96 | Medium - hög upplösning |
| 4 | 16:9, 1 280 x 720 (2 000 kbit/s) | 3,0 Mbit/s | _1280x720_2000K | 2000 | 1280x720 | Samma som källan | 128 | HD, widescreen |
| 5 | 4:3, 320x240 (400 kbit/s) | 500 | _320x240_400K | 400 | 320x240 | Samma som källan | 64 | Låg upplösning |
| 6 | 4:3, 480x360 (800 kbit/s) | 900 | _480x360_800K | 800 | 480x360 | Samma som källan | 80 | Medium |
| 7 | 4:3, 640x480 (1 200 kbit/s) | 1,5 Mbit/s | _640x480_1200K | 1200 | 640x480 | Samma som källan | 96 | Medium - hög upplösning |
| 8 | 4:3, 1 280 x 960 (2 000 kbit/s) | 3,0 Mbit/s | _1280x960_2000K | 2000 | 1280x960 | Samma som källan | 128 | HD |

**OGG Theora Vorbis: OGV-filtillägg**

|  | Kodningsförinställningsnamn/knappbeskrivningstext | Målanslutningshastighet (kbit/s) | Kodat filsuffix | Videodatahastighet (kbit/s) | Bredd/höjd (pixlar) | FPS | Bithastighet för ljud (kbit/s) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480x270 (400 kbit/s), OGG | 500 | _OGG_480x270_400K | 400 | 480x270 | Samma som källan | 64 | Låg widescreen-upplösning |
| 2 | 16:9, 640x360 (800 kbit/s), OGG | 900 | _OGG_640x360_800K | 800 | 640x360 | Samma som källan | 80 | Medium widescreen-upplösning |
| 3 | 16:9, 800x450 (1 200 kbit/s), OGG | 1,5 Mbit/s | _OGG_800x450_1200K | 1200 | 800x450 | Samma som källan | 96 | Medium - hög upplösning |
| 4 | 16:9, 1 280 x 720 (2 000 kbit/s), OGG | 3,0 Mbit/s | _OGG_1280x720_2000K | 2000 | 1280x720 | Samma som källan | 128 | HD, widescreen |
| 5 | 4:3, 320x240 (400 kbit/s), OGG | 500 | _OGG_320X240_400K | 400 | 320x240 | Samma som källan | 64 | Låg upplösning |
| 6 | 4:3, 480x360 (800 kbit/s), OGG | 900 | _OGG_480x360_800K | 800 | 480x360 | Samma som källan | 80 | Medium |
| 7 | 4:3, 640x480 (1 200 kbit/s), OGG | 1,5 Mbit/s | _OGG_640x480_1200K | 1200 | 640x480 | Samma som källan | 96 | Medium - hög upplösning |
| 8 | 4:3, 1 280 x 960 (2 000 kbit/s), OGG | 3,0 Mbit/s | _OGG_1280x960_2000K | 2000 | 1280x960 | Samma som källan | 128 | HD |

### Förinställningar för kodning av mobilvideo {#mobile-video-encoding-presets}

Samma som käll-fps. Förinställningar för videokodning för mobila enheter från iPhone, iPad och Android™.

Mer information om parametrar för kodningsalternativ finns i [Om alternativen för kodningsförinställningar](application-setup.md#about_encoding_preset_options).

**H264 Originalplan 2.1: Ljud-AAC, MP4-filtillägg**

|  | Kodningsförinställningsnamn/knappbeskrivningstext | Målanslutningshastighet (kbit/s) | Kodat filsuffix | Videobithastighet (kbit/s) | Pixelbredd/höjd | FPS | Bithastighet för ljud (kbit/s) | Recommendations |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512x288, mobil (400 kbit/s) | 500 | _Mobile_512x288_400K | 400 | 512x288 | Samma som källan | 64 | Låg upplösning, 3G |
| 2 | 16:9, 512x288, mobil (600 kbit/s) | 700 | _Mobile_512x288_600K | 600 | 512x288 | Samma som källan | 64 | Medium upplösning, 3G |
| 3 | 16:9, 512x288, mobil (800 kbit/s) | 900 | _Mobile_512x288_800K | 800 | 512x288 | Samma som källan | 80 | Medium-upplösning, Wi-Fi |
| 4 | 16:9, 512x288, mobil (1 000 kbit/s) | 1,2 Mbit/s | _Mobile_512x288_1000K | 1000 | 512x288 | Samma som källan | 80 | Hög upplösning, Wi-Fi |
| 5 | 16:9, 512x288, mobil (1 200 kbit/s) | 1,5 Mbit/s | _Mobile_512x288_1200K | 1200 | 512x288 | Samma som källan | 96 | Hög upplösning, Wi-Fi |
| 6 | 4:3, 384x288, mobil (400 kbit/s) | 500 | _Mobile_384x288_400K | 400 | 384x288 | Samma som källan | 64 | Låg upplösning, 3G |
| 7 | 4:3, 384x288, mobil (600 kbit/s) | 700 | _Mobile_384x288_600K | 600 | 384x288 | Samma som källan | 64 | Medium upplösning, 3G |
| 8 | 4:3, 448x336, mobil (800 kbit/s) | 900 | _Mobile_448x336_800K | 800 | 448x336 | Samma som källan | 80 | Medium-upplösning, Wi-Fi |
| 9 | 4:3, 448x336, mobil (1 000 kbit/s) | 1,2 Mbit/s | _Mobile_448x336_1000K | 1000 | 448x336 | Samma som källan | 80 | Hög upplösning, Wi-Fi |
| 10 | 4:3, 448x336, mobil (1 200 kbit/s) | 1,5 Mbit/s | _Mobile_448x336_1200K | 1200 | 448x336 | Samma som källan | 96 | Hög upplösning, Wi-Fi |

## Förinställningar för visningsprogram {#viewer-presets}

>[!NOTE]
>
>**Flash Viewers End-of-Life Notice**: Från och med den 31 januari 2017 upphörde Adobe Dynamic Media Classic officiellt stödet för visningsprogramplattformen för Flash.

En *visningsförinställning* är en samling inställningar som bestämmer hur användare visar mediefiler på datorskärmar och mobila enheter. Som administratör kan du skapa visningsförinställningar. Inställningarna är tillgängliga för en array med visningskonfigurationsalternativ. Du kan till exempel ändra visningsprogrammets visningsstorlek, zoombeteende, färgscheman, kanter och teckensnitt.

Det bästa sättet är att använda videovisningsprogram i Adobe Dynamic Media Classic HTML 5. De förinställningar som används i videovisningsprogram för HTML5 är robusta videospelare.

Genom att kombinera följande i en enda spelare:

* Möjlighet att utforma uppspelningskomponenterna med HTML5 och CSS.
* Ha inbäddad uppspelning.
* Använd adaptiv och progressiv strömning beroende på webbläsarens kapacitet.

Du kan nå ut med multimediematerial till både dator-, surfplatte- och mobilanvändare och få en smidig videoupplevelse.

Se [Om HTML5-visningsprogram](https://experienceleague.adobe.com/sv/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only) i referenshandboken för Adobe-visningsprogram.

Se [Kompatibilitetsmatris för förinställningar för Adobe Dynamic Media Classic Viewer](application-setup.md#scene7_viewer_preset_compatibility_matrix).

Se [Bästa praxis: Använda HTML5-videovisningsprogrammet](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer).

Beroende på visningsprogrammet kan du lägga till communityfunktioner. Community-funktionerna är bland annat knappen Bädda in, knappen E-post, knappen Länk och knappen Besök webbplats. Med de här knapparna kan personer som använder visningsprogrammen dela visningsprogrammet med andra eller öppna Adobe Dynamic Media Classic webbplats.

Se även [Exempel på referensbibliotek för visningsprogram i Adobe](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

### Stöd för visningsprogram för responsiva webbsidor {#viewer-support-for-responsive-designed-web-pages}

Olika webbsidor har olika behov. Ibland vill du ha en webbsida som innehåller en länk som öppnar visningsprogrammet för HTML 5 i ett separat webbläsarfönster. I andra fall måste du bädda in HTML5-visningsprogrammet direkt på värdsidan. I det senare fallet har webbsidan förmodligen en statisk layout. Eller så är den&quot;responsiv&quot; och visas på olika enheter eller för olika webbläsarfönsterstorlekar. För att tillgodose dessa behov har de HTML5-visningsprogram som medföljer Adobe Dynamic Media Classic stöd för både statiska webbsidor och responsiva webbsidor.

Mer information om hur du bäddar in responsiva visningsprogram på dina webbsidor finns i [Om bibliotek för responsiv bild](https://experienceleague.adobe.com/sv/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/c-about-responsive-static-image-library#image-serving-api), [Använd bibliotek för responsiv bild](https://experienceleague.adobe.com/sv/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library#image-serving-api) och [Kommandoreferens: Kommandoattribut](https://experienceleague.adobe.com/sv/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library#responsive-static-image-library).

### Förinställningstyper för visningsprogram {#viewer-preset-types}

Administratörer kan skapa och anpassa följande typer av visningsförinställningar:

* **[!UICONTROL eCatalog Viewer]**: Simulerar upplevelsen av att läsa en utskriven katalog. Du kan gå från sida till sida, zooma in och ut från objekt på en sida, använda Bildscheman för att visa mer information om objekt på sidan eller söka i katalogen. Du kan även inkludera en informationspanel för att visa detaljerad information och ett bildschemat objekt om mappningsområdet har ett giltigt rollover_key-attribut. Om du vill ta med en infopanel anger du en URL-adress för informationsservern på panelen Info i fönstret Förinställningar för eCatalog Viewer.

* **[!UICONTROL Swatch Set Viewer]**: Visar en bild i en annan färg, material, struktur, finish eller struktur. Användarna väljer en miniatyrbild för att se variationerna i bilden.

* **[!UICONTROL Mixed Media Set Viewer]**: Visar olika typer av media i ett visningsprogram. Du kan inkludera färgruteuppsättningar, snurruppsättningar, bilder och videoklipp. Du kan konfigurera flikar så att de innehåller olika typer av innehåll, till exempel en flik för Bilduppsättningar och en flik för videoklipp. Videofilmer som spelas upp från en blandad medieuppsättning använder ett standardvisningsprogram för video med en tidslinje och videokontroller, till exempel Stop, Pause, Rewind och Play. När du ställer in en visningsförinställning för blandad medieuppsättning anger du vilka visningsprogram du vill använda för de olika typerna av resurser i din uppsättning med blandade media. Du kan också använda stödrastervisningsprogrammet eller Carousel Viewer för att visa en blandad medieuppsättning.

* **[!UICONTROL Spin Set Viewer]**: Tillhandahåller flera vyer av en bild så att användare kan vrida objektet för att undersöka olika sidor och vinklar.

* **Videovisningsprogram**: Visar videoklipp med källfilens upplösningsdimensioner eller en anpassad storlek. Adobe Dynamic Media Classic innehåller många fördefinierade visningsförinställningar för uppspelning av video, och om du är administratör kan du skapa anpassade visningsförinställningar för video. Det finns mer än 12 olika inställningar för att konfigurera Video Viewer. Du kan konfigurera den:

   * size
   * förgrunds- och bakgrundsfärg
   * video- och ljudkontroller
   * förloppsindikator
   * skal för användargränssnitt
   * sociala funktioner
   * och hjälp

* **[!UICONTROL Zoom Viewers]**: Du kan välja mellan tre typer av zoomvisningsprogram:

* **[!UICONTROL Zoom Viewer]**: Låter användarna zooma in i området genom att markera det. De kan välja kontroller för att zooma in, zooma ut och återställa bilden till standardstorleken.

* **[!UICONTROL Zoom Viewer: Fly-out]**: Visar en andra bild av det zoomade området bredvid originalbilden. Det finns inga kontroller att använda. Användarna flyttar bara markeringen över det område som de vill visa.

När du fastställer den fullständiga bandbreddsanvändningen för det här visningsprogrammet bör du tänka på att både huvudbilden och den utfällbara bilden visas i visningsprogrammet. Huvudbildens storlek (scenens bredd och höjd) och zoomfaktorn bestämmer den utfällbara bildens storlek. Om du vill förhindra att den utfällbara filstorleken blir för stor ska du balansera dessa två värden: om du har en stor huvudbildstorlek ska du sänka värdet för zoomfaktor. (Utfällbar bredd och Utfällbar höjd bestämmer storleken på det utfällbara fönstret, men inte storleken på den utfällbara bild som visas i visningsprogrammet.)

Om huvudbildens storlek till exempel är 350 x 350 pixlar, med zoomfaktorn 3, blir den utfällbara bilden 1 050 x 1 050 pixlar. Om huvudbildstorleken är 300 x 300 pixlar, med zoomfaktorn 4, är den utfällbara bilden 1 200 x 1 200 pixlar. Beroende på kvalitetsinställningen för JPEG (rekommenderade inställningar är mellan 80 och 90) kan du minska filstorleken avsevärt. Rekommenderade zoomningsfaktorer är 2,5 till 4, beroende på storleken på huvudbilden.

### Kompatibilitetsmatris för Adobe Dynamic Media Classic Viewer-förinställning {#scene-viewer-preset-compatibility-matrix}

**Flash Viewers End-of-Life Notice**: Från och med den 31 januari 2017 upphörde Adobe Dynamic Media Classic officiellt stödet för visningsprogramplattformen för Flash.

Följande tabell visar vilka förinställningar för Adobe Dynamic Media Classic Viewer som är tillgängliga. Tabellen anger också visningsprogrammets kompatibilitet med datorer och mobila enheter samt vilken teknik som används för varje visningsprogram.

Se även [Exempel på referensbibliotek för visningsprogram i Adobe](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

Information om vilka webbläsare och operativsystemversioner som stöds för visningsprogram finns i versionsinformationen för visningsprogram.

Se [Referensinformation för visningsprogram för Adobe](https://experienceleague.adobe.com/sv/docs/dynamic-media-developer-resources).

|  | Viewer Technology | Skrivbord | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ Tablet PC |
|--- |--- |--- |--- |--- |--- |--- |
| Zooma visningsprogram |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | Viewer Technology | Skrivbord | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ Tablet PC |
|--- |--- |--- |--- |--- |--- |--- |
| Bilduppsättningsvisningsprogram |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | Viewer Technology | Skrivbord | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ Tablet PC |
|--- |--- |--- |--- |--- |--- |--- |
| Visningsprogram för färgrutor |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | Viewer Technology | Skrivbord | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ Tablet PC |
|--- |--- |--- |--- |--- |--- |--- |
| eCatalog Viewers |  |  |  |  |  |  |
| Universal_HTML5_eCatalog_Adv(Innehåller stöd för sociala medier och katalogsökning.) | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog(Innehåller stöd för sociala medier och katalogsökning.) | HTML5 | X | X | X | X | X |

|  | Viewer Technology | Skrivbord | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ Tablet PC |
|--- |--- |--- |--- |--- |--- |--- |
| Snurra visningsprogram |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**eVideo-visningsprogram**

Adobe Dynamic Media Classic har stöd för videouppspelning i mobiler för MP4 H.264-video.

* Du kan hitta BlackBerry®-enheter som stöder det här videoformatet på följande: [Videoformat som stöds på BlackBerry®](https://developers.blackberry.com/us/en)
* Du kan också hitta Windows®-enheter som stöder det här videoformatet på följande plats: [Videoformat som stöds på Windows® Phone](https://learn.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs)

|  | Viewer Technology | Skrivbord | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ Tablet PC | BlackBerry® Smartphone | Windows® Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video(Innehåller stöd för undertextning.) Se [Bästa praxis: Använda videovisningsprogrammet Universal HTML5.](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social(Innehåller stöd för undertexter och sociala medier.) | HTML5 | X | X | X | X | X | X | X |

|  | Viewer Technology | Skrivbord | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ Tablet PC |
|--- |--- |--- |--- |--- |--- |--- |
| Visningsprogram för blandad medieuppsättning |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### Matris för gester för mobilvisningsprogram som stöds {#supported-mobile-viewers-gestures-matrix}

Följande tabell visar vilka mobilvisningsgester som stöds på enheter med iOS, Android™ 2.x och Android™ 3.x.

|  | Viewer Technology | Skrivbord | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ Tablet PC |
|--- |--- |--- |--- |--- |--- |--- |
| Bilduppsättningsvisningsprogram |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### Om skärmen för visningsförinställningar {#about-the-viewer-preset-screen}

Skapa och hantera visningsförinställningar på skärmen Förinställningar för visningsprogram. Öppna den här skärmen genom att gå till **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.

Skärmen Förinställningar för visningsprogram innehåller verktyg för följande åtgärder:

* **Lägg till en förinställning**: Markera **[!UICONTROL Add]** och gör val i dialogrutan Lägg till visningsförinställning.

      Se [Lägg till och redigera visningsprogramförinställningar](application-setup.md#adding_and_editing_viewer_presets).
  
* **Redigera en förinställning**: Välj en förinställning och välj sedan **[!UICONTROL Edit]**.

      Se [Lägg till och redigera visningsprogramförinställningar](application-setup.md#adding_and_editing_viewer_presets).
  
* **Ta bort en förinställning**: Markera en förinställning och välj sedan **[!UICONTROL Delete]**.

* **Exportera en förinställning**: Välj en HTML5-visningsförinställning. Klicka sedan på **[!UICONTROL Export]** för att hämta visningsskalet så att du kan använda det som grund för att skapa och lägga till en annan visningsförinställning.

      Se [Exportera en HTML5-visningsförinställning](application-setup.md#exporting_an_html5_viewer_preset).
  
* **Filtrera listan med visningsförinställningar**: Använd de här verktygen för att filtrera listan:

      * Öppna listrutan **Aktiv/Inaktiv** och välj ett alternativ för att visa aktiva förinställningar, inaktiva förinställningar eller alla förinställningar.
     * Öppna listrutan **Viewer** och välj ett alternativ för att endast visa visningsprogram av en viss typ. Välj **[!UICONTROL All Viewers]** om du vill visa alla visningsprogram.
  
* **Sortera förinställningar**: Välj en kolumnrubrik (**[!UICONTROL Active]**, **[!UICONTROL Type]**, **[!UICONTROL Preset]** eller **[!UICONTROL Platform]**) för att sortera listan i en kolumn. Välj en kolumnrubrik en andra gång om du vill sortera listan i fallande (eller stigande) ordning.

* **Aktivera och inaktivera förinställningar**: Välj en förinställning och välj sedan alternativet Aktiv så att du kan aktivera eller inaktivera den.

      Se [Aktivera eller inaktivera visningsprogramförinställningar](application-setup.md#activating_or_deactivating_viewer_presets).
  
>[!NOTE]
>
>Välj **[!UICONTROL Preview]** till höger på sidan Viewer Presets (Förinställningar för visningsprogram) så att du kan se hur en resurs ser ut i den valda visningsförinställningen. Om du vill visa en annan resurs väljer du **[!UICONTROL Browse]** på sidan Visningsförinställningar och väljer en annan resurs i dialogrutan Välj förhandsgranskning av resurs.

### Lägga till och redigera visningsprogramförinställningar {#adding-and-editing-viewer-presets}

Förutom att lägga till visningsprogramförinställningar genom att använda **[!UICONTROL Add]** i användargränssnittet kan du även använda **[!UICONTROL Export]** för att lägga till en visningsförinställning. Du exporterar helt enkelt en befintlig HTML5-visningsförinställning och använder den som grund för den nya förinställningen.

Se [Exportera förinställningar för HTML5-visningsprogrammet](application-setup.md#exporting_an_html5_viewer_preset).

Se även utbildningsvideon [Visningsförinställningar](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS).

**Så här lägger du till och redigerar visningsprogramförinställningar:**

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]** i Adobe Dynamic Media Classic övre högra hörn.

   Du kan filtrera i listan med förinställningar. Om du till exempel bara vill visa förinställningar för videovisningsprogram väljer du Videovisningsprogram i listrutan Visare i verktygsfältet direkt ovanför tabellen.

1. Lägg till eller redigera visningsförinställningen på skärmen Förinställningar för visningsprogram på sidan Förinställningar för visningsprogram.

   * **Lägg till**: Välj **[!UICONTROL Add]** i verktygsfältet. I dialogrutan Lägg till visningsförinställning väljer du en plattform och väljer en medieresurstyp.

         Välj **[!UICONTROL Save As]** när du har skapat visningsförinställningen.
     
   * **Lägg till genom att starta från en befintlig visningsförinställning**: I tabellen väljer du en visningsförinställning för video och sedan **[!UICONTROL Edit]** i verktygsfältet.

         När du har konfigurerat om Video Viewer väljer du **[!UICONTROL Save As]** om du vill spara förinställningen med ett annat namn i textfältet Förinställningsnamn.
     
   * **Redigera**: Välj en befintlig visningsförinställning och välj sedan **[!UICONTROL Edit]**.

1. På sidan Konfigurera visningsprogram anger eller redigerar du förinställningens namn i fältet Förinställningsnamn.
1. Ange de återstående alternativen som du vill ha.

   >[!NOTE]
   >
   >Välj **[!UICONTROL Same As Source]** så att du automatiskt kan ändra storlek på Video Viewer till upplösningsstorleken för den kodade videon. Om du väljer det här alternativet kan du inte ange scenens bredd och höjd. I stället kommer dessa alternativ från själva videon. Om du väljer **[!UICONTROL Same As Source]** ställer du in alternativet Marginalstorlek så att skalets dimensioner utanför videouppspelningsområdet återspeglas. Marginalstorleken är pixelhöjden och bredden på videokontrollerna. Du kan använda följande bild för att avgöra vilka marginalstorlekar du vill använda.*

   ![Marginalkonfiguration för videovisningsprogrammet](assets/vs_video_viewer_configure_margin.png)

1. Gör något av följande:

   * Välj **[!UICONTROL Save As]** om du har lagt till en visningsförinställning genom att starta från en befintlig förinställning.
   * Välj **[!UICONTROL Save]** om du har lagt till eller redigerat en visningsförinställning.

### Exportera en HTML5-visningsförinställning {#exporting-an-html-viewer-preset}

Du kan exportera en befintlig HTML5-visningsförinställning som du kan använda som grund för att skapa en visningsförinställning för HTML5. Det här exportalternativet är användbart eftersom du inte behöver skapa visningsprogrammet från grunden. I stället exporterar du en förinställning som ser ut och beter sig ungefär som du vill ha den, och sedan kan du använda den som utgångspunkt för att göra designjusteringar.

Alla standardinställda CSS-filer för visningsförinställningar i Adobe Dynamic Media Classic använder relativa sökvägar som pekar på resurser på `Scene7SharedAssets`. Följande är till exempel en relativ sökväg till en bildresurs i en CSS-fil för visningsförinställningar i

`Scene7SharedAsset`: `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`

Om du däremot har Viewer CSS-filer på din egen plats, måste du lösa dessa relativa bildsökvägar genom att använda en explicit sökväg till Image Server i din egen miljö. Om du till exempel har uppdaterat den relativa sökvägen ovan till en explicit sökväg kan den se ut så här, där `https://s7d1.scene7.com` är den direkta sökvägen till din Image-server: `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**Så här exporterar du en visningsförinställning för HTML5:**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.
1. Välj **[!UICONTROL HTML5]** i den andra listrutan till vänster i verktygsfältet Visningsförinställningar.
1. Välj **[!UICONTROL All Viewers]** i den tredje listrutan från vänster.
1. Välj den visningsförinställning som du vill använda som bas för en ny visningsförinställning för HTML5.
1. Välj **[!UICONTROL Export]** i verktygsfältet.
1. I dialogrutan Exportera markerade Assets väljer du **[!UICONTROL Submit Export]**.

   Efter exporten får du en CSS-fil. Hämta och zippa upp filen.

1. Öppna CSS-filen i en CSS-redigerare, gör ändringarna och spara sedan filen.
1. Överför CSS-filen till Adobe Dynamic Media Classic.

   Se [Överför filer](uploading-files.md#uploading_files).

1. Publish CSS-filen till Dynamic Media Image Server.

   Se [Publish-filer](publishing-files.md#publishing_files).

1. Lägg till den nya visningsförinställningen som vanligt. Välj CSS-filen för visningsprogrammet som du överförde.

   Se [Lägg till och redigera visningsförinställningar](application-setup.md#adding_and_editing_viewer_presets).

### Aktivera eller inaktivera visningsprogramförinställningar {#activating-or-deactivating-viewer-presets}

Om du vill skapa en URL för att visa resurser öppnar användarna listrutan Förinställningar i dialogrutan Förhandsvisa, väljer en visningsförinställning och sedan **[!UICONTROL Copy URL]** (se [Kopiera URL:en för en visningsförinställning](application-setup.md#copying_the_url_of_a_viewer_preset)). Den här förinställningslistan innehåller förinställningar för visningsprogram som administratörer kan lägga till och hantera på skärmen Förinställningar för visningsprogram. Alla aktiva förinställningar för eCatalog-visningsprogrammet visas till exempel i listrutan Förinställningar i dialogrutan Förhandsvisa när en användare förhandsgranskar en e-katalog.

Om du inte inaktiverar visningsförinställningar på skärmen Förinställningar för visningsprogram kan listrutan Förinställningar i dialogrutan Förhandsvisa bli full.

**Så här aktiverar eller inaktiverar du visningsförinställningar:**

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.
1. På sidan Förinställningar för visningsprogram markerar eller avmarkerar du **[!UICONTROL Active]** alternativ för att aktivera eller inaktivera förinställningar för visningsprogram.

### Kopiera URL:en för en visningsförinställning {#copying-the-url-of-a-viewer-preset}

När du har publicerat en resurs kan du kopiera en URL för att visa resursen med inställningarna från en visningsförinställning.

URL:en kopieras till Urklipp. Du kan använda den om det behövs i HTML-koden för webbsidan, mobilenheten eller programmet.

**Så här kopierar du URL:en för en visningsförinställning:**

1. Markera resursen på panelen Bläddra.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Välj **[!UICONTROL Grid View]**. Dubbelklicka på en enskild resurs på panelen Resursbläddring för att öppna den i detaljvyn. I panelen URL:er och panelen Bädda in kod till höger väljer du **[!UICONTROL Copy URL]** till höger om det visningsprogram du vill använda.
   * Välj **[!UICONTROL Grid View]**. Markera en enskild resurs på panelen Resursbläddring och gå sedan till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** under miniatyrbilden.

   Välj **[!UICONTROL Copy URL]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Välj **[!UICONTROL List View]**. Markera en enskild resurs på panelen Resursbläddring och gå sedan till höger om miniatyrbilden till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

   Välj **[!UICONTROL Copy URL]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Välj **[!UICONTROL Grid View]**, **[!UICONTROL List View]** eller **[!UICONTROL Detail View]**. Gå till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** i samma verktygsfält.

   Välj **[!UICONTROL Copy URL]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

### Kopiera inbäddningskod för en visningsförinställning {#copying-the-embed-code-of-a-viewer-preset}

Med funktionen Bädda in kod kan du granska visningsprogramkoden för den valda visningsförinställningen. Du kan också kopiera koden till Urklipp så att du kan klistra in den på webbsidorna för att distribuera visningsprogrammet.

Det är inte tillåtet att redigera koden i dialogrutan Bädda in kod.

**Så här kopierar du inbäddningskoden för en visningsförinställning:**

1. Markera resursen på panelen Resursbläddring.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Välj **[!UICONTROL Grid View]**. Dubbelklicka på en enskild resurs på panelen Resursbläddring för att öppna den i detaljvyn. Välj **[!UICONTROL Embed Code]** på panelen URL:er till höger.
   * Välj **[!UICONTROL Grid View]**. Markera en enskild resurs på panelen Resursbläddring och gå sedan till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** under miniatyrbilden.

   Välj **[!UICONTROL Embed Code]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Välj **[!UICONTROL List View]**. Markera en enskild resurs på panelen Resursbläddring och gå sedan till höger om miniatyrbilden till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

   Välj **[!UICONTROL Embed Code]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Välj **[!UICONTROL Grid View]**, **[!UICONTROL List View]** eller **[!UICONTROL Detail View]**. Gå till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** i samma verktygsfält.

   Välj **[!UICONTROL Embed Code]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

1. Välj **[!UICONTROL Copy to Clipboard]** i dialogrutan Bädda in kod.
1. Välj **[!UICONTROL Close]**.

## Konfigurera standardvisningsprogram {#configure-default-viewers}

Du kan använda standardvisningsprogram för att konfigurera standardvisningsprogrammet som är kopplat till en resurs när du använder Förhandsvisa i Adobe Dynamic Media Classic. Du kan ställa in standardförhandsvisningen för följande resurstyper:

* Bild
* Video
* SpinSet
* Katalog
* ImageSet
* SwatchSet
* MediaSet

**Så här konfigurerar du standardvisningsprogram:**

1. Välj **[!UICONTROL Application Setup]** i listrutan Inställningar.
1. Gå till **[!UICONTROL Application Setup]** > **[!UICONTROL Viewers]** i det vänstra fönstret
1. Välj **[!UICONTROL Default Viewers]**.
1. Välj det visningsprogram som du vill associera med resursens förhandsgranskning i listrutan för varje resurstyp i fönstret Standardvisningsprogram.
1. Välj **[!UICONTROL Save Settings]** i det nedre högra hörnet av fönstret Standardvisningsprogram.
1. I det nedre högra hörnet av inställningsfönstret väljer du **[!UICONTROL Close]** för att återgå till fönstret Resurser.

## Metadatavyer {#metadata-views}

*Metadata* är standardiserad information om en resurs. Du kan använda metadata för att effektivisera arbetsflödet, ordna dina resurser och förbättra sökningen. Adobe Dynamic Media Classic stöder standarderna IPTC (International Press Telecommunications Council) och XMP (extensible metadata platform). Innan användarna visar eller anger metadata om en resurs i detaljvyn kan de öppna menyn Metadatavyer. Därifrån kan de välja den uppsättning metadatafält som de vill visa eller använda för att beskriva resursen.

Adobe Dynamic Media Classic levereras med fördefinierade metadatavyer, och administratörer kan skapa egna metadatavyer som användarna kan välja när de anger metadata.

### Skapa en metadatavy {#creating-a-metadata-view}

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Views]**.
1. Välj **[!UICONTROL Add]**.
1. Ange ett namn för vyn i textfältet Förinställningsnamn.
1. (Valfritt) Markera **[!UICONTROL Make Default]** om du vill att den här vyn ska vara den som visas för användarna när de öppnar panelen Metadata i detaljvyn.
1. (Valfritt) Välj **[!UICONTROL Include UDF]** om du vill inkludera användardefinierade fält i vyn. Användardefinierade fält visas högst upp på panelen Metadata i detaljvyn.
1. Markera de fält som du vill visa (markera **[!UICONTROL Select All]** för att markera alla fält).
1. Välj **[!UICONTROL Save]**.

   De markerade kategorierna och fälten för vyn visas på förhandsvisningspanelen.

### Hantera metadatavyer {#managing-metadata-views}

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Views]**.
1. Gör något av följande:

   * Om du vill förhandsgranska en vy markerar du den. Fälten i vyn visas på förhandsvisningspanelen.
   * Om du vill redigera en vy markerar du den och väljer sedan **[!UICONTROL Edit]**. Markera eller avmarkera sedan fältnamn på förhandsgranskningspanelen och markera eller avmarkera alternativet **[!UICONTROL Include UDF]**.
   * Om du vill ta bort en vy markerar du den och väljer sedan **[!UICONTROL Delete]**.
   * Om du vill göra en vy till standard markerar du den och väljer sedan **[!UICONTROL Make Default]**. Standardvyn är den vy som användarna ser när de öppnar en resurs i detaljvyn och går till panelen Metadata.

## Metadataförinställningar {#metadata-presets}

Med metadataförinställningar kan administratörer styra och reglera de metadata som tilldelas resurser. I detaljvyn kan en användare ange metadata om en resurs i fält som tillhandahålls för det ändamålet. En användare kan till exempel ange ett ägarnamn, en copyrightbeskrivning och en adress. Om du vill vara säker på att användarna anger den här informationen korrekt och fullständigt kan du skapa metadataförinställningar. Om du väljer en metadataförinställning i detaljvyn fylls metadatafält med fördefinierade värden. Exempel: Ägarnamn, copyrightbeskrivning och adress anges automatiskt.

Skapa en metadataförinställning för varje uppsättning metadatavärden som du vill att användarna ska kunna ange automatiskt i detaljvyn för att beskriva en resurs.

### Skapa eller redigera en metadataförinställning {#creating-or-editing-a-metadata-preset}

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Presets]**.
1. Gör något av följande på skärmen Metadataförinställningar:

   * Välj **[!UICONTROL Add]** om du vill skapa en förinställning. Skriv ett namn på förinställningen i textfältet Metadatamallnamn. Välj **[!UICONTROL Metadata Views]** och välj sedan en vy i listrutan (se [Metadatavyer](application-setup.md#metadata_views)).
   * Om du vill redigera en befintlig förinställning markerar du förinställningen i listan Metadataförinställningar och väljer sedan **[!UICONTROL Edit]**.

1. Expandera rubriker som du vill ta med i förinställningen och ange värden i de olika fält som du vill ta med i förinställningen.
1. Välj **[!UICONTROL Save]**.

   De valda kategorierna och fälten för förinställningen visas på panelen Förhandsgranska.

### Hantera metadataförinställningar {#managing-metadata-presets}

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Presets]**.
1. Gör något av följande:

   * Om du vill förhandsgranska en förinställning markerar du den förinställning som du vill förhandsgranska. Förinställningsinformationen (kategorier och fält) visas på förhandsgranskningsskärmen.
   * Om du vill ta bort en förinställning markerar du förinställningen och väljer sedan **[!UICONTROL Delete]**.

## Användardefinierade fält {#user-defined-fields}

En Media Portal-administratör eller en företagsadministratör kan skapa anpassade, användardefinierade metadatafält. Med anpassade fält kan du ordna resurser i Adobe Dynamic Media Classic. Du kan markera fälten som aktiva, efter behov. När du aktiverar det här alternativet visas namnen på dessa anpassade metadatafält på panelen Metadata i detaljvyn. Användare kan ange information i användardefinierade metadatafält för att beskriva resurser. Användarna kan också göra ett användardefinierat metadatafält till ett villkor i sökningar.

Ett effektivt sätt att använda användardefinierade metadatafält är att fördröja aktiveringstiden för en mediefil för en viss start eller försäljning. Du definierar ett aktiveringsfält baserat på typen *Date*. Med panelen **[!UICONTROL Metadata]** i detaljvyn eller **[!UICONTROL File]** > **[!UICONTROL Edit Info]** kan du sedan ange när resursen ska aktiveras. Adobe Dynamic Media Classic kontrollerar publiceringsstatus för en resurs och publiceringshistorik. Om det inte är inom aktiveringstiden visas publiceringsstatusen som Inte publicerad.

>[!NOTE]
>
>Om du vill att användardefinierade fält ska visas på panelen Metadata i detaljvyn, inkluderar du användardefinierade fält i metadatavyer. Markera alternativet Inkludera användardefinierat fält (Inkludera användardefinierat fält) på skärmen Metadatavyer. Mer information finns i [Vyer för metadata](application-setup.md#metadata_views).

>[!NOTE]
>
>Om du vill söka efter resurser med anpassade, användardefinierade fält går du till **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]** och väljer sedan **[!UICONTROL Include UDFs in Search]**. Se [Personliga inställningar](personal-setup.md#personal_setup).

### Skapa ett användardefinierat metadatafält {#creating-a-user-defined-metadata-field}

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL User-Defined Fields]**.
1. Välj **[!UICONTROL Add]**
1. Ange önskade alternativ i dialogrutan Anpassat fält.

   * **[!UICONTROL Name]**: Ange ett namn för metadatafältet.

   * **[!UICONTROL Type]**: Välj ett alternativ som definierar vilken typ av information som användare kan ange i metadatafältet:

   * **[!UICONTROL String]**: En textsträng.

   * **[!UICONTROL Int]**: Ett heltal.

   * **[!UICONTROL Float]**: Ett flyttal.

   * **[!UICONTROL Yes/No]**: Ett ja/nej-booleskt värde.

   * **[!UICONTROL Date]**: Ett datum. Formatet MM/DD/ÅÅÅÅ accepteras.

   * **[!UICONTROL Filename]**: Namnet på en fil.

   * **[!UICONTROL Color]**: Namnet på en färg.

   * **[!UICONTROL Dimension]**: Resursens bredd och höjd.

   * **[!UICONTROL Untyped]**: För bakåtkompatibilitet. Markera inte det här alternativet.

   * **[!UICONTROL Default Value]**: Valfritt. Ange det värde som användarna mest sannolikt anger i fältet. Värdet som du anger blir standardvärdet för fältet som du skapar.

   * **[!UICONTROL Applies To]**: Valfritt. Välj en resurstyp om du vill att metadatafältet bara ska gälla för en viss typ av resurs.

     >[!NOTE]
     >
     >Välj ett **[!UICONTROL Applies To]**-alternativ noggrant eftersom du inte kan ändra alternativet **[!UICONTROL Applies To]** när du har skapat ett användardefinierat fält. Med Adobe Dynamic Media Classic kan du redigera namn, typ och standardvärde för ett användardefinierat fält, men inte för inställningen **[!UICONTROL Applies To]**. *

1. Välj **[!UICONTROL Save]** när du har skapat metadatafältet.

### Hantera användardefinierade fält {#manage-user-defined-fields}

Skärmen Användardefinierade fält innehåller kommandon för att hantera anpassade, användardefinierade metadatafält.

Endast en Media Portal-administratör eller en företagsadministratör kan hantera användardefinierade fält.

Öppna den här skärmen genom att gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL User-Defined Fields]**.

* **Redigera ett fält**: Markera fältet och välj sedan **[!UICONTROL Edit]**.

* **Ta bort ett fält**: Markera fältet och välj sedan **[!UICONTROL Delete]**.

* **Aktivera fält**: Markera eller avmarkera alternativet **[!UICONTROL Active]** bredvid namnet på ett fält. Om du har en företagsadministrationsroll visas inte det här alternativet. Eftersom det här alternativet är relaterat till MediaPortal måste du markera (aktivera) Visa MediaPortal-funktioner i Personliga inställningar för att se de aktiverade fälten.

## Optimera filer {#optimize-files}

När du överför filer till Adobe Dynamic Media Classic optimeras de för lagring och publicering. Om överföringen avbryts kan vissa bilder inte optimeras. I det här fallet visas meddelandet &quot;Bilden är inte optimerad ännu&quot;. Du kan dock optimera dessa filer om du är administratör.

Adobe Dynamic Media Classic söker igenom filerna och optimerar endast de bilder som inte har optimerats fullständigt tidigare.

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** och välj sedan **[!UICONTROL Optimize Files]**.
1. Ange information för optimeringsjobbet och välj **[!UICONTROL Submit]**.

   Om du arbetar med mer än ett företag optimerar du filer som tillhör olika företag separat.

## Förinställningar för gruppuppsättning {#batch-set-presets}

Använd gruppuppsättningsförinställningar så att du automatiskt kan skapa bilduppsättningar eller snurruppsättningar när ett jobb körs för att överföra resurser till Adobe Dynamic Media Classic.

Företagsadministratörer definierar först namnkonventioner för de resurser som de vill gruppera i en uppsättning. Du kan sedan skapa en gruppuppsättningsförinställning som refererar till dessa bilder. Varje förinställning är en unik, självständig uppsättning instruktioner som definierar hur uppsättningen ska skapas med bilder som matchar de definierade namnkonventionerna i förinställningsreceptet.

Alla aktiva gruppuppsättningsförinställningar för ett företag visas i dialogrutan Alternativ för överföringsjobb, så att du kan ange vilken förinställning du vill använda under varje överföringssession. Företagsadministratörer ser alla aktiva och inaktiva förinställningar för gruppuppsättning. När du överför filer skapar Adobe Dynamic Media Classic automatiskt en uppsättning med alla filer som matchar den definierade namnkonventionen i de aktiva förinställningarna.

### Standardnamn {#default-naming}

Företagsadministratören skapar en standardnamnkonvention som används i alla förinställda gruppuppsättningar. Den standardnamnkonvention som valts i definitionen av gruppuppsättningsförinställning kan vara allt som ditt företag behöver för att batchgenerera uppsättningar för alla webbplatser. En förinställning för gruppuppsättning skapas för att använda den namnstandardnamnkonvention som du anger. Du kan skapa så många gruppuppsättningsförinställningar med alternativa, anpassade namnkonventioner som behövs för en viss uppsättning innehåll om det finns ett undantag från den företagsdefinierade standardnamngivningen.

Du behöver inte konfigurera en standardnamnkonvention för att kunna använda funktionen Förinställning för gruppuppsättning. Du bör emellertid använda en standardnamnkonvention för att definiera så många element i namnkonventionen som du vill gruppera i en uppsättning som är standard i Adobe. Om du gör det blir det enklare att skapa gruppuppsättningar.

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Batch Set Presets]** > **[!UICONTROL Default Naming]**.
1. Välj **[!UICONTROL View Form]** eller **[!UICONTROL View Code]** för att ange hur du vill visa och ange information om varje element.

   Du kan markera kryssrutan **[!UICONTROL View Code]** om du vill visa värdeuppbyggnaden för reguljära uttryck tillsammans med dina formulärval. Du kan ange eller ändra dessa värden för att underlätta definitionen av elementen i namnkonventionen, om du av någon anledning begränsas av formulärvyn. Om dina värden inte kan tolkas i formulärvyn blir formulärfälten inaktiva.

   >[!NOTE]
   >
   >Inaktiverade formulärfält indikerar inte ett ogiltigt reguljärt uttryck. Det finns ingen validering av att dina reguljära uttryck är korrekta. Resultaten av det reguljära uttryck som du skapar för varje element visas efter resultatraden. Det fullständiga reguljära uttrycket visas längst ned på sidan.

1. Expandera varje element efter behov och ange de namnkonventioner som du vill använda.
1. Välj **[!UICONTROL Add]** om det behövs för att lägga till en annan namnkonvention för ett element. Du kan också markera **[!UICONTROL Remove]** om du vill ta bort en namnkonvention för ett element.
1. Välj **[!UICONTROL Save As]** och ange ett namn för förinställningen. Du kan också markera **[!UICONTROL Save]** om du redigerar en befintlig förinställning.

Du kan också använda Visa kod utan några formulärfält. I den här vyn skapar du namnkonventionens definitioner helt med hjälp av reguljära uttryck.

Det finns två element för definition, Matcha och Basnamn. Dessa fält är alla element som du har definierat för en namnkonvention. De kan hjälpa till att identifiera den del av konventionen som används för att namnge den uppsättning i vilken de finns. Ett företags personliga namnkonvention kan använda en eller flera definitionsrader för vart och ett av dessa element. Du kan använda så många rader för din unika definition och gruppera dem i distinkta element, t.ex. för huvudbilden, Color-elementet, Alternate View-elementet och färgruteelementet.

### Skapa en förinställning för gruppuppsättning {#creating-a-batch-set-preset}

Adobe Dynamic Media Classic använder gruppuppsättningsförinställningar för att ordna resurser som delar viss gemensam information eller innehåll i uppsättningar med bilder som ska visas i visningsprogram. Batchinställningsrecepten körs automatiskt tillsammans med de resursimporteringsjobb som du schemalägger i Adobe Dynamic Media Classic.

Använd Förinställning för gruppuppsättning för att skapa, redigera och hantera dina förinställningar för gruppuppsättning. Du kan skapa så många förinställningar som behövs för att täcka alla tillgångsimportjobb som du behöver. Det finns två former av definitioner av gruppuppsättningsförinställningar: en för en standardnamnkonvention som du har konfigurerat och en för anpassade namnkonventioner som du skapar direkt.

Du kan antingen använda formulärfältets metod för att definiera en gruppuppsättningsförinställning eller kodmetoden, där du kan använda reguljära uttryck. Som i **[!UICONTROL Default Naming]** kan du välja **[!UICONTROL Code View]** samtidigt som du definierar i formulärvyn och använda reguljära uttryck för att skapa definitioner. Du kan också avmarkera en vy om du vill använda den ena eller den andra enbart.

Se även [Skapa en gruppuppsättningsförinställning för automatisk generering av en 2D-snurpuppsättning](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

Se även utbildningsvideon [2D Spin Set](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/537_2d-spin_converted%20renamed_Done-AVS).

**Så här skapar du en gruppuppsättningsförinställning:**

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Batch Set Presets]** > **[!UICONTROL Batch Set Preset]**. **[!UICONTROL View Form]**, som anges i det övre högra hörnet på detaljsidan, är standardvyn.
1. På panelen Förinställningslista väljer du **[!UICONTROL Add]** för att aktivera definitionsfälten på panelen Detaljer till höger på sidan.
1. Skriv ett namn på förinställningen i fältet Förinställningsnamn på panelen Detaljer.
1. Välj en förinställningstyp i listrutan Gruppuppsättningstyp.

   Om du vill generera en 2D-snurpuppsättning automatiskt väljer du **[!UICONTROL Multi-Axis Spin Set]** i listrutan Gruppuppsättningstyp.

1. Gör något av följande:

   * Om du använder en standardnamnkonvention som du tidigare ställt in under **[!UICONTROL Application Setup]** > **[!UICONTROL Batch Set Presets]** > **[!UICONTROL Default Naming]** expanderar du **[!UICONTROL Asset Naming Conventions]** och väljer **[!UICONTROL Default]** i listrutan Namnge fil.
   * Om du vill definiera en namnkonvention när du konfigurerar förinställningen expanderar du **[!UICONTROL Asset Naming Conventions]** och väljer sedan **[!UICONTROL Custom]** i listrutan Namnge fil.

1. I Sekvensordning definierar du ordningen för bilderna när uppsättningen har grupperats i Adobe Dynamic Media Classic. Som standard sorteras dina resurser alfanumeriskt. Du kan dock använda en kommaavgränsad lista med reguljära uttryck för att definiera ordningen.
1. Ange suffixet eller prefixet till basnamnet som du definierade i konventionen om namngivning av tillgångar för Ange namngivning och skapande. Definiera också var bilduppsättningen ska skapas i mappstrukturen för Adobe Dynamic Media Classic.

   Om du definierar ett stort antal bilduppsättningar ska du hålla uppsättningarna åtskilda från de mappar som innehåller själva resurserna. Många kunder skapar en mapp för bilduppsättningar och omdirigerar programmet till att placera gruppuppsättningar som genereras här.

1. Välj **[!UICONTROL Save]** på detaljpanelen.

### Skapa en gruppuppsättningsförinställning för automatisk generering av en 2D-snurpuppsättning {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

Du kan använda gruppuppsättningstypen **Spin-uppsättning för flera axlar** för att skapa ett recept som automatiserar genereringen av tvådimensionella snurruppsättningar. Vid gruppering av bilder används reguljära uttryck för rad och kolumn så att bildresurserna justeras korrekt på motsvarande plats i den flerdimensionella arrayen.

Se även [Skapa en förinställning för gruppuppsättning](application-setup.md#creating_a_batch_set_preset).

Det finns inget minsta eller högsta antal rader eller kolumner som du måste ha i en snurra uppsättning med flera axlar.

Anta till exempel att du vill skapa en fleraxelssnurra med namnet *spin-2dspin*. Det finns en uppsättning med bilder i snurra uppsättningar som innehåller tre rader, med 12 bilder per rad. Bilderna får följande namn:

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

![Hämta recept för gruppuppsättning](assets/se_batch_set_recipe.png)

Gruppering för den delade resursnamndelen i rotationsuppsättningen läggs till i fältet Matcha (markerat). Variabeldelen av resursnamnet som innehåller raden och kolumnen läggs till i fälten Rad och Kolumn.

När rotationsuppsättningen har överförts och publicerats aktiverar du namnet på det 2D-rotationsuppsättningsrecept som visas under **[!UICONTROL Batch Set Presets]** i dialogrutan Alternativ för överföringsjobb.

**Så här skapar du en gruppuppsättningsförinställning för automatisk generering av en 2D-snurpuppsättning:**

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Batch Set Presets]** > **[!UICONTROL Batch Set Preset]**. **[!UICONTROL View Form]**, som anges i det övre högra hörnet på detaljsidan, är standardvyn.
1. På panelen Förinställningslista väljer du **[!UICONTROL Add]** för att aktivera definitionsfälten på panelen Detaljer till höger på sidan.
1. Skriv ett namn på förinställningen i fältet Förinställningsnamn på panelen Detaljer.
1. Välj **[!UICONTROL Asset Set]** i listrutan Gruppuppsättningstyp.
1. Välj **[!UICONTROL Multi-Axis Spin Set]** i listrutan Undertyp.
1. Expandera **[!UICONTROL Asset Naming Conventions]** och välj sedan **[!UICONTROL Custom]** i listrutan Namnge fil.
1. Använd attributen **[!UICONTROL Match]** och (valfritt) **[!UICONTROL Base Name]** för att definiera ett reguljärt uttryck för namngivning av bildresurser som utgör grupperingen.

   Det reguljära uttrycket för literal Match kan till exempel se ut så här:

   `(\w+)-\w+-\w+`

1. Expandera **[!UICONTROL Row Column Position]** och definiera sedan namnformatet för bildresursens position i 2D-rotationsmatrisen.

   Använd parentesen för att omsluta rad- eller kolumnpositionen i filnamnet.

   För radens reguljära uttryck kan det till exempel se ut så här:

   `\w+-R([0-9]+)-\w+`

   eller

   `\w+-(\d+)-\w+`

   För det reguljära uttrycket i kolumnen kan det se ut så här:

   `\w+-\w+-C([0-9]+)`

   eller

   `\w+-\w+-C(\d+)`

   Kom ihåg att dessa uttryck bara är exempel. Du kan skapa det reguljära uttrycket hur du vill.

   >[!NOTE]
   >
   >Om kombinationen av reguljära uttryck i rader och kolumner inte kan avgöra positionen för resursen i den flerdimensionella rotationsmatrisen, läggs resursen inte till i uppsättningen. Ett fel loggas.

1. Ange suffixet eller prefixet till basnamnet som du definierade i konventionen om namngivning av tillgångar för Ange namngivning och skapande. Definiera också var bilduppsättningen ska skapas i mappstrukturen för Adobe Dynamic Media Classic.

   Om du definierar ett stort antal bilduppsättningar ska du hålla uppsättningarna åtskilda från de mappar som innehåller själva resurserna. Många kunder skapar en mapp för bilduppsättningar och omdirigerar programmet till att placera gruppuppsättningar som genereras här.

1. Välj **[!UICONTROL Save]** på detaljpanelen.
1. Ladda upp och publicera din snurruppsättning som vanligt och se till att du aktiverar namnet på din 2D-snurruppsättning i dialogrutan Alternativ för jobbinläsning under Gruppera förinställningar.

>[!MORELIKETHIS]
>
>* [Förhandsgranska en resurs](previewing-asset.md#previewing_an_asset)
>* [Konfigurera bildförinställningar](setting-image-presets.md#setting_up_image_presets)
>* [Visa, lägga till och exportera metadata](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
>* [Kontrollera jobbfiler](checking-job-files.md#checking_job_files)
