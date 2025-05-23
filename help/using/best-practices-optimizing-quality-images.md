---
title: Bästa tillvägagångssätt för att optimera bildkvaliteten
description: Lär dig de bästa sätten att optimera bildkvaliteten.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 3c50e706-b9ed-49db-8c08-f179de52b9cf
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '1604'
ht-degree: 0%

---

# Bästa tillvägagångssätt för att optimera bildkvaliteten{#best-practices-for-optimizing-the-quality-of-your-images}

Att optimera bildkvaliteten kan ta lång tid. Många faktorer bidrar till att återge godtagbara resultat. Resultatet är delvis subjektivt eftersom individer upplever olika bildkvalitet. Strukturerade experiment är avgörande.

Adobe Dynamic Media Classic innehåller över 100 bildserverkommandon för justering och optimering av bilder och återgivning. Följande riktlinjer kan hjälpa dig att effektivisera processen och uppnå goda resultat snabbt med några viktiga kommandon och bästa metoder.

Se även [Smart bildbehandling](https://experienceleague.adobe.com/sv/docs/experience-manager-65/content/assets/dynamic/imaging-faq).

>[!TIP]
>
>Prova och upptäck fördelarna med Dynamic Media bildmodifierare och Smart Imaging med Dynamic Media [_Snapshot_](https://snapshot.scene7.com/).
>
> Ögonblicksbild är ett visuellt demonstrationsverktyg som är utformat för att illustrera styrkan hos Dynamic Media för optimerad och dynamisk bildleverans. Experimentera med testbilder eller Dynamic Media-URL:er, så att du kan se resultatet av olika bildmodifierare i Dynamic Media och optimera smarta bilder för följande:
>
>* Filstorlek (med WebP- och AVIF-leverans)
>* Nätverksbandbredd
>* DPR (Device Pixel Ratio)
>
>Om du vill lära dig hur enkelt det är att använda ögonblicksbild kan du spela upp utbildningsvideon [för ögonblicksbild](https://experienceleague.adobe.com/sv/docs/experience-manager-learn/assets/dynamic-media/images/dynamic-media-snapshot) (3 minuter och 17 sekunder).


## Bästa tillvägagångssätt för bildformat (&amp;fmt=) {#best-practices-for-image-format-fmt}

* JPG eller PNG är de bästa alternativen för att leverera bilder med god kvalitet och hanterbar storlek och vikt.
* Om inget formatkommando anges i URL:en används som standard Dynamic Media Image Serving JPG för leverans.
* JPG komprimerar med förhållandet 10:1 och ger vanligtvis mindre bildfiler. PNG komprimeras med ett förhållande på cirka 2:1, förutom ibland när bilder innehåller en tom bakgrund. Vanligtvis är PNG-filernas storlek större än JPG filer.
* JPG använder förstörande komprimering, vilket innebär att bildelement (pixlar) tas bort under komprimeringen. PNG använder däremot förlustfri komprimering.
* JPG komprimerar ofta foton med bättre återgivning än syntetiska bilder med skarpa kanter och kontrast.
* Om dina bilder innehåller genomskinlighet använder du PNG eftersom JPG inte stöder genomskinlighet.

Ett tips för bildformat är att börja med den vanligaste inställningen `&fmt=JPG`.

## Bästa tillvägagångssätt för bildstorlek {#best-practices-for-image-size}

Att minska bildstorleken dynamiskt är en av de vanligaste uppgifterna som Dynamic Media Image Serving utför. Det handlar om att ange storleken och, om så önskas, vilket nedsamplingsläge som används för att nedskala bilden.

* För storleksändring av bilder är det bästa och enklaste sättet att använda `&wid=<value>` och `&hei=<value>` eller bara `&hei=<value>`. Dessa parametrar ställer automatiskt in bildbredden i enlighet med proportionerna.
* `&resMode=<value>` styr den algoritm som används för nedsampling. Börja med `&resMode=sharp2`. Det här värdet ger den bästa bildkvaliteten. Nedsamplingsvärdet `=bilin` är snabbare men resulterar ofta i aliasing av artefakter.

Använd `&wid=<value>&hei=<value>&resMode=sharp2` eller `&hei=<value>&resMode=sharp2` om du vill ändra bildstorlek

## Bästa tillvägagångssätt för bildskärpa {#best-practices-for-image-sharpening}

Bildskärpa är den mest komplicerade aspekten när det gäller att styra bilder på webbplatsen och var många misstag görs. Ta dig tid att lära dig mer om hur skärpa och oskarp maskning fungerar i Adobe Dynamic Media Classic med hjälp av följande resurser:

Best practices white paper [Öka skärpan i bilder i Adobe Dynamic Media Classic och på Image Server](/help/using/assets/s7_sharpening_images.pdf).

<!-- Give a 404 See also [Sharpening an image with unsharp mask](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html). -->

Med Adobe Dynamic Media Classic kan du öka skärpan i bilder vid intag, vid leverans eller både och. Vanligtvis kan du skärpa upp bilder med bara en metod eller med en annan, men inte med båda metoderna. Att skärpa bilderna vid leverans, på en URL-adress, ger oftast bäst resultat.

Det finns två metoder för bildskärpa som du kan använda:

* Enkel skärpa ( `&op_sharpen`): Precis som skärpefiltret som används i Photoshop, tillämpar enkel skärpa grundläggande skärpa på den slutliga vyn av bilden efter dynamisk storleksändring. Den här metoden kan dock inte konfigureras av användaren. Det bästa sättet är att undvika användning av `&op_sharpen` om det inte krävs.
* Oskarp maskering ( `&op_USM`): Oskarp maskering är ett branschstandardfilter för skärpa. Det bästa sättet är att göra bilder skarpare med oskarp maskering enligt riktlinjerna nedan. Med Oskarp maskning kan du styra följande tre parametrar:

   * `&op_sharpen=amount,radius,threshold`

      * `amount` (0-5, effektens styrka.)
      * `radius` (0-250, bredden på de&quot;skärpelinjer&quot; som ritas runt det skarpa objektet, mätt i pixlar.)

        Kom ihåg att parametrarna `radius` och `amount` fungerar mot varandra. Minskning av `radius` kan kompenseras genom att `amount` ökas. `Radius` ger bättre kontroll eftersom ett lägre värde bara ökar skärpan på kantpixlarna, medan ett högre värde ökar skärpan på ett större antal pixlar.

      * `threshold` (0-255, effektkänslighet.)

        Den här parametern avgör hur annorlunda de pixlar som ska göras skarpare måste vara från det omgivande området innan de betraktas som kantpixlar och filtret gör dem skarpare. Tröskelvärdet hjälper dig att undvika att göra områden med liknande färger, som hudtoner, för skarpare. Ett tröskelvärde på 12 ignorerar till exempel små variationer i hudtonens ljusstyrka för att undvika att lägga till&quot;brus&quot;, samtidigt som kantkontrasten läggs till i områden med hög kontrast, till exempel där ögonfransarna möter huden.

        Mer information om hur du ställer in de här tre parametrarna, inklusive de bästa sätten att använda med filtret, finns i [Öka skärpan i bilder i Adobe Dynamic Media Classic och på Image Server](/help/using/assets/s7_sharpening_images.pdf).

      * Med Adobe Dynamic Media Classic kan du även styra en fjärde parameter: monokrom ( `0,1`). Den här parametern avgör om oskarp maskering används separat för varje färgkomponent med värdet `0` eller bildens intensitet/intensitet med värdet `1`.

Ett tips är att börja med parametern unsharp mask radius. Radie-inställningar som du kan börja med är följande:

* Webbplats: 0,2-0,3 pixlar
* Fotografisk utskrift (250-300 ppi): 0,3-0,5 pixlar
* Offsettryck (266-300 ppi): 0,7-1,0 pixlar
* Utskrift på arbetsytan (150 ppi): 1,5-2,0 pixlar

Öka mängden gradvis från 1,75 till 4. Om skärpan fortfarande inte är som du vill ha den ökar du radien med ett decimalkomma och kör mängden igen från 1,75 till 4. Upprepa vid behov.

Lämna den monokroma parameterinställningen på 0.

## Bästa tillvägagångssätt för komprimering av JPEG (`&qlt=`) {#best-practices-for-jpeg-compression-qlt}

* Den här parametern styr JPG kodningskvaliteten. Ett högre värde innebär en bild med högre kvalitet men en stor filstorlek. Ett lägre värde innebär en bild med lägre kvalitet men mindre filstorlek. Intervallet för parametern är 0-100.
* Om du vill optimera kvaliteten ska du inte ange parametervärdet 100. Skillnaden mellan en inställning på 90 eller 95 och 100 är nästan osynlig. Men 100 ökar storleken på bildfilen i onödan. Om du vill optimera för kvaliteten men undvika att bildfilerna blir för stora anger du därför värdet `qlt=` till 90 eller 95.
* Om du vill optimera för en liten bildfilsstorlek men behålla bildkvaliteten på en acceptabel nivå, anger du värdet `qlt=` till 80. Värden under 70 till 75 ger en signifikant försämring av bildkvaliteten.
* För att vara i mitten bör du ange värdet `qlt=` till 85 så att det ligger kvar i mitten.
* Använda kroma-flaggan i `qlt=`

   * Parametern `qlt=` har en andra inställning som gör att du kan aktivera nedsampling av färgvärden i RGB med det normala värdet `,0` (standard) eller inaktivera den med värdet `,1`.
   * Om du vill göra det enkelt kan du börja med att nedsampling av färgförändringar i RGB är inaktiverat ( `,1`). Den här inställningen ger vanligtvis bättre bildkvalitet, särskilt för syntetiska bilder med många skarpa kanter och kontrast.

Använd `&qlt=85,0` som bästa praxis för komprimering JPG.

## Bästa tillvägagångssätt för storleksändring av JPEG (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

Parametern `jpegSize` är användbar om du vill garantera att en bild inte överskrider en viss storlek för leverans till enheter som har begränsat minne.

* Den här parametern anges i kilobyte ( `jpegSize=<size_in_kilobytes>`). Det definierar den största tillåtna storleken för bildleverans.
* `&jpegSize=` interagerar med JPG komprimeringsparametern `&qlt=`. Om JPG svar med den angivna JPG-komprimeringsparametern ( `&qlt=`) inte överskrider värdet `jpegSize` returneras bilden med `&qlt=` enligt definitionen. Annars minskas `&qlt=` gradvis tills bilden får plats i den högsta tillåtna storleken. Eller tills systemet avgör att det inte får plats och returnerar ett fel.

Det bästa är att ange `&jpegSize=` och lägga till parametern `&qlt=` om du levererar JPG-bilder till enheter med begränsat minne.

## Sammanfattning av bästa praxis {#best-practices-summary}

Det bästa sättet att uppnå hög bildkvalitet och liten filstorlek är att börja med följande kombination av parametrar:

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

Den här kombinationen av inställningar ger utmärkta resultat under de flesta omständigheter.

Om bilden behöver optimeras ytterligare finjusterar du stegvis skärpeparametrarna (oskarp maskning) genom att börja med radien 0,2 eller 0,3. Därefter ökar du mängden gradvis från 1,75 till maximalt 4 (vilket motsvarar 400 % i Photoshop). Kontrollera att resultatet är det önskade.

Om skärpeeffekten fortfarande inte är tillräcklig ökar du radien i decimalsteg. För varje decimalsteg startar du om beloppet vid 1,75 och ökar det gradvis till 4. Upprepa den här processen tills du uppnår önskat resultat. Värdena ovan är en metod som de kreativa studierna har validerat, men kom ihåg att du kan börja med andra värden och följa andra strategier. Oavsett om resultaten är tillfredsställande för dig eller inte är en subjektiv fråga, så är strukturerade experiment avgörande.

Följande allmänna förslag är användbara när du experimenterar för att optimera arbetsflödet:

* Testa och testa olika parametrar i realtid, antingen direkt på en webbadress eller med Adobe Dynamic Media Classic bildjusteringsfunktioner. Den senare ger förhandsvisningar i realtid för justeringsåtgärder.
* Det är en god vana att gruppera Dynamic Media Image Serving-kommandon i en bildförinställning. En bildförinställning är i princip URL-kommandomakron med anpassade förinställningsnamn som `$thumb_low$` och `&product_high$`. Det anpassade förinställningsnamnet i en URL-sökväg anropar de här förinställningarna. Den här funktionen hjälper dig att hantera kommandon och kvalitetsinställningar för olika användningsmönster för bilder på webbplatsen och förkortar den totala längden på URL-adresser.
* Adobe Dynamic Media Classic har också mer avancerade sätt att finjustera bildkvaliteten, t.ex. genom att tillämpa bildskärpa vid intag. För avancerade användningsområden där ytterligare justering och optimering av återgivna resultat är ett alternativ kan Adobe Professional Services hjälpa dig med anpassade insikter och bästa metoder.
