---
title: Öka skärpan i en bild
description: Lär dig hur du ökar skärpan i en bild i Adobe Dynamic Media Classic.
uuid: d86af74a-89c5-4f2b-96ba-f2e7da600bca
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 11cd5362-d90a-4c1e-bfbd-46a65a554409
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 4b3e8368-f8f5-46d9-9130-361a8273de2c
topic: Content Management
level: Intermediate
source-git-commit: ae7d0c6d3047d68ed3da4187ef516dc51c95de30
workflow-type: tm+mt
source-wordcount: '2154'
ht-degree: 0%

---

# Öka skärpan i en bild {#sharpening-an-image}

Skärpa är en bildändringsteknik som används för att göra konturerna i en digital bild mer distinkta. Skärpa ökar kontrasten mellan kantpixlar och framhäver övergången mellan mörka och ljusa områden. Skärpa ökar lokal kontrast och ger detaljskärpa. Det finns ingen strikt formel för att göra alla bilder skarpare. För lite skärpa kan skapa en mjuk bild, men för mycket skärpa ger haloeffekter, artefakter och brus.

Adobe Dynamic Media Classic rekommenderar att du använder bildförinställningar för alla bilder. De ger en enhetlig storlek och skärpan används för alla bilder som kallas för bildförinställningar. Dessutom kan du enkelt redigera och ändra en förinställd bilds skärpeparametrar. Nästa gång du publicerar får alla bilder som anropas med den förinställningen de nya värdena.

Adobe Dynamic Media Classic rekommenderar också att du lägger till skärpa i visningsförinställningar och sedan anropar ett visningsprogram med den förinställningen. På så sätt blir bilderna skarpa och tilltalande i dina visningsprogram.

Oavsett om du använder bildförinställningar och visningsförinställningar, eller någon metod för att öka skärpan, så är den sista raden att du måste göra bilderna skarpare. Om du inte gör det kan dina bilder (och din webbplats) se mjuka och luddiga ut.

>[!NOTE]
>
>Kommandona Skärpa åsidosätter inställningarna för bildförinställningar, inklusive deras skärpeeffekter. En bildförinställning styr storleken och formateringen som bilder levereras med från Dynamic Media bildservrar. Adobe Dynamic Media Classic rekommenderar att du använder bildförinställningar för att leverera alla bilder så att bilderna levereras med en enhetlig storlek och skärpa. När skärpeinställningarna för en enskild bild har ändrats gäller skärpeinställningarna inte längre för bilden. Den levereras utan skärpeinställningar för bildförinställningar.

Det är ofta nödvändigt att göra bilder skarpare. Adobe Dynamic Media Classic- och bildservrar erbjuder flera olika skärpealternativ. Det är viktigt att du förstår vad skärpa gör i en bild och hur mycket skärpa du behöver. De flesta bilder behöver skärpa, men mängden som krävs beror på bilden.

Bildskärpa ökar pixlarnas kontrast för att skapa effekten av framhävda kanter. Människan uppfattar den här förbättrade kantkontrasten som skärpa. Det är enkelt att förbättra en bild genom att köra skärpefilter på en bild, men det är också enkelt att öka skärpan i en bild för mycket.

Om du ökar skärpan i en bild för mycket skapas en ljusgårdseffekt, eller ränder från kantens linjer.

Det finns god praxis som du kan följa för att optimera skärpan i dina bilder i Adobe Dynamic Media Classic och på Dynamic Media Image Server.

Se [Bästa tillvägagångssätt för att öka skärpan i bilder i Adobe Dynamic Media Classic och på Dynamic Media Image Server](/help/using/assets/s7_sharpening_images.pdf).

Se även [Skärpa](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) utbildningsvideo.

**Så här gör du en bild skarpare:**

Om du vill göra en bild skarpare väljer du dess överrullning **[!UICONTROL Edit]** och välj **[!UICONTROL Sharpen]** eller öppna den i panelen Bläddra i detaljvyn och markera sedan **[!UICONTROL Sharpen]**. Sidan Skärperedigeraren öppnas med skärpekommandon. Välj kommandon och välj sedan **[!UICONTROL Save]**.

>[!NOTE]
>
>Innan du gör en bild skarpare kan du välja menyn Använd förinställning och välja en bildförinställning för att se vilka skärpeeffekter den har. Skärpeeffekterna i en bildförinställning passar bra för din bild. The **[!UICONTROL Apply Preset]** menyn finns längst ned på sidan för skärperedigeraren.

