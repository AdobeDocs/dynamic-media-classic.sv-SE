---
title: Visa, lägga till och exportera metadata
seo-title: Visa, lägga till och exportera metadata
description: 'null'
seo-description: Lär dig hur du visar, lägger till och exporterar metadata.
uuid: a5254c51-9e04-45ae-8236-3eab2925e5fc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 5414b4f5-6e05-468c-8725-385423596342
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '2262'
ht-degree: 0%

---


# Visa, lägga till och exportera metadata{#viewing-adding-and-exporting-metadata}

Du kan lagra information som är specifik för de filer du arbetar med i Dynamic Media Classic; den här informationen kallas *metadata*. Du kan använda metadata i Dynamic Media Classic för att ordna, söka, filtrera och sortera dina resurser.

Metadata visas i detaljvyn tillsammans med information som genereras av Dynamic Media Classic, till exempel datum då filen skapades, publiceringsdatum och nyckelord. Om du vill visa metadata öppnar du resursen i detaljvyn och väljer panelen Metadata. Du kan ange och redigera metadata i detaljvyn.

Vissa metadata bäddas in direkt i en fil. Om en fil innehåller dessa metadata överförs den automatiskt med filen. Du kan bädda in metadata i källmaterial i Adobe Photoshop, InDesign, Illustrator och andra program; Dynamic Media Classic känner igen dessa metadata. Du kan också lägga till metadata till enskilda filer på panelen Metadata i detaljvyn. Företagsadministratörer skapar metadatamallar som innehåller metadatafält som kan fyllas i för att vara konsekventa för alla resurser.

