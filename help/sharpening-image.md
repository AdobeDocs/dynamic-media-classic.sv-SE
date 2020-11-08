---
title: Öka skärpan i en bild
seo-title: Öka skärpan i en bild
description: 'null'
seo-description: Lär dig hur du ökar skärpan i en bild.
uuid: d86af74a-89c5-4f2b-96ba-f2e7da600bca
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 11cd5362-d90a-4c1e-bfbd-46a65a554409
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '2159'
ht-degree: 0%

---


# Öka skärpan i en bild {#sharpening-an-image}

Skärpa är en bildändringsteknik som används för att göra konturerna i en digital bild mer distinkta. Skärpa ökar kontrasten mellan kantpixlar och framhäver övergången mellan mörka och ljusa områden. Skärpa ökar lokal kontrast och ger detaljskärpa. Det finns ingen strikt formel för att göra alla bilder skarpare. För lite skärpa kan skapa en mjuk bild, men för mycket skärpa ger haloeffekter, artefakter och brus.

Du bör använda bildförinställningar för alla bilder i Dynamic Media Classic. Detta garanterar en enhetlig storlek och skärpa används på alla bilder som kallas för bildförinställningar. Dessutom kan du enkelt redigera och ändra en bildförinställnings skärpeparametrar. Nästa gång du publicerar får alla bilder som anropas med den förinställningen de nya värdena.

Dynamic Media Classic rekommenderar också att du lägger till skärpa i visningsförinställningar och sedan anropar ett visningsprogram med den förinställningen. Detta gör att bilderna i tittarna blir skarpa och tilltalande.

Oavsett om du använder bildförinställningar och visningsförinställningar, eller någon annan metod för att öka skärpan, är den sista raden att du bör göra bilderna skarpare. Om du inte gör det kan dina bilder (och din webbplats) se mjuka och oskarpa ut.

>[!NOTE]
>
>Kommandona Skärpa åsidosätter inställningarna för bildförinställningar, inklusive deras skärpeeffekter. En bildförinställning styr storleken och formateringen som bilder levereras med från dynamiska mediabildsservrar. Dynamic Media Classic rekommenderar starkt att du använder bildförinställningar för att leverera alla bilder, så att du kan vara säker på att bilderna levereras med samma storlek och skärpa. När skärpeinställningarna för en enskild bild har ändrats gäller skärpeinställningarna inte längre för bilden. Den levereras utan skärpeinställningar för bildförinställningar.

Det är ofta nödvändigt att göra bilder skarpare. Dynamic Media Classic och Image Servers erbjuder flera skärpealternativ. Det är viktigt att du förstår vad skärpa gör i en bild och hur mycket skärpa du behöver. De flesta bilder behöver skärpa, men mängden som krävs beror på bilden.

Bildskärpa ökar pixlarnas kontrast för att skapa effekten av framhävda kanter. Människan uppfattar den här förbättrade kantkontrasten som skärpa. Det är enkelt att förbättra en bild genom att köra skärpefilter på en bild, men det är också enkelt att öka skärpan i en bild för mycket.

Om du ökar skärpan i en bild för mycket skapas en ljusgårdseffekt, eller ränder från kantens linjer.

Det finns god praxis som du kan följa för att optimera skärpan i dina bilder i Dynamic Media Classic och på Dynamic Media Image Server.

Mer information finns i [Bästa tillvägagångssätt för att öka skärpan i bilder i Dynamic Media Classic och på Dynamic Media Image Server](/help/assets/s7_sharpening_images.pdf).

**Göra en bild skarpare**

Om du vill öka skärpan i en bild klickar du på **knappen Redigera** överrullning och väljer Skärpa, eller öppnar den i panelen Bläddra i detaljvyn och klickar sedan på **Skärpa**. Skärmen för skärperedigeraren öppnas med skärpekommandon. Välj kommandon och klicka på **Spara**.

>[!NOTE]
>
>Innan du gör en bild skarpare kan du välja menyn Använd förinställning och välja en bildförinställning för att se vilka skärpeeffekter den har. Skärpeeffekterna i en bildförinställning kan vara lämpliga för din bild. Menyn Använd förinställning finns längst ned i skärperedigeraren.

