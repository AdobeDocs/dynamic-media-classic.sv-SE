---
title: Sök efter Dynamic Media Classic-resurser
description: Lär dig söka efter resurser i Adobe Dynamic Media Classic.
uuid: 058209bc-bac4-4d5c-8261-e242a543beaf
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: effef4e7-37c5-42e2-9266-ecd026cad628
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 4b3f690c-7dff-4bf0-9366-085ba918fe6b
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '1373'
ht-degree: 0%

---

# Söka efter resurser i Adobe Dynamic Media Classic{#searching-assets}

Om du vill söka efter filresurser i Adobe Dynamic Media Classic kan du visa resurser efter typ, sortera resurser på panelen Bläddra, utföra en enkel sökning, utföra en avancerad sökning och filtrera efter resurser.

>[!NOTE]
>
>På sidan Personliga inställningar finns alternativ för att välja hur du vill utföra sökningar. Du kan t.ex. välja en standardsöktyp och välja om användardefinierade fält ska inkluderas i sökningar. Mer information finns i [Personliga inställningar](personal-setup.md#personal_setup).

## Visa resurser efter typ {#viewing-assets-by-type}

Om du bara vill visa filer av en viss typ när du bläddrar, går du till resursbiblioteket till vänster i dialogrutan **[!UICONTROL Show]** väljer du en filtyp. Endast resurser av den typ som du väljer att visa visas i resursbiblioteket.

>[!NOTE]
>
>Om du inte ser panelen Resursbibliotek till vänster väljer du den högra triangelpilen till vänster, halvvägs nedåt i Adobe Dynamic Media Classic-fönstret, för att öppna resursbiblioteket.)

## Sortera filer i panelen Bläddra {#sorting-files-in-the-browse-panel}

Om du vill sortera innehållet i en mapp eller sökresultaten som visas i panelen Bläddra till höger väljer du alternativet i fältet Global navigering **[!UICONTROL Sort]** och välj sedan ett alternativ. Alternativen är **[!UICONTROL Name]**, **[!UICONTROL Size (KB)]**, **[!UICONTROL Type]**, **[!UICONTROL Date Created]** och **[!UICONTROL Last Modified]**.

Du kan också välja **[!UICONTROL Ascending]** eller **[!UICONTROL Descending]** om du vill sortera resurser i stigande eller fallande ordning efter de villkor du väljer.

I listvyn kan du sortera genom att klicka på ett kolumnnamn.

## Genomför en enkel sökning {#conducting-a-simple-search}

Använd sökfältet i resursbiblioteket för att utföra enkla sökningar. Du kan söka efter objekt efter namn eller söka efter objekt vars metadata innehåller ett nyckelord.

1. I resursbiblioteket i **[!UICONTROL Folders]** markerar du mappen som du vill söka i en viss mapp och dess undermappar.
1. Till vänster om sökfältet i resursbiblioteket väljer du **[!UICONTROL Magnifying Glass]** för att öppna listrutan.
1. I listrutan väljer du ett alternativ som beskriver hur smal eller bred du vill att sökningen ska vara. Du kan välja **[!UICONTROL Within All Files & Folders]**, **[!UICONTROL Within Selected Folder]**, eller **[!UICONTROL Within Selected Folder & Subfolders]**.
1. Ange en sökterm i fältet Sök.
1. Till höger om sökfältet väljer du **[!UICONTROL Go]** eller tryck **[!UICONTROL Enter]**.

   Resultatet av sökningen visas i panelen Bläddra till höger.

<!-- Does not appear to be working anymore >[!NOTE]
>
>Adobe Dynamic Media Classic tracks searches. To run a search a second time, select **[!UICONTROL Search]** and choose the name of a search at the bottom of the Search menu. -->

## Utföra en avancerad sökning {#conducting-an-advanced-search}

I resursbiblioteket, direkt under sökfältet, väljer du **[!UICONTROL Advanced Search]** om du vill söka med många villkor, inklusive värden i metadatafält.

Ange något av följande villkor i den avancerade sökningen:

* **Filtrera efter resurstyp** - Begränsa sökningen till en resurstyp genom att välja en resurstyp på menyn.

