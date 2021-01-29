---
title: Skapa bildscheman
description: Lär dig hur du skapar bildscheman.
uuid: 0dcc4956-006e-4a74-9d6a-6d4bb23790ce
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4eddf983-38cb-4f00-b3be-85c20bdd6f69
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '2440'
ht-degree: 0%

---


# Skapa bildscheman{#creating-image-maps}

En bildschema är ett område på en bild, en eCatalog-sida eller en bild i en SpinSet som visar en överrullningspanel med text. När användaren klickar på en bildschema utlöses en åtgärd av något slag. En webbsida startas till exempel så att användaren kan lära sig mer om en produkt. Om du vill fästa uppmärksamheten på bildscheman visas en kontur runt en bildschema när användaren flyttar pekaren över den.

Förutom möjligheten att skapa ett bildschema i Dynamic Media Classic kan du även skapa bildscheman när du designar en katalog i Adobe Acrobat eller Adobe InDesign.

När du skapar bildscheman kan du göra något av följande:

* Ange överrullningstext.
* Ange JavaScript och URL:er för att starta webbsidor.
* Skapa URL-mallar för bildscheman.
* Kopiera bildscheman till andra bilder, eCatalog-sidor eller SpinSets.
* Exportera bildscheman till CSV eller till XML.
* Importera bildmetadata från en tabbavgränsad fil eller från en XML-fil.
* Definiera andra åtgärder enligt World Wide Web Consortium.
* Förhandsgranska bildscheman.

## Rita och justera en bildschema {#drawing-and-adjusting-an-image-map}

1. Gör något av följande:

   * Om du arbetar med en bild i stödrastervyn eller listvyn klickar du på **Bildschema** i listrutan Redigera. Du kan också öppna den i detaljvyn och sedan klicka på **Bildschema** ovanför bilden.
   * Om du arbetar med en SpinSet i stödrastervyn eller listvyn klickar du på **Redigera**. Du kan också öppna den i detaljvyn och sedan klicka på **Redigera**. Välj en bildresurs och klicka sedan på **Bildschema**.
   * Om du arbetar med en e-katalog klickar du på **Redigera** i Stödrastervisning, listvy eller detaljvy. Klicka på fliken **Mappa sidor**.

   ![](assets/ma_image_map.png)

1. Rita ett rektangulärt eller polygonalt (flersidigt) bildschema:

   **Rektangulär** kartaVälj verktyget Rektangelbildschema och dra på sidan för att skapa rektangeln. Om du vill lägga till en punkt i ett rektangulärt schema (och på så sätt ändra den till ett polygonschema) trycker du på Ctrl, placerar insättningsverktyget på önskad plats och klickar.

   **PolygonkartaVälj** verktyget Polygonbildschema och klicka på punkterna vid det område i bilden som du vill omsluta. Använd reglaget för polygondensitet för att ändra polygonens punktdensitet. Den ursprungliga densiteten sparas om du väljer andra kartor. Om en punkt läggs till, tas bort eller flyttas i polygonen, försvinner den ursprungliga densiteten och reglaget återställs till sitt högsta värde.

1. Ange ett namn för bildschemat, om du vill, i listan Bildschema. När du har ritat en bildschema ger Dynamic Media Classic den ett namn.

   För att skapa namnet lägger Dynamic Media Classic till ett sekventiellt nummer till namnet på den bild- eller e-katalogsida som du arbetar med. Du kan ange ett namn.

