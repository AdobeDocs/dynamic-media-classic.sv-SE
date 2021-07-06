---
title: Söka efter resurser
description: Lär dig hur du söker efter resurser.
uuid: 058209bc-bac4-4d5c-8261-e242a543beaf
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: effef4e7-37c5-42e2-9266-ecd026cad628
feature: Dynamic Media Classic,Resurshantering
role: User
exl-id: 4b3f690c-7dff-4bf0-9366-085ba918fe6b
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '1372'
ht-degree: 0%

---

# Söka efter resurser{#searching-assets}

Om du vill söka efter filresurser i Dynamic Media Classic kan du visa resurser efter typ, sortera resurser i panelen Bläddra, utföra en enkel sökning, utföra en avancerad sökning och filtrera efter resurser.

>[!NOTE]
>
>På sidan Personliga inställningar finns alternativ för att välja hur du vill utföra sökningar. Du kan t.ex. välja en standardsöktyp och välja om användardefinierade fält ska inkluderas i sökningar. Mer information finns i [Personliga inställningar](personal-setup.md#personal_setup).

## Visa resurser efter typ {#viewing-assets-by-type}

Om du bara vill visa filer av en viss typ när du bläddrar väljer du en filtyp i resursbiblioteket till vänster i listrutan **[!UICONTROL Show]**. Endast resurser av den typ som du väljer att visa visas i resursbiblioteket.

>[!NOTE]
>
>Om du inte ser panelen Resursbibliotek till vänster klickar du på den högra triangelpilen till vänster, halvvägs nedåt i Dynamic Media Classic-fönstret, så öppnas resursbiblioteket.)

## Sortera filer i panelen Bläddra {#sorting-files-in-the-browse-panel}

Om du vill sortera innehållet i en mapp eller sökresultaten som visas i panelen Bläddra till höger klickar du på **[!UICONTROL Sort]** i fältet Global navigering och väljer sedan ett alternativ. Alternativen är **[!UICONTROL Name]**, **[!UICONTROL Size (KB)]**, **[!UICONTROL Type]**, **[!UICONTROL Date Created]** och **[!UICONTROL Last Modified]**.

Du kan också välja **[!UICONTROL Ascending]** eller **[!UICONTROL Descending]** om du vill sortera resurser i stigande eller fallande ordning efter de villkor du väljer.

I listvyn kan du sortera genom att klicka på ett kolumnnamn.

## Genomföra en enkel sökning {#conducting-a-simple-search}

Använd sökfältet i resursbiblioteket för att utföra enkla sökningar. Du kan söka efter objekt efter namn eller söka efter objekt vars metadata innehåller ett nyckelord.

1. I resursbiblioteket i panelen **[!UICONTROL Folders]** markerar du mappen som du vill söka i en viss mapp och dess undermappar.
1. Klicka på ikonen **[!UICONTROL Magnifying Glass]** till vänster om sökfältet i resursbiblioteket för att öppna listrutan.
1. I listrutan väljer du ett alternativ som beskriver hur smal eller bred du vill att sökningen ska vara. Du kan välja **[!UICONTROL Within All Files & Folders]**, **[!UICONTROL Within Selected Folder]** eller **[!UICONTROL Within Selected Folder & Subfolders]**.
1. Ange en sökterm i fältet Sök.
1. Klicka på **[!UICONTROL Go]** eller tryck på **[!UICONTROL Enter]** till höger om sökfältet.

   Resultatet av sökningen visas i panelen Bläddra till höger.

<!-- Does not appear to be working anymore >[!NOTE]
>
>Dynamic Media Classic tracks searches. To run a search a second time, click **[!UICONTROL Search]** and choose the name of a search at the bottom of the Search menu. -->

## Använda avancerad sökning {#conducting-an-advanced-search}

I resursbiblioteket, direkt under sökfältet, klickar du på **[!UICONTROL Advanced Search]** för att söka efter många villkor, inklusive värden i metadatafält.

Ange något av följande villkor i den avancerade sökningen:

* **Filtrera efter resurstyp**  - Begränsa sökningen till en resurstyp genom att välja en resurstyp på menyn.