* **Filer och mappar** - Välj var du vill söka: **[!UICONTROL Within All Files & Folders]**, **[!UICONTROL Within Selected Folder]**, eller **[!UICONTROL Within Selected Folder & Subfolders]**.

* **Alla publiceringslägen** - Sök efter filer som har markerats som klara för publicering, som inte har markerats som klara för publicering eller alla filer.

* **Villkor** - Om du anger metadatavillkor för sökning väljer du om sökningen måste matcha alla villkor (en ALL-sökning) eller något villkor (en OR-sökning).

* **Sökvillkor** - Skapa ett eller flera sökfält för sökning av metadata. Så här skapar du sökfält:

   1. I Avancerad sökning, under **[!UICONTROL Search criteria]** och till vänster om **[!UICONTROL Add a Field]** väljer du den nedåtriktade triangelpilen för att öppna listrutan. Välj en metadatavy. Du kan välja **[!UICONTROL All properties with values]**, **[!UICONTROL Compact View]**, **[!UICONTROL IPTC]**, **[!UICONTROL Metadata Server Publish Fields]**, eller **[!UICONTROL XMP]**.
   1. Välj **[!UICONTROL Add a Field]** och välj ett fältnamn.
   1. Välj en **[!UICONTROL Contains]** alternativ: **[!UICONTROL Contains]**, **[!UICONTROL Does Not Contain]**, **[!UICONTROL Begins With]**, **[!UICONTROL Ends With]**, eller **[!UICONTROL Equals]**.
   1. För numeriska fält väljer du ett värde eller anger ett anpassat datumintervall.
   1. (Valfritt) Upprepa steg 1-4 om du vill skapa fler sökfält.

Välj **[!UICONTROL Remove search field]** -ikon (cirkel med &quot;X&quot; inuti) så att sökfältet tas bort.

I det nedre högra hörnet av panelen Avancerad sökning väljer du **[!UICONTROL Search]** för att börja söka. Resultatet av sökningen visas i panelen Bläddra till höger. Du kan ändra alla sökvillkor och välja **[!UICONTROL Search]** för att köra sökningen igen.

Välj **[!UICONTROL Clear]** om du vill ta bort sökvillkoren och starta en ny sökning. Välj **[!UICONTROL Close]** när du har avslutat sökningen för att stänga sökpanelen.

## Filtrera resurser med metadata {#filter-assets-using-metadata}

Filtrera resurser på fliken Filter i resursbiblioteket. Om du vill filtrera resurser använder du metadatavärden som villkor. När du har valt ett metadatafält som du vill filtrera på visas alla metadatavärden som har angetts i det valda fältet på fliken Filter. Här visas även antalet resurser som tilldelats varje värde. I en filteråtgärd på **[!UICONTROL Creator]** metadatafält, **[!UICONTROL Filters]** På fliken visas alla namn som du har angett i **[!UICONTROL Creator]** metadatafält för olika resurser. Den visar också för varje namn antalet resurser som har tilldelats namnet. Sedan väljer du ett metadatavärde för att se alla resurser som har tilldelats det värdet. I exemplet väljer du `Prairie Cat` metadatavärde för att visa alla resurser där namnet `Prairie Cat` har angetts i **[!UICONTROL Creator]** metadatafält. Du kan filtrera med hjälp av mer än ett metadatafält som filtreringskriterium.

Du kan spara filteråtgärder för att köra dem många gånger.

>[!NOTE]
>
>Endast metadatafält i standardmetadatavyn kan användas för filteråtgärder. På sidan Metadatavyer visas namnet på standardmetadatavyn.

