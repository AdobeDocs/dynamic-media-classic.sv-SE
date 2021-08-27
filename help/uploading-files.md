---
title: Överför filer
description: Lär dig hur du överför filer i Adobe Dynamic Media Classic.
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
source-git-commit: 44045daa35052f01a26c67e0b2a0fb1405c53292
workflow-type: tm+mt
source-wordcount: '3654'
ht-degree: 0%

---

# Överför filer{#uploading-files}

Innan du överför resursfiler till Adobe Dynamic Media Classic måste du se till att resursfilerna har rätt namn och att mappstrukturen är konfigurerad och ordnad som du vill ha den. Du kan överföra filer från en FTP-plats som tillhandahålls av Adobe Dynamic Media Classic eller direkt från datorn eller nätverket. I Adobe Dynamic Media Classic finns alternativ för att optimera filer när du överför dem. Om du har installerat Adobe Dynamic Media Classic kan du överföra filer och mappar genom att dra dem direkt från skrivbordet. Se [Allmänna inställningar för program](application-setup.md#general_settings).

## Förbered dina resurser och mappar för överföring {#preparing-your-assets-and-folders-for-uploading}

Innan du överför resurser till Adobe Dynamic Media Classic bör du kontrollera att de har rätt format och storlek. Du måste också följa Adobe Dynamic Media Classic-reglerna för att namnge resurser. Genom att konfigurera en mappstruktur för filerna ser du till att du enkelt kan hitta och arbeta med filerna.

### Filformat som stöds {#supported-asset-file-formats}

I den här tabellen visas de filformat som Adobe Dynamic Media Classic har stöd för. Information om vilka Camera Raw filer som stöds finns i [https://helpx.adobe.com/camera-raw/using/supported-cameras.html](https://helpx.adobe.com/camera-raw/using/supported-cameras.html).

| Resursfilformat | Beskrivning |
| --- | --- |
| Ljud | AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3 |
| Cascading Style Sheet | CSS |
| Färgprofiler | ICC, ICM |
| Teckensnitt | AFM, OTF, PFB, PFM, PhotoFont, TTC, TTF |
| FXG | FXG |
| Illustrator | AI, FXG |
| Bilder | BMP, FPX, GIF, JPEG, JPG, PNG, PICT (endast Windows®), TIF, TIFF |
| InDesign | INDD, INDT |
| MS® Office | DOC, PPT, RTF, XLS |
| PDF | PDF |
| Photoshop | PSD, FXG och Camera Raw |
| PostScript | EPS, PS |
| Adobe Dynamic Media Classic Image Authoring | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| Video | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

Stöd för TAR- och ZIP-överföring innehåller en kryssruta för att välja om du vill packa upp filerna.

### Bildformat som inte stöds i Dynamic Media {#unsupported-image-formats-dynamic-media}

I följande lista beskrivs de undertyper av rasterbildfilformat som *inte* stöds i Dynamic Media.

Se även [Identifiera filformat som inte stöds för Dynamic Media](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html).

* PNG-filer som har en IDAT-segmentstorlek som är större än 100 MB.
* PSB-filer.
* PSD-filer med en annan färgrymd än CMYK, RGB, Gråskala eller Bitmapp stöds inte. Färgrymderna DuoTone, Lab och Indexed stöds inte.
* PSD-filer med ett bitdjup som är större än 16.
* TIFF-filer som har flyttalsdata.
* TIFF-filer med Lab-färgrymd.

### Resurstyper {#asset-types}

För att få bästa möjliga resultat med Adobe Dynamic Media Classic bör du använda de rekommenderade filformaten och storlekarna. I den här tabellen visas resurstyper, vissa med rekommenderade format och filstorlekar för resurser som används ofta.

| Tillgångstyp | Beskrivning/Recommendations |
| --- | --- |
| Ljud | Bland indatafilformaten för ljudresurser finns AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3. Du kan koda om ljud till följande format: MP3, AAC och HE-AAC. |
| Bilder (för Bildstorlek, Zooma, Bilduppsättningar, Snurra uppsättningar) | Bilderna måste ha minst 2 000 pixlar med den längsta storleken. de vanliga bildstorlekarna varierar mellan 1 500 och 2 500 pixlar i den längsta storleken. Vi rekommenderar förlustfria bildformat, inklusive TIFF- och PNG-filer. Om du använder en JPEG-bild bör du använda inställningarna för den högsta kvaliteten. Animate GIF-filer hanteras som annat statiskt innehåll. |
| eCatalogs | Använd högupplösta PDF-filer som skapats i Adobe® Acrobat® eller ett Creative Suite-program som sparats som &quot;tryckoriginal&quot;. PDF-filer innehåller alla teckensnitt, bilder, masker och refererade grafiska element som behövs, antingen som enkelsidiga, dubbelsidiga uppslag eller i ett flersidigt format. Ordna sidorna genom att namnge filerna i alfanumerisk ordning. Placera alla PDF-filer för din e-katalog i en enda mapp för att underlätta överföringen. Du kan välja beskärningsalternativ när du överför för att ta bort beskärningsområdet från PDF-filer, inklusive skärmärken, registreringsmål eller färgfält. De flesta tryckfärdiga PDF-filer finns i CMYK-färgmodellen, så det är viktigt att du hämtar den ICC-färgprofil för CMYK som används med PDF-filerna. |
| Mallar | Bild- eller layoutdesign med flera lager som kan innehålla text, bilder och lager. Bildlager, textsträngar och attribut, som färg och storlek, kan parametriseras så att variabeldata kan anpassas. Bildkraven för användning i mallar är desamma som för andra bilder. Förbered bilderna i Photoshop eller något annat bildredigeringsprogram. Spara varje bild som en förenklad genomskinlig fil i TIFF- eller PNG-format. Kontrollera att bildupplösningen är lämplig för förväntad användning. Bilder för utskrift är 300 ppi. |
| Videor | Adobe Dynamic Media Classic stöder videofiler som sparats i formaten OGV och MP4. Du kan omkoda filer till MP4-format vid överföring. Se [Resursfilformat som stöds](#supported-static-file-formats). |
| Teckensnitt | Överförda TrueType, Type1 (endast Windows®), OpenType®-teckensnitt och PhotoFonts. |
| Bilder | Bilder och bildfiler med flera lager. |
| Bilduppsättningar och färgruteuppsättningar | En uppsättning närliggande bilder som kan visas i ett visningsprogram. |
| ICC-profiler | En färgprofil som du kan använda för att konvertera en överförd bild från dess källfärgrymd till en annan färgrymd. |
| Vinjetter | Bilder som skapats med bildredigeringsprogrammet och relaterade filer. |
| Innehållsfiler | Adobe InDesign, Illustrator eller Photoshop innehållsfiler. |
| FXG-filer | Upplösningsoberoende grafikformatfiler som du kan använda för att skapa anpassningsbara mallar för utskrift, webb, e-post, dator och enheter. |
| SVG-filer | Skalbara vektorgrafikfiler som Image Serving-servrar kan återge. |
| XML-filer | Filer som definierar förbearbetningsregler som används för att ändra sökväg och frågedelar för begäranden. |
| Cascading Style Sheet-filer. | Överför CSS-skal för anpassning av HTML5-visningsprogram. |
| JavaScript-filer | JavaScript-filer används för visningsprograminstrumentering för kontoinformation. Adobe Security rekommenderar att den här resurstypen endast används för klientkonton som har en separat domän som används för leverans (för att undvika serveröverskridande skript). |

>[!NOTE]
>
>När du överför bildfiler och PDF-filer till Adobe Dynamic Media Classic konverteras dessa källfiler till P-TIFF-filer (Pyramid TIFF). Dessa P-TIFF-filer är de filer som senare publiceras till Dynamic Media Image Servers. I Adobe Dynamic Media Classic används filformatet Pyramid Tiff eftersom det innehåller olika zoomningsförhållanden som möjliggör snabb zoomning när det visas med Adobe Dynamic Media Classic Zoom Viewer.

### Statiska filformat som stöds {#supported-static-file-formats}

Adobe Dynamic Media Classic stöder flera statiska filformat. Statiskt innehåll är alla resurser som publiceras i befintligt skick, t.ex. CSS, PDF, SVG och XML.

Följande filtyper kan publiceras:

* Animerad GIF
* Ljudfiler
* CSS
* JavaScript (när företaget har konfigurerats med sin egen domän)
* Överordnad video
* PDF (när PDF har markerats för publicering efter överföring, för att undvika att alla PDF-filer levereras för det befintliga eCatalog/PDF-arbetsflödet)
* PrX-video
* SVG
* XML
* ZIP

I Adobe Dynamic Media Classic går det inte att generera en förhandsgransknings-URL för statiskt innehåll.

### Krav för filnamn {#filename-requirements}

Eftersom filnamnstillägg tas bort från filnamn under överföringsprocessen tillåter inte systemet att filer har samma rotnamn. I Adobe Dynamic Media Classic-systemet blir resursfilens namn minus filnamnstillägget resurs-ID för resursen. Därför kan två resurser inte ha samma namn.

Se till att alla användare på företaget förstår följande regler för filnamngivning:

* Tillgångs-ID:n med samma exakta namn tillåts inte i systemet.
* Resurs-ID:n är skiftlägeskänsliga.
* Ett tips är att se till att resurs-ID:n inte innehåller blanksteg (t.ex. svart jacka.tif och blå jpg). Adobe Dynamic Media Classic ASCII-kodar tomma utrymmen i resursnamn när resursnamn används för att skapa URL-strängar. Dessa ASCII-koder är svåra att läsa, vilket kan göra det svårare att läsa URL:er.
* Språkspecifika tecken får användas i filnamn. Följande tecken får dock inte användas i filnamn:

   \ ; / ? : @ &amp; = + $ , * &quot; &lt; > | &#39; {} %

   Om ett filnamn innehåller ett eller flera av ovanstående tecken tas tecknen bort från filnamnet vid överföringen.

Vanligtvis kan ett filnamn för en resurs vara samma som dess artikelnummer, produkt-SKU eller annat namn som i följande exempel:

| Objekt | Filnamn | Tillgångs-ID |
|--- |--- |--- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Mappstruktur {#folder-organization-and-structure}

Ordna och strukturera mappar och undermappar för ditt innehåll i Adobe Dynamic Media Classic innan du överför innehållet till systemet. Planering framåt på det här sättet har två stora fördelar:

* När du överför ditt innehåll till Adobe Dynamic Media Classic via FTP kan du ange att systemet ska replikera mappstrukturen under överföringen. På så sätt ordnas ditt innehåll i samma mappar och undermappar i Adobe Dynamic Media Classic som det finns på datorn eller i nätverket. (Om du vill replikera mappstrukturen i Adobe Dynamic Media Classic markerar du alternativet Inkludera undermappar när du överför resurser via FTP.)
* Det är mycket svårare att ordna om mappar i systemet efter att filer har överförts än att börja med en noggrant genomtänkt mappstruktur.

Vilken mappnamnsmetod och struktur du väljer för att lagra ditt innehåll på Adobe Dynamic Media Classic beror på organisationens behov. Här följer några exempel på mappstrukturer:

**SKU-baserade**  mappar namnges enligt SKU:er eller artikelnummer. Separata mappar skapas till exempel för alla serier med 0-, 20- och 30-tal.

**Varumärkesbaserad**  - För tillverkare med flera varumärken och detaljhandlare som marknadsför andra varumärken från andra företag, kan du dela upp filer i produktmappar som namngetts för olika varumärken.

**Projektbaserad**  - Mappar ordnas efter datum för utrullning/släppning eller projektnamn. Kunder som främst producerar e-kataloger gillar detta.

**Spegling av webbplatsens mapphierarki**  - Mappstrukturen speglar webbplatsens mappstruktur, med mapparna till exempel namngivna för produktkategorier.

## Om att överföra filer {#uploading-your-files}

Du kan överföra enskilda filer från skrivbordet eller överföra mappar via FTP. Om du vill överföra mer än 100 MB filer eller överföra hela mappar och undermappar väljer du fliken **VIA FTP**.

Adobe Dynamic Media Classic skickar ett e-postmeddelande till dig för att bekräfta när överföringsjobbet påbörjas och avslutas samt för att meddela dig om eventuella problem.

Under (eller omedelbart efter) ett stort överföringsjobb kan vissa nya objekt visa meddelandet&quot;Bilden är ännu inte optimerad&quot;. Det här meddelandet visas eftersom filerna ännu inte har bearbetats fullständigt och lagts till i Adobe Dynamic Media Classic. Du kan optimera dessa filer senare. Se [Optimera filer](application-setup.md#optimize_files).

### Överföra filer med hjälp av fliken Från skrivbord {#upload-files-using-sps-desktop-application}

Med Adobe Dynamic Media Classic för datorer kan du överföra filer och mappar genom att dra.

1. I Adobe Dynamic Media Classic Desktop-programmet väljer du **[!UICONTROL Upload]** i fältet Global navigering.
1. På sidan Överför väljer du fliken **[!UICONTROL From Desktop]**.
1. Till vänster på sidan Överför väljer du **[!UICONTROL Select Files for Upload]** i området **[!UICONTROL Browse]** för att markera de filer eller mappar som du vill överföra och väljer sedan **[!UICONTROL Open]**.
1. Till höger på sidan Överför går du till en målmapp där du vill lägga till de överförda filerna eller mapparna i området **Välj mappdestination**.
1. (Valfritt) Ange det nya namnet på överföringsjobbet i textfältet Jobbnamn längst ned på sidan Överför. Du kan också använda det standardnamn som genereras av systemet i Adobe Dynamic Media Classic. Jobbet och andra överförings- och publiceringsjobb registreras på sidan Jobs, där du kan kontrollera jobbens status. Se [Kontrollera jobbfiler](checking-job-files.md#checking_job_files).
1. (Valfritt) Långt ned på sidan Överför väljer du **[!UICONTROL Publish After Uploading]** om du vill publicera de resurser som du överför automatiskt.
När du publicerar filer skickas filer till liveservrar. URL:er för dessa filer kan sedan användas på externa webbplatser och i externa program. Det här alternativet är också tillgängligt i dialogrutan Jobbalternativ.
1. (Valfritt) Långt ned på sidan Överför väljer du **[!UICONTROL Overwrite in any folder, same base asset name regardless of extension]** om du vill att de filer du överför ska ersätta befintliga filer med samma namn. Det här alternativet är också tillgängligt i dialogrutan Jobbalternativ.
Namnet på det här alternativet kan vara annorlunda, beroende på inställningarna i **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Upload to Application]** > **[!UICONTROL Overwrite Images]**.
1. I det nedre högra hörnet av sidan Överför väljer du **[!UICONTROL Job Options]** och anger sedan önskade alternativ.

   Se [Överföringsalternativ](uploading-files.md#upload_options).

1. Välj **[!UICONTROL Save]** i dialogrutan Alternativ för överföringsjobb.
1. Välj **[!UICONTROL Submit Upload]** längst ned till höger på sidan Överför.
Om du vill visa överföringsförloppet väljer du **[!UICONTROL Jobs]** i det globala navigeringsfältet. Du kan fortsätta arbeta i Adobe Dynamic Media Classic och när som helst återgå till jobbsidan för att granska ett pågående jobb. Om du vill avbryta ett pågående överföringsjobb väljer du **[!UICONTROL Cancel]** bredvid Varaktighet.

### Överföra filer med fliken VIA FTP {#upload-files-using-via-ftp}

1. Logga in på Adobe Dynamic Media Classic FTP-webbplatsen som är specifik för just din region. Använd det FTP-användarnamn och -lösenord som du fick från administratören.
1. I Adobe Dynamic Media Classic väljer du **[!UICONTROL Upload]** i fältet Global Navigation.
1. På sidan Överför väljer du fliken **[!UICONTROL VIA FTP]**.
1. Till vänster på sidan Överför väljer du en FTP-mapp att överföra filer från i **[!UICONTROL Choose FTP Folder For Upload]**-området.
1. Till höger på sidan Överför väljer du en målmapp i Adobe Dynamic Media Classic i området **[!UICONTROL Choose Adobe Dynamic Media Folder Destination]**.
1. (Valfritt) Ange det nya namnet på överföringsjobbet i textfältet Jobbnamn längst ned på sidan Överför. Du kan också använda det standardnamn som genereras av systemet i Adobe Dynamic Media Classic. Jobbet och andra överförings- och publiceringsjobb registreras på sidan Jobs, där du kan kontrollera jobbens status.
Se [Kontrollera jobbfiler](checking-job-files.md#checking_job_files).
1. (Valfritt) Långt ned på sidan Överför väljer du **[!UICONTROL Publish After Upload]** om du vill publicera de resurser som du överför automatiskt.
När du publicerar filer skickas filer till liveservrar. URL:er för dessa filer kan sedan användas på externa webbplatser och i externa program. Det här alternativet är också tillgängligt i dialogrutan Jobbalternativ.
1. (Valfritt) Långt ned på sidan Överför väljer du **[!UICONTROL Overwrite in any folder, same base asset name regardless of extension]** om du vill att de filer du överför ska ersätta befintliga filer med samma namn. Det här alternativet är också tillgängligt i dialogrutan Jobbalternativ.
Namnet på det här alternativet kan vara annorlunda, beroende på inställningarna i **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Upload to Application]** > **[!UICONTROL Overwrite Images]**.
1. Valfritt är bara tillgängligt om du klickade på fliken **[!UICONTROL VIA FTP]**. Långt ned på sidan Överför väljer du **[!UICONTROL Uncompress Zip or Tar Files on Upload]** om du automatiskt vill extrahera alla filer från den överförda ZIP- eller TAR-filen. Det här alternativet är också tillgängligt i dialogrutan Jobbalternativ.
1. I det nedre högra hörnet av sidan Överför väljer du **[!UICONTROL Job Options]** och anger sedan önskade alternativ.

   Se [Överföringsalternativ](uploading-files.md#upload_options).

1. Välj **[!UICONTROL Save]** i dialogrutan Alternativ för överföringsjobb.
1. Välj **[!UICONTROL Submit Upload]** längst ned till höger på sidan Överför.

   Om du vill visa överföringsförloppet väljer du **[!UICONTROL Jobs]** på det globala navigeringsfältet. På sidan Jobs visas överföringsförloppet. Du kan fortsätta arbeta i Adobe Dynamic Media Classic och när som helst återgå till jobbsidan för att granska ett pågående jobb.

Om du vill avbryta ett pågående överföringsjobb väljer du **[!UICONTROL Cancel]** bredvid Varaktighet.

## Dialogrutan Alternativ för överföringsjobb {#upload-options}

När du överför filer kan du välja mellan följande alternativ i dialogrutan Alternativ för överföringsjobb:

* **JOBB** - Välj  **[!UICONTROL JOB]** om du vill välja alternativ som påverkar hela överföringsjobbet.

   Du kan också välja *standard*-alternativ för överföring av jobb genom att använda dialogrutan **[!UICONTROL Default Upload Options]** i Allmänna inställningar. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Default Upload Options]** och ange sedan de standardalternativ du vill använda.

   * **[!UICONTROL When]** - Det här alternativet är bara tillgängligt om du har valt  **[!UICONTROL VIA FTP]** fliken.
      * **[!UICONTROL One-Time]** - Ange ett överföringsjobb som körs en gång. Alternativen är följande:
         * **[!UICONTROL Now]** - Kör överföringsjobbet omedelbart efter att du har valt  **[!UICONTROL Save]** i dialogrutan Alternativ för överföringsjobb och sedan valt  **[!UICONTROL Submit Upload]** på sidan Överför.
         * **[!UICONTROL Schedule For Later]** - Välj året, månaden, dagen och tiden (i 15-minuterssteg) som du vill att överföringsjobbet ska köras.
      * **[!UICONTROL Recurring]** - Ange ett överföringsjobb som körs varje dag, vecka eller månad. Eller anpassa överföringsjobbet efter dina egna specifikationer.
         * **[!UICONTROL Daily]** - Ange den tid du vill att jobbet ska köras varje dag. Om du vill att jobbet endast ska köras måndag till fredag väljer du **[!UICONTROL Weekdays Only]**.
         * **[!UICONTROL Weekly]** - Välj en specifik veckodag och tid som du vill att jobbet ska köras.
         * **[!UICONTROL Monthly]** - Välj en specifik dag i månaden eller dagen i veckan, inklusive starttiden, som du vill att jobbet ska köras.
         * **[!UICONTROL Custom]** - Anpassa tidsintervallet för överföring eller publicering enligt dina egna specifikationer. Se [Skapa ett anpassat tidsintervall för överföring eller publicering](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).
   * **[!UICONTROL Publish After Uploading]** - Tillgängligt om du har valt  **[!UICONTROL FROM DESKTOP]** fliken eller  **[!UICONTROL VIA FTP]** fliken. Välj det här alternativet om du automatiskt vill publicera de resurser som du överför. När du publicerar filer skickas filer till liveservrar. URL:er för dessa filer kan sedan användas på externa webbplatser och i externa program. Det här alternativet är även tillgängligt på sidan Överför.

   * **[!UICONTROL Overwrite in any folder, same base asset name regardless of extension]** - Tillgängligt om du har valt  **[!UICONTROL FROM DESKTOP]** fliken eller  **[!UICONTROL VIA FTP]** fliken. Välj det här alternativet om du vill att de filer du överför ska ersätta befintliga filer med samma namn. Det här alternativet är även tillgängligt på sidan Överför. Namnet på det här alternativet kan vara annorlunda, beroende på inställningarna i **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Upload to Application]** > **[!UICONTROL Overwrite Images]**.

   * **[!UICONTROL Uncompress Zip or Tar Files on Upload]** - Tillgängligt om du har valt  **[!UICONTROL FROM DESKTOP]** fliken eller  **[!UICONTROL VIA FTP]** fliken.
Välj det här alternativet om du automatiskt vill extrahera alla filer från den överförda ZIP- eller TAR-filen. Det här alternativet är också tillgängligt i dialogrutan Jobbalternativ.

   * **[!UICONTROL Include subfolders]** - Endast tillgängligt om du har valt  **[!UICONTROL VIA FTP]** fliken.
Välj det här alternativet om du vill överföra undermappar till mappen som du vill överföra. Namnen på mappen och dess undermappar som du överför anges automatiskt i Adobe Dynamic Media Classic.

   * **[!UICONTROL Process metadata files]** - Endast tillgängligt om du har valt någon av  **[!UICONTROL VIA FTP]** flikarna. Välj det här alternativet om du vill överföra en tabbavgränsad fil eller XML-fil för att lägga till metadata i flera resurser.
Se [Importera metadata (via FTP)](viewing-adding-exporting-metadata.md#import-metadata).


* **BESKÄR OPTIONS**  - Om du vill beskära pixlar med tomt utrymme automatiskt från en bild öppnar du  **[!UICONTROL Crop]** menyn, markerar  **[!UICONTROL Manual]** och anger pixelmått i textrutorna Överkant, Höger, Underkant och Vänster för att beskära från sidorna. Du kan också välja **[!UICONTROL Trim]** på menyn Beskär och välja följande alternativ:

   * **[!UICONTROL Trim Away Based On]** - Välj om du vill beskära baserat på färg eller genomskinlighet:
      * **[!UICONTROL Color]** - Välj alternativet Färg. Välj sedan menyn Hörn och välj hörnet på bilden med den färg som bäst motsvarar den tomrumsfärg som du vill beskära.
Trimma baserat på färg: Ange 0 om du bara vill beskära pixlar om de exakt matchar färgen som du valde i hörnet av bilden. Nummer som ligger närmare 1 ger större färgskillnader.
      * **[!UICONTROL Transparency]** - Välj  **[!UICONTROL Transparency]** alternativet.
Trimma baserat på genomskinlighet: Ange 0 om du bara vill beskära pixlar om de är genomskinliga. siffror närmare 1 ger större genomskinlighet.
      * **[!UICONTROL Tolerance]** - Dra skjutreglaget för att ange en tolerans mellan 0 och 1.

* **COLOR PROFILE OPTIONS**  - Välj en färgkonvertering när du skapar optimerade filer som används för dynamisk leverans i Adobe Dynamic Media Classic:

   * **[!UICONTROL Default Color Preservation]** - Behåller källbildens färger när bilderna innehåller färgrymdsinformation. det inte finns någon färgkonvertering. Nästan alla bilder idag har rätt färgprofil inbäddad. Om en CMYK-källbild inte innehåller någon inbäddad färgprofil konverteras färgerna till sRGB-färgrymden (standard röd grön). sRGB är den rekommenderade färgrymden för visning av bilder på webbsidor.
   * **[!UICONTROL Keep Original Color Space]** - Bevarar de ursprungliga färgerna utan färgkonvertering vid den tidpunkt då du tar bilden till Adobe Dynamic Media Classic. För bilder utan inbäddad färgprofil görs all nödvändig färgkonvertering för att bearbeta begäranden om bilden med hjälp av standardfärgprofilerna som konfigurerats i publiceringsinställningarna. Dessa färgprofiler justeras inte alltid mot färgen i de filer som skapas med det här alternativet. Därför bör du använda alternativet Standardfärgbevaring.
   * **[!UICONTROL Custom From]** >  **[!UICONTROL To]** - Öppnar menyer så att du kan välja en  **[!UICONTROL Convert From]** och en  **[!UICONTROL Convert To]** färgrymd. Det här avancerade alternativet åsidosätter eventuell färginformation som är inbäddad i källfilen. Välj bara det här alternativet när alla bilder som du skickar in innehåller felaktiga eller saknade färgprofildata.

* **Bildredigeringsalternativ**  - Du kan bevara  &lt;> urklippsmaskerna i bilder och välja en färgprofil.
Se [Alternativ för finjustering av bilder vid överföring](image-editing-options-upload.md#image-editing-options-at-upload).

* **Alternativ**  för PostScript® - Du kan rastrera PostScript®, beskära filer, behålla genomskinliga bakgrunder, välja en upplösning och välja en färgrymd.
Se [Arbeta med PostScript- och Illustrator-filer](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Photoshop-alternativ**  - Du kan skapa mallar från Adobe® Photoshop®-filer, behålla lager, ange hur lager ska namnges, extrahera text och ange hur bilder ska förankras i mallar.
Se [PSD-överföringsalternativ](psd-files.md#psd_upload_options).

* **PDF-alternativ**  - Du kan rastrera filerna, extrahera sökord och länkar, generera en e-katalog automatiskt, ange upplösningen och välja en färgrymd.
Se [Alternativ för PDF-överföring](pdfs.md#pdf_upload_options).

* **Illustrator-alternativ**  - Du kan rastrera Adobe Illustrator®-filer, behålla genomskinliga bakgrunder, välja en upplösning och välja en färgrymd.
Se [Arbeta med PostScript- och Illustrator-filer](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **EVIDEO-alternativ**  - Du kan omkoda en videofil genom att välja en videoförinställning.
Se [Arbeta med förinställningar för videokodning](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **Ytterligare metadata**  - Ange nyckelord som beskriver de filer som du vill överföra. Separera nyckelord med kommatecken. Nyckelord gör det enklare att söka efter resurser.
Se [Utför en avancerad sökning](searching-assets.md#conducting_an_advanced_search).

* **Gruppuppsättningsförinställningar**  - Om du vill skapa en bilduppsättning, snurruppsättning eller färgruteuppsättning från de överförda filerna markerar du  **[!UICONTROL Active]** kolumnen för den förinställning som du vill använda. Du kan markera flera förinställningar. Du skapar förinställningarna på sidan Programinställningar/Gruppera förinställningar.
Se [Gruppuppsättningsförinställningar](application-setup.md#batch_set_presets).

* **Avancerat**  - Se  [Följ upp en överföring med ett annat jobb](uploading-files.md#follow-an-upload-with-another-job).

## Följ en överföring med ett annat jobb {#follow-an-upload-with-another-job}

När du överför objekt med FTP kan du schemalägga ett efterföljande jobb så att det börjar när överföringen är klar. Om andra jobb är schemalagda att starta, köas det jobb som du schemalägger här efter dem.

Det nya jobbet skickar ett meddelande till den adress du anger så att koden på den platsen kan utlösas. Detta uppföljningspubliceringsjobb använder samma namn som överföringsjobbet, men med texten *Pub_* tillagd i början.

**Så här utför du en överföring med ett annat jobb:**

1. Välj **[!UICONTROL Upload]** och sedan fliken **[!UICONTROL VIA FTP]**.
1. Välj **[!UICONTROL Job Options]** längst ned till höger på sidan Överför.
1. Expandera avsnittet **[!UICONTROL ADVANCED]** i dialogrutan Alternativ för överföringsjobb.
1. Välj något av följande i listrutan **[!UICONTROL Follow Upload with another job]**:

   * Ingen
   * HTTP-begäran
   * Image Serving Publish
   * Publicera bildåtergivning
   * Video Publish

1. Ange HTTP-adressen.
1. Ange om du bara vill köra filer som har överförts.
1. Ange om du vill köra den här begäran varje gång jobbet slutförs, eller endast när filer publicerades.

   >[!NOTE]
   >
   >Vanliga schemalagda jobb kan ibland leda till att inga filer publiceras.

>[!MORELIKETHIS]
>
>* [Arbeta med resursmappar](asset-folders.md#working_with_asset_folders)
>* [Hantera återkommande överförings- och publiceringsjobb](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Använd ett överförings- eller publiceringsjobb som utlösare](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

