---
title: Flytta, byta namn på och ta bort resurser
description: Lär dig hur du flyttar, byter namn på och tar bort resurser.
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Resurshantering
role: Business Practitioner
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
translation-type: tm+mt
source-git-commit: 38d09bb78834c6b3614bf2b96fd6aee5661e0a5a
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# Flytta, byta namn på och ta bort resurser{#moving-renaming-and-deleting-assets}

Du kan flytta, byta namn på och ta bort resurser från panelen Bläddra. Du kan också ta bort många resurser samtidigt med en textfil.

## Flytta resurser {#move-assets}

Du kan flytta resurser till olika mappar i panelen Bläddra.

1. Markera resursen eller resurserna på panelen Bläddra och gör något av följande:

   * Visa mappen som du vill flytta resurserna till i resursbiblioteket och dra resurserna till mappen.
   * Klicka på **[!UICONTROL File]** > **[!UICONTROL Move]**, markera en mapp i fönstret Flytta resurser och välj **[!UICONTROL Move]**.

## Byt namn på resurser {#rename-assets}

1. Markera resursen i panelen Bläddra och gör något av följande:

   * Markera namnet, skriv in ett nytt namn och tryck på **[!UICONTROL Enter]** eller klicka utanför namnet.
   * Klicka på **[!UICONTROL File]** > **[!UICONTROL Rename]**. Namnet på resursen markeras. Ange ett nytt namn och tryck på **[!UICONTROL Enter]**.

Se till att du inte anger namnet på en befintlig Dynamic Media Classic-resurs.

## Ta bort resurser {#delete-assets}

Du kan ta bort markerade resurser på panelen Bläddra och ta bort hela mappar. Borttagna resurser och mappar flyttas till papperskorgen, där de finns kvar i sju dagar innan de tas bort permanent.

När du tar bort en resurs tas även alla resurser som härletts från den bort. Om du t.ex. tar bort en bild som du har skapat zoommål för tas även zoommålen bort tillsammans med bilden.

>[!NOTE]
>
>Zoommål, bildattribut och historikposter tas bort permanent när du tar bort de resurser som de härleds från. De flyttas inte tillsammans med resursen till papperskorgen. de inte kan återställas från papperskorgen.

1. Gör något av följande:

   * Om du vill ta bort en eller flera resurser markerar du resurserna på panelen Bläddra och trycker på **[!UICONTROL Delete]** eller klickar på **[!UICONTROL File]** > **[!UICONTROL Delete]**.
   * Om du vill ta bort en mapp markerar du mappen i resursbiblioteket och klickar på **[!UICONTROL Remove Folder]**.

      Om du tar bort en mapp tas mappen, alla resurser i mappen och alla resurser i dess undermappar bort.

>[!NOTE]
>
>Dynamic Media Classic rekommenderar att du skriver över resursfiler i stället för att ta bort dem om du vill ersätta en resursfil med en annan med samma namn.

## Ta bort flera resurser med en textfil {#delete-multiple-assets-with-a-text-file}

Om du vill ta bort flera resurser samtidigt i resursbiblioteket kan du visa de resurser du vill ta bort i en textfil och skicka listan till Dynamic Media Classic.

Skapa en lista med Dynamic Media Classic ID:n och spara den som en textfil (.txt). Varje Dynamic Media Classic-ID måste finnas på sin egen rad (följt av en hård retur).

När du har skapat listan följer du de här stegen för att använda den för att ta bort resurser:

1. Klicka på **[!UICONTROL File]** > **[!UICONTROL Delete Asset List]**.
1. I dialogrutan Ta bort resurs bläddrar du till eller skriver sökvägen till textfilen med listan över resurser som du vill ta bort.
1. Klicka på **[!UICONTROL Delete]**.

När du tar bort resurser med en textfil visas meddelandet&quot;Det går inte att validera de här posterna i listan:&quot; och listan över poster om det inte finns något Dynamic Media Classic-ID i listan. Dynamic Media Classic genererar dock inget fel på jobbsidan.

>[!MORELIKETHIS]
>
>* [Välja resurser i panelen Bläddra](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Förbereda dina resurser och mappar för överföring](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Återställa resurser från papperskorgen](trash-folder.md#restoring_assets_from_the_trash_folder)

