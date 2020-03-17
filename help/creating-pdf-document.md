---
title: Skapa ett PDF-dokument
seo-title: Skapa ett PDF-dokument
description: 'null'
seo-description: Lär dig hur du skapar ett PDF-dokument med hjälp av processen Web-to-Print i Dynamic Media Classic.
uuid: 274fb06b-320b-40fa-8b61-c224d8aceaa1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: 87e91e8e-10a2-4fba-87c7-aad2bd798146
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Skapa ett PDF-dokument {#creating-a-pdf-document}

Det sista steget i processen för webb-till-utskrift är att generera en anpassad PDF. När slutanvändarna har anpassat mallen med webbprogrammet som du skapade, skapar de ett slutligt PDF-dokument. Den slutliga PDF-filen skickas vanligtvis till en tryckleverantör för professionell utskrift. För att vara säker på att den slutliga PDF-filen skrivs ut som förväntat använder utvecklarna rätt joboptions-fil och ställer in teckensnitt, skrivarmärken och färger på rätt sätt.

## Konfigurera PDF-förinställningar {#setting-up-pdf-presets}

Ange PDF-kompatibilitetsnivå och skrivarinställningar genom att skapa och överföra en PDF-joboptions-fil till Dynamic Media Classic Server. Du kan t.ex. välja PDF/X-4-kompatibla PDF-utdata (rekommenderas för PDF-tryckpubliceringsarbetsflöden). Du kan skapa joboptions-filen i redigeringsprogrammet (till exempel Adobe Illustrator) eller i Acrobat. Kontrollera alltid med skrivaren, som kan ge dig råd om lämpliga jobbalternativ för utskriftsjobbet.

Mer information om hur du skapar joboptions-filer och hur du skapar joboptions-filer i Acrobat finns i hjälpen för Adobe Acrobat.

Så här skapar du en joboptions-fil i Illustrator:

1. Välj Redigera > Adobe PDF-förinställningar.
1. Välj den förinställning som du vill använda i dialogrutan.

   Följande jobbalternativsinställningar stöds av Dynamic Media Classic:

   | Jobbalternativ | Beskrivning |
   |--- |--- |
   | Allmänt | <ul><li>Kompatibilitet </li><li>Objektnivåkomprimering</li><li>Bädda in miniatyrer</li><li>Optimera för snabb webbvisning</li></ul> |
   | Bilder | <ul><li>Nedsampla</li><li>Upplösning</li><li>Tröskelvärde</li><li>Komprimering för färg, grått och mono</li></ul> |
   | Teckensnitt | <ul><li>Bädda in alla teckensnitt (teckensnitt bäddas in som standard)</li><li>Bädda in OpenType-teckensnitt</li><li>Skapa delmängder av inbäddade teckensnitt när andelen tecken som används är mindre än:</li><li>Inkludera alltid lista</li><li>Inkludera aldrig lista</li></ul> |
   | Färg | <ul><li>Färgstrategi (tagga endast bilder behandlas som tagga allt)</li><li>Dokumentåtergivningsmetod</li><li>Endast följande arbetsfärgrymder stöds i 4.2.5. 4.3 kommer att göra det möjligt att använda alla kundprofiler som har överförts till IPS.</li><li>Som en tillfällig lösning kan du ange målfärgrymden för teckningen som ska konverteras till med hjälp av företagets standardfärgprofiler.</li></ul> |
   | RGB | <ul><li>e-sRGB </li><li>scRGB med kodningsintervall [-4.0, 4.0]</li><li>Lab D50</li><li>PCS XYZ</li><li>Platt XYZ</li><li>Linjär ROMM-RGB</li><li>ROMM-RGB</li><li>sYCC 8-bitars</li><li>e-YCC 8-bitars</li></ul> |
   | Grå | <ul><li>Grå gamma 1.8</li><li>Grå gamma 2.2</li><li>Punktförstoring 10 %</li><li>Punktförstoring 15 %</li><li>Punktförstoring 20 %</li><li>Punktförstoring 25 %</li><li>Punktförstoring 30 %</li><li>sGray</li></ul> |
   | Bevara CMYK-värden för kalibrerade CMYK-färgmodeller |  |
   | Avancerat | Bevara OPI-kommentarer är alltid aktiverat |
   | Standarder | Kompatibilitetsstandard |

   >[!NOTE]
   >
   >Dynamic Media Classic ignorerar skrivarmärkesinställningarna i joboptions-filen. Skrivarmärken konfigureras i stället med hjälp av Dynamic Media Classic URL-kommandon.

1. Klicka på Exportera, ange ett namn och en plats och klicka på Spara.
1. Överför jobbalternativfilen som en resurs till Scene7 Publishing System.

   Använd den med din publicerade mall genom att referera till den i webbadressen. Exempel:

   `https://yourpublishserver.scene7.com/is/agm/SiliconPublishing/PetNews?&fmt=pdf,cmyk&joboption=SPSfilenameid`

## Förbereda PDF-filen för utskrift {#preparing-the-pdf-for-print}

Innan du slutför PDF-filen för utskrift måste du följa riktlinjerna i det här avsnittet.

**Bilder**

Kontrollera att alla bilder i publiceringsjobbet har överförts till din Dynamic Media Classic Server och publicerats.

**Teckensnitt**

Kontrollera att alla teckensnitt i publiceringsjobbet har överförts till din Dynamic Media Classic Server och publicerats. Se till att du har laglig rätt att lagra teckensnitten om du tänker tillåta slutanvändarna att ändra dem.

**Bildupplösning (pixlar per tum)**

Bitmappsbildernas upplösning bevaras av Dynamic Media Classic-servern i genererade utskriftsklara PDF-filer. Med Dynamic Media Classic skalas bildupplösningen vid behov upp. För att resultatet ska bli optimalt låter du upplösningen vara standardvärdet (vanligtvis 72 dpi) när du förhandsgranskar på webben. Standardupplösningen för alla bilder i företaget anges i fönstret Publiceringsinställningar/Bildserver i avsnittet Standardutskriftsupplösning. Högre upplösningar (t.ex. 300 dpi) kan ge längre bearbetningstid och bör bara användas för en utskriftsklar PDF-fil. Använd kommandot imageRes= i URL:en för att manuellt åsidosätta standardupplösningen för PDF-jobb.

**Färghantering**

I dokument och bilder kan du använda gråskale-, CMYK-, namngivna dekorfärger, RGB- eller Lab-färgmodeller. Var och en kan antingen vara okalibrerad eller kalibrerad med en ICC-färgprofil. För bästa resultat bör du bädda in profilen i den genererade utskriftsklara PDF-filen. Dynamic Media Classic Server gör detta som standard. Kontrollera att alla färgprofiler som krävs har överförts till Dynamic Media Classic-plattformen. Kontrollera helst att färghanteringsalternativen som angetts i designprogrammet matchar dem som angetts i Dynamic Media Classic Server:

* **Inställningar för färghantering för designprogram:** I Färginställningar för redigeringsprogrammet (till exempel Adobe Illustrator) anger du RGB- och CMYK-färgprofilerna i avsnittet Arbetsytor.

* **Inställningar för Dynamic Media Classic-färghantering:** Normalt bör färghanteringsinställningarna i designprogrammet matcha standardfärgprofilerna på Dynamic Media Classic-servern. Du hittar de här inställningarna i fönstret Publiceringsinställningar/Bildserver.

## Visa skrivarmärken {#displaying-printer-marks}

Du kan skapa en PDF-fil för något av följande:

* Ett färdigt dokument
* Ett mellanliggande dokument, t.ex. en film eller plåt, som kan skickas till en skrivare för produktion

Ett mellanliggande dokument kan innehålla ytterligare produktionsinnehåll, t.ex. utfallsmarginaler, skrivarmärken osv. Det här innehållet visas vanligtvis utanför den färdiga sidans gränser.

Alla märken som finns på skärmen&quot;Lägg till skrivarmärken&quot; i Acrobat stöds. Skrivarmärkena styrs av `printerMark` parametern. Syntaxen är `&printerMark=trim marks, bleed marks, registration marks, color bars, page information, style, line weight, layer embed`.

* ytmärken = 0|1
* utfallsmärken = 0|1
* passmärken = 0|1
* färgfält = 0|1
* sidinformation = 0|1
* style = Illustrator| IllustratorJ| QuarkXPress
* linjevikt = 0,125| 0,25| 0,50
* inbäddning av lager = 0|1

När du förbereder ett dokument för tryckproduktion kan det behövas skrivarmärken för att hjälpa tryckeriet att justera separationsfilmer för att producera korrektur, mäta film för korrekt kalibrering och tryckfärgsdensitet, rensa film till storlek och så vidare. Skrivarmärken anger gränserna för dokumentrutor som TrimBox och BleedBox. Produktionsrelaterat innehåll kan vara:

* **Media box** The boundaries of the physical medium on which the page will be printed. Innehåll utanför medierutan kan tas bort utan att det påverkar filens betydelse.

* **BleedBox** Det område där sidans innehåll klipps ut när det skrivs ut i en produktionsmiljö. BleedBox kan innehålla områden som är nödvändiga för de fysiska begränsningarna av skärnings-, viknings- och beskärningsutrustning. Standardvärdet är sidans beskärningsruta.

* **TrimBox** Den färdiga sidans avsedda mått efter beskärning. TrimBox kan vara mindre än MediaBox för att tillåta produktionsrelaterat innehåll, t.ex. utskriftsinstruktioner, skärmärken och färgremsor. Standardvärdet är sidans beskärningsruta.

* **Art box** Omfattningen av sidans meningsfulla innehåll (inklusive potentiell blanktecken) enligt vad sidans skapare har tänkt sig. Standardvärdet är sidans beskärningsruta.

Du kan använda modifieringarna som visas i den här tabellen för att återge skrivarmärkena som finns i Adobe Illustrator, InDesign och Acrobat:

| Modifierare/värden | Beskrivning |
|--- |--- |
| bleedMargin=top,left,bottom,right | Anges i Acrobat med alternativet Ange sidrutor. Välj BleedBox och ange sedan marginaler med alternativet Marginalreglage.<br><br>Värden representerar avståndet mellan den övre, vänstra, nedre och högra kanten och teckningens ursprungliga kanter (medierutan) och inåt. Värdena (0-1 000) anges i punkter.<br><br>New height=original height - (top+bottom)<br><br>New width= original width - (left+right) |
| mediaMargin=top,left,bottom,right | Anges i Acrobat med alternativet Ange sidrutor. Ändra anpassad sidstorlek under alternativet Ändra sidstorlek.<br><br>Värden representerar avståndet mellan de övre, vänstra, nedre och högra kanterna och teckningens ursprungliga kanter (medierutan) och utåt. Värdena (0-1 000) anges i punkter.<br><br>Ny höjd=top+bottom+original<br><br>heightNy bredd=top+bottom+original<br><br>widthDe nya värdena för höjd och bredd bestämmer den nya sidstorleken för den genererade PDF-filen.<br><br>När en ny Media Box har definierats måste alla beräkningar av trimningsmarginal och utfallsmarginal betraktas som den nya Media Box som kanten på teckningen. |
| trimMargin=top,left,bottom,right | Anges i Acrobat med alternativet Ange sidrutor. Välj TrimBox och ange sedan marginaler med alternativet Marginalreglage.<br><br>Värden representerar avståndet mellan den övre, vänstra, nedre och högra kanten och teckningens ursprungliga kanter (medierutan) och inåt. Värdena (0-1 000) anges i punkter.<br><br>New height=original height - (top+bottom)<br><br>New width=original width - (left+right) |
| printerMark= ytmärken, utfallsmärken, passmärken, färgfält, sidinformation, format, linjebredd, inbäddning av lager | Värdena är följande:<br><br>ytmärken = 0,1 (standard är 0)<br><br>utfallsmärken = 0,1 (standard är 0)<br><br>passmärken = 0,1 (standard är 0)<br><br>färgfält = 0,1 (standard är 0)<br><br>sidinformation = 0,1 (standard är 0)<br><br>format = standard, InDesignJ1, InDesignJ2, Illustrator, illustrator J, QuarkXPress (standard är Standard)<br><br>linjebredd= 0.125-0.2, båda värdena är inkluderade (standard är 0.25)<br><br>lagerinbäddning = 0, 1, där 1 skapar ett nytt lager som innehåller alla skrivarmärken (standard är 1)<br><br>Beroende på vilken stil som används visas märkena och färgfälten annorlunda och matchar de motsvarande format som används i Acrobat. |

Observera följande om skrivarmärken:

* Ange utfallsmarginaler, ytmarginaler och mediemarginaler via URL-anrop när du anger skrivarmärken. Om du anger skrivarmärken utan att ange dessa marginaler, kommer dessa märken att visas utanför det synliga området i den genererade PDF-filen. Ytmärkena och utfallsmärken överlappar varandra.
* Om du anger samma marginalvärden för trimningsmarginalen och utfallsmarginalen överlappas ytmärken och utfallsmärken när båda dessa flaggor är 1 tum `&printerMark`.
* Om du anger fmt=swf/image-format via URL-anrop skapas utdata utan skrivarmärken eller marginaler eftersom den här funktionen är specifik för PDF-utdata.
* Om du anger `&printerMark=`via URL:en används standardvärden för alla parametrar. Om du anger `&printerMark=1` blir ytmärkena inställda på 1 och standardvärdena för andra parametrar. Men om du vill ställa in det n:te elementet på ON måste alla (n-1) parametrar anges via URL.
* Om du bara anger ett värde för `&trimMargin`, `&bleedMargin`och `&mediaMargin` används det värdet på alla övre, nedre, vänstra och högra marginaler i den ursprungliga teckningen.
* Om du bara anger värdena top och left through `&trimMargin`, `&bleedMargin`och `&mediaMargin` tilldelas det översta värdet till det nedersta värdet och det vänstra värdet till höger.
* Om du inte anger det högra värdet via `&trimMargin`, `&bleedMargin`och `&mediaMargin` blir det vänstra värdet tilldelat till höger.
* För en flersidig PDF-fil används skrivarmärken/marginaler på alla sidor (i Acrobat kan användarna välja sidintervall för skrivarmärken/marginaler).
* Utdata från en PDF-fil med skrivarmärken/marginaler aktiverade matchar exakt med Acrobat X om inget annat anges.

Om du vill skapa en PDF/X-4-kompatibel PDF-fil via modifieraren i &amp;joboption i URL:en, bör du vara medveten om de begränsningar som gäller skrivarmärken som anges i PDF ISO_15930-7-2008.pdf:

* Varje sidobjekt i en PDF-fil innehåller en MediaBox. Varje sidobjekt i en fil som överensstämmer med PDF/X-4 ska innehålla en TrimBox eller en ArtBox, men inte båda. MediaBox kan inkluderas genom arv.
* Om BleedBox finns får ArtBox eller TrimBox inte sträcka sig utanför gränserna för BleedBox. Om CropBox finns tillgänglig får ingen av ArtBox, TrimBox eller BleedBox sträcka sig utanför gränserna för CropBox.
* Ingen av ArtBox, TrimBox, CropBox eller BleedBox får sträcka sig utanför MediaBox gränser.
* Vissa branschmetoder kräver att BleedBox används. Lämpliga handelspraxis bör följas.
* Du bör använda TrimBox framför ArtBox.
* Alla anteckningar utom TrapNet- och PrinterMark-anteckningar ska ha ett värde för Rect som ligger helt utanför BleedBox (eller TrimBox eller ArtBox om det inte finns någon BleedBox). Alla PrinterMark-anteckningar ska ha ett värde för Rect som ligger helt utanför TrimBox eller ArtBox. En PDF/X-4-kompatibel läsare kan helt ignorera anteckningar förutom PDF TrapNet-anteckningar.
* En Rect ska anses vara helt utanför en begränsningsram om alla Rect-koordinater antingen ligger utanför begränsningsramen eller på dess kant och skärningspunkten för de två rektanglarna är noll.
* Om ViewerPreferences-ordlistan innehåller tangenterna ViewArea, ViewClip, PrintArea eller PrintClip, ska var och en av dessa tangenter ha värdet MediaBox eller (om det finns en BleedBox i alla sidobjekt i filen) BleedBox.