* **Filer och mappar**  - Välj var du vill söka:  **[!UICONTROL Within All Files & Folders]**,  **[!UICONTROL Within Selected Folder]** eller  **[!UICONTROL Within Selected Folder & Subfolders]**.

* **Alla publiceringslägen**  - Sök efter filer som har markerats som klara för publicering, som inte har markerats som klara för publicering eller alla filer.

* **Villkor**  - Om du anger metadatavillkor för sökning väljer du om sökningen måste matcha alla villkor (en ALL-sökning) eller något villkor (en OR-sökning).

* **Sökvillkor**  - Skapa ett eller flera sökfält för sökning av metadata. Så här skapar du sökfält:

   1. I Avancerad sökning, under rubriken **[!UICONTROL Search criteria]** och till vänster om menyn **[!UICONTROL Add a Field]** klickar du på den nedrullningsbara triangelpilen för att öppna listrutan. Välj en metadatavy. Du kan välja **[!UICONTROL All properties with values]**, **[!UICONTROL Compact View]**, **[!UICONTROL IPTC]**, **[!UICONTROL Metadata Server Publish Fields]** eller **[!UICONTROL XMP]**.
   1. Klicka på listrutan **[!UICONTROL Add a Field]** och välj ett fältnamn.
   1. Välj ett **[!UICONTROL Contains]**-alternativ: **[!UICONTROL Contains]**, **[!UICONTROL Does Not Contain]**, **[!UICONTROL Begins With]**, **[!UICONTROL Ends With]** eller **[!UICONTROL Equals]**.
   1. För numeriska fält väljer du ett värde eller anger ett anpassat datumintervall.
   1. (Valfritt) Upprepa steg 1-4 om du vill skapa fler sökfält.

Klicka på ikonen **[!UICONTROL Remove search field]** (cirkel med &quot;X&quot; inuti) så att sökfältet tas bort.

Klicka på **[!UICONTROL Search]** längst ned till höger på panelen Avancerad sökning för att börja söka. Resultatet av sökningen visas i panelen Bläddra till höger. Du kan ändra alla sökvillkor och klicka på **[!UICONTROL Search]** för att köra sökningen igen.

Klicka på **[!UICONTROL Clear]** för att rensa sökvillkoren och starta en ny sökning. Klicka på **[!UICONTROL Close]** när du är klar med sökningen för att stänga sökpanelen.

## Filtrera resurser med metadata {#filter-assets-using-metadata}

Filtrera resurser på fliken Filter i resursbiblioteket. Om du vill filtrera resurser använder du metadatavärden som villkor. När du har valt ett metadatafält som du vill filtrera på visas alla metadatavärden som har angetts i det valda fältet på fliken Filter. Här visas även antalet resurser som tilldelats varje värde. I en filteråtgärd i metadatafältet för Skapare visas till exempel alla namn som har angetts i metadatafältet för Skapare för olika resurser på fliken Filter. Den visar också för varje namn antalet resurser som har tilldelats namnet. Klicka sedan på ett metadatavärde för att visa alla resurser som har tilldelats det värdet. I exemplet klickar du på metadatavärdet för Paririe Cat för att visa alla resurser där namnet Prairie Cat angavs i metadatafältet för Skapare. Du kan filtrera med hjälp av mer än ett metadatafält som filtreringskriterium.

Du kan spara filteråtgärder för att köra dem många gånger.

>[!NOTE]
>
>Endast metadatafält i standardmetadatavyn kan användas för filteråtgärder. På sidan Metadatavyer visas namnet på standardmetadatavyn.

