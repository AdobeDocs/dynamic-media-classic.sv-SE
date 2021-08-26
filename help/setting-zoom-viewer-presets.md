---
title: Konfigurera förinställningar för Zoom Viewer
description: Lär dig hur du ställer in förinställningar för zoomvisningsprogrammet.
uuid: 202d80cb-8282-45d4-89e8-942c8677aa93
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 5023a933-e229-4d3c-8e91-3ac5e9f4970b
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ddaaff6c-5447-408e-9c92-bcdfd1a0e72e
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 0%

---

# Konfigurera förinställningar för Zoom Viewer{#setting-up-zoom-viewer-presets}

Förinställningarna för zoomvisningsprogrammet bestämmer stilen, beteendet och utseendet för zoomningsvisningsprogrammen. Adobe Dynamic Media Classic har många alternativ för att anpassa och skalförändra visningsprogram. Adobe Dynamic Media Classic innehåller förinställningar för grundläggande (snabb), utfällbar och anpassad zoomningsvisning. Om du är administratör kan du skapa förinställningar för zoomvisning i företaget eller redigera en standardförinställning och spara den med ett nytt namn.

Alla zoomningsvisningsprogram har knappar för att zooma in, zooma ut, panorera och återställa bilden till det ursprungliga läget efter zoomning. Hur de här knapparna ser ut och hur själva fönstret visas beror på vad du har valt för Zoom Viewer Presets. Du kan konfigurera en förinställning för Zoomvisningsprogram med olika färger, kanter, teckensnitt och bildinställningar. När du konfigurerar ett visningsprogram för guidad zoomning kan du även välja var du vill placera zoommålen. Zoommål är de miniatyrbilder som användarna klickar på för att zooma till de områden som du anger.

## Om förinställningar för Zoom Viewer {#about-zoom-viewer-presets}

Adobe Dynamic Media Classic har följande förinställningar för zoomvisning:

* **Zoomvisningsprogram: Grundläggande**  - Ger en enkel zoomning på originalbilden.

* **Zoomvisningsprogram: Flyg ut**  - Visar en andra bild av det zoomade området bredvid originalbilden. Det finns inga kontroller att använda. Användarna flyttar bara markeringen över det område som de vill visa.

När du fastställer den fullständiga bandbreddsanvändningen för det här visningsprogrammet bör du tänka på att både huvudbilden och den utfällbara bilden visas i visningsprogrammet. Storleken på den utfällbara bilden bestäms av huvudbildens storlek (scenens bredd och höjd) och zoomfaktorn. Om du vill förhindra att den utfällbara filstorleken blir för stor ska du balansera dessa två värden: om du har en stor huvudbildstorlek, sänker du zoomfaktorn. (Utfällbar bredd och Utfällbar höjd bestämmer storleken på det utfällbara fönstret, men inte storleken på den utfällbara bild som visas i visningsprogrammet.)

Om huvudbildens storlek till exempel är 350 x 350 pixlar, med zoomfaktorn 3, blir den utfällbara bilden 1 050 x 1 050 pixlar. Om huvudbildstorleken är 300 x 300 pixlar, med zoomfaktorn 4, är den utfällbara bilden 1 200 x 1 200 pixlar. Beroende på kvalitetsinställningen för JPEG (rekommenderade inställningar är mellan 80 och 90) kan du minska filstorleken avsevärt. Rekommenderade zoomningsfaktorer är 2,5 till 4, beroende på storleken på huvudbilden.

Adobe Dynamic Media Classic rekommenderar följande parametrar för de utfällbara förinställningarna för Zoom Viewer:

* **Förstorad bildstorlek**  - cirka 1 500 x 1 500 pixlar, inte över 2 000 gånger 2 000 pixlar.

* **Bildstorlek**  - 100 kB eller mindre, inte över 150 kB (komprimera filen så att den hålls under 150 kB).

* **Zoomvisningsprogram: Anpassad**  - Tillhandahåller guidad eller oguidad zoomning med bilder, bilduppsättningar med flera vyer eller färgruteuppsättningar.

## Skapa och redigera förinställningar för Zoomvisningsprogram {#creating-and-editing-zoom-viewer-presets}

1. Klicka på **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]** i fältet Global Navigation.
1. Gör något av följande:

   * **Skapa en förinställning**  - klicka  **[!UICONTROL Add]**. I dialogrutan Lägg till visningsförinställning väljer du en plattform, väljer ett zoomvisningsprogram och klickar sedan på **[!UICONTROL Add]**. Ange ett namn för förinställningen i rutan Förinställningsnamn.

   * **Redigera en förinställning**  - Välj en förinställning för zoomvisning och klicka sedan på  **[!UICONTROL Edit]**.

1. Ange önskade inställningar.

   Om du vill visa en beskrivning av ett alternativ klickar du på ikonen **[!UICONTROL Info Tip]** bredvid alternativet.

   På sidan Förhandsgranska visas visningsprogrammet när du uppdaterar och ändrar inställningar.

1. Klicka på **[!UICONTROL Save]** eller **[!UICONTROL Save As]**.
1. Granska den förinställning för zoomvisningsprogram eller den förinställning för guidad zoomningsvisning som du skapade på sidan Förinställningar för visningsprogram för visningsprogram. Om det behöver justeras klickar du på **[!UICONTROL Edit]**, ändrar inställningarna på sidan Konfigurera visningsprogram och klickar på ****[!UICONTROL Save]****.

Mer information om hur du hanterar visningsförinställningar på skärmen Förinställningar för visningsprogram finns i [Förinställningar för visningsprogram](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Skapa och redigera visningsförinställningar](application-setup.md#adding_and_editing_viewer_presets)

