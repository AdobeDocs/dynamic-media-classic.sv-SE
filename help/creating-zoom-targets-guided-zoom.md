---
title: Skapa zoommål för guidad zoomning
description: Lär dig hur du skapar zoommål för guidad zoomning.
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---


# Skapa zoommål för guidad zoomning{#creating-zoom-targets-for-guided-zoom}

Zoommål vägleder tittarna till vissa delar av en bild. Förutom att zooma fritt kan användarna klicka på en zoommålminiatyrbild och zooma till den del av bilden som de ska fokusera på. Zoommål ger dig möjlighet att markera de attraktiva eller intressanta delarna i en bild.

![Skapa zoommål för guidad zoomning](/help/assets/zo_guided_zoom.png)

## Om zoommål {#about-zoom-targets}

Den maximala zoomprocenten för zoommål är 100 procent. Den minsta zoomprocenten varierar beroende på en kombination av visningsprogrammets storlek och bildstorleken, vilket visas i följande tabell:

| Bildstorlek | Storlek på visningsprogram | Zoomningsprocent |
|--- |--- |--- |
| Stor | Mindre | Mindre minimum |
| Liten | Större | Större minimum |

Du kan ändra storleken på Zoomvisningsprogrammet så att den matchar storleken som används på webbsidan. Om du vill ändra inställningen permanent kan du ändra visningsprogrammets storlek på installationsskärmen (om du är administratör). Se [Konfigurera förinställningar för zoomvisningsprogrammet](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## Skapa och redigera zoommål {#creating-and-editing-zoom-targets}

Skapa och redigera zoommål på skärmen för zoommålredigeraren. Om du vill öppna den här skärmen markerar du en bild och gör något av följande:

* Klicka på knappen för överrullning **[!UICONTROL Edit]** och välj Zoommål.
* Visa bilden i **[!UICONTROL Detail View]** på panelen Bläddra och klicka sedan på **[!UICONTROL Zoom Targets]**.

Klicka på knappen **[!UICONTROL Select Target]** (pil) i zoommålredigeraren för att markera ett mål innan du ändrar dess storlek eller position. Klicka på **[!UICONTROL Add Targets]** (rektangel) för att skapa ett zoommål på bilden. Skärmen Zoom Target Editor innehåller även verktyg för att ta bort, kopiera och namnge zoommål.

### Skapa ett zoommål {#creating-a-zoom-target}

Öppna fönstret för zoommålredigeraren och följ de här stegen för att skapa ett zoommål:

1. Klicka på **[!UICONTROL Add Targets]** (rektangel), flytta pekaren över bilden och klicka där du vill att zoommålet ska vara.

   En miniatyrbild av zoommålet visas på panelen till höger på skärmen.

1. Klicka på **[!UICONTROL Select Target]** (pil), klicka för att välja det zoommål som du skapade och justera målets storlek och position.

   * **Ändra**
storlekFlytta pekaren över ett hörn av zoommålet och dra för att förstora eller förminska målet.

   * **Placering**
Flytta pekaren över zoommålet och dra den till en annan plats.

1. Ange ett namn för zoommålet i rutan Namn.

   >[!NOTE]
   >
   >Det du anger i rutan Namn är mer än ett namn. När användare flyttar pekaren över zoommålet ser de vad du anger i rutan Namn. Ange en kort beskrivning av zoommålet i rutan Namn så att användarna vet vad de kan zooma i.

1. Du kan också ange användardata i fältet Användardata. Det här fältet är till för webbdesigners som vill lägga till information till zoommålet.
1. Klicka på **[!UICONTROL Save]**.

   Koordinaterna och zoomnivån för zoommålet sparas. En miniatyrbild av zoommålet med det namn du angav visas till höger på skärmen.

>[!NOTE]
>
>Om du vill se hur dina zoommål ser ut i ett zoomvisningsprogram klickar du på knappen Förhandsvisa i zoommålredigeraren och väljer ett zoomvisningsprogram på förhandsvisningsskärmen. Mer information om den här skärmen finns i [Förhandsvisa bilder med olika zoomningsvisningsprogram](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Redigera zoommål {#editing-zoom-targets}

Använd de här teknikerna på skärmen för zoommålredigeraren för att redigera zoommål:

* **Flytta**
omKlicka på målet för att markera det med knappen Välj mål (pilen). Dra sedan målet till en annan plats.

* **Ändra**
storlekMarkera målet genom att klicka på det med knappen Välj mål (pilen). Flytta sedan pekaren över ett hörn av zoommålet och dra för att förstora eller förminska målet.

* **Ta**
bortKlicka på målets miniatyrbild till höger på skärmen. Klicka sedan på **[!UICONTROL Delete Target]**.

* **Byt**
namnKlicka på målets miniatyrbild till höger på skärmen. Ange sedan ett namn i textfältet **[!UICONTROL Name]** och klicka på **[!UICONTROL Save]**.

### Kopierar zoommål {#copying-zoom-targets}

Du kan kopiera zoommål från en bild till en annan. Kopiera mål när två bilder har liknande innehåll och deras zoommål hör till samma platser. Så här kopierar du zoommål till en annan bild:

1. Öppna bilden med de zoommål som du vill kopiera på skärmen för zoommålredigeraren.
1. Klicka på **[!UICONTROL Copy Targets To]**.
1. Markera en bild i dialogrutan Välj bilder och klicka på **[!UICONTROL Select]**.