1. Om du vill att användarna ska öppna en ny webbsida när de klickar på bildschemat anger du URL:en i listan Bildschema.

   Se [för att ange JavaScript och URL:er](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. Om du vill visa överrullningstext när användare flyttar pekaren över bildschemat anger du texten i listan Bildschema. I listan Bildschema väljer du menyn Visa och sedan Överrullningstext. Ange sedan den text som du vill att användarna ska se på skärmen. Du kan skriva texten i en ordbehandlare och kopiera den till textfältet Över.
1. Om du vill att en annan åtgärdseffekt ska inträffa när användaren flyttar musen över en bildschema definierar du åtgärden. Klicka på Andra åtgärder i listrutan Visa. Ange åtgärdens attribut. (Klicka på Visa > Båda för att skapa överrullningstext och en åtgärd för en bildschema.)

   Se [Definiera andra åtgärder för bildscheman](creating-image-maps.md#defining_other_actions_for_image_maps).

1. (Valfritt) Gör något av följande:

   * Klicka på Förhandsgranska för att förhandsgranska bildscheman.
   * Om du vill ta bort ett bildschema eller en polygonhörnpunkt markerar du en form i bilden och klickar sedan på Ta bort. Du kan också klicka på Rensa kartor för att ta bort bildscheman från alla sidor på fliken Ordna sidor i en e-katalog.
   * Om du tillfälligt vill ta bort en bildschema från en bild, en bild i en SpinSet eller en eCatalog-sida utan att ta bort den, avmarkerar du motsvarande På-alternativ i listan Bildschema.

1. Klicka på Spara.

### Justera placering, form och storlek för bildscheman {#adjusting-the-position-shape-and-size-of-image-maps}

Om du vill ändra placering, form och storlek för ett bildschema väljer du knappen Bildschema. Välj sedan panoreringsverktyget och följ dessa instruktioner:

**Ändra** positionFlytta pekaren nära, men inte över, kanten på bildschemat. När du ser ikonen med fyra pilar drar du kartan till en ny plats.

**Ändra storlek och** formHur du ändrar form och storlek på ett bildschema beror på om du arbetar med ett rektangulärt eller polygonbildschema:

***Tips **: Du kan dra storleksreglaget längst ned på skärmen för att ändra vyer och få en bättre överblick över din bildschema.*

**Rektangulär** bildschemaFlytta pekaren över en sida eller ett hörn i bildschemat. När du ser den dubbelriktade pilikonen börjar du dra. Håll ned Skift-tangenten när du drar om du vill ändra storlek men behålla proportionerna (formen).

**Polygonbild** MapDra ett fyrkantigt markeringshandtag. Om du vill skapa ett markeringshandtag klickar du på kanten på bildschemat och börjar dra.

### Hantera överlappande bildscheman {#handling-overlapping-image-maps}

Om bilden eller eCatalog-sidan innehåller mer än en bildschema och kartorna överlappar varandra, kan du bestämma hur kartor överlappar. Om du vill göra det ändrar du ordningen på kartorna i listan Bildschema. Dra namnen uppåt eller nedåt i listan. Hur högt ett namn finns på listan avgör om dess bildschema överlappar andra bildscheman.

### Importerar data för bildschema {#importing-image-map-data}

I stället för att ange bildschemadata på varje sida kan du importera data för bilden, den nya uppsättningen eller eCatalog till fönstret Kartsammanfattning. Du importerar bildschemadata i form av en tabbavgränsad fil eller XML DTD. Fälten i filen måste vara i den ordning som visas i fönstret Mappningssammanfattning: Namn, etiketter för innehållsförteckning, kartor, URL:er, överrullningstext, andra åtgärder och söksträngar. Om du importerar data från bildschemat slipper du problem med att ange data i listan Bildschema när du skapar bildschemat.

**Importera bildkartsdata**

1. Gå till redigeringssidan för bildscheman (för bilder eller bilder i SpinSets) eller fliken Kartsidor på redigeringsskärmen för eCatalog.
1. Klicka på Importera metadata.
1. I dialogrutan Överför metadata klickar du på Bild eller Bildschema för att överföra metadata från den önskade resursegenskapstypen.
1. Välj den typ av fil du vill skapa i listrutan Generera fil.
1. (Valfritt) Klicka på Generera om du vill förhandsgranska de data som skapas baserat på den typ av fil som du vill skapa. Klicka på Stäng för att återgå till dialogrutan Överför metadata.
1. Bläddra till filen som du vill överföra. Ange namnet på den genererade filen i textfältet Filnamn.
1. (Valfritt) I fältet Jobbnamn anger du ett namn för metadataöverföringsjobbet.
1. Klicka på Överför.

### Kopierar bildscheman {#copying-image-maps}

Du kan kopiera bildscheman från en bild eller en eCatalog-sida till en annan. Använd Kopiera bildschema för att få ett försprång när du börjar skapa dem. Du kan också kopiera bildscheman för att återskapa dem i bilder eller på sidor som har samma layout eller mappningsstruktur.

Om du till exempel kopierar bildscheman i en eCatalog kan du enkelt kopiera alla bildscheman mellan olika språkversioner av samma eCatalog. Det bästa resultatet får du om du kopierar mellan e-kataloger med samma antal sidor och samma bilder. Om den eCatalog som du kopierar till redan innehåller bildscheman ska du vara medveten om att dessa bildscheman tas bort när kopian görs.

**Kopiera bildscheman**

1. Gå till redigeringssidan för bildscheman (för bilder eller bilder i SpinSets) eller fliken Kartsidor på redigeringsskärmen för eCatalog.
1. Klicka på Kopiera kartor till.
1. Gör något av följande, baserat på om du kopierar bildscheman från bilder eller kopierar bildscheman från en e-katalog:

   * (Bilder) Markera de bilder du vill kopiera bildscheman till på skärmen Välj bilder.
   * (eCatalog) På skärmen Välj resurs markerar du de bilder eller e-katalogsidor som du vill kopiera bildscheman till.

1. Klicka på Välj.

## Använda en mall för att ange JavaScript och URL:er {#using-a-template-to-enter-javascript-and-urls}

Du kan definiera en URL-mall (kallas även Href-mall) för att göra det enklare och effektivare att ange URL:er för bildschema. Definiera en URL-mall om de flesta URL:er för bildschemat har ett gemensamt, fast format. Genom att ange den del av URL-adressen som är fast som URL-mall behöver du inte ange den här delen av URL-adressen varje gång du skapar en bildschema. URL-mallen kan även innehålla JavaScript-kommandon, sökvägsnamn och parametrar. Som standard innehåller URL-mallen en Dynamic Media Classic JavaScript-hanterare med namnet `loadProduct` som öppnar bilden i ett nytt fönster.

>[!NOTE]
>
>Tänk på att koden körs på klientens dator när du lägger till Javascript-koden i HREF-attributet för bildschemat. Kontrollera därför att JavaScript-koden är säker.

### Om URL-mallar {#about-url-templates}

URL-mallen fungerar genom att ersätta innehållet i URL-kolumnen i listan Bildschema med dubbla dollartecken (&quot;$$&quot;) i mallen:

```as3
Javascript:loadProduct(‘$$’);void(0);
```

Du placerar alla värden som inte ändras mellan bildscheman i URL-mallen. Lägg bara till de värden som ändras i URL-kolumnen i listan Bildschema. Exempel:

* URL-mall: j `avascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* URL-värde: `product.htm`
* Faktisk URL som genererats: `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

Som standard innehåller URL-mallen en Dynamic Media Classic JavaScript-hanterare med namnet `loadProduct` som öppnar ett nytt fönster med URL-målet. Du kan dock använda vilken JavaScript-kod som helst för att ersätta den här JavaScript-hanteraren eller använda någon av följande Dynamic Media Classic-hanterare:

* `loadProductCW`

   Visar URL-målet som anges i URL-kolumnen i det aktuella fönstret. Hanteraren är främst avsedd för e-kataloger som är integrerade på en sida på en webbplats.

* `loadProductPW`

   Visar URL-målet som anges i URL-kolumnen i det överordnade fönstret (sidan som öppnade det aktuella fönstret). Det aktuella fönstret förblir öppet, men det överordnade fönstret ändras så att URL-målet visas.

   ***Obs **! Hanteraren  `loadProductPW` stöder inte DHTML- och HTML5-visningsprogram.*

### Skapa en URL-mall {#creating-a-url-template}

Så här skapar du en URL-mall:

1. Välj Redigera bredvid alternativet URL-mall på skärmen i Kartredigeraren (bilder eller SpinSets) eller på fliken Kartsidor på skärmen eCatalog (eCatalogs). Dialogrutan Redigera kartmall öppnas.
1. Ange JavaScript-koden och den fullständiga URL:en (med variabeldelen ersatt med dollartecken [$]). Du kan klistra in koden genom att högerklicka och välja Klistra in.
1. Klicka på knappen Spara.

### Hantera URL-mallar {#handling-url-templates}

På mallredigeringssidan (bilder och SpinSets) och fliken Kartsidor på eCatalog-skärmen (eCatalogs) finns följande kommandon för hantering av URL-mallar:

**URL-mall-** alternativVälj alternativet URL-mall om du vill använda URL-mallen på alla bildscheman på en bild- eller eCatalog-sida.

**Mallalternativ** Avmarkera ett mallalternativ i listan URL-bildschema om du inte vill att en enskild bildschema ska använda URL-mallen.

## Definiera andra åtgärder för bildscheman {#defining-other-actions-for-image-maps}

Du kan välja menyn Visa och välja Andra åtgärder om du vill aktivera andra åtgärder än överrullningstext och webbsidor som öppnas. När användaren flyttar pekaren över ett bildschema kan du initiera en åtgärd. Dessa åtgärder är attribut som definieras för Image Maps på klientsidan av HTML-specifikationer för World Wide Web Consortium. De omfattar följande:

**hjälpmedel** Startar en åtgärd när användaren trycker på en tangent på tangentbordet.

**** onfocusUtlöser en händelse när bildschemat får fokus - av markören, genom att tabba eller genom att trycka på en åtkomsttangent. Du kan till exempel starta en webbsida när bildschemat får fokus och stänga den när bildkartan förlorar fokus.

**** onblurUtlöser en händelse när bildschemat förlorar fokus, antingen med markören eller med tabbtangenten.

**Definiera andra åtgärder för bildscheman**

1. På kartredigerarens skärm (bilder och SpinSets) eller på fliken Kartsidor på eCatalog-skärmen (eCatalogs) väljer du Visa-menyn och sedan Andra åtgärder.
1. Använd den syntax som anges av HTML-specifikationerna för World Wide Web Consortium för att lägga till de attribut som stöds i kolumnen Andra åtgärder i listan Bildschema.
1. Klicka på **Spara**.

Välj menyn Visa och välj Båda om du vill att en bildschema ska innehålla både överrullningstext och en åtgärd.

## Skapa bildscheman i Adobe Acrobat eller Adobe InDesign {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

Du kan skapa bildscheman när du utformar din e-katalog i Adobe Acrobat eller Adobe InDesign.

I Acrobat eller InDesign skapar du hyperlänksreferenser där du vill att bildscheman ska visas och anger URL-adresser för bildschemat. Om du väljer alternativet Extrahera länkar när du överför PDF-filen till Dynamic Media Classic konverteras länkarna automatiskt till Bildscheman.

Mer information finns i hjälpen för InDesign och Acrobat.

### Skapa bildscheman i Adobe InDesign {#to-create-image-maps-in-adobe-indesign}

1. Öppna panelen Hyperlänkar genom att klicka på Fönster > Interaktivt > Hyperlänkar i InDesign.
1. Markera texten, ramen eller grafiken som du vill göra till ett bildschema.
1. Klicka på Ny hyperlänk på panelmenyn på panelen Hyperlänkar.
1. Välj URL på menyn Länka till i dialogrutan Ny hyperlänk.
1. Skriv eller klistra in produkt-id:t i rutan URL och klicka på OK. (Dynamic Media Classic slutför URL:en med hjälp av URL-mallen för bildschema.)

   >[!NOTE]
   >
   >Du behöver inte ange utseendealternativ i InDesign. Du kan ange utseende i Dynamic Media Classic.

1. Upprepa steg 2 till 5 för alla bildscheman som du vill skapa.
1. Exportera filen som en PDF-fil.
1. Överför PDF-filen till Dynamic Media Classic och välj Extrahera länkar under PDF-alternativ.

### Skapa bildscheman i Adobe Acrobat {#to-create-image-maps-in-adobe-acrobat}

1. I Acrobat väljer du Verktyg > Avancerad redigering > Länkverktyg.
1. Dra för att skapa bildschemat. Rutan Skapa länk öppnas.
1. Välj Egen länk och klicka på Nästa.

   ***Obs **! Du behöver inte ange utseendealternativ i Acrobat. Du kan ange utseende i Dynamic Media Classic.*

1. Klicka på Åtgärder i rutan Länkegenskaper.
1. Välj Öppna en webblänk på menyn Välj åtgärd och klicka sedan på Lägg till.
1. Skriv produkt-id:t för bildschemat i rutan Redigera URL och klicka på OK. (Dynamic Media Classic slutför URL:en med hjälp av URL-mallen för bildscheman.)
1. Upprepa steg 1 till 7 för alla bildscheman som du vill skapa.
1. Spara filen.
1. Överför PDF-filen till Dynamic Media Classic och välj Extrahera länkar under PDF-alternativ.

