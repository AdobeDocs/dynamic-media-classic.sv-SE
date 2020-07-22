---
title: Bästa tillvägagångssätt för att optimera bildkvaliteten
seo-title: Bästa tillvägagångssätt för att optimera bildkvaliteten
description: 'null'
seo-description: Lär dig de bästa sätten att optimera bildkvaliteten.
uuid: 102e83fe-ee2a-443b-ba92-6ad5cc3daef0
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 8164466e-2520-482a-88ec-6191fdc77ea3
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '1527'
ht-degree: 3%

---


# Bästa tillvägagångssätt för att optimera bildkvaliteten{#best-practices-for-optimizing-the-quality-of-your-images}

Att optimera bildkvaliteten kan vara en tidskrävande process eftersom många faktorer bidrar till att återge godtagbara resultat. Resultatet är delvis subjektivt eftersom individer upplever olika bildkvalitet. Strukturerade experiment är avgörande.

Dynamic Media Classic innehåller mer än 100 bildspelskommandon för att justera och optimera bilder och återge resultat. Följande riktlinjer kan hjälpa dig att effektivisera processen och uppnå goda resultat snabbt med några viktiga kommandon och bästa metoder.

Se även [Smart bildbehandling](https://helpx.adobe.com/experience-manager/6-3/assets/using/imaging-faq.html).

## Bästa tillvägagångssätt för bildformat (&amp;fmt=) {#best-practices-for-image-format-fmt}

* JPG eller PNG är de bästa alternativen för att leverera bilder med god kvalitet och hanterbar storlek och vikt.
* Om inget formatkommando anges i URL:en används som standard JPG för leverans i Dynamic Media Image Serving.
* JPG komprimeras med förhållandet 10:1 och ger vanligtvis mindre bildfilsstorlekar. PNG komprimeras med ett förhållande på cirka 2:1, utom i vissa fall, till exempel när bilder innehåller en tom bakgrund. Vanligtvis är PNG-filernas storlek större än JPG-filer.
* JPG använder förstörande komprimering, vilket innebär att bildelement (pixlar) tas bort under komprimeringen. PNG använder däremot förlustfri komprimering.
* JPG komprimerar ofta fotografiska bilder med bättre återgivning än syntetiska bilder med skarpa kanter och kontrast.
* Om dina bilder innehåller genomskinlighet kan du använda PNG eftersom JPG inte har stöd för genomskinlighet.

Ett tips för bildformat är att börja med den vanligaste inställningen `&fmt=JPG`.

## Bästa tillvägagångssätt för bildstorlek {#best-practices-for-image-size}

Att minska bildstorleken dynamiskt är en av de vanligaste åtgärderna som utförs i Dynamic Media Image Serving. Det handlar om att ange storleken och, om så önskas, vilket nedsamplingsläge som används för att nedskala bilden.

* För storleksändring av bilder är det bästa och enklaste sättet att använda `&wid=<value>` och `&hei=<value>` eller bara `&hei=<value>`. Dessa parametrar ställer automatiskt in bildbredden i enlighet med proportionerna.
* `&resMode=<value>` styr den algoritm som används för nedsampling. Börja med `&resMode=sharp2`. Det här värdet ger den bästa bildkvaliteten. Nedsamplingsvärdet `=bilin` är snabbare, men resulterar ofta i alias av artefakter.

Det bästa sättet att ändra storlek på bilder är att använda `&wid=<value>&hei=<value>&resMode=sharp2` eller `&hei=<value>&resMode=sharp2`

## Bästa tillvägagångssätt för bildskärpa {#best-practices-for-image-sharpening}

Bildskärpa är den mest komplicerade aspekten när det gäller att styra bilder på webbplatsen och var många misstag görs. Ta dig tid att lära dig mer om hur skärpa och oskarp maskning fungerar i Dynamic Media Classic med hjälp av följande resurser:

Best practices white paper [Sharpening images in Adobe Dynamic Media Classic and on Image Server](/help/assets/s7_sharpening_images.pdf).

Se även [Öka skärpan i en bild med oskarp mask](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html).

Med Dynamic Media Classic kan du öka skärpan i bilder vid intag, vid leverans eller både och. I de flesta fall bör du emellertid skärpa upp bilder med endast en metod eller med en annan, men inte med båda metoderna. Att skärpa bilderna vid leverans, på en URL-adress, ger oftast bäst resultat.

Det finns två metoder för bildskärpa:

* Enkel skärpa ( `&op_sharpen`) - Precis som skärpefiltret som används i Photoshop, tillämpar enkel skärpa grundläggande skärpa på den slutliga vyn av bilden efter den dynamiska storleksändringen. Den här metoden kan dock inte konfigureras av användaren. Det bästa sättet är att inte använda produkten `&op_sharpen` om det inte är nödvändigt.
* Oskarp maskering ( `&op_USM`) - Oskarp maskning är ett skärpefilter som är branschstandard. Det bästa sättet är att göra bilder skarpare med oskarp maskering enligt riktlinjerna nedan. Med Oskarp maskning kan du styra följande tre parametrar:

   * `&op_sharpen=amount,radius,threshold`

      * `amount` (0-5, effektens styrka.)
      * `radius` (0-250, bredden på de&quot;skärpelinjer&quot; som ritas runt objektet med skärpa, mätt i pixlar.)

         Kom ihåg att parametrarna `radius` och `amount` arbetet står i motsatsförhållande till varandra. Minskningen `radius` kan kompenseras genom ökning `amount`. `Radius` ger bättre kontroll när ett lägre värde gör endast kantpixlarna skarpare, medan ett högre värde ökar skärpan för ett större antal pixlar.

      * `threshold` (0-255, effektkänslighet.)

         Den här parametern avgör hur annorlunda de pixlar som ska göras skarpare måste vara jämfört med det omgivande området innan de betraktas som kantpixlar och filtret gör dem skarpare. Tröskelvärdet hjälper dig att undvika att göra områden med liknande färger, som hudtoner, för skarpare. Ett tröskelvärde på 12 ignorerar till exempel små variationer i hudtonens ljusstyrka för att undvika att lägga till ”brus”, men lägger ändå till kantkontrast i områden med hög kontrast, till exempel där ögonfransarna möter huden.
      Mer information om hur du ställer in de här tre parametrarna, inklusive de bästa sätten att använda med filtret, finns i följande resurser:

      Hjälpavsnittet för Dynamic Media Classic om [skärpa i en bild](https://help.adobe.com/en_US/scene7/using/WS389B162D-2981-41e5-9253-15D22D2ECBC8.html).

      Best practices white paper [Sharpening images in Adobe Scene7 Publishing System and on Image Server](/help/assets/s7_sharpening_images.pdf).

   * I Dynamic Media Classic kan du även styra en fjärde parameter: monokrom ( `0,1`). Den här parametern avgör om oskarp maskering används separat på varje färgkomponent med hjälp av värdet `0` eller bildens intensitet/intensitet med hjälp av värdet `1`.


Det bästa sättet är att börja med parametern oskarp maskradie. Radie-inställningar som du kan börja med är följande:

* Webbplats: 0,2-0,3 pixlar
* Fotografisk utskrift (250-300 ppi): 0,3-0,5 pixlar
* Offsettryck (266-300 ppi): 0,7-1,0 pixlar
* Arbetsyteutskrift (150 ppi): 1,5-2,0 pixlar

Öka mängden gradvis från 1,75 till 4. Om skärpan fortfarande inte är som du vill ha den ökar du radien med ett decimalkomma och kör mängden igen från 1,75 till 4. Upprepa vid behov.

Lämna den monokroma parameterinställningen på 0.

## Metodtips för JPEG-komprimering (&amp;qlt=) {#best-practices-for-jpeg-compression-qlt}

* Den här parametern styr JPG-kodningskvaliteten. Ett högre värde innebär en bild av högre kvalitet men en stor filstorlek. Ett lägre värde innebär en bild med lägre kvalitet men mindre filstorlek. Intervallet för den här parametern är 0-100.
* Om du vill optimera kvaliteten ska du inte ställa in parametervärdet på 100. Skillnaden mellan en inställning på 90 eller 95 och 100 är nästan otydlig, men 100 ökar storleken på bildfilen i onödan. Om du vill optimera kvaliteten men undvika att bildfilerna blir för stora anger du därför `qlt=` värdet 90 eller 95.
* Om du vill optimera för en liten bildfilsstorlek men behålla bildkvaliteten på en acceptabel nivå, anger du `qlt=` värdet 80. Värden under 70 till 75 ger en signifikant försämring av bildkvaliteten.
* Ett tips är att du bör behålla mitten genom att ange värdet 85 för att behålla mitten `qlt=` .
* Använda chroma-flaggan i `qlt=`

   * Parametern har en andra inställning som gör att du kan aktivera nedsampling av RGB-kromaticitet med hjälp av det normala värdet `qlt=` (standard), eller inaktivera den med hjälp av värdet `,0` `,1`.
   * Börja med att stänga av nedsampling av RGB-kromaticitet ( `,1`) för att göra det enkelt. Den här inställningen ger vanligtvis bättre bildkvalitet, särskilt för syntetiska bilder med många skarpa kanter och kontrast.

Ett tips för JPG-komprimering är att använda `&qlt=85,0`.

## Bästa tillvägagångssätt för JPEG-storleksändring (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

`jpegSize` är en användbar parameter om du vill garantera att en bild inte överskrider en viss storlek för leverans till enheter som har begränsat minne.

* Den här parametern anges i kilobyte ( `jpegSize=<size_in_kilobytes>`). Det definierar den största tillåtna storleken för bildleverans.
* `&jpegSize=` interagerar med JPG-komprimeringsparametern `&qlt=`. Om JPG-svaret med den angivna JPG-komprimeringsparametern ( `&qlt=`) inte överskrider `jpegSize` värdet returneras bilden med `&qlt=` det definierade värdet. Annars `&qlt=` minskas bilden gradvis tills bilden får plats i den högsta tillåtna storleken, eller tills systemet fastställer att den inte får plats och returnerar ett fel.

Det bästa sättet är att ange `&jpegSize=` och lägga till parametern `&qlt=` om du levererar JPG-bilder till enheter med begränsat minne.

## Sammanfattning av bästa praxis {#best-practices-summary}

Det bästa sättet att uppnå en hög bildkvalitet och liten filstorlek är att börja med följande kombination av parametrar:

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

Den här kombinationen av inställningar ger utmärkta resultat under de flesta omständigheter.

Om bilden behöver optimeras ytterligare finjusterar du stegvis skärpeparametrarna (oskarp maskning) genom att börja med radien 0,2 eller 0,3. Öka sedan mängden gradvis från 1,75 till maximalt 4 (motsvarande 400 % i Photoshop). Kontrollera att resultatet är det önskade.

Om skärpeeffekten fortfarande inte är tillräcklig ökar du radien i decimalsteg. För varje decimalsteg startar du om beloppet vid 1,75 och ökar det gradvis till 4. Upprepa den här processen tills du uppnår önskat resultat. Värdena ovan är en metod som de kreativa studierna har validerat, men kom ihåg att du kan börja med andra värden och följa andra strategier. Oavsett om resultaten är tillfredsställande för dig eller inte är en subjektiv fråga, så är strukturerade experiment avgörande.

När du experimenterar kan du också hitta följande allmänna förslag som kan hjälpa dig att optimera arbetsflödet:

* Testa och testa olika parametrar i realtid, antingen direkt på en Dynamic Media Classic-URL eller med hjälp av bildjusteringsfunktionen i Dynamic Media Classic som ger förhandsgranskning i realtid för justeringsåtgärder.
* Det är en god vana att gruppera Dynamic Media Image Serving-kommandon i en bildförinställning. En bildförinställning är i princip URL-kommandomakron med anpassade förinställningsnamn som `$thumb_low$` och `&product_high$`. Det anpassade förinställningsnamnet i en URL-sökväg gör att dessa förinställningar anropas. Den här funktionen hjälper dig att hantera kommandon och kvalitetsinställningar för olika användningsmönster för bilder på webbplatsen och förkortar den totala längden på URL-adresser.
* I Dynamic Media Classic finns också mer avancerade sätt att finjustera bildkvaliteten, till exempel genom att använda skärpebilder vid inhämtning. I avancerade fall där detta kan vara ett alternativ för att ytterligare finjustera och optimera återgivningsresultaten kan Adobe Professional Services hjälpa dig med anpassade insikter och metodtips.