**Skärpealternativ**

I följande tabell visas skärpealternativen för bildservern.

| Namn | URL-protokoll | Värden | Exempel |
|--- |--- |--- |--- |
| Enkel skärpa | op_sharpen | `0 | 1` | op_sharpen=1 |
| Sampla om läge | resMode | `bilin | bicub | sharp2 | trilin`<br><br>bilin: Väljer bilinjär standardinterpolation. Snabbaste omsamplingsmetod. vissa aliaseringsartefakter kan bli märkbara.<br>bikub: Väljer bikubisk interpolation. Processorintensivare än bilin, men ger skarpare bilder med mindre märkbara aliasfelaktigheter.<br><br>sharp2: Väljer en modifierad Lanczos Window-funktion som en interpoleringsalgoritm. Kan ge något tydligare resultat än bikubisk till en högre CPU-kostnad.<br><br>trilin: Väljer en ändrad trilinjär interpolation, som använder både högre och lägre upplösningar, om sådana finns. Rekommenderas endast när alias är ett problem. Minskar JPEG-storlekar på grund av reducerade högfrekventa data. | resMode=sharp2 |
| Oskarp mask | op_usm | mängd, radie, tröskelvärde,<br><br>monokromeamount: filterstyrkefaktor (verklig 0...5)<br><br>radie: filtrera kernelradien i pixlar (verklig 0...250) <br><br>tröskelvärde: filtertröskelnivå (int 0...255)<br><br>monokrom: ange 0 för att oskarp maskera varje färgkomponent separat, ange 1 till oskarp maskbildintensitet (intensitet) | op_usm=1,1,10,0 |

Välj menyn Skärpa och välj ett alternativ:

**Ingen** Inaktiverar skärpa.

**Skärpa** Kör ett enkelt skärpesteg på filen när den har ändrat storlek. Detta liknar &quot;Skärpa&quot;-filtret i Photoshop och stöder alla användarparametrar. Normalt använder du det här filtret eller Oskarp mask, men inte båda. Det är en god praxis att inte rekommendera den här metoden, men den kan kompensera för oskärpa. (URL: op_sharpen)

**Med Oskarp mask** kan du finjustera en skärpefiltereffekt på den slutliga nedsamplade bilden. Du kan styra effektens intensitet, radie (mätt i pixlar) och ett kontrasttröskelvärde som ska ignoreras. Effekten har samma alternativ som filtret Oskarp mask i Photoshop. (URL: op_usm)

Välj följande alternativ för att finjustera skärpan med Oskarp mask:

**Mängd** Styr mängden kontrast som används på kantpixlar. Standardvärdet är 0,0. För högupplösta bilder kan du öka den till upp till 5.0. Tänk på Mängd som ett mått på filterintensiteten. Tänk på att inställningen Mängd i Dynamic Media Classic inte är densamma som inställningen Mängd i Photoshop. Photoshop använder en mängd mellan 1 % och 500 %, medan Dynamic Media Classic skalar från 0,0 till 5,0. (5.0 motsvarar ungefär 500 % i Photoshop, 0,9 motsvarar 90 % och så vidare.)

**Radie** Anger antalet pixlar runt kantpixlarna som påverkar skärpan. Effekten körs på alla pixlar i bilden och strålar ut i alla riktningar.

Det bästa radievärdet beror på bildens storlek. Med ett lågt värde ökas skärpan endast för kantpixlarna. Med ett högt värde ökas skärpan för ett större antal pixlar.

Om du till exempel vill få en liknande skärpeeffekt för en bild på 2 000 x 2 000 pixlar och en bild på 500 x 500 pixlar kan du ange radievärdet två pixlar för bilden på 2 000 x 2 000 pixlar. Ange sedan radien 1 pixel i bilden med 500 x 500 pixlar (ett större värde för en bild med fler pixlar).

**Tröskelvärde** bestämmer vilket kontrastintervall som ska ignoreras när filtret för oskarp mask används. Med det här alternativet anger du hur olika de pixlar som ska göras skarpare måste vara från det omgivande området innan de betraktas som kantpixlar och blir skarpare.

