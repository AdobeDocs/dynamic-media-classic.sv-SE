---
title: Parametrisera en mall i Dynamic Media Classic
seo-title: Parametrisera en mall i Dynamic Media Classic
description: 'null'
seo-description: Lär dig hur du parametriserar en mall i Dynamic Media Classic
uuid: 27c8c8b4-47f3-4270-a6db-d304648ba357
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: df1a9ff5-a5ba-4480-ba0d-a19bc665f907
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Parametrisera en mall i Dynamic Media Classic{#parameterizing-a-template-in-scene}

När du har överfört en Illustrator-mall som du har sparat som Dynamic Media Classic FXG till Scene7 Publishing System kan du definiera dess variabelelement. Det gör du genom att parametrisera variabelelement i mallpubliceringsbygget och förhandsvisningsskärmarna. I Dynamic Media Classic finns verktyg för att definiera text- och objektparametrar för lager och deras respektive egenskaper. Du kan också skapa olika versioner av en mall.

Genom att parametrisera en FXG-mall kan du anpassa variabiliteten för text, bilder och grafik i mallen. Du kan till exempel parametrisera en textrad så att slutanvändarna kan ändra texten via ett webbanvändargränssnitt. Du kan definiera tomma textfält som variabler så att slutanvändarna kan fylla i dessa fält med anpassad text. Du kan också parametrisera attribut och egenskaper för designelement på skärmen Dynamic Media Classic Template Publishing Build.

>[!NOTE]
>
>Det är inte nödvändigt att parametrisera mallen i Dynamic Media Classic om du tänker använda DOM-manipulering.

## Definiera parametrar i FXG-mallar {#defining-parameters-in-fxg-templates}

Följ de här stegen i Dynamic Media Classic för att definiera parametrar för en FXG-mall:

1. Välj FXG-filen i bläddringsfönstret.
1. Klicka på **Skapa** och välj **mallpublicering** eller klicka på filens **Redigera** -knapp.

   Skärmen Mallpublicering öppnas.

1. Välj LRCo\FXG\Welcome_Summit_10 (FXG-fil) och klicka på **Skapa** > **Mallpublicering**.</p>

   ![](assets/wp_fxg_edit.png)

1. Markera lagret med de element du vill parametrisera på panelen Lager på skärmen Mallpublicering.

   >[!NOTE]
   >
   >Klicka på ögonikonen på och av för att kontrollera att du har markerat det objekt du vill använda.

1. Klicka på en parameter i kolumnen Namn (för att parameterisera text) eller i kolumnen Parameter (för att parameterisera objekt) på panelen Egenskaper.

   * **Text** Klicka i textfältet (bläddra längst ned i egenskapslistan för att hitta det). Dialogrutan Parametrar visas. Markera texten som du vill parametrisera och klicka på **Lägg till**. Du kan skapa flera parametrar från samma textegenskap genom att markera olika delar av texten och lägga till parametrar för varje del. Om du vill ändra namnet på parametern klickar du på den, anger ett nytt namn och klickar på **Stäng**.

   * **Objekt** Klicka på en ruta i kolumnen Parameter. Dialogrutan Redigera parameter visas. Ange ett namn och klicka på **OK**.
   Om du vill anpassa flera attribut samtidigt med samma värde använder du samma parameternamn för varje attribut. Om mallen till exempel har en rektangel och en stjärna kan du skriva `newcolor` parameternamnet för attributet SolidColor för varje färg. När du ändrar `newcolor` värdet ändras både rektangeln och stjärnan till den nya färgen.

1. Ange ett standardvärde för attributet i fältet Värde eller Data. Ange alla egenskaper för det markerade objektet för att ange exakt vilket utseende du vill ha.
1. (Valfritt) Upprepa steg 3-5 för alla objekt eller lager som du vill parametrisera.
1. Klicka på **Spara** eller **Spara som**.
1. Klicka på **Förhandsgranska** för att öppna fönstret FXG-förhandsvisning och se parametrarna som du skapade med deras standardvärden.

## Visa eller dölja ett objekt eller lager i FXG-mallen {#show-or-hide-an-object-or-layer-in-the-fxg-template}

Dolda objekt och lager visas inte vid förhandsvisning eller utdata, men tas inte bort från filen. Du kan göra dem synliga igen efter behov. Synlighet är ett attribut som du kan göra variabel. Om du klickar på ögonikonen på eller av anges standardvärdet för synligheten för ett objekt eller lager.

1. På objektpanelen klickar du på ögonikonen bredvid ett objekt- eller lagernamn för att dölja det i filen.
1. Klicka igen för att göra objektet synligt.

## Skapa olika versioner av en mall {#create-different-versions-of-a-template}

Du kan redigera attribut för att skapa olika versioner av mallen för olika användningsområden.

På skärmen Mallpublicering klickar du på Spara som för att spara filen som en ny FXG-mall utan att skriva över den ursprungliga FXG-mallen.

## Använda linjerad text {#using-stroked-text}

Linjerad text är ett exempel på hur du kan parametrisera attribut. Dynamic Media Classic har stöd för följande funktioner för linjerad text:

* Linjebredd
* Streckat linjemönster
* Olika kopplingsformat
* Olika ändformat för ändpunkter
* Övertryck av linje
* Separat färghantering för linjer, inklusive stöd för dekorfärger

I den här tabellen beskrivs de attribut som stöder linjerad text.

| Attribut | Beskrivning |
|--- |--- |
| s7:fill `<Boolean>`(endast S7FXG) | Anger om fyllning är aktiverad för text. Standardvärdet är true. |
| s7:linje `<Boolean>` (endast S7FXG) | Anger om linje är aktiverat för text. Standardvärdet är false. |
| s7:weight `<number>` (endast S7FXG) | Anger linjebredden för text i punkter. Standardvärdet är 1 punkt. |
| s7:leder `<string>` (spetsig, rund, avfasad) (endast S7FXG) | Anger linjens typ av förening. Standardvärdet är rund. |
| s7:caps `<string>` (none, round, square) (endast S7FXG) | Anger linjens ändtyp. Standardvärdet är rund. |
| s7:miterLimit `<number>` (endast S7FXG) | Anger gränsen för spetsen när hörnet är spetsigt hörn för linjen. Standardvärdet är 4. |
| s7:strokeOverprint `<Boolean>` (endast S7FXG) | Anger om övertryck är aktiverat för linje. Standardvärdet är false. |
| s7:strokeColorName (endast S7FXG) | Samma som s7:colorName, förutom att namnet på färgen för linjen definieras. |
| s7:strokeColorValue (endast S7FXG) | Samma som s7:colorValue, förutom att det definierar värdet på den färg som används för linjen. |
| s7:strokeColorSpace (endast S7FXG) | Samma som s7:färgrymd, förutom att färgrymden för linjen definieras. |
| flm:dashPattern `<array>` (endast S7FXG) | Som standard finns det inga mönster för strecken och mellanrummen. Det här attributet definierar strecket/mellanrumsmönstret för linjen. Det första värdet är strecket på linjen. Den andra är mellanrummet mellan strecken. Du kan utöka arrayen för flera värden på samma sätt med alternativa värden som streck och mellanrum. |

## Använda tänjd text {#using-warped-text}

Med tänjd text kan du ändra utseendet på text med effekter som våg, flagga, sträcka ut och så vidare.

Tänjd text stöds för RichText-objekt. Texten kan vara lodrät eller vågrät och kan vara punkttext, figurtext och text på bana. Hela textobjektet måste markeras innan tänjd text kan användas.

Tänjd text kan skapas i Adobe Illustrator.

När du tänjer text kan du ange följande attribut:

* Stil
* Riktning
* Böj
* Vågrät förvrängning
* Hörlförvrängning

Varje attribut innehåller en uppsättning värden.

| Attribut | Värden | Standard |
|--- |--- |--- |
| Stilar7:warpStyle | nonearcarcLowerarcUpperarkbulgeshellLowershellUpperflagwavefishrisefishEyeinflatesqueezetwist | ingen |
| Riktningar7:warpDirection | vågrät lodrät | vågrät |
| Bends7:warpBend | -1 till 1 | 0.5 |
| Vågrät förvrängning7:warpHorizontalDistortion | -1 till 1 | 0 |
| Lodrät förvrängning7:warpVerticalDistortion | -1 till 1 | 0 |

>[!NOTE]
>
>För `inflate` och `fishEye`om du ändrar `s7:warpDirection` flaggan mellan vågrät och lodrät påverkas inte utdata.

Mer information om hur du skapar och använder tänjd text finns i dokumentationen för Adobe Illustrator.

>[!MORELIKETHIS]
>
>* [Skapa den ursprungliga mallen i Illustrator](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator)
>* [Överför filer för mallpublicering](upload-files-template-publishing.md#upload_files_for_template-publishing)

