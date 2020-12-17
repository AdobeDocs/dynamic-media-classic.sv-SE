---
title: Konfigurera förinställningar för Zoom Viewer
seo-title: Konfigurera förinställningar för Zoom Viewer
description: 'null'
seo-description: Lär dig hur du ställer in förinställningar för zoomvisningsprogrammet.
uuid: 202d80cb-8282-45d4-89e8-942c8677aa93
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 5023a933-e229-4d3c-8e91-3ac5e9f4970b
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 0%

---


# Konfigurera förinställningar för Zoom Viewer{#setting-up-zoom-viewer-presets}

Förinställningarna för zoomvisningsprogrammet bestämmer stilen, beteendet och utseendet för zoomningsvisningsprogrammen. I Dynamic Media Classic finns många alternativ för att anpassa och skalförändra visningsprogram. Dynamic Media Classic innehåller standardförinställningar för grundläggande (snabb), utfällbar och anpassad zoomningsvisning. Om du är administratör kan du skapa nya förinställningar för zoomvisningsprogrammet eller redigera en standardförinställning och spara den med ett nytt namn.

Alla zoomvisningsprogram har knappar för att zooma in, zooma ut, panorera och återställa bilden till det ursprungliga läget efter zoomning. Hur dessa knappar ser ut och hur själva fönstret ser ut beror på vad du väljer bland förinställningarna för Zoom Viewer. Du kan konfigurera en förinställning för Zoomvisningsprogram med olika färger, kanter, teckensnitt och bildinställningar. När du konfigurerar ett visningsprogram för guidad zoomning kan du även välja var du vill placera zoommålen. Zoommål är de miniatyrbilder som användarna klickar på för att zooma till de områden som du anger.

## Om förinställningar för Zoom Viewer {#about-zoom-viewer-presets}

I Dynamic Media Classic finns följande förinställningar för Zoom Viewer:

* **Zoomvisningsprogram: Grundläggande**
Ger en enkel zoomning på originalbilden.

* **Zoomvisningsprogram: Flyt**
utVisar en andra bild av det zoomade området bredvid originalbilden. Det finns inga kontroller att använda. Användarna flyttar bara markeringen över det område som de vill visa.

När du fastställer den fullständiga bandbreddsanvändningen för det här visningsprogrammet bör du tänka på att både huvudbilden och den utfällbara bilden visas i visningsprogrammet. Storleken på den utfällbara bilden bestäms av huvudbildens storlek (scenens bredd och höjd) och zoomfaktorn. Om du vill förhindra att den utfällbara filstorleken blir för stor ska du balansera dessa två värden: om du har en stor huvudbildstorlek, sänker du zoomfaktorn. (Utfällbar bredd och Utfällbar höjd bestämmer storleken på det utfällbara fönstret, men inte storleken på den utfällbara bild som visas i visningsprogrammet.)

Om huvudbildens storlek till exempel är 350 x 350 pixlar, med zoomfaktorn 3, blir den utfällbara bilden 1 050 x 1 050 pixlar. Om huvudbildstorleken är 300 x 300 pixlar, med zoomfaktorn 4, är den utfällbara bilden 1 200 x 1 200 pixlar. Beroende på kvalitetsinställningen för JPEG (rekommenderade inställningar är mellan 80 och 90) kan du minska filstorleken avsevärt. Rekommenderade zoomningsfaktorer är 2,5 till 4, beroende på storleken på huvudbilden.

Dynamic Media Classic rekommenderar följande parametrar för de utfällbara förinställningarna för Zoom Viewer:

* **Förstorad**
bildstorlekUngefär 1 500 gånger 1 500 pixlar, inte över 2 000 gånger 2 000 pixlar.

* **Bildstorleken**
 100 kB eller mindre, får inte överstiga 150 kB (komprimera filen så att den hålls under 150 kB).

* **Zoomvisningsprogram:**
AnpassadVisar guidad eller oguidad zoomning med bilder, bilduppsättningar med flera vyer eller färgruteuppsättningar.

## Skapa och redigera förinställningar för zoomvisningsprogrammet {#creating-and-editing-zoom-viewer-presets}

Följ de här stegen för att skapa eller redigera en förinställning för zoomvisningsprogrammet:

1. Klicka på **Inställningar** > **Visningsförinställningar**.
1. Gör något av följande:

   * **Skapa en**
förinställningKlicka på Lägg till. I dialogrutan Lägg till visningsförinställning väljer du en plattform, väljer ett zoomvisningsprogram och klickar sedan på Lägg till. Ange ett namn för förinställningen i rutan Förinställningsnamn.

   * **Redigera en**
förinställningVälj en förinställning för zoomvisning och klicka sedan på 
**Redigera**.

1. Ange önskade inställningar.

   Om du vill visa en beskrivning av ett alternativ klickar du på ikonen för informationstips bredvid alternativet.

   Visningsprogrammet visas på förhandsgranskningsskärmen när du uppdaterar och ändrar inställningarna.

1. Klicka på **Spara** eller **Spara som**.
1. Granska den förinställning för zoomvisningsprogram eller den förinställning för guidad zoomningsvisning som du har skapat på skärmen Förinställningar för visningsprogram för visningsprogram. Om det behöver justeras klickar du på **Redigera**, ändrar inställningarna på skärmen Konfigurera visningsprogram och klickar på **Spara**.

Mer information om hur du hanterar visningsförinställningar på skärmen Förinställningar för visningsprogram finns i [Förinställningar för visningsprogram](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Skapa och redigera visningsförinställningar](application-setup.md#adding_and_editing_viewer_presets)