Mer information om inbäddade metadata finns i [www.adobe.com/go/learn_s7_xmp_en](https://www.adobe.com/go/learn_s7_xmp_en).

## Visa metadata {#view-metadata}

Om du vill visa metadata för en resurs öppnar du resursen i detaljvyn och klickar på panelen Metadata. Välj sedan ett alternativ på menyn Metadatavy för att välja en uppsättning metadatafält. Dynamic Media Classic erbjuder följande metadatavyer:

* **Komprimerad vy** En grundläggande lista med värden.

* **IPTC**-värden enligt International Press Telecommunications Council.

* **XMP** värden som definieras av den utbyggbara metadataplattformen.

Administratörer kan skapa metadatavyer. De här vyerna visas även på menyn Metadatavyer. Mer information om hur du skapar metadatavyer finns i [Metadatavyer](application-setup.md#metadata_views).

## Ange metadata för en resurs manuellt {#manually-enter-metadata-for-an-asset}

1. Öppna resursen i detaljvyn.
1. Öppna panelen Metadata och gör något eller båda av följande:

   * Välj en metadatavy för att bestämma vilka metadatafält som ska visas på panelen.
   * Välj ett förinställt värde och klicka på Använd för att fylla i metadatafält med förinställda värden. Företagsadministratörer skapar dessa förinställda värden.

1. Ange värden på panelen Metadata.

>[!NOTE]
>
>Om du vill redigera metadata för flera resurser samtidigt markerar du resurserna och väljer Arkiv > Redigera information. De ändringar du gör i metadata i fönstret Redigera information gäller för alla markerade resurser.

## Lägga till eller redigera nyckelord {#add-or-edit-keywords}

Förutom metadata kan du använda nyckelord som hjälp när du söker efter och hanterar resurser.

Om du har lagt till nyckelord till andra filer under den här sessionen, eller om du har tagit bort nyckelord från listan, visas de i tabellen Nyckelordsförslag.

1. Öppna filen i detaljvyn.
1. Klicka på Nyckelord.
1. Gör något av följande om du vill lägga till nyckelord:

   * Skriv ett nyckelord i textrutan och klicka på Lägg till.
   * Klicka på ett nyckelord i tabellen Nyckelordsförslag.

1. Om du vill ta bort ett nyckelord markerar du det och klickar på Ta bort. Det går till tabellen Nyckelordsförslag.

>[!NOTE]
>
>Du kan lägga till nyckelord till filer när du överför dem till Dynamic Media Classic. I dialogrutan Alternativ för överföringsjobb väljer du Övriga metadata och anger nyckelord. Se [Överföringsalternativ](uploading-files.md#upload_options).

## Importera metadata {#import-metadata}

I stället för att manuellt ange metadata för en resurs i taget kan du importera metadata för många olika resurser från en tabbavgränsad fil eller XML-fil. Att ange metadata i en tabbavgränsad fil eller XML-fil och importera filen är mindre tidsödande än att ange metadata i enskilda resurser. I den första raden i den tabbavgränsade filen anger du ID:t och namnen på de fält som du vill registrera metadata för. I varje efterföljande rad anger du ett resurs-ID-namn följt av metadatavärden. Fält som inte finns med i den tabbavgränsade filen eller XML-filen ändras inte. Om du vill importera metadata från en XML-fil måste du kontrollera att den överensstämmer med DTD:n.

>[!NOTE]
>
>Du kan skapa en mall för att ange metadata så att de kan importeras korrekt till Dynamic Media Classic. När du har skapat mallen kan du använda den för att ange metadata. Se [Skapa en mall för att ange metadata som ska överföras](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload).

Mer information om standardiserade egenskaper finns i: https://www.adobe.com/devnet/xmp.html

1. På panelen Bläddra väljer du de bilder som du vill lägga till metadata för från den tabbavgränsade filen eller XML-filen.
1. Klicka på **Arkiv** > **Importera metadata**.
1. Klicka på **Bläddra i dialogrutan** Överför metadata ****.
1. I dialogrutan **Välj filer som ska överföras** markerar du den tabbavgränsade filen eller XML-filen med metadata.
1. Ange ett jobbnamn.
1. Klicka på **Överför**.

**Identifiera olika metadatatyper i importen**

Tänk på följande när du identifierar olika metadatatyper som ska importeras:

* Användardefinierade fält identifieras med sitt namn enligt inställningarna > Programinställningar > Metadata > Användardefinierade fält. Använd filfunktionen Generera för att få en lista över alla definierade UDF-filer i rätt importformat.
* XMP metadataegenskaper måste ha det relaterade XMP-prefixet före (egenskap-) namnet. Ett kolon avgränsar prefixet och namnet. Det XMP prefixet finns i Konfigurera > Programinställningar > Metadata > Metadataschredigeraren. De tekniska namnen finns i dokumentationen för det relaterade XMP schemat. Observera att XMP egenskapsnamn inte visas i funktionen Generera fil.
* Egenskaper för metadataschema måste ha det relaterade prefixet före (egenskap-) namnet. Ett kolon avgränsar prefixet och namnet. Prefixet och egenskapsnamnen definieras i metadataschredigeraren. Observera att namn på metadataschemaegenskaper inte visas i funktionen Generera fil.

Till exempel: Egenskapen XMP för nyckelord är det XMP schemat &quot;Dublin Core&quot; med prefixet &quot;dc&quot; och &quot;subject&quot; är det tekniska XMP. Prefixet och det tekniska XMP namnet kombineras till det fullständiga egenskapsnamnet&quot;dc:subject&quot;. I XML-metadataimportformatet måste &quot;dc.subject&quot; vara egenskapsnamnet. I det tabbavgränsade importformatet måste det vara column-header.

**Importera nyckelord**

Nyckelord kan importeras som kommaseparerade listor. Om ett kommatecken visas i något av de enskilda värdena måste det föregås av ett omvänt snedstreck (\). Ett literalt omvänt snedstreck är det vanliga dubbla snedstrecket (\\).

En metadataimportfil som innehåller värdet &quot;Hello\, World!,back\\slash,foo&quot; för &quot;dc:subject&quot; anger tre XMP nyckelord för resursen: &quot;Hello, World!&quot;, &quot;back\slash&quot; och &quot;foo.&quot;

**Importera metadata för XMP och metadatamatchema XMP filer**

XML-importen accepterar endast giltig XML. När du importerar XMP- eller metadataschefält läggs namnområdesprefixet till och fungerar här som ett XMP-namnutrymme. Detta namnutrymme måste deklareras t.ex. i taggen på den översta nivån.

Exempel:

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

**Importera XMP- och metadatamatametadataavgränsade filer**

Prefixet måste läggas till i den relaterade kolumnrubriken i importfältet.

## Importera metadata (via FTP) {#import-metadata-via-ftp}

Du kan importera metadata för flera filer genom att ange metadata i en tabbavgränsad fil eller XML-fil och välja alternativet Bearbeta metadatafiler på skärmen Överför (via FTP).

Kontrollera att data i den tabbavgränsade filen eller XML-filen har rätt format. På den första raden anger du ID-fältet följt av namnen på metadatafälten som ska ändras. I varje efterföljande rad anger du ett resurs-ID-namn följt av metadatavärden. Fält som inte finns med i den tabbavgränsade filen eller XML-filen ändras inte.

Klicka på knappen Överför i det globala navigeringsfältet och välj fliken Via FTP på jobbskärmen för att importera metadata. Klicka sedan på Alternativ för jobb. Välj Bearbeta metadatafiler i dialogrutan Alternativ för överföringsjobb.

## Döp om ID:n i grupp med hjälp av metadata {#batch-rename-ids-using-metadata}

Med hjälp av metadata som importerats från en tabbavgränsad fil eller XML-fil kan du byta namn på Dynamic Media Classic ID:n. Importerade metadata används bara för de bilder som anges i själva metadatafilen. Det spelar ingen roll om bilder är markerade på panelen Bläddra.

Om du vill byta namn på en bilds Dynamic Media Classic ID lägger du till en kolumn med namnet *newipsid* i den tabbavgränsade filen eller lägger till ett fält med namnet* new_vc_objectname* i XML-data.

Exempel:

| ipsid | newipsid |
|--- |--- |
| testjacka_1 | Jacket_test_1 |
| testjacka_blå | Jacket_test_2 |


Jobbloggen för metadatajobbet visar vilka ID som har ändrats och vilka som inte gjorde det.

## Skapa en mall för att ange metadata som ska överföras {#create-a-template-for-entering-metadata-to-upload}

Med Dynamic Media Classic kan du skapa en mall för att spela in metadata. Genom att använda mallen ser du till att metadata anges i rätt format så att de kan överföras korrekt till Dynamic Media Classic. Följ de här stegen för att skapa en mall för att spela in och importera metadata till Dynamic Media Classic:

1. Välj bildresurser med metadatafält som du vill använda för mallen.
1. Välj Arkiv > Importera metadata.
1. Välj Bild som resursegenskapstyp.
1. Välj Tabbavgränsad mall, Resursens XML-metadata eller XML-DTD på menyn Generera fil.
1. Klicka på Generera.
1. Kopiera data i dialogrutan som visas. Använd dessa data för att konstruera mallen.

## Arbeta med metadatascheman {#working-with-metadata-schemas}

En företagsadministratör kan visa en lista med alla tillgängliga scheman. Öppna Programinställningar -> Metadata -> Metadataschema.

Till att börja med är listan med globala standardscheman som XMP dold. De kan visas med hjälp av kryssrutan längst ned i listan.

Företagsadministratören kan skapa ett nytt anpassat schema eller redigera ett befintligt anpassat schema.

Du kan använda redigeraren för metadatamatchning för att utföra följande åtgärder:

| Åtgärd | Beskrivning |
|--- |--- |
| Lägg till | Lägger till en ny egenskap i schemat. En modal dialogruta samlar in informationen: ID, etikett, struktur och datatyp. |
| Lägg till alternativvärde | Lägger till ett nytt valbart alternativ till en egenskap med strukturen Open Choice eller Closed Choice. Alla alternativvärden har samma typ. Du måste markera själva egenskapen för att aktivera knappen. |
| Redigera | Redigera Label för en egenskap eller ett valfritt värde. Du kan bara ändra etikett-, ID- och typinformation som inte kan ändras. |
| Flytta upp/Flytta ned | Ordningen i schemat återspeglas i användargränssnittet. Om du vill ändra ordningen markerar du en egenskap eller ett valvärde och flyttar den med knapparna. Dra och släpp stöds för närvarande inte. |
| Ta bort | Tar bort en egenskap eller ett urvalsvärde från schemat. Detta tar inte bort värden från XMP eller databasen. Egenskapen är inte längre tillgänglig för metadatavyer och tas bort från vyn Resursdetaljer.Om egenskapen publicerades på metadataservern utför du en tvingad publicering för att ta bort data från den offentliga metadataservern. |

Systemet genererar automatiskt ett anpassat schema för användardefinierade fält med prefixet &quot;s7udf&quot;. Detta är de befintliga användardefinierade fälten och redigeras i ett eget inställningsavsnitt.

>[!NOTE]
>
>Ändringar i schemat ändrar aldrig metadata för resursen. De är dock inte synliga för alla funktioner i Dynamic Media Classic och Metadata Server och går inte att komma åt när de har ändrats. Om det finns metadata för en resurs gör skapandet av det matchande schemat att metadata kan användas i Dynamic Media Classic och Metadataservern.

Metadata Schema Editor erbjuder ett grafiskt sätt att lägga till eller redigera ett anpassat företagsschema i Dynamic Media Classic. Ett schema definieras av ett prefix, ett namnutrymme och en lista med egenskaper.

* Namn

   Schemats gränssnittsnamn. Används för att identifiera egenskaperna i metadatavyer och avancerad sökning. Liknar XMP avsnitt som Basic, IPTC, PDF.

* Prefix

   Teknisk unik identifierare för schemat. Begränsat till bokstäverna a-z och A-Z. Prefixet visas inte i gränssnittet för Dynamic Media Classic, men används när metadata för en resurs lagras i XMP och i vår databas. Prefixet används för att unikt identifiera metadatafält i metadatasökning på Metadataservern eller import.

* Namnutrymme

   Teknisk unik identifierare för schemat, vanligtvis en URL i formuläret `https://your.company.com/name/version/`. Se listan med standardscheman för exempel. Namnutrymmet visas inte i det dynamiska Media Classic-gränssnittet, men används för att lagra metadata i XMP.

* Beskrivning

   Beskrivning av schemat i fritt format.

>[!NOTE]
>
>Prefixet och namnutrymmet kan inte redigeras. Om du vill ändra de här egenskaperna måste du ta bort och återskapa schemat.

Egenskaper beskriver de metadata som kan lagras med det här schemat i XMP. En egenskap består av:

| Egenskap | Beskrivning |
|--- |--- |
| ID | Teknisk identifierare för den här egenskapen. ID:t visas inte i gränssnittet för Dynamic Media Classic, utan används när metadata för en resurs lagras i XMP och i vår databas. ID:t används för att skapa sökfrågor på metadataservern. ID:t har vissa begränsningar som: <ul><li>Inga blanksteg</li><li>Nej &quot;.&quot;, &quot;:&quot;, &quot;$&quot;</li><li>Inget tal som första tecken</li><li>Bästa sättet är att använda a-z eller A-Z som första tecken</li></ul> <br>När du har skapat det går det inte att ändra ID:t. |
| Etikett | Användargränssnittsnamn för den här egenskapen. |
| Struktur | Anger egenskapens typ tillsammans med datatypen. Strukturen kan vara någon av:<ul><li>Enkel typ: ett värde för datatypen</li><li>Sekvens: en lista med värden av samma datatyp</li><li>Open Choice: markera ett objekt i en lista med fördefinierade värden, eller ange fritext. Kan bara vara av datatypen String eller Integer</li><li>Stängt val: markera ett objekt i en lista med fördefinierade värden (ett popup-fönster eller kombinationsruta)</li></ul> |
| Datatyp | Välj bland följande tillgängliga typer: <ul><li>Sträng</li><li>Heltal</li><li>Float</li><li>Ja/Nej (booleskt)</li><li>Datum</li></ul> |


När egenskapen har strukturen Open Choice eller Closed Choice måste du ange minst ett Choice-värde. Open Choice kan ändras. Stängt val kan inte ändras. Alla alternativvärden har egenskapens datatyp.

| Egenskap | Beskrivning |
|--- |--- |
| ID | Teknisk identifierare för det här värdet. ID:t visas inte i gränssnittet för Dynamic Media Classic, men används när metadata för en resurs lagras i XMP och i databasen. ID:t används i sökfrågor på metadataservern. ID:t får inte innehålla blanksteg. När du har skapat det går det inte att ändra ID:t. |
| Etikett | Gränssnittsnamn för det här värdet. |

>[!MORELIKETHIS]
>
>* [Förinställningar för visningsprogram](application-setup.md#viewer_presets)
>* [Metadataförinställningar](application-setup.md#metadata_presets)

