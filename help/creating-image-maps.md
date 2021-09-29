---
title: Skapa bildscheman
description: Lär dig hur du skapar bildscheman i Adobe Dynamic Media Classic.
uuid: 0dcc4956-006e-4a74-9d6a-6d4bb23790ce
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4eddf983-38cb-4f00-b3be-85c20bdd6f69
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: deafbd03-06bc-4d7e-87a1-5620ebcac426
source-git-commit: 0e2271924f49edd6ac424bb7cbd56af1e6afd817
workflow-type: tm+mt
source-wordcount: '2349'
ht-degree: 0%

---

# Skapa bildscheman {#creating-image-maps}

En bildschema är ett område på en bild, en eCatalog-sida eller en bild i en SpinSet som visar en överrullningspanel med text. När användaren väljer en bildschema utlöses en åtgärd av något slag. En webbsida startas till exempel så att användaren kan lära sig mer om en produkt. En kontur visas runt en bildschema när användaren flyttar pekaren över den.

Förutom möjligheten att skapa bildscheman i Adobe Dynamic Media Classic kan du även skapa bildscheman när du designar en katalog i Adobe Acrobat eller Adobe InDesign.

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

   * Om du arbetar med en bild i stödrastervyn eller listvyn väljer du **[!UICONTROL Image Map]** i listrutan Redigera. Du kan också öppna den i detaljvyn och sedan välja **[!UICONTROL Image Map]** ovanför bilden.
   * Om du arbetar med en SpinSet i stödrastervyn eller listvyn väljer du **[!UICONTROL Edit]**. Du kan också öppna den i detaljvyn och sedan välja **[!UICONTROL Edit]**. Välj en bildresurs och välj sedan **[!UICONTROL Image Map]**.
   * Om du arbetar med en e-katalog väljer du **[!UICONTROL Edit]** i Stödrastervisning, Listvy och Detaljvy. Välj fliken **[!UICONTROL Map Pages]**.

   ![Bild på bildschema](assets/ma_image_map.png)

1. Rita ett rektangulärt eller polygonalt (flersidigt) bildschema:

   * **Rektangulärt schema** - Välj verktyget Rektangelbildschema och dra på sidan för att skapa rektangeln. Om du vill lägga till en punkt i ett rektangulärt schema (och på så sätt ändra den till ett polygonschema) trycker du på Ctrl, placerar insättningsverktyget på önskad plats och markerar.

   * **Polygonkarta**  - Välj verktyget Polygonbildschema och markera punkter vid omkretsen av det område i bilden som du vill omsluta. Använd reglaget för polygondensitet för att ändra polygonens punktdensitet. Den ursprungliga densiteten sparas om du väljer andra kartor. Om en punkt läggs till, tas bort eller flyttas i polygonen, försvinner den ursprungliga densiteten och reglaget återställs till sitt högsta värde.

1. Ange ett namn för bildschemat, om du vill, i listan Bildschema. När du har ritat en bildschema får den ett namn av Adobe Dynamic Media Classic.

   För att skapa namnet lägger Adobe Dynamic Media Classic till ett sekventiellt nummer till namnet på den bild- eller eCatalog-sida som du arbetar med. Du kan ange ett namn.

