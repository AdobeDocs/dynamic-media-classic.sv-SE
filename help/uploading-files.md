---
title: Överför filer
description: Lär dig hur du överför filer.
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
feature: Dynamic Media Classic,Resurshantering
role: Business Practitioner
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
translation-type: tm+mt
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '3681'
ht-degree: 0%

---

# Överför filer{#uploading-files}

Innan du överför resursfiler till Dynamic Media Classic måste du se till att resursfilerna har rätt namn och att mappstrukturen är konfigurerad och ordnad som du vill ha den. Du kan överföra filer från en FTP-plats som tillhandahålls av Dynamic Media Classic eller direkt från datorn eller nätverket. I Dynamic Media Classic finns alternativ för att optimera filer när du överför dem. Om du har installerat Adobe Dynamic Media Classic kan du överföra filer och mappar genom att dra dem direkt från skrivbordet. Se [Allmänna inställningar för program](application-setup.md#general_settings).

## Förbereder dina resurser och mappar för överföring av {#preparing-your-assets-and-folders-for-uploading}

Innan du överför resurser till Dynamic Media Classic bör du kontrollera att de har rätt format och storlek. Du måste också följa Dynamic Media Classic-reglerna för att namnge resurser. Genom att konfigurera en mappstruktur för filerna ser du till att du enkelt kan hitta och arbeta med filerna.

### Resursfilformat som stöds {#supported-asset-file-formats}

I den här tabellen visas de filformat som stöds i Dynamic Media Classic. Information om vilka Camera Raw filer som stöds finns i [https://www.adobe.com/go/learn_s7_cameraraw_en](https://www.adobe.com/go/learn_s7_cameraraw_en).

| Resursfilformat | Beskrivning |
|--- |--- |
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
| Dynamic Media Classic Image Authoring | VNC, VNT, VNW |
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

För att få bästa möjliga resultat med Dynamic Media Classic bör du använda de rekommenderade filformaten och storlekarna. I den här tabellen visas resurstyper, vissa med rekommenderade format och filstorlekar för resurser som används ofta.

| Tillgångstyp | Beskrivning/Recommendations |
|--- |--- |
| Ljud | Bland indatafilformaten för ljudresurser finns AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3. Du kan koda om ljud till följande format: MP3, AAC och HE-AAC. |
| Bilder (för Bildstorlek, Zooma, Bilduppsättningar, Snurra uppsättningar) | Bilderna måste ha minst 2 000 pixlar med den längsta storleken. de vanliga bildstorlekarna varierar mellan 1 500 och 2 500 pixlar i den längsta storleken. Vi rekommenderar förlustfria bildformat, inklusive TIFF- och PNG-filer. Om du använder en JPEG-bild bör du använda inställningarna för den högsta kvaliteten. Animate GIF-filer hanteras som annat statiskt innehåll. |
| eCatalogs | Använd högupplösta PDF-filer som skapats i Adobe® Acrobat® eller ett Creative Suite-program som sparats som &quot;tryckoriginal&quot;. PDF-filer innehåller alla teckensnitt, bilder, masker och refererade grafiska element som behövs, antingen som enkelsidiga, dubbelsidiga uppslag eller i ett flersidigt format. Ordna sidorna genom att namnge filerna i alfanumerisk ordning. Placera alla PDF-filer för din e-katalog i en enda mapp för att underlätta överföringen. Du kan välja beskärningsalternativ när du överför för att ta bort beskärningsområdet från PDF-filer, inklusive skärmärken, registreringsmål eller färgfält. De flesta tryckfärdiga PDF-filer finns i CMYK-färgmodellen, så det är viktigt att du hämtar den ICC-färgprofil för CMYK som används med PDF-filerna. |
| Mallar | Bild- eller layoutdesign med flera lager som kan innehålla text, bilder och lager. Bildlager, textsträngar och attribut, som färg och storlek, kan parametriseras så att variabeldata kan anpassas. Bildkraven för användning i mallar är desamma som för andra bilder. Förbered bilderna i Photoshop eller något annat bildredigeringsprogram. Spara varje bild som en förenklad genomskinlig fil i TIFF- eller PNG-format. Kontrollera att bildupplösningen är lämplig för förväntad användning. Bilder för utskrift är 300 ppi. |
| Videor | Dynamic Media Classic stöder videofiler som sparats i formaten OGV och MP4. Du kan omkoda filer till MP4-format vid överföring. Se [Resursfilformat som stöds](#supported-static-file-formats). |
| Teckensnitt | Överförda TrueType, Type1 (endast Windows®), OpenType®-teckensnitt och PhotoFonts |
| Bilder | Bilder och bildfiler med flera lager. |
| Bilduppsättningar och färgruteuppsättningar | En uppsättning närliggande bilder som kan visas i ett visningsprogram. |
| ICC-profiler | En färgprofil som du kan använda för att konvertera en överförd bild från dess källfärgrymd till en annan färgrymd. |
| Vinjetter | Bilder som skapats med bildredigeringsprogrammet och relaterade filer. |
| Innehållsfiler | Adobe InDesign, Illustrator eller Photoshop innehållsfiler. |
| FXG-filer | Upplösningsoberoende grafikformatfiler som du kan använda för att skapa anpassningsbara mallar för utskrift, webb, e-post, dator och enheter. |
| SVG-filer | Skalbara vektorgrafikfiler som Image Serving-servrar kan återge. |
| XML-filer | Filer som definierar förbearbetningsregler som används för att ändra sökväg och frågedelar för begäranden. |
| Cascading Style Sheet-filer. | Överför CSS-skal för anpassning av HTML5-visningsprogram. |
| JavaScript™-filer | JavaScript™-filer används för visningsprograminstrumentering för kontoinformation. Adobe Security rekommenderar att den här resurstypen endast används för klientkonton som har en separat domän som används för leverans (för att undvika serveröverskridande skript). |

>[!NOTE]
>
>När du överför bildfiler och PDF-filer till Dynamic Media Classic konverteras dessa källfiler till P-TIFF-filer (Pyramid TIFF). Dessa P-TIFF-filer är de filer som senare publiceras till Dynamic Media Image Servers. I Dynamic Media Classic används filformatet Pyramid Tiff eftersom det innehåller olika zoomningsförhållanden som möjliggör snabb zoomning när det visas med en Dynamic Media Classic Zoom Viewer.

### Statiska filformat {#supported-static-file-formats} som stöds

Dynamic Media Classic stöder flera statiska filformat. Statiskt innehåll är alla resurser som publiceras i befintligt skick, t.ex. CSS, PDF, SVG och XML.

Följande filtyper kan publiceras:

* Animerad GIF
* Ljudfiler
* CSS
* JavaScript™ (när företaget är konfigurerat med sin egen domän)
* Överordnad video
* PDF (när PDF har markerats för publicering efter överföring, för att undvika att alla PDF-filer levereras för det befintliga eCatalog/PDF-arbetsflödet)
* PrX-video
* SVG
* XML
* ZIP

I Dynamic Media Classic går det inte att generera en förhandsgransknings-URL för statiskt innehåll.

### Krav för filnamn {#filename-requirements}

Eftersom filnamnstillägg tas bort från filnamn under överföringsprocessen tillåter inte systemet att filer har samma rotnamn. I Dynamic Media Classic-systemet blir filnamnet minus filnamnstillägget resurs-ID för resursen. Därför kan två resurser inte ha samma namn.

Se till att alla användare på företaget förstår följande regler för filnamngivning:

* Tillgångs-ID:n med samma exakta namn tillåts inte i systemet.
* Resurs-ID:n är skiftlägeskänsliga.
* Ett tips är att se till att resurs-ID:n inte innehåller blanksteg (t.ex. svart jacka.tif och blå jpg). Dynamic Media Classic ASCII kodar tomma utrymmen i resursnamn när resursnamn används för att skapa URL-strängar. Dessa ASCII-koder är svåra att läsa, vilket kan göra det svårare att läsa URL:er.
* Språkspecifika tecken får användas i filnamn. Följande tecken får dock inte användas i filnamn:

   \ ; / ? : @ &amp; = + $ , * &quot; &lt; > | &#39; {} %

   Om ett filnamn innehåller ett eller flera av ovanstående tecken tas tecknen bort från filnamnet vid överföringen.

Vanligtvis kan ett filnamn för en resurs vara samma som dess artikelnummer, produkt-SKU eller annat namn som i följande exempel:

| Objekt | Filnamn | Tillgångs-ID |
|--- |--- |--- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Mappordning och struktur {#folder-organization-and-structure}

Ordna och strukturera mappar och undermappar för ditt innehåll i Dynamic Media Classic innan du överför innehållet till systemet. Planering framåt på det här sättet har två stora fördelar:

* När du överför innehåll till Dynamic Media Classic via FTP kan du ange att systemet ska replikera mappstrukturen under överföringen. På så sätt ordnas ditt innehåll i samma mappar och undermappar i Dynamic Media Classic som det finns på datorn eller i nätverket. (Om du vill replikera mappstrukturen i Dynamic Media Classic markerar du alternativet Inkludera undermappar när du överför resurser via FTP.)
* Det är mycket svårare att ordna om mappar i systemet efter att filer har överförts än att börja med en noggrant genomtänkt mappstruktur.

Vilken mappnamnsmetod och struktur du väljer för att lagra ditt innehåll på Dynamic Media Classic beror på organisationens behov. Här följer några exempel på mappstrukturer:

**SKU-baserade**  mappar namnges enligt SKU:er eller artikelnummer. Separata mappar skapas till exempel för alla serier med 0-, 20- och 30-tal.

**Varumärkesbaserad**  - För tillverkare med flera varumärken och detaljhandlare som marknadsför andra varumärken från andra företag, kan du dela upp filer i produktmappar som namngetts för olika varumärken.

**Projektbaserad**  - Mappar ordnas efter datum för utrullning/släppning eller projektnamn. Kunder som främst producerar e-kataloger gillar detta.

**Spegling av webbplatsens mapphierarki**  - Mappstrukturen speglar webbplatsens mappstruktur, med mapparna till exempel namngivna för produktkategorier.

## Om att överföra filer {#uploading-your-files}

Du kan överföra enskilda filer från skrivbordet eller överföra mappar via FTP. Om du vill överföra mer än 100 MB filer eller överföra hela mappar och undermappar väljer du fliken **VIA FTP**.

Dynamic Media Classic skickar ett e-postmeddelande till dig för att bekräfta när överföringsjobbet påbörjas och avslutas samt för att meddela dig om eventuella problem.

Under (eller omedelbart efter) ett stort överföringsjobb kan vissa nya objekt visa meddelandet&quot;Bilden är ännu inte optimerad&quot;. Det här meddelandet visas eftersom filerna ännu inte har bearbetats fullständigt och lagts till i Dynamic Media Classic. Du kan optimera dessa filer senare. Se [Optimera filer](application-setup.md#optimize_files).

### Överföra filer med hjälp av fliken Från skrivbord {#upload-files-using-sps-desktop-application}

Med Dynamic Media Classic för datorer kan du överföra filer och mappar genom att dra.

1. Klicka på **[!UICONTROL Upload]** i fältet Global Navigation i Dynamic Media Classic Desktop.
1. På sidan Överför klickar du på fliken **[!UICONTROL From Desktop]**.
1. Klicka på **[!UICONTROL Browse]** till vänster på sidan Överför i området **[!UICONTROL Select Files for Upload]** för att markera de filer eller mappar som du vill överföra och klicka sedan på **[!UICONTROL Open]**.
1. Till höger på sidan Överför går du till en målmapp där du vill lägga till de överförda filerna eller mapparna i området **Välj mappdestination**.
1. (Valfritt) Ange det nya namnet på överföringsjobbet i fältet **[!UICONTROL Job Name]** längst ned på sidan Överför. Du kan också använda det standardnamn som genereras av systemet i Dynamic Media Classic. Jobbet och andra överförings- och publiceringsjobb registreras på sidan Jobs, där du kan kontrollera jobbens status. Se [Kontrollera jobbfiler](checking-job-files.md#checking_job_files).
1. (Valfritt) Långt ned på sidan Överför väljer du **[!UICONTROL Publish After Uploading]** om du vill publicera de resurser som du överför automatiskt.
När du publicerar filer skickas filer till liveservrar. URL:er för dessa filer kan sedan användas på externa webbplatser och i externa program. Det här alternativet är också tillgängligt i dialogrutan Jobbalternativ.
1. (Valfritt) Långt ned på sidan Överför väljer du **[!UICONTROL Overwrite in any folder, same base asset name regardless of extension]** om du vill att de filer du överför ska ersätta befintliga filer med samma namn. Det här alternativet är också tillgängligt i dialogrutan Jobbalternativ.
Namnet på det här alternativet kan vara annorlunda, beroende på inställningarna i **Programinställningar > Allmänna inställningar > Överför till program > Skriv över bilder**.
1. Klicka på **[!UICONTROL Job Options]** längst ned till höger på sidan Överför och ange önskade alternativ.

   Se [Överföringsalternativ](uploading-files.md#upload_options).

1. Klicka på **[!UICONTROL Save]** i dialogrutan Alternativ för överföringsjobb.
1. Klicka på **[!UICONTROL Submit Upload]** längst ned till höger på sidan Överför.
Klicka på **[!UICONTROL Jobs]** i det globala navigeringsfältet om du vill se överföringsförloppet. Du kan fortsätta arbeta i Dynamic Media Classic och när som helst återgå till jobbsidan för att granska ett pågående jobb. Om du vill avbryta ett pågående överföringsjobb väljer du **[!UICONTROL Cancel]** bredvid Varaktighet.

### Överföra filer med fliken VIA FTP {#upload-files-using-via-ftp}

1. Logga in på den Dynamic Media Classic FTP-plats som är specifik för just din region. Använd det FTP-användarnamn och -lösenord som du fick från administratören.
1. Klicka på **[!UICONTROL Upload]** i fältet Global navigering i Dynamic Media Classic.
1. På sidan Överför klickar du på fliken **[!UICONTROL VIA FTP]**.
1. Till vänster på sidan Överför väljer du en FTP-mapp att överföra filer från i **[!UICONTROL Choose FTP Folder For Upload]**-området.
1. Till höger på sidan Överför väljer du en målmapp i Dynamic Media Classic i området **[!UICONTROL Choose Adobe Dynamic Media Folder Destination]**.
1. (Valfritt) Ange det nya namnet på överföringsjobbet i fältet **[!UICONTROL Job Name]** längst ned på sidan Överför. Du kan också använda det standardnamn som genereras av systemet i Dynamic Media Classic. Jobbet och andra överförings- och publiceringsjobb registreras på sidan Jobs, där du kan kontrollera jobbens status.
Se [Kontrollera jobbfiler](checking-job-files.md#checking_job_files).
1. (Valfritt) Långt ned på sidan Överför väljer du **[!UICONTROL Publish After Upload]** om du vill publicera de resurser som du överför automatiskt.
När du publicerar filer skickas filer till liveservrar. URL:er för dessa filer kan sedan användas på externa webbplatser och i externa program. Det här alternativet är också tillgängligt i dialogrutan Jobbalternativ.
1. (Valfritt) Långt ned på sidan Överför väljer du **[!UICONTROL Overwrite in any folder, same base asset name regardless of extension]** om du vill att de filer du överför ska ersätta befintliga filer med samma namn. Det här alternativet är också tillgängligt i dialogrutan Jobbalternativ.
Namnet på det här alternativet kan vara annorlunda, beroende på inställningarna i **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Upload to Application]** > **[!UICONTROL Overwrite Images]**.
1. Valfritt är bara tillgängligt om du klickade på fliken **[!UICONTROL VIA FTP]**. Långt ned på sidan Överför väljer du **[!UICONTROL Uncompress Zip or Tar Files on Upload]** om du automatiskt vill extrahera alla filer från den överförda ZIP- eller TAR-filen. Det här alternativet är också tillgängligt i dialogrutan Jobbalternativ.
1. Klicka på **[!UICONTROL Job Options]** längst ned till höger på sidan Överför och ange önskade alternativ.

   Se [Överföringsalternativ](uploading-files.md#upload_options).

1. Klicka på **[!UICONTROL Save]** i dialogrutan Alternativ för överföringsjobb.
1. Klicka på **[!UICONTROL Submit Upload]** längst ned till höger på sidan Överför.

   Klicka på **[!UICONTROL Jobs]** på det globala navigeringsfältet för att se överföringsförloppet. På sidan Jobs visas överföringsförloppet. Du kan fortsätta arbeta i Dynamic Media Classic och när som helst återgå till jobbsidan för att granska ett pågående jobb.

Om du vill avbryta ett pågående överföringsjobb klickar du på **[!UICONTROL Cancel]** bredvid Varaktighet.

## Dialogrutan Alternativ för överföringsjobb {#upload-options}

När du överför filer kan du välja mellan följande alternativ i dialogrutan Alternativ för överföringsjobb:

* **JOBB** - Klicka  **[!UICONTROL JOB]** för att välja alternativ som påverkar hela överföringsjobbet.

   Du kan också välja *standard*-alternativ för överföring av jobb genom att använda dialogrutan **[!UICONTROL Default Upload Options]** i Allmänna inställningar. Klicka på **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Default Upload Options]** och ange sedan de standardalternativ du vill använda.

   * **När**  - Det här alternativet är bara tillgängligt om du har valt  **[!UICONTROL VIA FTP]** fliken.
      * **Engångsjobb**  - Ange ett överföringsjobb som körs en gång. Alternativen är följande:
         * **Nu** - Kör överföringsjobbet omedelbart efter att du har klickat  **[!UICONTROL Save]** i dialogrutan Alternativ för överföringsjobb och sedan klickat  **[!UICONTROL Submit Upload]** på sidan Överför.
         * **Schemalägg för senare** - Välj det år, månad, dag och tid (i 15-minutersintervall) som du vill att överföringsjobbet ska köras.
      * **Återkommande**  - Ange ett överföringsjobb som körs varje dag, varje vecka eller varje månad. Eller anpassa överföringsjobbet efter dina egna specifikationer.
         * **Dagligen**  - Ange den tid du vill att jobbet ska köras varje dag. Om du vill att jobbet endast ska köras måndag till fredag väljer du **[!UICONTROL Weekdays Only]**.
         * **Veckovis**  - Välj en specifik dag i veckan och den tidpunkt då du vill att jobbet ska köras.
         * **Månadsvis**  - Välj en specifik dag i månaden eller dagen i veckan, inklusive starttiden, som du vill att jobbet ska köras.
         * **Anpassad**  - Anpassa ett tidsintervall för överföring eller publicering enligt dina egna specifikationer. Se [Skapa ett anpassat tidsintervall för överföring eller publicering](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).
   * **Publicera efter överföring**  - Tillgängligt om du har valt  **[!UICONTROL FROM DESKTOP]** fliken eller  **[!UICONTROL VIA FTP]** fliken. Välj det här alternativet om du automatiskt vill publicera de resurser som du överför. När du publicerar filer skickas filer till liveservrar. URL:er för dessa filer kan sedan användas på externa webbplatser och i externa program. Det här alternativet är även tillgängligt på sidan Överför.

   * **Skriv över i valfri mapp, samma basresursnamn oavsett tillägg**  - Tillgängligt om du har valt  **[!UICONTROL FROM DESKTOP]** fliken eller  **[!UICONTROL VIA FTP]** fliken. Välj det här alternativet om du vill att de filer du överför ska ersätta befintliga filer med samma namn. Det här alternativet är även tillgängligt på sidan Överför. Namnet på det här alternativet kan vara annorlunda, beroende på inställningarna i **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Upload to Application]** > **[!UICONTROL Overwrite Images]**.

   * **Avkomprimera zip- eller målfiler vid överföring**  - Tillgängligt om du har valt  **[!UICONTROL FROM DESKTOP]** fliken eller  **[!UICONTROL VIA FTP]** fliken.
Välj det här alternativet om du automatiskt vill extrahera alla filer från den överförda ZIP- eller TAR-filen. Det här alternativet är också tillgängligt i dialogrutan Jobbalternativ.

   * **Inkludera undermappar**  - Endast tillgängligt om du har valt  **[!UICONTROL VIA FTP]** fliken.
Välj det här alternativet om du vill överföra undermappar till mappen som du vill överföra. Namnen på mappen och dess undermappar som du överför anges automatiskt i Dynamic Media Classic.

   * **Bearbeta metadatafiler**  - Endast tillgängligt om du har valt någon av  **[!UICONTROL VIA FTP]** flikarna. Välj det här alternativet om du vill överföra en tabbavgränsad fil eller XML-fil för att lägga till metadata i flera resurser.
Se [Importera metadata (via FTP)](viewing-adding-exporting-metadata.md#import-metadata).


* **BESKÄR OPTIONS**  - Om du vill beskära pixlar med tomt utrymme automatiskt från en bild öppnar du  **[!UICONTROL Crop]** menyn, klickar  **[!UICONTROL Manual]** och anger pixelmått i textrutorna Överkant, Höger, Underkant och Vänster för att beskära från sidorna. Du kan också klicka på **[!UICONTROL Trim]** på menyn Beskär och välja följande alternativ:

   * **Rensa bort baserat på**  - Välj om du vill beskära baserat på färg eller genomskinlighet:
      * **Färg**  - Välj alternativet Färg. Välj sedan menyn Hörn och välj hörnet på bilden med den färg som bäst motsvarar den tomrumsfärg som du vill beskära.
Trimma baserat på färg: Ange 0 om du bara vill beskära pixlar om de exakt matchar färgen som du valde i hörnet av bilden. Nummer som ligger närmare 1 ger större färgskillnader.
      * **Genomskinlighet**  - Välj  **[!UICONTROL Transparency]** alternativet.
Trimma baserat på genomskinlighet: Ange 0 om du bara vill beskära pixlar om de är genomskinliga. siffror närmare 1 ger större genomskinlighet.
      * **Tolerans**  - Dra i skjutreglaget för att ange en tolerans mellan 0 och 1.

* **COLOR PROFILE OPTIONS**  - Välj en färgkonvertering när du skapar optimerade filer som används för dynamisk leverans i Dynamic Media Classic:

   * **Standardfärgbevaring**  - Behåller källbildens färger när bilderna innehåller färgrymdsinformation. det inte finns någon färgkonvertering. Nästan alla bilder idag har rätt färgprofil inbäddad. Om en CMYK-källbild inte innehåller någon inbäddad färgprofil konverteras färgerna till sRGB-färgrymden (standard röd grön). sRGB är den rekommenderade färgrymden för visning av bilder på webbsidor.
   * **Behåll ursprunglig färgrymd** - Behåller originalfärgerna utan någon färgkonvertering vid den tidpunkt då färgen hämtas in till Dynamic Media Classic. För bilder utan inbäddad färgprofil görs all nödvändig färgkonvertering för att bearbeta begäranden om bilden med hjälp av standardfärgprofilerna som konfigurerats i publiceringsinställningarna. Dessa färgprofiler justeras inte alltid mot färgen i de filer som skapas med det här alternativet. Därför bör du använda alternativet Standardfärgbevaring.
   * **Anpassad från > Till** - Öppnar menyer så att du kan välja en  **[!UICONTROL Convert From]** och  **[!UICONTROL Convert To]** en färgrymd. Det här avancerade alternativet åsidosätter eventuell färginformation som är inbäddad i källfilen. Välj bara det här alternativet när alla bilder som du skickar in innehåller felaktiga eller saknade färgprofildata.

* **BILDREDIGERING AV OPTIONS** - Du kan bevara  &lt;> urklippsmaskerna i bilder och välja en färgprofil.
Se [Bildredigeringsalternativ vid överföring](image-editing-options-upload.md#image-editing-options-at-upload).

* **PostScript®**  - Du kan rastrera PostScript®, beskära filer, behålla genomskinliga bakgrunder, välja en upplösning och välja en färgrymd.
Se [Arbeta med PostScript- och Illustrator-filer](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Photoshop OPTIONS**  - Du kan skapa mallar från Adobe® Photoshop®-filer, behålla lager, ange hur lager ska namnges, extrahera text och ange hur bilder ska förankras i mallar.
Se [PSD-överföringsalternativ](psd-files.md#psd_upload_options).

* **PDF OPTIONS**  - Du kan rastrera filerna, extrahera sökord och länkar, generera en e-katalog automatiskt, ange upplösningen och välja en färgrymd.
Se [Alternativ för PDF-överföring](pdfs.md#pdf_upload_options).

* **Illustrator OPTIONS**  - Du kan rastrera Adobe Illustrator®-filer, behålla genomskinliga bakgrunder, välja en upplösning och välja en färgrymd.
Se [Arbeta med PostScript- och Illustrator-filer](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **EVIDEO OPTIONS**  - Du kan koda om en videofil genom att välja en videoförinställning.
Se [Arbeta med förinställningar för videokodning](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **YTTERLIGARE METADATA**  - Ange nyckelord som beskriver de filer som du tänker överföra. Separera nyckelord med kommatecken. Nyckelord gör det enklare att söka efter resurser.
Se [Avancerad sökning](searching-assets.md#conducting_an_advanced_search).

* **FÖRINSTÄLLNINGAR**  FÖR BATCH-INSTÄLLNINGAR - Om du vill skapa en bilduppsättning, en fleraxelssnurra eller en färgruteuppsättning från de överförda filerna klickar du på kolumnen Aktiv för den förinställning som du vill använda. Du kan markera flera förinställningar. Du skapar förinställningarna på sidan Programinställningar/Gruppera förinställningar.
Se [Gruppuppsättningsförinställningar](application-setup.md#batch_set_presets).

* **AVANCERAD**  - Se  [Följ upp en överföring med ett annat jobb](uploading-files.md#follow-an-upload-with-another-job).

## Följ upp en överföring med ett annat jobb {#follow-an-upload-with-another-job}

När du överför objekt med FTP kan du schemalägga ett efterföljande jobb så att det börjar när överföringen är klar. Om andra jobb är schemalagda att starta, köas det jobb som du schemalägger här efter dem.

Det nya jobbet skickar ett meddelande till den adress du anger så att koden på den platsen kan utlösas. Detta uppföljningspubliceringsjobb använder samma namn som överföringsjobbet, men med texten *Pub_* tillagd i början.

**Så här utför du en överföring med ett annat jobb:**

1. Klicka på **[!UICONTROL Upload]** och sedan på fliken **[!UICONTROL VIA FTP]**.
1. Klicka på **[!UICONTROL Job Options]** längst ned till höger på sidan Överför.
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
>* [Använda ett överförings- eller publiceringsjobb som utlösare](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

