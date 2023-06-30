---
title: Skapa eCatalog-bildscheman
description: Lär dig hur du skapar eCatalog-bildscheman i Adobe Dynamic Media Classic.
uuid: 943ad3f7-a885-4bc2-88cb-77083384bdf8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 4cf63359-63b5-4da7-9498-335d91b4776c
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
topic: Integrations, Development
level: Experienced
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '1449'
ht-degree: 0%

---

# Skapa eCatalog-bildscheman{#creating-ecatalog-image-maps}

En bildschema är ett område på en eCatalog-sida som du kan rulla över med musen eller välja att aktivera åtgärder av olika slag. När du till exempel flyttar pekaren över ett bildschema visas en beskrivning av ett objekts överrullningstext. När du väljer en bildschema initieras en annan åtgärd. Du kan till exempel öppna en webbsida så att tittarna kan lära sig mer om ett objekt eller köpa det, eller så kan du starta en video för att se ett objekt som används.

## Rita eCatalog-bildscheman {#drawing-ecatalog-image-maps}

För e-kataloger ritar du bildscheman på fliken Kartsidor på skärmen eCatalog. Den här skärmen består av området Bildschema där eCatalog-sidor visas och, till höger, listan Bildschema. När du skapar bildscheman anges deras namn i listan Bildschema.

1. Välj eCatalogs rollover **[!UICONTROL Edit]** -knappen.
1. Välj **[!UICONTROL Map Pages]**.
1. Till vänster på skärmen Kartsidor markerar du den sida du vill ha.
1. I området Bildschema ritar du ett rektangulärt eller flersidigt bildschema:

   * **Rektangulär karta** - Välj verktyget Rektangelbildschema och dra på sidan för att skapa rektangeln.

   * **Polygonkarta** - Välj verktyget Polygonbildschema och markera sedan så många gånger som behövs runt bildens omkrets. När du väljer det här alternativet ritar Adobe Dynamic Media Classic kanterna på bildschemat.

     När du har ritat en bildschema ger Adobe Dynamic Media Classic den ett namn i listan Bildschema. För att bilda namnet lägger Adobe Dynamic Media Classic till ett sekventiellt nummer till namnet på den eCatalog-sida där du arbetar.

1. (Valfritt) I listan Bildschema i dialogrutan [!UICONTROL Name] kan du ange ett nytt namn för bildschemat. Använd inte blanksteg i det namn du anger.
1. Du kan låta tittarna öppna en ny webbsida när de väljer Bildschema. Ange webbsidans URL i URL-kolumnen på listpanelen Bildschema.

   Om du vill göra det enklare att ange URL:er (Href-mallar) väljer du **[!UICONTROL Edit]** och ange en mall.

