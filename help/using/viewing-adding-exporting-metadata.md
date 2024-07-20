---
title: Visa, lägga till och exportera metadata
description: Lär dig att visa, lägga till och exportera metadata i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Metadata
role: User
exl-id: 2be50cc7-9a8b-4f7b-8ebf-18a3208654f2
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '2154'
ht-degree: 0%

---

# Visa, lägga till och exportera metadata{#viewing-adding-and-exporting-metadata}

Du kan lagra information som är specifik för de filer du arbetar med i Adobe Dynamic Media Classic. Den här informationen kallas *metadata*. Du kan använda metadata i Adobe Dynamic Media Classic för att ordna, söka, filtrera och sortera dina resurser.

Metadata visas i detaljvyn. Det visas tillsammans med information som genererats av Adobe Dynamic Media Classic. Till exempel datum då filen skapades, publiceringsdatum och nyckelord. Om du vill visa metadata öppnar du resursen i detaljvyn och väljer sedan panelen Metadata. Du kan ange och redigera metadata i detaljvyn.

Vissa metadata bäddas in direkt i en fil. Om en fil innehåller dessa metadata överförs de automatiskt av Adobe Dynamic Media Classic tillsammans med filen. Du kan bädda in metadata i källresurser i Adobe Photoshop, InDesign, Illustrator och andra program. Adobe Dynamic Media Classic känner igen dessa metadata. Du kan också lägga till metadata till enskilda filer på panelen Metadata i detaljvyn. Företagsadministratörer skapar metadatamallar som innehåller metadatafält som kan fyllas i för att vara konsekventa för alla resurser.