**Skärpealternativ**

I följande tabell visas skärpealternativen för bildservern.

| Namn | URL Protocol | Värden | Exempel |
| --- | --- | --- | --- |
| Enkel skärpa | `op_sharpen` | `0` eller `1` | `op_sharpen=1` |
| Sampla om läge | `resMode` | `bilin`, `bicub`, `sharp2`, `trilin`<br><br>`bilin`: Väljer bilinjär standardinterpolation. Den snabbaste omsamplingsmetoden. Vissa aliasing-artefakter är ofta märkbara.<br>`bicub`: Väljer bikubisk interpolation. Mer processorintensivt än `bilin`, men ger skarpare bilder med mindre märkbara aliasing-artefakter.<br><br>`sharp2`: Väljer en modifierad Lanczos Windows®-funktion som interpoleringsalgoritm. Kan ge något tydligare resultat än bikubisk till en högre processorkostnad.<br><br>`trilin`: Väljer en ändrad trilinjär interpolation, som använder både högre och lägre upplösningar, om en sådan finns. Rekommenderas endast när kantutjämning är ett problem. Minskar storleken på JPEG på grund av reducerade högfrekventa data. | `resMode=sharp2` |
| Oskarp mask | `op_usm` | `amount`, `radius`, `threshold`, `monochrome`<br><br>`amount`: filterstyrkefaktor (verklig 0...5)<br><br>`radius`: filterkärnradie i pixlar (verklig 0...250) <br><br>`threshold`: filtertröskelnivå (int 0...255)<br><br>`monochrome`: inställd på `0` för att göra varje färgkomponent oskarp separat, ange `1` till intensitet för oskarp mask (intensitet) | `op_usm=1,1,10,0` |

Välj **[!UICONTROL Sharpening]** och välj ett alternativ:

* **Ingen** - Inaktiverar skärpa.

* **Skärpa** - Kör ett enkelt skärpesteg för filen när den har ändrat storlek. Den liknar filtret &quot;Skärpa&quot; i Adobe Photoshop och stöder alla användarparametrar. Normalt använder du det här filtret eller **[!UICONTROL Unsharp Mask]**, men inte båda. Det är en god praxis att inte rekommendera den här metoden, men den kan kompensera för oskärpa. (URL: `op_sharpen`)

* **Oskarp mask** - Du kan finjustera en skärpefiltereffekt på den nedsamplade bilden. Du kan styra intensiteten för effekten, radien för effekten (mätt i pixlar) och ett tröskelvärde för kontrast som ignoreras. Den här effekten använder samma alternativ som Photoshop Oskarp mask-filter. (URL: `op_usm`)

Välj följande alternativ så att du kan finjustera skärpan med Oskarp mask:

* **Belopp** - Styr mängden kontrast som används på kantpixlar. Standardvärdet är 0,0. För högupplösta bilder kan du öka den till upp till 5.0. Tänk på Mängd som ett mått på filterintensiteten. The **[!UICONTROL Amount]** inställningen i Adobe Dynamic Media Classic är inte densamma som inställningen Mängd i Adobe Photoshop. Adobe Photoshop använder ett värde mellan 1 % och 500 %, medan Adobe Dynamic Media Classic kan skalas från 0,0 till 5,0. (5.0 motsvarar ungefär 500 % i Photoshop, 0,9 motsvarar 90 % och så vidare.)

* **Radie** - Anger antalet pixlar runt kantpixlarna som påverkar skärpan. Effekten körs på alla pixlar i bilden och strålar ut i alla riktningar.

Det bästa radievärdet beror på bildens storlek. Med ett lågt värde ökas skärpan endast för kantpixlarna. Med ett högt värde ökas skärpan för ett större antal pixlar.

Om du till exempel vill få en liknande skärpeeffekt för en bild på 2 000 × 2 000 pixlar och en bild på 500 × 500 pixlar, kan du ange ett radievärde på två pixlar för bilden på 2 000 × 2 000 pixlar. Ange sedan radien 1 pixel på bilden med 500 × 500 pixlar (ett större värde för en bild med fler pixlar).

* **Tröskelvärde** - Anger det kontrastintervall som ska ignoreras när det oskarpa maskfiltret används. Med det här alternativet anger du hur olika de pixlar som ska göras skarpare måste vara från det omgivande området innan de betraktas som kantpixlar och blir skarpare.