Se [Använd en mall för att ange JavaScript och URL:er](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. (Valfritt) I listrutan Visa väljer du **[!UICONTROL Rollover Text]** och ange sedan den text som du vill att användarna ska se på skärmen när de flyttar pekarna över bildschemat.
1. (Valfritt) I listrutan Visa väljer du **[!UICONTROL Other Actions]** och anger ett attribut som utlöser en oskärpa eller fokusåtgärd när användarna flyttar pekarna över en bildschema.

   Se [Definiera andra åtgärder för bildscheman](creating-image-maps.md#defining_other_actions_for_image_maps).

1. Välj **[!UICONTROL Save]**.
1. (Valfritt) Välj **[!UICONTROL Preview]** om du vill visa e-katalogen med standardförinställningen för eCatalog Viewer.

Om du vill ta bort en bildschema markerar du dess namn i listan Bildschema och väljer **[!UICONTROL Delete]**. Om du tillfälligt vill inaktivera ett bildschema på en sida utan att ta bort bildschemat, avmarkerar du alternativet På på panelen Bildschema.

## Bädda in multimedia i en e-katalog {#embedding-rich-media-in-an-ecatalog}

Med alternativet Multimedia i eCatalog kan du lägga till videoklipp i MP4-format eller snurruppsättningar i bildscheman som du har lagt till i en e-katalog. När en användare väljer området Bildschema i eCatalog visas den tillhörande rotationsuppsättningen eller videon. Den här funktionen är särskilt användbar om du vill att kunderna ska se ett objekt som används eller se ett objekt från olika vinklar och perspektiv.

Du kan också visa verktygstipstext när kunderna flyttar pekarna över bildschemat så att de vet vad de väljer.

**Så här bäddar du in multimedia i en e-katalog:**

1. Rita en eCatalog Image Map.

   Se [Rita eCatalog-bildscheman](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps).

1. I listrutan Visa väljer du **[!UICONTROL Rich Media]**.
1. I panelen Lägg till resurser till vänster navigerar du till en mapp som innehåller den rotationsuppsättning eller videoresurs (MP4-format) som du vill bädda in.
1. Dra resursen till bildschemat.
1. (Valfritt) I listpanelen Bildschema, under **[!UICONTROL Tool Tip]** kolumnrubriken anger du den text som du vill att tittarna ska se på skärmen när de flyttar sin pekare över bildschemat.
1. Välj **[!UICONTROL Save]**.

## Redigera bildkartor för eCatalog {#editing-ecatalog-image-maps}

Använd följande tekniker för att redigera eCatalog-bildscheman från och med på fliken Kartsidor i eCatalog-skärmen:

* **Justera positionen** - Välj panoreringsverktyget och flytta pekaren nära, men inte över, kartkanten. När pekaren visar en fyrhörig pil drar du hela bildschemat till en ny plats.

  Se [Justera placering, form och storlek för bildscheman](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Ändra form och storlek** - Om du vill ändra storlek på ett rektangulärt bildschema väljer du panoreringsverktyget. Flytta sedan pekaren över en kantlinje eller ett hörn och dra när du ser den dubbelriktade pilikonen. Dra i ett fyrkantigt markeringshandtag om du vill ändra storlek på ett flersidigt bildschema. Om du vill skapa ett markeringshandtag markerar du kanten på bildschemat och drar.

  Se [Justera placering, form och storlek för bildscheman](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Ta bort bildscheman** - Välj panoreringsverktyget, markera bildschemat och markera det sedan **[!UICONTROL Delete]**.

  Om du vill ta bort alla bildscheman från en e-katalog väljer du **[!UICONTROL Order Pages]** och sedan välja **[!UICONTROL Clear Maps]**.

* **Hantera överlappande bildscheman** - Dra om du vill ändra ordningen på bildscheman i listan Bildschema.

  Se [Hantera överlappande bildscheman](creating-image-maps.md#handling_overlapping_image_maps).

* **Kopiera bildscheman till andra sidor** - Välj **[!UICONTROL Copy Maps To]** (Kontrollera att du är på fliken Kartsidor). På skärmen Välj bilder markerar du den eller de sidor där du vill kopiera bildscheman och väljer **[!UICONTROL Select]**.

  Se [Kopiera bildscheman till andra bilder](creating-image-maps.md#copying_image_maps).

>[!NOTE]
>
>Förutom att kopiera bildscheman till olika sidor i en e-katalog kan du kopiera alla bildscheman i en e-katalog till en annan e-katalog. Se [Kopiera bildscheman mellan e-kataloger](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs).

## Granska och importera data från bildschemat {#reviewing-and-importing-image-map-data}

Skärmen Kartsammanfattning innehåller metadata om din eCatalog. Du kan också batchimportera bildschemadata för din eCatalog med början på skärmen Kartsammanfattning. Om du importerar data från bildschemat på det här sättet blir det enklare att ange URL:er för bildschema och överrullningstext.

Om du vill visa fönstret Mappningssammanfattning väljer du alternativet på fliken Kartsidor på skärmen i eCatalog **[!UICONTROL Summary]**.

### Granska sammanfattning av bildschemadata {#review-image-map-data-summary}

1. På skärmen Kartsidor väljer du **[!UICONTROL Summary]**.

   På skärmen Sammanfattning av kartor visas hur många bildscheman, URL:er, beskrivningar av rollover-text och andra åtgärder som finns i din eCatalog.

1. Om det finns överrullningsnyckelfel väljer du felet i **[!UICONTROL Rollover_Key Error]** för att se vad som måste ändras i kalkylbladet för att rätta till felet. Du kan markera och kopiera texten från det här meddelandet och klistra in den i kalkylbladet.
1. Välj **[!UICONTROL Preview]** så att du kan granska en sida i eCatalog Viewer; välj X för att stänga fönstret Sammanfattning och gå tillbaka till skärmen Karta sidor, eller markera **[!UICONTROL Close]** för att återgå till Bläddra.

### Importera data för bildschema {#import-image-map-data}

I stället för att ange bildschemadata på varje sida kan du importera data för hela eCatalog till fönstret Kartsammanfattning. Du importerar bildschemadata i form av en tabbavgränsad fil eller XML DTD. Fälten i filen måste vara i den ordning som visas i fönstret Mappningssammanfattning: Namn, etiketter för innehållsförteckning, kartor, URL:er, överrullningstext, andra åtgärder och söksträngar. Om du importerar data från bildschemat slipper du problem med att ange data i listan Bildschema när du skapar bildschemat.

>[!NOTE]
>
>Innan du importerar data från bildschemat måste du ha skapat bildscheman.

Från och med fönstret Kartsammanfattning följer du de här stegen för att importera bildschemadata för bildscheman som du har skapat:

1. Välj **[!UICONTROL Import Map Data]**.
1. I dialogrutan Importera metadata väljer du **[!UICONTROL Browse]** och välj sedan den tabbavgränsade eller XML DTD-filen.
1. Skriv ett namn på filen i fältet Jobbnamn (var noga med att behålla filtillägget).
1. Välj **[!UICONTROL Upload]**.

## Kopiera bildscheman mellan e-kataloger {#copying-image-maps-between-ecatalogs}

Du kan kopiera alla bildscheman i en e-katalog till en annan e-katalog. Att kopiera bildscheman på det här sättet är ett bekvämt sätt att kopiera bildscheman mellan översättningar på främmande språk i samma eCatalog. För att kopieringen ska lyckas rekommenderar Adobe Dynamic Media Classic att du kopierar mellan e-kataloger med samma antal sidor och samma bilder.

>[!NOTE]
>
>Om den eCatalog som du kopierar bildscheman till redan innehåller bildscheman tas dessa bildscheman bort när kopian görs.

Så här kopierar du alla bildscheman i en e-katalog till en annan eCatalog:

1. Markera e-katalogen med de bildscheman som du vill kopiera och välj e-katalogens överrullning **[!UICONTROL Edit]** -knappen.
1. På fliken Ordna sidor väljer du **[!UICONTROL Copy Maps]**.
1. I dialogrutan Välj resurs markerar du den e-katalog där du vill kopiera bildscheman och väljer sedan **[!UICONTROL Select]**.

Ett varningsmeddelande visas i Adobe Dynamic Media Classic om målkatalogen (den eCatalog som du kopierar bildscheman till) har ett annat antal sidor eller bilder med en annan storlek. Välj **[!UICONTROL Continue]** om du vill kopiera bildscheman trots varningen.