Tröskelvärdet använder ett värde mellan 0 och 255, vilket är antalet steg för intensitet i en gråskalebild. 0=svart, 128=50% grått och 255=vitt. Ett tröskelvärde på 12 ignorerar till exempel små variationer i hudtonens ljusstyrka, så att inte brus läggs till, medan kantkontrasten läggs till i kontrastrika områden, till exempel där ögonfransarna möter huden.

Anta att du har ett foto på någons ansikte. Oskarp mask påverkar de delar av bilden som har mest kontrast och utjämnad hud. Även den jämnaste huden uppvisar subtila förändringar i intensitetsvärden. Om du inte använder ett tröskelvärde framhäver filtret dessa små förändringar i hudpixlar, vilket skapar en bruseffekt (troligen inte önskvärd) samtidigt som kontrasten på ögonfransarna ökas, vilket ökar skärpan (troligen önskvärd). För att undvika det här problemet bör du använda ett tröskelvärde som anger för filtret att ignorera pixlar som inte förändrar kontrasten dramatiskt, till exempel mjuk hud. Om du vill undvika brus eller färgreduktion - i bilder med hudtoner till exempel - kan du experimentera med tröskelvärden mellan 2 och 20. Med standardvärdet 0 för Tröskelvärde ökas skärpan för alla pixlar i bilden.

**Använd för** att välja varje färg om du vill använda skärpa separat på varje färgkomponent, Välj Intensitet om du vill använda skärpa i bildernas intensitetsområden.

**Omsampling**

Välj menyn Omsampling och välj ett alternativ. Dessa alternativ gör bilden skarpare när den nedsamplas:

**Ingen** inaktiverar omsampling.

**Bilinjär** den snabbaste omsamplingsmetoden. vissa aliaseringsartefakter är märkbara.

**Bikubisk** ökar processoranvändningen på bildservern men ger skarpare bilder med mindre framträdande aliasartefakter.

**Skärpa2** kan ge något skarpare resultat än bikubisk, men till ännu högre processorkostnad på bildservern.

**Trilinjär** använder både högre och lägre upplösningar om sådana finns. rekommenderas bara när alias är ett problem. Den här metoden minskar JPEG-storleken på grund av reducerade högfrekventa data.

**Förinställningar för skärpa och bilder**

Du kan blanda alla tre skärpeeffekterna för att uppnå det slutliga resultatet. Detta rekommenderas dock inte. Dynamic Media Classic rekommenderar att du sparar dina skärpeeffekter som en del av en bildförinställning.Med bildförinställningar kan du paketera de vanligaste bildmodifieringarna för att skapa en bild med dynamiskt storlek i en liten textsträng. En bildförinställning innehåller värden för filformatet (vanligtvis JPEG för webben), pixelantal och bildskärpa. I stället för att lägga till URL:en med varje bildmodifierare som behövs för att skapa en viss typ av bildstorlek, skapar du en namngiven bildförinställning, till exempel&quot;miniatyrbild&quot;, konfigurerar miniatyrbildens förinställning med rätt storlek, filformat och skärpealternativ och anropar sedan bilden med namnet Bildförinställning. Bildförinställningar förkortar den övergripande URL:en.Dessa två URL:er ger samma 350 x 350 JPEG-bild med skärpa:

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

Bildförinställningar kan ändras och uppdateras när som helst. Du ser resultatet av en ändring av en bildförinställning när du har publicerat och när cachen för URL:en har rensats.

Om du använder en förinställning för varje bild i en storlekskategori kan alla företagsadministratörer uppdatera definitionen för den förinställningen, publicera om och påverka alla bilder som använder det formatet, utan att ändra någon webbkod. Det bästa sättet är att använda en bildförinställning per unik storlek på webbplatsen. Om du vill lägga till en bildförinställning går du till Inställningar > Programinställningar > Bildförinställningar. Sedan lägger du till eller redigerar en befintlig förinställning. Det enda obligatoriska fältet är namnet på själva förinställningen. Du bör emellertid inkludera en viss nivå av skärpa i alla förinställningar.

