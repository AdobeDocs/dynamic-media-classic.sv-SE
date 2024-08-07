---
title: Beskära en bild
description: Lär dig beskära en bild i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 0%

---

# Beskära en bild{#cropping-an-image}

Du kan beskära bilder i Adobe Dynamic Media Classic. Systemet sparar information om beskurna bilder så att du kan återställa dem till ursprungligt läge. Du kan också beskära en bild och spara den beskurna versionen under ett nytt namn.

Du kan beskära en bild för att ta bort tomt utrymme runt den eller beskära ett område i bilden.

>[!NOTE]
>
>När du har beskurit kan du markera **[!UICONTROL Save As]** och spara en beskuren version av bilden under ett annat namn. I fönstret Spara som väljer du **[!UICONTROL Save As New Primary]** om du vill spara en andra kopia av bilden. Välj **[!UICONTROL Save As Addition View Of Primary]** så att du kan spara originalet och den beskurna versionen med ett annat namn. Välj **[!UICONTROL Replace Original]** om du vill ta bort originalfilen som du beskurit bilden från. Ange sedan ett namn för bilden och välj **[!UICONTROL Submit]**.

## Beskära för att ta bort tomt utrymme runt en bild {#crop-to-remove-white-space-around-an-image}

Du kan beskära av de genomskinliga eller enfärgade pixlarna från bildens kant.

1. Om du vill beskära en bild markerar du dess överrullningsknapp **[!UICONTROL Edit]** och väljer sedan **[!UICONTROL Crop]** eller visar den i panelen Bläddra i detaljvyn och väljer knappen **[!UICONTROL Crop]** .
1. Gör något av följande på sidan Beskärningsredigerare:

   * Om du vill trimma färgpixlar går du till **[!UICONTROL Trim]** > **[!UICONTROL Color]**. Välj menyn **[!UICONTROL Corner]** i dialogrutan **[!UICONTROL Auto Crop By Color]** och välj ett hörn med bakgrundsfärgen som du vill beskära bort. Ange sedan en **[!UICONTROL Tolerance]**-inställning från 0 till 1. Inställningen 0 beskär bara pixlar om de exakt matchar färgen som du valde i bildens hörn. Nummer som ligger närmare 1 ger större färgskillnader. Välj **[!UICONTROL Crop]**.
   * Om du vill trimma genomskinliga pixlar går du till **[!UICONTROL Trim]** > **[!UICONTROL Transparent]**. Ange en toleransinställning från 0 till 1 i dialogrutan **[!UICONTROL Auto Crop By Transparency]**. Inställningen 0 beskär bara pixlar om de är genomskinliga. Siffror närmare 1 ger större genomskinlighet. Välj **[!UICONTROL Crop]**.

1. Välj **[!UICONTROL Save]**.

>[!NOTE]
>
>Om du vill återställa en bild till det ursprungliga läget efter att du har beskurit den, visar du bilden på beskärningsredigeraren och väljer **[!UICONTROL Reset]**.

## Markera ett område att beskära {#select-an-area-to-crop}

1. Om du vill beskära en bild markerar du dess överrullningsknapp **[!UICONTROL Edit]**, väljer **[!UICONTROL Crop]** eller visar den i panelen Bläddra i detaljvyn och väljer **[!UICONTROL Crop]**.

1. I beskärningsredigeraren placerar du den del av bilden som du inte vill beskära i beskärningsrutan. Vad som än visas i rutan är vad som återstår efter att du har markerat **[!UICONTROL Save]** och beskär bilden.
1. Justera beskärningsområdet genom att göra något av följande:

   * Dra en sida eller ett hörn av rutan. Håll ned Skift-tangenten när du drar om du vill ändra storleken men behålla proportionerna (formen) för beskärningsrutan.
   * Ange pixelmått i rutorna Storlek.
   * Dra för att flytta beskärningsrutan. Flytta pekaren innanför rutans kant. När du ser den fyrhövdade pilen drar du rutan till en ny plats i bilden.

1. Välj **[!UICONTROL Save]**.

>[!NOTE]
>
>Om du vill återställa en bild till det ursprungliga läget efter att du har beskurit den, visar du bilden på beskärningsredigeraren och väljer **[!UICONTROL Reset]**.

>[!MORELIKETHIS]
>
>* [Alternativ för bildredigering vid överföring](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Beskär tomt utrymme från en PDF-fil](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Beskär från sidorna på PDF](pdfs.md#cropping_from_the_sides_of_pdf_pages)