Tröskelvärdet använder ett värde mellan 0 och 255, vilket är antalet steg för intensitet i en gråskalebild. 0=svart, 128=50% grått och 255=vitt. Ett tröskelvärde på 12 ignorerar till exempel små variationer i hudtonens ljusstyrka, så att inte brus läggs till, medan kantkontrasten läggs till i kontrastrika områden, till exempel där ögonfransarna möter huden.

Anta till exempel att du har ett foto på någons ansikte. Oskarp mask påverkar de delar av bilden som har mest kontrast och utjämnad hud. Även den jämnaste huden uppvisar subtila förändringar i intensitetsvärden. Om du inte använder ett tröskelvärde framhäver filtret dessa små förändringar i hudpixlar, vilket skapar en bruseffekt (troligen inte önskvärd) samtidigt som kontrasten på ögonfransarna ökas, vilket ökar skärpan (troligen önskvärd). För att undvika det här problemet bör du använda ett tröskelvärde som anger för filtret att ignorera pixlar som inte förändrar kontrasten dramatiskt, till exempel mjuk hud. För att undvika brus eller färgreducering av bilder med hudtoner kan du till exempel experimentera med **[!UICONTROL Threshold]** värden två till 20. Standardvärdet **[!UICONTROL Threshold]** värdet 0 gör alla pixlar i bilden skarpare.

* **Använd på** - Välj **[!UICONTROL Each Color]** om du vill använda skärpa separat för varje färgkomponent, väljer du **[!UICONTROL Brightness]** om du vill använda skärpa i bildernas intensitetsområden.

**Omsampling**

Välj **[!UICONTROL Resampling]** och välj ett alternativ. Dessa alternativ gör bilden skarpare när den nedsamplas:

* **[!UICONTROL None]** - Inaktiverar omsampling.

* **[!UICONTROL Bilinear]** - Den snabbaste omsamplingsmetoden. Vissa aliasing-artefakter är märkbara.

* **[!UICONTROL Bicubic]** - Ökar processoranvändningen på bildservern men ger skarpare bilder med mindre märkbara aliaseringsartefakter.

* **[!UICONTROL `Sharpen2`]** - Ger något skarpare resultat än **[!UICONTROL Bicubic]**, men till ännu högre CPU-kostnader på Image Server.

* **[!UICONTROL Trilinear]** - Använder både högre och lägre upplösningar om sådana finns. Rekommenderas endast när alias är ett problem. Den här metoden minskar storleken på JPEG på grund av reducerade högfrekventa data.

**Förinställningar för skärpa och bilder**

Du kan använda alla tre skärpeeffekterna för att uppnå det slutliga resultatet. Den här metoden rekommenderas dock inte. Adobe Dynamic Media Classic rekommenderar att du sparar dina skärpeeffekter som en del av en bildförinställning. Med bildförinställningar kan du paketera de vanligaste bildmodifieringarna för att skapa en dynamiskt storleksändrad bild i en liten textsträng. En bildförinställning innehåller värden för filformatet (vanligtvis JPEG för webben), pixelantal och bildskärpa. I stället för att lägga till URL:en med varje bildmodifierare som du måste använda för att skapa en viss typ av bildstorlek skapar du en namngiven bildförinställning, till exempel&quot;miniatyrbild&quot;. Konfigurera sedan miniatyrbildens förinställning med rätt storlek, filformat och skärpealternativ. Anropa bilden med namnet Bildförinställning. Bildförinställningar förkortar den övergripande URL:en. Dessa två URL:er ger samma bild på 350 x 350 JPEG med skärpa:

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

Bildförinställningar kan ändras och uppdateras när som helst. Du ser resultatet av en ändring av en bildförinställning när du har publicerat och efter att cachen för URL:en har rensats.

Om du använder en förinställning för varje bild i en storlekskategori kan alla företagsadministratörer uppdatera definitionen för den förinställningen, publicera om och påverka alla bilder som använder det formatet, utan att ändra någon webbkod. Det bästa sättet är att använda en bildförinställning per unik storlek på webbplatsen. Om du vill lägga till en bildförinställning går du till navigeringsfältet Global **[!UICONTROL Setup]** > **[!UICONTROL Application Settings]** > **[!UICONTROL Image Presets]**. Välj sedan **[!UICONTROL Add]** eller markera **[!UICONTROL Edit]** om du vill ändra en befintlig förinställning. Det enda obligatoriska fältet är namnet på själva förinställningen. Det är dock bäst att ta med en viss nivå av skärpa i varje förinställning.

