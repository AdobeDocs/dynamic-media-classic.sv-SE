---
title: Flytta, byta namn på och ta bort resurser
description: Lär dig hur du flyttar, byter namn på och tar bort resurser i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# Flytta, byta namn på och ta bort resurser{#moving-renaming-and-deleting-assets}

Du kan flytta, byta namn på och ta bort resurser från panelen Bläddra. Du kan också ta bort många resurser samtidigt med en textfil.

## Flytta resurser {#move-assets}

Du kan flytta resurser till olika mappar i panelen Bläddra.

**Så här flyttar du resurser:**

1. Markera resursen eller resurserna på panelen Bläddra och gör något av följande:

   * Visa mappen som du vill flytta resurserna till i resursbiblioteket och dra resurserna till mappen.
   * Gå till **[!UICONTROL File]** > **[!UICONTROL Move]**, markera en mapp i fönstret Flytta Assets och välj **[!UICONTROL Move]**.

## Byt namn på resurser {#rename-assets}

1. Markera resursen på panelen Bläddra och gör något av följande:

   * Markera namnet, skriv in ett nytt namn och tryck på **[!UICONTROL Enter]** eller välj ett annat namn.
   * Gå till **[!UICONTROL File]** > **[!UICONTROL Rename]**. Namnet på resursen markeras. Ange ett nytt namn och tryck på **[!UICONTROL Enter]**. Se till att du inte anger namnet på en befintlig Adobe Dynamic Media Classic-resurs.

## Ta bort resurser {#delete-assets}

Du kan ta bort markerade resurser på panelen Bläddra och ta bort hela mappar. Borttagna resurser och mappar flyttas till papperskorgen, där de finns kvar i sju dagar innan de tas bort permanent.

När du tar bort en resurs tas även alla resurser som är härledda från den bort. Om du t.ex. tar bort en bild som du har skapat zoommål för tas zoommålen bort tillsammans med bilden.

Zoommål, bildattribut och historikposter tas bort permanent när du tar bort de resurser som de härleds från. De flyttas inte tillsammans med resursen till papperskorgen utan kan inte återställas från papperskorgen.

>[!IMPORTANT]
>
>Massborttagning är en intensiv åtgärd. Se till att du kör massborttagningar sekventiellt i stället för som samtidiga, tunga raderingsåtgärder. Adobe rekommenderar att du begränsar borttagningsåtgärder till 5 000 eller färre borttagningar av resurser per timme. Ett tal som är större än 5000 per timme kan orsaka hastighetsbegränsning.

**Så här tar du bort resurser:**

1. Gör något av följande:

   * Om du vill ta bort en eller flera resurser markerar du resurserna på panelen Bläddra och trycker på **[!UICONTROL Delete]** eller går till **[!UICONTROL File]** > **[!UICONTROL Delete]**.
   * Om du vill ta bort en mapp markerar du mappen i resursbiblioteket och väljer **[!UICONTROL Remove Folder]**.

     Om du tar bort en mapp tas mappen, alla resurser i mappen och alla resurser i dess undermappar bort.

Adobe Dynamic Media Classic rekommenderar att du skriver över resursfiler i stället för att ta bort dem, om du vill ersätta en resursfil med en annan med samma namn.

## Ta bort flera resurser med en textfil {#delete-multiple-assets-with-a-text-file}

Om du vill ta bort flera resurser samtidigt i resursbiblioteket kan du visa de resurser du vill ta bort i en textfil och skicka listan till Adobe Dynamic Media Classic.

Skapa en lista med Adobe Dynamic Media Classic-id:n och spara den som en textfil (.txt). Varje Adobe Dynamic Media Classic-id måste finnas på sin egen rad (följt av en hård retur).

När du har skapat listan följer du de här stegen för att använda den för att ta bort resurser:

1. Gå till **[!UICONTROL File]** > **[!UICONTROL Delete Asset List]**.
1. I dialogrutan **[!UICONTROL Deleted Asset list]** anger du sökvägen till textfilen med listan över resurser som du vill ta bort.
1. Välj **[!UICONTROL Delete]**.

När du tar bort resurser med en textfil visas meddelandet&quot;Det går inte att validera de här posterna i listan:&quot; om något Adobe Dynamic Media Classic-ID inte finns med i listan. Listan med poster visas också. Adobe Dynamic Media Classic genererar dock inget fel på jobbsidan.

>[!MORELIKETHIS]
>
>* [Välj resurser på panelen Bläddra](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Förbered dina resurser och mappar för överföring](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Återställ resurser från papperskorgen](trash-folder.md#restoring_assets_from_the_trash_folder)
