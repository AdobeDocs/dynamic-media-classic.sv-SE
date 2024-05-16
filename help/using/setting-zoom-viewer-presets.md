---
title: Konfigurera förinställningar för Zoomvisningsprogram
description: Lär dig hur du ställer in förinställningar för zoomvisningsprogrammet i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ddaaff6c-5447-408e-9c92-bcdfd1a0e72e
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---

# Konfigurera förinställningar för Zoomvisningsprogram{#setting-up-zoom-viewer-presets}

Zoomvisningsförinställningarna avgör stil, beteende och utseende för dina zoomningsvisningsprogram. Adobe Dynamic Media Classic erbjuder många alternativ för att anpassa och skala visningsprogram. Adobe Dynamic Media Classic levereras med standardförinställningar för grundläggande (snabb), utfällbar och anpassad zoomningsvisning. Om du är administratör kan du skapa förinställningar för zoomvisning i företaget eller redigera en standardförinställning och spara den med ett nytt namn.

Alla zoomningsvisningsprogram har knappar för att zooma in, zooma ut, panorera och återställa bilden till det ursprungliga läget efter zoomning. Hur de här knapparna ser ut och hur själva fönstret visas beror på vad du har valt för Zoom Viewer Presets. Du kan konfigurera en förinställning för Zoomvisningsprogram med olika färger, kanter, teckensnitt och bildinställningar. När du konfigurerar ett visningsprogram för guidad zoomning kan du även välja var du vill placera zoommålen. Zoommål är de miniatyrbilder som användarna klickar på för att zooma till de områden som du anger.

## Om förinställningar för Zoom Viewer {#about-zoom-viewer-presets}

Adobe Dynamic Media Classic har följande förinställningar för Zoom Viewer:

* **Zoomvisningsprogram: Grundläggande**: Ger en grundläggande zoom på originalbilden.

* **Zoomvisningsprogram: Flyg ut**: Visar en andra bild av det zoomade området bredvid den ursprungliga bilden. Det finns inga kontroller att använda. Användarna flyttar bara markeringen över det område som de vill visa.

När du fastställer den fullständiga bandbreddsanvändningen för det här visningsprogrammet bör du tänka på att både huvudbilden och den utfällbara bilden visas i visningsprogrammet. Storleken på den utfällbara bilden bestäms av huvudbildens storlek (scenens bredd och höjd) och zoomfaktorn. Om du vill förhindra att den utfällbara filstorleken blir för stor ska du balansera dessa två värden: om du har en stor huvudbildstorlek ska du sänka värdet för zoomfaktor. (Utfällbar bredd och Utfällbar höjd bestämmer storleken på det utfällbara fönstret, men inte storleken på den utfällbara bild som visas i visningsprogrammet.)

Om huvudbildens storlek till exempel är 350 x 350 pixlar, med zoomfaktorn 3, blir den utfällbara bilden 1 050 x 1 050 pixlar. Om huvudbildstorleken är 300 x 300 pixlar, med zoomfaktorn 4, är den utfällbara bilden 1 200 x 1 200 pixlar. Beroende på kvalitetsinställningen för JPEG (rekommenderade inställningar är mellan 80 och 90) kan du minska filstorleken avsevärt. Rekommenderade zoomningsfaktorer är 2,5 till 4, beroende på storleken på huvudbilden.

Adobe Dynamic Media Classic rekommenderar följande parametrar för de utfällbara förinställningarna för Zoom Viewer:

* **Förstorad bildstorlek**: Cirka 1 500 gånger 1 500 pixlar, får inte överskrida 2 000 gånger 2 000 pixlar.

* **Bildstorlek**: 100 kB eller lägre, får inte överskrida 150 kB (komprimera filen så att den hålls under 150 kB).

* **Zoomvisningsprogram: Anpassad**: Tillhandahåller guidad eller oguidad zoomning med bilder, bilduppsättningar med flera vyer eller färgruteuppsättningar.

## Skapa och redigera förinställningar för Zoomvisningsprogram {#creating-and-editing-zoom-viewer-presets}

1. I fältet Global Navigation går du till **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.
1. Gör något av följande:

   * **Skapa en förinställning**: Välj **[!UICONTROL Add]**. I dialogrutan Lägg till visningsförinställning väljer du en plattform, väljer ett zoomvisningsprogram och väljer sedan **[!UICONTROL Add]**. Ange ett namn för förinställningen i rutan Förinställningsnamn.

   * **Redigera en förinställning**: Välj en förinställning för Zoomvisningsprogram och välj sedan **[!UICONTROL Edit]**.

1. Ange önskade inställningar.

   Om du vill visa en beskrivning av ett alternativ väljer du **[!UICONTROL Info Tip]** -ikonen bredvid alternativet.

   På sidan Förhandsgranska visas visningsprogrammet när du uppdaterar och ändrar inställningar.

1. Välj **[!UICONTROL Save]** eller **[!UICONTROL Save As]**.
1. Granska den förinställning för zoomvisningsprogram eller den förinställning för guidad zoomningsvisning som du skapade på sidan Förinställningar för visningsprogram för visningsprogram. Om det behöver justeras väljer du **[!UICONTROL Edit]**, ändra inställningarna på `Configure Viewer` sida och sedan markera **[!UICONTROL Save]**.

Mer information om hur du hanterar visningsförinställningar på skärmen Förinställningar för visningsprogram finns i [Förinställningar för visningsprogram](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Skapa och redigera visningsförinställningar](application-setup.md#adding_and_editing_viewer_presets)