**JPG-kvalitet**

Alternativen för JPG-kvalitet styr JPG-komprimeringsnivån:

**JPG-kvalitet** Välj det här alternativet om du vill styra komprimeringsnivåer och krominansnedsampling.

**Slider** avgör JPG-komprimeringsnivån. Den här inställningen påverkar både filstorlek och bildkvalitet. JPG-kvalitetsskalan är 1-100.

**Aktivera JPG-krominansnedsampling** Eftersom ögat är mindre känsligt för högfrekvent färginformation än högfrekvent luminans delas bildinformationen upp i JPEG-bilder i luminans och färgkomponenter. När en JPEG-bild komprimeras lämnas luminanskomponenten i full upplösning, medan färgkomponenterna nedsamplas genom att medelvärdet av grupper av pixlar ökas. Nedsampling minskar datavolymen med en halv eller en tredjedel utan att det påverkar den upplevda kvaliteten. Nedsampling kan inte användas för gråskalebilder. Den här tekniken minskar mängden komprimering som är användbar för bilder med hög kontrast (till exempel bilder med överlagrad text).

**Ställa in skärpealternativ för hela företaget**

Om du inte använder en bildförinställning eller skickar specifika bildserverskärpeprotokoll längs URL-strängen blir bilden inte skarpare när den nedsamplas. Om detta inträffar kan du dock ange standardvärden för skärpa, och då får alla bilder alltid viss skärpa.

Om du vill ange företagets standardalternativ för skärpa går du till Inställningar > Programinställningar > Publiceringsinställningar > Bildserver. Om du ställer in standardomsamplingsläget till Sharp2 kommer skärpan alltid att öka vid nedsampling.

**Lägga till skärpa i visningsförinställningar**

Om du inte lägger till bildmodifieringar för skärpa i förinställningen kan den lilla inledande inläsningsbilden se mjuk ut eftersom den nedsamplas så att den passar i visningsfönstret utan att skärpan ökas.

I Dynamic Media Classic kan du använda visningsförinställningar (som bildförinställningar) för att centralisera många alternativ till en plats, inklusive val av skal och visningsalternativ (som att inkludera en Skriv ut-knapp eller styra hastigheten på zoomanimeringen). Förinställningar för visningsprogram finns i samma avsnitt som Bildförinställningar, under Konfigurera > Programinställningar > Visningsförinställningar.

Alternativet Modifierare (Modifierare) finns i avsnittet Core Settings (Grundinställningar) för alla förinställningar för eCatalog, Spin och Custom Zoom Viewer. Genom att lägga till kommandona för URL-skärpa i rutan Modifierare lägger du till skärpa varje gång som visningsprogrammet anropas med den förinställningen.

Om du vill anropa visningsförinställningen använder du kommandot config= på visningsprogrammets URL. Här är ett exempel på hur du anropar en bilduppsättning (skor) med en visningsförinställning (FantasticoZoom2009):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2009`

Förinställningen här gör visningsprogrammet skarpare och ändrar standardskalet.

**Skapa bildspecifika åsidosättningar**

Den sista, och minst rekommenderade, skärpningsmetoden är att skapa skärpeåsidosättningar bild för bild. Detta åsidosätter skärpan i en bildförinställning med egna värden. Detta åsidosätter dock alla andra skärpemetoder oavsett storlek. Det bästa användningsområdet för den här metoden är om vissa av dina bilder inte har hög upplösning och värdena i Bildförinställningar är för höga för dessa små bilder. I det här fallet kan en viss skärpa per bild behövas.

I Dynamic Media Classic markerar du en bild, går till detaljvyn (genom att dubbelklicka eller trycka på knappen Detaljvy) och klickar på Skärpa. Ändra en parameter och klicka sedan på Spara. Detta anger för bildservern att de här skärpeparametrarna ska användas i stället för de kommandon som du anropar i URL:en, till exempel en skärpemodifierare eller bildförinställning. Du måste publicera för att se ändringarna börja gälla.