Mer information om inbäddade metadata finns i [Extensible Metadata Platform](https://www.adobe.com/products/xmp.html).

## Visa metadata {#view-metadata}

Om du vill visa metadata för en resurs öppnar du resursen i detaljvyn och trycker på panelen Metadata. Om du vill välja en uppsättning metadatafält väljer du ett alternativ på menyn Metadatavy. Adobe Dynamic Media Classic erbjuder följande metadatavyer:

* **Kompakt vy**: En grundläggande lista med värden.

* **IPTC**: Värden som definierats av International Press Telecommunications Council.

* **XMP**: Värden som definieras av det utökningsbara metadataprogrammet.

Administratörer kan skapa metadatavyer. De här vyerna visas även på menyn Metadatavyer.

Mer information om hur du skapar metadatavyer finns i [Metadatavyer](application-setup.md#metadata_views).

## Ange metadata för en resurs manuellt {#manually-enter-metadata-for-an-asset}

1. Öppna resursen i detaljvyn.
1. Öppna panelen Metadata och gör något eller båda av följande:

   * Välj en metadatavy för att bestämma vilka metadatafält som ska visas på panelen.
   * Välj ett förinställt värde och välj sedan **[!UICONTROL Apply]** för att fylla i metadatafält med förinställda värden. Företagsadministratörer skapar dessa förinställda värden.

1. Ange värdena på panelen Metadata.

>[!NOTE]
>
>Om du vill redigera metadata för flera resurser samtidigt markerar du resurserna och går till **[!UICONTROL File]** > **[!UICONTROL Edit Info]**. De ändringar du gör i metadata i fönstret Redigera information gäller alla markerade resurser.

## Lägga till eller redigera nyckelord {#add-or-edit-keywords}

Förutom metadata kan du använda nyckelord för att söka efter och hantera dina resurser.

Om du har lagt till nyckelord till andra filer under den här sessionen, eller om du har tagit bort nyckelord från listan, visas de i tabellen Nyckelordsförslag.

1. Öppna filen i detaljvyn.
1. Välj **[!UICONTROL Keywords]**.
1. Gör något av följande om du vill lägga till nyckelord:

   * Skriv ett nyckelord i textrutan och välj **[!UICONTROL Add]**.
   * Markera ett nyckelord i tabellen **[!UICONTROL Keyword Suggestions]**.

1. Om du vill ta bort ett nyckelord markerar du det och väljer **[!UICONTROL Remove]**. Det går vidare till tabellen Nyckelordsförslag.

>[!NOTE]
>
>Du kan lägga till nyckelord till filer när du överför dem till Adobe Dynamic Media Classic. I dialogrutan Alternativ för överföring av jobb väljer du **[!UICONTROL More Metadata]** och anger nyckelord.
>Se [Överföringsalternativ](uploading-files.md#upload_options).

## Importera metadata {#import-metadata}

I stället för att manuellt ange metadata för en resurs i taget kan du importera metadata för många olika resurser från en tabbavgränsad fil eller XML-fil. Att ange metadata i en tabbavgränsad fil eller XML-fil och importera filen är mindre tidsödande än att ange metadata i enskilda resurser. I den första raden i den tabbavgränsade filen anger du ID:t och namnen på de fält som du vill registrera metadata för. I varje efterföljande rad anger du ett resurs-ID-namn följt av metadatavärden. Fält som inte finns med i den tabbavgränsade filen eller XML-filen ändras inte. Om du vill importera metadata från en XML-fil måste du kontrollera att den överensstämmer med DTD:n.

>[!NOTE]
>
>Du kan skapa en mall för att ange metadata så att de kan importeras på rätt sätt till Adobe Dynamic Media Classic. När du har skapat mallen kan du använda den för att ange metadata.
>Se [Skapa en mall för att ange metadata som ska överföras](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload).

Mer information om standardiserade egenskaper finns på [Adobe XMP Developer Center](https://www.adobe.com/devnet/xmp.html).

1. På panelen Bläddra väljer du de bilder som du vill lägga till metadata för från den tabbavgränsade filen eller XML-filen.
1. Gå till **[!UICONTROL File]** > **[!UICONTROL Import Metadata]**.
1. Välj **[!UICONTROL Browse]** i dialogrutan **[!UICONTROL Upload Metadata]**.
1. I dialogrutan **[!UICONTROL Select files to upload]** väljer du den tabbavgränsade eller XML-fil som innehåller metadata.
1. Ange ett jobbnamn.
1. Välj **[!UICONTROL Upload]**.

### Identifiera olika metadatatyper i importen

Tänk på följande när du identifierar olika metadatatyper som ska importeras:

* Namn på användardefinierade fält identifieras som skapade i **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL User-Defined fields]**. Använd funktionen `Generate file` för att få en lista över alla definierade UDF-filer i rätt importformat.
* XMP metadataegenskaper måste ha det relaterade XMP-prefixet före (egenskap-) namnet. Ett kolon avgränsar prefixet och namnet. Det XMP prefixet finns i **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Schema]**-redigeraren. De tekniska namnen finns i dokumentationen för det relaterade XMP schemat. XMP egenskapsnamn visas inte i funktionen `Generate file`.
* Egenskaper för metadataschema måste ha det relaterade prefixet före (egenskap-) namnet. Ett kolon avgränsar prefixet och namnet. Prefixet och egenskapsnamnen definieras i metadataschredigeraren. Namnen på metadataschemaegenskaperna visas inte i funktionen `Generate file`.

Till exempel: Egenskapen XMP för nyckelord är det XMP schemat &quot;Dublin Core&quot; med prefixet `dc` och `subject` är det tekniska XMP. Prefixet och det tekniska XMP namnet kombineras till det fullständiga egenskapsnamnet för `dc:subject`. I XML-metadataimportformatet måste `dc.subject` vara egenskapsnamnet. I det tabbavgränsade importformatet måste det vara kolumnrubriken.

### Importera nyckelord

Nyckelord kan importeras som kommaavgränsade listor. Om ett kommatecken visas i något av de enskilda värdena kan du undvika det genom att använda ett omvänt snedstreck (\). Ett literalt omvänt snedstreck är det vanliga dubbla snedstrecket (\\).

En metadataimportfil som innehåller värdet `Hello\, World!,back\\slash,foo` för `dc:subject` anger till exempel tre XMP nyckelord för resursen: `Hello, World!,` `back\slash,` och `foo`.

### Importera metadata för XMP och metadatamatchema XMP filer

XML-importen accepterar endast giltig XML. När du importerar XMP- eller metadataschfält läggs namnområdesprefixet till och fungerar här som ett XMP-namnutrymme. Det här namnutrymmet måste deklareras. I taggen på den översta nivån.

Till exempel:

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

### Importera XMP och metadata för metadatamatabell, flikavgränsade filer

Prefixet måste läggas till i den relaterade kolumnrubriken i importfältet.

## Importera metadata (via FTP) {#import-metadata-via-ftp}

Du kan importera metadata för flera filer. Du anger metadata i en tabbavgränsad fil eller XML-fil. Välj sedan **[!UICONTROL Process metadata files]** på sidan Alternativ för överföringsjobb (via fliken FTP).

Kontrollera att data i den tabbavgränsade filen eller XML-filen har rätt format. På den första raden anger du ID-fältet följt av namnen på metadatafälten som ska ändras. I varje efterföljande rad anger du ett resurs-ID-namn följt av metadatavärden. Fält som inte finns med i den tabbavgränsade filen eller XML-filen ändras inte.

Välj **[!UICONTROL Upload]** i fältet Global navigering. Om du vill importera metadata på sidan Överför väljer du fliken **[!UICONTROL Via FTP]** och sedan **[!UICONTROL Job Options]**. I dialogrutan Alternativ för överföring av jobb markerar du **[!UICONTROL Job]** och markerar sedan kryssrutan **[!UICONTROL Process metadata files]**.

## Döp om ID:n i grupp med hjälp av metadata {#batch-rename-ids-using-metadata}

Med metadata som importerats från en tabbavgränsad fil eller XML-fil kan du byta namn på Adobe Dynamic Media Classic-ID:n. Importerade metadata används bara för de bilder som anges i själva metadatafilen. Det spelar ingen roll om bilder är markerade på panelen Bläddra.

Om du vill byta namn på en bilds Adobe Dynamic Media Classic-ID lägger du till en kolumn med namnet *newipsid* i den tabbavgränsade filen eller lägger till ett fält med namnet `new_vc_objectname` i XML-data.

Till exempel:

| | newipsid |
| --- | --- |
| testjacka_1 | Jacket_test_1 |
| testjacka_blå | Jacket_test_2 |

Jobbloggen för metadatajobbet visar vilka ID:n som har namnändrats och vilka som inte har namnändrats.

## Skapa en mall för att ange metadata som ska överföras {#create-a-template-for-entering-metadata-to-upload}

I Adobe Dynamic Media Classic finns ett kommando för att skapa en mall för att spela in metadata. Genom att använda mallen ser du till att metadata anges i rätt format så att de kan överföras korrekt till Adobe Dynamic Media Classic. Så här skapar du en mall för att spela in och importera metadata till Adobe Dynamic Media Classic:

1. Välj bildresurser med metadatafält som du vill använda för mallen.
1. Gå till **[!UICONTROL File]** > **[!UICONTROL Import Metadata]**.
1. För **[!UICONTROL Asset Properties Type]** väljer du **[!UICONTROL Image]**.
1. Välj **[!UICONTROL Tab-delimited Template]**, **[!UICONTROL Asset's XML Metadata]** eller **[!UICONTROL XML DTD]** i listrutan **[!UICONTROL `Generate File`]**.
1. Välj **[!UICONTROL Generate]**.
1. Kopiera data i dialogrutan som visas. Använd dessa data för att konstruera mallen.

## Arbeta med metadatascheman {#working-with-metadata-schemas}

En företagsadministratör kan visa en lista med alla tillgängliga scheman. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Metadata]** > **[!UICONTROL Metadata Schema]** i fältet Global navigering.

Till att börja med är listan med globala standardscheman som XMP dold. De kan visas med hjälp av kryssrutan längst ned i listan.

Företagsadministratören kan skapa ett anpassat schema eller redigera ett befintligt anpassat schema.

Du kan använda redigeraren för metadatamatchning för att utföra följande åtgärder:

| Åtgärd | Beskrivning |
| --- | --- |
| Lägg till | Lägger till en egenskap i schemat. En modal dialogruta samlar in information: ID, Label, Structure och Data Type. |
| Lägg till alternativvärde | Lägger till ett nytt valbart alternativ till en egenskap med strukturen Open Choice eller Closed Choice. Alla alternativvärden har samma typ. Markera själva egenskapen för att aktivera knappen. |
| Redigera | Redigera Label för en egenskap eller ett valfritt värde. Du kan bara ändra etikett-, ID- och typinformation som inte kan ändras. |
| Flytta upp/Flytta ned | Ordningen i schemat återspeglas i användargränssnittet. Om du vill ändra ordningen markerar du en egenskap eller ett valvärde och flyttar den med knapparna. Dra och släpp stöds för närvarande inte. |
| Ta bort | Tar bort en egenskap eller ett urvalsvärde från schemat. Värden tas inte bort från XMP eller databasen. Egenskapen är inte längre tillgänglig för metadatavyer och tas bort från vyn Resursdetaljer. Om egenskapen publicerades på metadataservern utför du en tvingad publicering för att ta bort data från den publika metadataservern. |

Systemet genererar automatiskt ett anpassat schema för användardefinierade fält med prefixet `s7udf`. Schemat består av befintliga användardefinierade fält som redigeras i deras eget inställningsavsnitt.

>[!NOTE]
>
>Ändringar i schemat ändrar aldrig metadata för resursen. De är dock inte synliga för alla funktioner i Adobe Dynamic Media Classic och Metadata Server och kan inte nås efter att de har ändrats. Om det finns metadata för en resurs gör skapandet av det matchande schemat att metadata kan användas i Adobe Dynamic Media Classic och metadataservern.

Metadata Schema Editor är ett grafiskt sätt att lägga till eller redigera ett anpassat företagsschema i Adobe Dynamic Media Classic. Ett prefix, ett namnutrymme och en lista med egenskaper definierar ett schema.

* **[!UICONTROL Name]**: Schemats gränssnittsnamn. Används för att identifiera egenskaperna i metadatavyer och avancerad sökning. Liknar XMP avsnitt som Basic, IPTC, PDF.

* **[!UICONTROL Prefix]**: Teknisk unik identifierare för schemat. Begränsat till bokstäverna a-z och A-Z. Prefixet visas inte i Adobe Dynamic Media Classic-gränssnittet, men används när metadata för en resurs lagras i XMP och i databasen. Prefixet identifierar enkelt metadatafält i metadatasökning på metadataservern eller import.

* **[!UICONTROL Namespace]**: Teknisk unik identifierare för schemat, vanligtvis en URL i formatet `https://your.company.com/name/version/`. Se listan med standardscheman för exempel. Namnutrymmet visas inte i Adobe Dynamic Media Classic-gränssnittet, men används för att lagra metadata i XMP.

* **[!UICONTROL Description]**: Beskrivning av schemat i fri form.

>[!NOTE]
>
>Prefixet och namnutrymmet kan inte redigeras. Om du vill ändra de här egenskaperna måste du ta bort och återskapa schemat.

Egenskaper beskriver de metadata som kan lagras med det här schemat i XMP. En egenskap består av:

| Egenskap | Beskrivning |
| --- | --- |
| ID | Teknisk identifierare för den här egenskapen. ID:t visas inte i Adobe Dynamic Media Classic-gränssnittet, men används när metadata för en resurs lagras i XMP och i databasen. ID:t används för att skapa sökfrågor på metadataservern. ID:t har vissa begränsningar som: `<ul><li>No spaces</li><li>No ".", ":", "$"</li><li>No number as first character</li><li>Best practice is to use a-z or A-Z as first character</li></ul>` <br>När det har skapats går det inte att ändra ID:t. |
| Etikett | Användargränssnittsnamn för den här egenskapen. |
| Struktur | Bestämmer egenskapens typ tillsammans med datatypen. Strukturen kan vara någon av:<ul><li>Enkel typ: ett värde för datatypen</li><li>Sekvens: en lista med värden av samma datatyp</li><li>Öppna alternativ: markera ett objekt i en lista med fördefinierade värden eller ange text. Det kan bara vara av datatypen String eller Integer</li><li>Stängt alternativ: välj ett objekt i en lista med fördefinierade värden (ett popup-fönster eller kombinationsruta)</li></ul> |
| Datatyp | Välj bland följande tillgängliga typer: <ul><li>Sträng</li><li>Heltal</li><li>Float</li><li>Ja/Nej (booleskt)</li><li>Datum</li></ul> |

När egenskapen har strukturen Open Choice eller Closed Choice måste du ange minst ett alternativvärde. Open Choice kan ändras. Stängt val kan inte ändras. Alla urvalsvärden har egenskapens datatyp.

| Egenskap | Beskrivning |
| --- | --- |
| ID | Teknisk identifierare för det här värdet. ID:t visas inte i Adobe Dynamic Media Classic-gränssnittet, men används när metadata för en resurs lagras i XMP och i databasen. ID används i sökfrågor på metadataservern. ID:t får inte innehålla blanksteg. När du har skapat det går det inte att ändra ID:t. |
| Etikett | Gränssnittsnamn för det här värdet. |

>[!MORELIKETHIS]
>
>* [Förinställningar för visningsprogram](application-setup.md#viewer_presets)
>* [Metadataförinställningar](application-setup.md#metadata_presets)