1. Om du vill att användarna ska öppna en ny webbsida när de väljer bildschemat anger du URL:en i listan Bildschema.

   Se [för att ange JavaScript och URL:er](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. Om du vill visa överrullningstext när användare flyttar pekaren över bildschemat anger du texten i listan Bildschema. Välj menyn **[!UICONTROL Show]** i listan Bildschema och välj **[!UICONTROL Rollover Text]**. Ange sedan den text som du vill att användarna ska se på skärmen. Du kan skriva texten i en ordbehandlare och kopiera den till textfältet Över.

1. Om du vill att en annan åtgärdseffekt ska inträffa när användaren flyttar musen över en bildschema definierar du åtgärden. I listrutan **[!UICONTROL Show]** väljer du **[!UICONTROL Other Actions]**. Ange åtgärdens attribut. (Gå till **[!UICONTROL Show]** > **[!UICONTROL Both]** om du vill skapa överrullningstext och en åtgärd för en bildschema.)

   Se [Definiera andra åtgärder för Bildscheman](creating-image-maps.md#defining_other_actions_for_image_maps).

1. (Valfritt) Gör något av följande:

   * Om du vill förhandsgranska bildscheman väljer du **[!UICONTROL Preview]**.
   * Om du vill ta bort en bildschema eller polygonhörnpunkt markerar du en form i bilden och väljer sedan **[!UICONTROL Delete]**. Eller, för en e-katalog, på fliken Ordna sidor väljer du **[!UICONTROL Clear Maps]** om du vill ta bort bildscheman från alla sidor.
   * Om du tillfälligt vill ta bort en bildschema från en bild, en bild i en SpinSet eller en eCatalog-sida utan att ta bort den, avmarkerar du motsvarande På-alternativ i listan Bildschema.

1. Välj **[!UICONTROL Save]**.

### Justera placering, form och storlek för bildscheman {#adjusting-the-position-shape-and-size-of-image-maps}

Om du vill ändra placering, form och storlek för ett bildschema väljer du knappen Bildschema. Välj sedan verktyget **[!UICONTROL Pan]** och följ dessa instruktioner:

* **Ändra position**  - Flytta pekaren nära, men inte över, kanten på bildschemat. När du ser ikonen med fyra pilar drar du kartan till en ny plats.

* **Ändra storlek och form** - Hur du ändrar form och storlek på ett bildschema beror på om du arbetar med ett rektangulärt eller polygonbildschema:

>[!TIP]
>
>Du kan dra storleksreglaget längst ned på skärmen för att ändra vyer och få en bättre överblick över din bildschema.

* **Rektangulär bildschema**  - Flytta pekaren över en sida eller ett hörn av bildschemat. När du ser den dubbelriktade pilikonen börjar du dra. Håll ned Skift-tangenten när du drar om du vill ändra storlek men behålla proportionerna (formen).

* **Polygonbildschema**  - Dra ett fyrkantigt markeringshandtag. Om du vill skapa ett markeringshandtag markerar du kanten på bildschemat och börjar dra.

### Hantera överlappande bildscheman {#handling-overlapping-image-maps}

Om bilden eller eCatalog-sidan innehåller mer än en bildschema och kartorna överlappar varandra, kan du bestämma hur kartor överlappar. Om du vill göra det ändrar du ordningen på kartorna i listan Bildschema. Dra namnen uppåt eller nedåt i listan. Hur högt ett namn finns på listan avgör om dess bildschema överlappar andra bildscheman.

### Importera data för bildschema {#importing-image-map-data}

I stället för att ange bildschemadata på varje sida kan du importera data för bilden, den nya uppsättningen eller eCatalog till fönstret Kartsammanfattning. Du importerar bildschemadata i form av en tabbavgränsad fil eller XML DTD. Fälten i filen måste vara i den ordning som visas i fönstret Mappningssammanfattning: Namn, etiketter för innehållsförteckning, kartor, URL:er, överrullningstext, andra åtgärder och söksträngar. Om du importerar data från bildschemat slipper du problem med att ange data i listan Bildschema när du skapar bildschemat.

**Så här importerar du data för bildschema:**

1. Gå till redigeringssidan för bildscheman (för bilder eller bilder i SpinSets) eller fliken Kartsidor på redigeringsskärmen för eCatalog.
1. Välj **[!UICONTROL Import Metadata]**.
1. I dialogrutan Överför metadata väljer du Bild eller Bildschema för att överföra metadata från den önskade resursegenskapstypen.
1. Välj den typ av fil du vill skapa i listrutan Generera fil.
1. (Valfritt) Välj **[!UICONTROL Generate]** om du vill förhandsgranska resultatet baserat på den typ av fil som du vill skapa. Välj **[!UICONTROL Close]** för att återgå till dialogrutan Överför metadata.
1. Bläddra till filen som du vill överföra. Ange namnet på den genererade filen i textfältet Filnamn.
1. (Valfritt) I fältet Jobbnamn anger du ett namn för metadataöverföringsjobbet.
1. Välj **[!UICONTROL Upload]**.

### Kopiera bildscheman {#copying-image-maps}

Du kan kopiera bildscheman från en bild eller en eCatalog-sida till en annan. Använd **[!UICONTROL Copy Image Map]** om du vill få ett försprång att börja skapa dem. Du kan också kopiera bildscheman för att återskapa dem i bilder eller på sidor som delar en layout- eller mappningsstruktur.

Om du till exempel kopierar bildscheman i en eCatalog kan du enkelt kopiera alla bildscheman mellan olika språkversioner av samma eCatalog. Det bästa resultatet får du om du kopierar mellan e-kataloger med samma antal sidor och samma bilder. Om den eCatalog som du kopierar till redan innehåller bildscheman tas dessa bildscheman bort när kopian görs.

**Så här kopierar du bildscheman:**

1. Gå till redigeringssidan för bildscheman (för bilder eller bilder i SpinSets) eller fliken Kartsidor på redigeringsskärmen för eCatalog.
1. Välj **[!UICONTROL Copy Maps to]**.
1. Gör något av följande, baserat på om du kopierar bildscheman från bilder eller kopierar bildscheman från en e-katalog:

   * (Bilder) Markera de bilder du vill kopiera bildscheman till på skärmen Välj bilder.
   * (eCatalog) På skärmen Välj resurs markerar du de bilder eller e-katalogsidor som du vill kopiera bildscheman till.

1. Välj **[!UICONTROL Select]**.

## Använd en mall för att ange JavaScript och URL:er {#using-a-template-to-enter-javascript-and-urls}

Du kan definiera en URL-mall (kallas även Href-mall) för att göra det enklare och effektivare att ange URL:er för bildschema. Definiera en URL-mall om de flesta URL:er för bildschemat har ett gemensamt, fast format. Genom att ange den del av URL-adressen som är fast som URL-mall behöver du inte ange den här delen av URL-adressen varje gång du skapar en bildschema. URL-mallen kan även innehålla JavaScript-kommandon, sökvägsnamn och parametrar. Som standard innehåller URL-mallen en egen JavaScript-hanterare för Adobe Dynamic Media Classic med namnet `loadProduct` som öppnar bilden i ett nytt fönster.

>[!NOTE]
>
>När du lägger till JavaScript-koden i HREF-attributet för bildschemat körs koden på klientens dator. Kontrollera därför att JavaScript-koden är säker.

### Om URL-mallar {#about-url-templates}

URL-mallen fungerar genom att ersätta innehållet i URL-kolumnen i listan Bildschema med dubbla dollartecken (&quot;$$&quot;) i mallen:

```as3
Javascript:loadProduct(‘$$’);void(0);
```

Du placerar alla värden som inte ändras mellan bildscheman i URL-mallen. Lägg bara till de värden som ändras i URL-kolumnen i listan Bildschema. Exempel:

* URL-mall - `javascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* URL-värde - `product.htm`
* Faktisk URL genererad - `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

Som standard innehåller URL-mallen en egen JavaScript-hanterare för Adobe Dynamic Media Classic som heter `loadProduct` som öppnar ett nytt fönster med URL-målet. Du kan dock använda vilken JavaScript-kod som helst för att ersätta den här JavaScript-hanteraren eller använda någon av följande Adobe Dynamic Media Classic-hanterare:

* `loadProductCW` - Visar URL-målet som anges i URL-kolumnen i det aktuella fönstret. Hanteraren är främst avsedd för e-kataloger som är integrerade på en sida på en webbplats.

* `loadProductPW` - Visar URL-målet som anges i URL-kolumnen i det överordnade fönstret (sidan som öppnade det aktuella fönstret). Det aktuella fönstret förblir öppet, men det överordnade fönstret ändras så att URL-målet visas.

   >[!NOTE]
   >
   >Hanteraren `loadProductPW` stöder inte DHTML- och HTML5-visningsprogram.

### Skapa en URL-mall {#creating-a-url-template}

1. Välj Redigera bredvid alternativet URL-mall på skärmen i Kartredigeraren (bilder eller SpinSets) eller på fliken Kartsidor på skärmen eCatalog (eCatalogs). Dialogrutan Redigera kartmall öppnas.
1. Ange JavaScript-koden och den fullständiga URL:en (med variabeldelen ersatt med dollartecken [$]). Du kan klistra in koden genom att högerklicka och välja **[!UICONTROL Paste]**.
1. Välj **[!UICONTROL Save]**.

### Hantera URL-mallar {#handling-url-templates}

På mallredigeringssidan (bilder och SpinSets) och fliken Kartsidor på eCatalog-skärmen (eCatalogs) finns följande kommandon för hantering av URL-mallar:

* **Alternativet**  URL-mall - Välj alternativet URL-mall om du vill använda URL-mallen på alla bildscheman på en bild- eller eCatalog-sida.

* **Mallalternativ**  - Avmarkera ett mallalternativ i listan URL-bildschema om du inte vill att en enskild bildschema ska använda URL-mallen.

## Definiera andra åtgärder för bildscheman {#defining-other-actions-for-image-maps}

Du kan välja menyn **[!UICONTROL Show]** och välja **[!UICONTROL Other Actions]** om du vill utlösa andra åtgärder än överrullningstext och webbsidor öppnas. När användaren flyttar pekaren över ett bildschema kan du initiera en åtgärd. Dessa åtgärder är attribut som definieras för Image Maps på klientsidan av HTML-specifikationer för World Wide Web Consortium. De omfattar följande:

* **`accesskey`** - Startar en åtgärd när användaren trycker på en tangent på tangentbordet.

* **`onfocus`** - Startar en händelse när bildschemat får fokus - med pekaren, genom tabbning eller genom att trycka på en åtkomsttangent. Du kan till exempel starta en webbsida när bildschemat får fokus och stänga den när bildkartan förlorar fokus.

* **`onblur`** - Startar en händelse när bildschemat förlorar fokus, antingen med markören eller med tabbtangenten.

**Så här definierar du andra åtgärder för bildscheman:**

1. På kartredigerarens skärm (bilder och SpinSets) eller på fliken Kartsidor på eCatalog-skärmen (eCatalogs) väljer du **[!UICONTROL Show]**-menyn och väljer **[!UICONTROL Other Actions]**.
1. Använd den syntax som anges av HTML-specifikationerna för World Wide Web Consortium för att lägga till de attribut som stöds i kolumnen Andra åtgärder i listan Bildschema.
1. Välj **[!UICONTROL Save]**.

Välj menyn **[!UICONTROL Show]** och välj **[!UICONTROL Both]** om du vill att en bildschema ska innehålla överrullningstext och en åtgärd.

## Skapa bildscheman i Adobe Acrobat eller Adobe InDesign {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

Du kan skapa bildscheman när du utformar din e-katalog i Adobe Acrobat eller Adobe InDesign.

I Acrobat eller InDesign skapar du hyperlänksreferenser där du vill att bildscheman ska visas och anger URL-adresser för bildschemat. Om du markerar alternativet Extrahera länkar när du överför PDF-filen till Adobe Dynamic Media Classic konverteras länkarna automatiskt till Bildscheman.

Mer information finns i hjälpen till Adobe InDesign eller Adobe Acrobat.

### Skapa bildscheman i Adobe InDesign {#to-create-image-maps-in-adobe-indesign}

1. Gå till **[!UICONTROL Windows®]** > **[!UICONTROL Interactive]** > **[!UICONTROL Hyperlinks]** i InDesign.
1. På panelen Hyperlänkar markerar du den text, ram eller grafik som du vill göra till en bildschema.
1. Välj **[!UICONTROL New Hyperlink]** på panelmenyn.
1. Välj **[!UICONTROL URL]** på menyn **[!UICONTROL Link To]** i dialogrutan Ny hyperlänk.
1. Skriv eller klistra in produkt-ID:t i rutan URL.
1. Välj **[!UICONTROL OK]**. (Adobe Dynamic Media Classic slutför URL:en med hjälp av URL-mallen för bildschema.)

   >[!NOTE]
   >
   >Du behöver inte ange utseendealternativ i Adobe InDesign. Du kan ange utseende i Adobe Dynamic Media Classic.

1. Upprepa steg 2 till 6 för alla bildscheman som du vill skapa.
1. Exportera filen som en PDF-fil.
1. Överför PDF-filen till Adobe Dynamic Media Classic.
1. I **[!UICONTROL PDF Options]** väljer du **[!UICONTROL Extract Links]**.

### Skapa bildscheman i Adobe Acrobat {#to-create-image-maps-in-adobe-acrobat}

1. I Acrobat går du till **[!UICONTROL Tools]** > **[!UICONTROL Advanced Editing]** > **[!UICONTROL Link Tool]**.
1. Dra för att skapa bildschemat.
1. Markera **[!UICONTROL Custom Link]** i rutan Skapa länk och välj **[!UICONTROL Next]**.

>[!NOTE]
>
>Du behöver inte ange utseendealternativ i Adobe Acrobat. Du kan ange utseende i Adobe Dynamic Media Classic.

1. Välj **[!UICONTROL Actions]** i rutan Länkegenskaper.
1. Välj **[!UICONTROL Open A Web Link]** på Välj åtgärd-menyn och välj sedan **[!UICONTROL Add]**.
1. Skriv produkt-id:t för bildschemat i rutan Redigera URL och välj **[!UICONTROL OK]**. (Adobe Dynamic Media Classic slutför URL:en med hjälp av URL-mallen för bildscheman.)
1. Upprepa steg 1 till 7 för alla bildscheman som du vill skapa.
1. Spara filen.
1. Överför PDF-filen till Adobe Dynamic Media Classic och välj Extrahera länkar under PDF-alternativ.