Se [Metadatavyer](application-setup.md#metadata_views).

### Köra en filteråtgärd {#running-a-filter-operation}

Följ de här stegen för att hitta resurser genom att filtrera med deras metadatavärden:

1. Klicka på fliken **[!UICONTROL Filters]** i resursbiblioteket.

   Kriterierna för den tidigare filteråtgärden visas i filterrutan. Panelen Filter är uppdelad i paneler där varje panel representerar ett metadatafält. Använd panelerna för att välja vilka metadatafält som ska filtreras med och inom varje fält för att välja ett metadatavärde för filteråtgärden.

   Om du vill köra en filteråtgärd som du har skapat och sparat klickar du på **[!UICONTROL Select Preset]** och väljer sedan åtgärdens namn på menyn.

   Se [Spara, upprepa och ta bort filteråtgärder](searching-assets.md#saving_repeating_and_deleting_filter_operations).

1. Klicka på **[!UICONTROL Field]** på en panel och följ sedan dessa instruktioner så att du kan visa filtreringsmenyn och skapa filteråtgärden:

   * **Välj ett metadatafält** - Markera fältets namn på filtreringsmenyn.

      >[!NOTE]
      >
      >Endast namnen på metadatafälten i standardmetadatavyn visas på filtreringsmenyn.

      Se [Metadatavyer](application-setup.md#metadata_views).

   * **Lägga till ett metadatafält**  - Klicka  **[!UICONTROL Add a Panel]**. När panelen visas på filterpanelen klickar du på knappen **[!UICONTROL Field]** och väljer namnet på ett metadatafält på filtreringsmenyn.

   * **Ta bort ett metadatafält** - klicka  **[!UICONTROL Remove This Panel]** på filtreringsmenyn.

   När du väljer ett metadatafält visas följande på panelen:

   * Alla metadatavärden som anges i fältet.
   * För varje metadatavärde, antalet resurser som anges av värdet.


1. Upprepa steg 2 så många gånger som behövs för att lista alla metadatafält för filteråtgärden på paneler.
1. Välj ett metadatavärde att filtrera på på varje panel. Du kan inte markera mer än ett metadatavärde på varje panel.

   Resurser som matchar alla värden du valde visas i panelen Bläddra.

   >[!NOTE]
   >
   >Om du vill ta bort ett fält tillfälligt från filteråtgärden klickar du på **[!UICONTROL Deselect All]**. Det här alternativet visas högst upp på varje panel, ovanför metadatavärden.

1. (Valfritt) Om du vill spara filteråtgärden och kunna köra den senare klickar du på **[!UICONTROL Select Preset]** > **[!UICONTROL Save Current As New Presets]** och anger sedan ett namn i dialogrutan **[!UICONTROL Save]**.

### Spara, upprepa och ta bort filteråtgärder {#saving-repeating-and-deleting-filter-operations}

Följ dessa instruktioner på fliken Filter så att du kan spara, upprepa och ta bort filteråtgärder:

* **Spara en filteråtgärd**  - Klicka  **[!UICONTROL Select Preset]** >  **[!UICONTROL Save Current As New Presets]** och ange sedan ett namn i  **[!UICONTROL Save]** dialogrutan.

* **Upprepa en filteråtgärd** - Klicka  **[!UICONTROL Select Preset]** och välj namnet på en filteråtgärd på menyn. I menyn visas filteråtgärder som du har sparat.

* **Tar bort en filteråtgärd från menyn**  Välj förinställning - Kör filteråtgärden. Klicka sedan på **[!UICONTROL Select Preset]** > **[!UICONTROL Delete Preset]** på menyn.

## Använda metadataservern {#using-the-metadata-server}

Metadataservern är ett offentligt API som du kan använda för att söka efter resurser via metadata via http-begäranden.

Konfigurera metadataservern genom att klicka på **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Metadata Server]**.

På sidan Publicera för metadataserver kan du ange följande alternativ:

* **Direktpublicering**  - Alla metadataändringar skickas automatiskt när de görs, inklusive nya resurser, nyckelordsändringar och så vidare.

* **XMP Packet**  - Publicerar XMP. Paketet används inte för sökning, men innehåller den senaste XMP.

* **Nyckelord**  - Publicerar dina nyckelord till metadataservern för användning i sökningar.

* **Metadataserverns publiceringsfält**  - Markera de fält som ska inkluderas i metadata. Med det här alternativet kan du avgöra hur mycket information om dina resurser som är tillgänglig för allmänheten. Dessa fält visas också i metadatavyer, men kan bara ändras på metadataservern.

Klicka på **[!UICONTROL Publish Now]** för att starta jobbet. En bekräftelse visas som talar om att jobbet har startat.

>[!MORELIKETHIS]
>
>* [Navigeringsgrunder](navigation-basics.md#navigation_basics)
* [Visa, lägga till och exportera metadata](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)

