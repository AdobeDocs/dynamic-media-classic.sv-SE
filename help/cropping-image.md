---
title: Beskära en bild
seo-title: Beskära en bild
description: 'null'
seo-description: Lär dig beskära en bild.
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
translation-type: tm+mt
source-git-commit: b8d245bfc8375966af314ed95e81a519c5ee6c24

---


# Beskära en bild{#cropping-an-image}

Du kan beskära bilder i Scene7 Publishing System. Systemet sparar information om beskurna bilder så att du kan återställa dem till ursprungligt läge. Du kan också beskära en bild och spara den beskurna versionen under ett nytt namn.

Du kan beskära en bild för att ta bort tomt utrymme runt den eller beskära ett område i bilden.

>[!NOTE]
>
>När du har beskurit kan du klicka på knappen Spara som och spara en beskuren version av bilden under ett annat namn. I fönstret Spara som väljer du Spara som ny mallsida om du vill spara en andra kopia av bilden. Välj Spara som tilläggsvy för mallsida om du vill spara originalet och den beskurna versionen med ett annat namn. Välj Ersätt original om du vill ta bort originalfilen som du beskurit bilden från. Ange sedan ett namn för bilden och välj knappen Skicka.

## Beskära för att ta bort tomt utrymme runt en bild {#crop-to-remove-white-space-around-an-image}

Du kan beskära de genomskinliga eller enfärgade pixlarna från bildens kant.

1. Om du vill beskära en bild klickar du på knappen Redigera överrullning och väljer Beskär. Du kan också visa den i panelen Bläddra i detaljvyn och klicka på knappen Beskär. Skärmen Beskärningsredigeraren öppnas.
1. Gör något av följande:

   * Om du vill trimma färgpixlar väljer du menyn Rensa och sedan Färg. Dialogrutan Beskär automatiskt efter färg visas. Välj menyn Hörn och välj ett hörn med bakgrundsfärgen som ska beskäras. Ange sedan en toleransinställning från 0 till 1. Inställningen 0 beskär bara pixlar om de exakt matchar färgen som du valde i bildens hörn. Nummer som ligger närmare 1 ger större färgskillnader. Välj knappen Beskär.
   * Om du vill trimma genomskinliga pixlar väljer du Rensa och sedan Genomskinlig. Dialogrutan Beskär automatiskt efter genomskinlighet visas. Ange en toleransinställning mellan 0 och 1. Inställningen 0 beskär bara pixlar om de är helt genomskinliga. Siffror närmare 1 ger större genomskinlighet. Välj knappen Beskär.

1. Klicka på **Spara**.

>[!NOTE]
>
>Om du vill återställa en bild till det ursprungliga läget efter att du har beskurit den, visar du bilden på skärmen Beskärningsredigeraren och väljer knappen Återställ.

## Markera ett område att beskära {#select-an-area-to-crop}

1. Om du vill beskära en bild klickar du på knappen Redigera överrullning och väljer **Beskär**. Du kan också visa den i panelen Bläddra i detaljvyn och klicka på **Beskär**.

1. I beskärningsredigeraren placerar du den del av bilden som du inte vill beskära i beskärningsrutan. Det som visas i rutan kvarstår när du klickar på **Spara** och beskär bilden.
1. Justera beskärningsområdet genom att göra något av följande:

   * Dra en sida eller ett hörn av rutan. Håll ned Skift-tangenten när du drar om du vill ändra storlek men behålla proportionerna (formen) för beskärningsrutan.
   * Ange pixelmått i rutorna Storlek.
   * Dra för att flytta beskärningsrutan. Flytta pekaren innanför rutans kant. När du ser den fyrhövdade pilen drar du rutan till en ny plats i bilden.

1. Klicka på **Spara**.

>[!NOTE]
>
>Om du vill återställa en bild till det ursprungliga läget efter att du har beskurit den, visar du bilden på skärmen Beskärningsredigeraren och väljer knappen Återställ.

>[!MORELIKETHIS]
>
>* [Bildredigeringsalternativ vid överföring](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Beskära tomt utrymme från en PDF-fil](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Beskära från sidorna på PDF-sidor](pdfs.md#cropping_from_the_sides_of_pdf_pages)

