---
title: Söka efter resurser
seo-title: Söka efter resurser
description: 'null'
seo-description: Lär dig hur du söker efter resurser.
uuid: 058209bc-bac4-4d5c-8261-e242a543beaf
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: effef4e7-37c5-42e2-9266-ecd026cad628
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Söka efter resurser{#searching-assets}

Om du vill hitta filresurser i Scene7 Publishing System kan du visa resurser efter typ, sortera resurser i panelen Bläddra, göra en enkel sökning, utföra en avancerad sökning och filtrera efter resurser.

>[!NOTE]
>
>Skärmen Personliga inställningar innehåller alternativ för hur du vill utföra sökningar. Du kan t.ex. välja en standardsöktyp och välja om användardefinierade fält ska inkluderas i sökningar. Mer information finns i [Personliga inställningar](personal-setup.md#personal_setup).

## Visa resurser efter typ {#viewing-assets-by-type}

Om du bara vill visa filer av en viss typ när du bläddrar öppnar du listrutan Visa i resursbiblioteket och väljer sedan en filtyp. Endast resurser av den typ du valde visas i resursbiblioteket.

## Sortera filer i panelen Bläddra {#sorting-files-in-the-browse-panel}

Om du vill sortera innehållet i en mapp eller sökresultaten på panelen Bläddra väljer du menyn Sortera och väljer ett alternativ. Alternativen är Namn, Storlek, Typ, Skapad och Senast ändrad.

Du kan välja Stigande eller Fallande om du vill sortera resurser i stigande eller fallande ordning efter de villkor du väljer.

I listvyn kan du sortera genom att klicka på ett kolumnnamn.

## Genomföra en enkel sökning {#conducting-a-simple-search}

Använd sökfältet för att utföra enkla sökningar. Du kan söka efter objekt efter namn eller söka efter objekt vars metadata innehåller ett nyckelord.

Gör en enkel sökning:

1. Markera mappen i resursbiblioteket om du vill söka i en viss mapp och dess undermappar
1. Klicka i resursbiblioteket och välj ett alternativ som beskriver hur smal eller bred du vill att sökningen ska vara. Du kan välja Inom alla filer och mappar, i den markerade mappen eller i den valda mappen och undermapparna.
1. Ange ett sökord.
1. Klicka på Gå eller tryck på Enter.

   Resultatet av sökningen visas i panelen Bläddra.

>[!NOTE]
>
>Dynamic Media Classic spårar sökningar. Om du vill göra en sökning en andra gång markerar du knappen Sök och väljer namnet på en sökning längst ned på menyn Sök.

## Använda avancerad sökning {#conducting-an-advanced-search}

Klicka på Avancerad sökning i resursbiblioteket om du vill söka efter många villkor, inklusive värden i metadatafält.

Ange något av följande villkor i sökningen:

**Filtrera efter resurstyp** Begränsa sökningen till en resurstyp genom att välja en resurstyp på menyn.

**Filer och mappar** Välj var du vill söka: I alla filer och mappar, i den valda mappen eller i den valda mappen och undermapparna.

**Alla Publiceringslägen** Sök efter filer som har markerats som klara för publicering, har inte markerats som klara för publicering eller alla filer.

**Villkor** Om du anger metadatavillkor för sökning väljer du om sökningen måste matcha alla villkor (en ALL-sökning) eller något villkor (en OR-sökning).

**Ange sökvillkor för metadata** Skapa ett eller flera sökfält för sökning av metadata. Så här skapar du sökfält:

1. Öppna listan Metadatavy (till vänster om menyn Lägg till ett fält) och välj en metadatavy. Du kan välja en kompakt vy, IPTC, XMP eller en vy som administratören har konfigurerat.
1. Välj menyn Lägg till ett fält och välj ett fältnamn i listrutan.
1. Välj alternativet Innehåller (Innehåller, Innehåller inte, Börjar med, Slutar med eller Likhetstecken).
1. För numeriska fält väljer du ett värde eller anger ett anpassat datumintervall.
1. (Valfritt) Upprepa steg 1-4 om du vill skapa fler sökfält.

Du kan klicka på knappen Ta bort sökfält för att ta bort ett sökfält.

Klicka på Sök för att börja söka. Resultatet av sökningen visas i panelen Bläddra. Du kan ändra sökvillkoren och klicka på Sök för att köra sökningen igen.

Klicka på Rensa för att rensa sökvillkoren och starta en ny sökning. Klicka på Stäng när du är klar med sökningen för att stänga sökpanelen.

## Filtrera resurser med metadata {#filter-assets-using-metadata}

Filtrera resurser på fliken Filter i resursbiblioteket. Om du vill filtrera resurser använder du metadatavärden som villkor. När du har valt ett metadatafält som du vill använda för filtrering visar fliken Filter alla metadatavärden som har angetts i det valda fältet och antalet resurser som har tilldelats varje värde. I en filteråtgärd i metadatafältet för skapare visar till exempel fliken Filter alla namn som har angetts i metadatafältet för skapare för olika resurser, och för varje namn, antalet resurser som har tilldelats namnet. Klicka sedan på ett metadatavärde för att visa alla resurser som har tilldelats det värdet. I exemplet klickar du på metadatavärdet för Jimmy för att visa alla resurser där namnet Jimmy har angetts i metadatafältet för Skapare. Du kan filtrera med hjälp av mer än ett metadatafält som filtreringskriterium.

Du kan spara filteråtgärder för att kunna köra dem många gånger.

>[!NOTE]
>
>Endast metadatafält i standardmetadatavyn kan användas för filteråtgärder. På skärmen Metadatavyer visas namnet på standardvyn för metadata.

Se [Metadatavyer](application-setup.md#metadata_views).

### Köra en filteråtgärd {#running-a-filter-operation}

Följ de här stegen för att söka efter resurser genom att filtrera med deras metadatavärden:

1. Klicka på fliken Filter i resursbiblioteket.

   Kriterierna för den tidigare filteråtgärden visas i filterrutan. Panelen Filter är uppdelad i paneler där varje panel representerar ett metadatafält. Använd panelerna för att välja vilka metadatafält som ska filtreras med och inom varje fält för att välja ett metadatavärde för filteråtgärden.

   Om du vill köra en filteråtgärd som du har skapat och sparat klickar du på knappen Välj förinställning och väljer åtgärdens namn på menyn.

   Se [Spara, upprepa och ta bort filteråtgärder](searching-assets.md#saving_repeating_and_deleting_filter_operations).

1. Klicka på knappen Fält på en panel, följ dessa instruktioner för att visa filtermenyn och skapa filteråtgärden:

   **Välj ett metadatafält** Välj fältets namn på filtreringsmenyn.

   ***Obs **! Endast namnen på metadatafälten i standardmetadatavyn visas på filtreringsmenyn.*

   Se [Metadatavyer](application-setup.md#metadata_views).

   **Lägg till ett metadatafält** Välj Lägg till en panel. När panelen visas på filterpanelen klickar du på knappen Fält och väljer namnet på ett metadatafält på filtreringsmenyn.

   **Ta bort ett metadatafält** Välj Ta bort den här panelen på filtreringsmenyn.

   När du väljer ett metadatafält visas en lista i panelen:

   * Alla metadatavärden som anges i fältet.
   * För varje metadatavärde, antalet resurser som anges av värdet.

1. Upprepa steg 2 så många gånger som behövs för att lista alla metadatafält för filteråtgärden på paneler.
1. Välj ett metadatavärde att filtrera på på varje panel. Du kan inte markera mer än ett metadatavärde på varje panel.

   Resurser som matchar alla värden du valde visas i panelen Bläddra.

   >[!NOTE]
   >
   >Om du vill ta bort ett fält tillfälligt från filteråtgärden klickar du på Avmarkera alla. Det här alternativet finns högst upp på varje panel, ovanför metadatavärden.

1. (Valfritt) Om du vill spara filteråtgärden och kunna köra den senare klickar du på knappen Välj förinställning, väljer Spara aktuella som nya förinställningar och anger ett namn i dialogrutan Spara.

### Spara, upprepa och ta bort filteråtgärder {#saving-repeating-and-deleting-filter-operations}

Följ dessa anvisningar på fliken Filter för att spara, upprepa och ta bort filteråtgärder:

**Spara en filteråtgärd** Klicka på knappen Välj förinställning, välj Spara aktuella som nya förinställningar och ange ett namn i dialogrutan Spara.

**Upprepa en filteråtgärd** Klicka på knappen Välj förinställning och välj namnet på en filteråtgärd på menyn. I menyn visas filteråtgärder som du har sparat.

**Om du tar bort en filteråtgärd från menyn Välj förinställning** kör du filteråtgärden. Klicka sedan på knappen Välj förinställning och välj Ta bort förinställning på menyn.

## Använda metadataservern {#using-the-metadata-server}

Metadataservern är ett offentligt API som du kan använda för att söka efter resurser via metadata via http-begäranden.

Om du vill konfigurera metadataservern klickar du på Konfigurera > Programinställningar > Publiceringsinställningar > Metadataserver.

Metadataserverns publiceringsskärm öppnas. På den här skärmen kan du ange följande alternativ:

**Med Direktpublicering** överförs automatiskt alla metadataändringar när de görs, inklusive nya resurser, nyckelordsändringar och så vidare.

**XMP-paket** Publicerar XMP-paket. Paketet används inte för sökning, men innehåller den senaste XMP/

**Nyckelord** Publicerar dina nyckelord till metadataservern för användning i sökningar.

**Metadataserverns publiceringsfält** Välj de fält som ska inkluderas i metadata. På så sätt kan du avgöra hur mycket information om dina resurser som är tillgänglig för allmänheten. Dessa fält visas också i metadatavyer, men kan bara ändras på metadataservern.

Klicka på **Publicera nu** för att starta jobbet. En bekräftelse visas som talar om att jobbet har startat.

>[!MORELIKETHIS]
>
>* [Navigeringsgrunder](navigation-basics.md#navigation_basics)
>* [Visa, lägga till och exportera metadata](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)