Se [Metadatavyer](application-setup.md#metadata_views).

### Köra en filteråtgärd {#running-a-filter-operation}

Följ de här stegen för att hitta resurser genom att filtrera med deras metadatavärden:

1. I resursbiblioteket väljer du **[!UICONTROL Filters]** -fliken.

   Kriterierna för den tidigare filteråtgärden visas i filterrutan. Panelen Filter är uppdelad i paneler där varje panel representerar ett metadatafält. Använd panelerna för att välja vilka metadatafält som ska filtreras med och inom varje fält för att välja ett metadatavärde för filteråtgärden.

   Om du vill köra en filteråtgärd som du har skapat och sparat väljer du **[!UICONTROL Select Preset]** och välj sedan åtgärdens namn på menyn.

   Se [Spara, upprepa och ta bort filteråtgärder](searching-assets.md#saving_repeating_and_deleting_filter_operations).

1. Välj **[!UICONTROL Field]** Följ sedan dessa instruktioner på en panel så att du kan visa filtermenyn och skapa filteråtgärden:

   * **Välj ett metadatafält** - Välj fältets namn på filtreringsmenyn.

     >[!NOTE]
     >
     >Endast namnen på metadatafälten i standardmetadatavyn visas på filtreringsmenyn.

     Se [Metadatavyer](application-setup.md#metadata_views).

   * **Lägg till ett metadatafält** - Välj **[!UICONTROL Add a Panel]**. När panelen visas på filterpanelen väljer du dess **[!UICONTROL Field]** och välj namnet på ett metadatafält på filtreringsmenyn.

   * **Ta bort ett metadatafält** - Välj **[!UICONTROL Remove This Panel]** på filtreringsmenyn.

   När du väljer ett metadatafält visas följande på panelen:

   * Alla metadatavärden som anges i fältet.
   * För varje metadatavärde, antalet resurser som anges av värdet.

1. Upprepa steg 2 så många gånger som behövs för att lista alla metadatafält för filteråtgärden på paneler.
1. Välj ett metadatavärde att filtrera på på varje panel. Du kan inte markera mer än ett metadatavärde på varje panel.

   Resurser som matchar alla värden som du har valt visas i panelen Bläddra.

   >[!NOTE]
   >
   >Om du tillfälligt vill ta bort ett fält från filteråtgärden markerar du **[!UICONTROL Deselect All]**. Det här alternativet visas högst upp på varje panel, ovanför metadatavärden.

1. (Valfritt) Om du vill spara filteråtgärden och kunna köra den senare väljer du **[!UICONTROL Select Preset]** > **[!UICONTROL Save Current As New Presets]** och ange sedan ett namn i **[!UICONTROL Save]** -dialogrutan.

### Spara, upprepa och ta bort filteråtgärder {#saving-repeating-and-deleting-filter-operations}

Följ dessa instruktioner på fliken Filter så att du kan spara, upprepa och ta bort filteråtgärder:

* **Spara en filteråtgärd** - Gå till **[!UICONTROL Select Preset]** > **[!UICONTROL Save Current As New Presets]** och ange sedan ett namn i **[!UICONTROL Save]** -dialogrutan.

* **Upprepa en filteråtgärd** - Välj **[!UICONTROL Select Preset]** och välj namnet på en filteråtgärd på menyn. I menyn visas filteråtgärder som du har sparat.

* **Ta bort en filteråtgärd från menyn Välj förinställning** - Kör filteråtgärden. Gå sedan till **[!UICONTROL Select Preset]** > **[!UICONTROL Delete Preset]** på menyn.

## Använda metadataservern {#using-the-metadata-server}

Metadataservern är ett offentligt API som du kan använda för att söka efter resurser via metadata via http-begäranden.

Om du vill konfigurera metadataservern går du till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Metadata Server]**.

På sidan Publicera för metadataserver kan du ange följande alternativ:

* **[!UICONTROL Instant Publish]** - Överför automatiskt alla metadataändringar när de görs, inklusive nya resurser, nyckelordsändringar o.s.v.

* **[!UICONTROL XMP Packet]** - Publicerar XMP. Paketet används inte för sökning, men innehåller den senaste XMP.

* **[!UICONTROL Keywords]** - Publicerar dina nyckelord till metadataservern för användning i sökningar.

* **[!UICONTROL Metadata Server Publish Fields]** - Markera de fält som ska inkluderas i metadata. Med det här alternativet kan du avgöra hur mycket information om dina resurser som är tillgänglig för allmänheten. Dessa fält visas också i metadatavyer, men kan bara ändras på metadataservern.

Välj **[!UICONTROL Publish Now]** för att starta jobbet. En bekräftelse visas som talar om att jobbet har startat.

>[!MORELIKETHIS]
>
>* [Navigeringsgrunder](navigation-basics.md#navigation_basics)
>* [Visa, lägga till och exportera metadata](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