**JPG-kvalitet**

Alternativen för JPG-kvalitet styr komprimeringsnivån JPG:

* **JPG-kvalitet** - Välj det här alternativet om du vill styra komprimeringsnivåer och krominansnedsampling.

* **Skjutreglage** - Anger komprimeringsnivån JPG. Den här inställningen påverkar både filstorlek och bildkvalitet. Kvalitetsskalan JPG är 1-100.

* **Aktivera nedsampling av JPG krominans** - Eftersom ögat är mindre känsligt för högfrekvent färginformation än högfrekvent luminans delas bildinformationen i JPEG i luminans och färgkomponenter. När en JPEG-bild komprimeras lämnas luminanskomponenten i full upplösning, medan färgkomponenterna nedsamplas genom att medelvärdet av alla pixelgrupper ökas. Nedsampling minskar datavolymen med en halv eller en tredjedel utan att det påverkar den upplevda kvaliteten. Nedsampling kan inte användas för gråskalebilder. Den här tekniken minskar mängden komprimering som är användbar för bilder med hög kontrast (till exempel bilder med överlagrad text).

**Ange skärpealternativ för hela företaget**

Om du inte använder en bildförinställning eller skickar specifika bildserverskärpeprotokoll längs URL-strängen blir bilden inte skarpare när den nedsamplas. Om skärpan inte är tillräckligt hög kan du ange standardvärden för skärpa, och sedan har alla bilder alltid en viss skärpa.

Om du vill ange ditt företags standardalternativ för skärpa går du till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]**. Om du ställer in standardomsamplingsläget till **`Sharp2`** blir bilden alltid skarpare vid nedsampling.

**Lägga till skärpa i visningsförinställningar**

Om du inte lägger till bildmodifieringar för skärpa i förinställningen kan den lilla inledande inläsningsbilden se mjuk ut eftersom den nedsamplas så att den passar i visningsfönstret utan att skärpan ökas.

Med visningsförinställningar (t.ex. bildförinställningar) kan du centralisera flera alternativ till en plats, inklusive val av skal och visningsalternativ (t.ex. en Skriv ut-knapp eller styra hastigheten på zoomanimeringen). Förinställningar för visningsprogram finns i samma avsnitt som Bildförinställningar, under **[!UICONTROL Setup]** > **[!UICONTROL Application Settings]** > **[!UICONTROL Viewer Presets]**.

Se [Förinställningar för visningsprogram](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) utbildningsvideo.

Alternativet Modifierare (Modifierare) finns i avsnittet Core Settings (Grundinställningar) för alla förinställningar för eCatalog, Spin och Custom Zoom Viewer. Genom att lägga till kommandona för URL-skärpa i rutan Modifierare lägger du till skärpa varje gång som visningsprogrammet anropas med den förinställningen.

Använd kommandot `config=` på visningsprogrammets URL. Här är ett exempel på hur du anropar en bilduppsättning (skor) med en visningsförinställning (`FantasticoZoom2022`):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2022`

Förinställningen här gör visningsprogrammet skarpare och ändrar standardskalet.

**Skapa bildspecifika åsidosättningar**

Den sista, och minst rekommenderade, skärpningsmetoden är att skapa skärpeåsidosättningar bild för bild. Den här metoden åsidosätter skärpan i en bildförinställning med egna specifika värden. Den här metoden åsidosätter emellertid även alla andra skärpemetoder av alla storlekar. Det bästa användningsområdet för den här metoden är om vissa av dina bilder inte har hög upplösning och värdena i Bildförinställningar är för höga för dessa små bilder. I det här fallet kan skärpa per bild behövas.

I Adobe Dynamic Media Classic väljer du en bild, går till detaljvyn (genom att dubbelklicka eller trycka på **[!UICONTROL Detail View]** och välj **[!UICONTROL Sharpen]**. Ändra en parameter och markera sedan **[!UICONTROL Save]**. Den här processen anger för bildservern att de här skärpeparametrarna ska användas i stället för de kommandon som du anropar i URL:en, till exempel en skärpemodifierare eller bildförinställning. Se till att du publicerar för att se att ändringarna börjar gälla.
