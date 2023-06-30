---
title: Länka zoomningsvisningsprogram till dina webbsidor
description: Lär dig hur du länkar zoomningsvisningsprogram till webbsidor i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: 2073d95b-1600-481f-8038-d29e8acacf7d
topic: Administration, Content Management, Development
level: Intermediate
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 0%

---

# Länka zoomningsvisningsprogram till dina webbsidor{#linking-zoom-viewers-to-your-web-pages}

Dina webbplatser och program har åtkomst till Dynamic Media Image Server-innehåll, inklusive primära bilder och associerade zoommål, och förinställningar för Zoom Viewer, via URL-strängar eller inbäddad kod. Dessa URL-strängar aktiveras under publiceringsprocessen. Om du vill placera dessa URL-strängar eller den inbäddade koden på dina webbsidor och i dina program kopierar du dem från Adobe Dynamic Media Classic.

>[!NOTE]
>
>URL:en är inte aktiv förrän du publicerar resursen.

## Kopiera en URL för zoomvisningsprogrammet {#copying-a-zoom-viewer-url}

1. navigera till resursmappen som innehåller det zoomvisningsprogram vars URL du vill kopiera i resurspanelen till vänster.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Välj **[!UICONTROL Grid View]** eller **[!UICONTROL List View]**. Dubbelklicka på en enskild resurs på panelen Resursbläddring för att öppna den i detaljvyn. I panelen URL:er och panelen Bädda in kod till höger väljer du **[!UICONTROL Copy URL]** till höger om det visningsprogram du vill använda.
   * Välj **[!UICONTROL Grid View]**. Markera en resurs i panelen Resurssökning och gå sedan till under miniatyrbilden **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     På sidan Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Copy URL]**.

   * Välj **[!UICONTROL List View]**. Välj en resurs i panelen Resursbläddring och gå sedan till höger om miniatyrbilden till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     På sidan Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Copy URL]**.

   * Välj **[!UICONTROL Grid View]**, **[!UICONTROL List View]**, eller **[!UICONTROL Detail View]**. På samma verktygsfält går du till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     På sidan Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Copy URL]**.

## Lägga till URL-adresser för Zoom-visningsprogram på webbsidan {#adding-zoom-viewer-urls-to-your-web-page}

Vanligtvis zoomar besökarna bilder på en webbplats genom att först välja en zoomningsikon (ofta visas bilden av ett förstoringsglas). Om du väljer den här ikonen öppnas en dynamisk webbsida (ASP eller JSP) som visar bilden i ett popup-fönster. I popup-fönstret kan besökarna zooma in bilden.

Mer information och kodexempel finns i [Bädda in HTML5 Basic Zoom Viewer i referenshandboken för visningsprogrammen för Adobe](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Kopiera den inbäddade kopian av ett Zoom-visningsprogram {#copying-the-embed-copy-of-a-zoom-viewer}

Med funktionen Bädda in kod kan du granska visningsprogramkoden för det valda zoomvisningsprogrammet. Du kan också kopiera koden till Urklipp så att du kan klistra in den på dina webbsidor för att distribuera visningsprogrammet. Det är inte tillåtet att redigera koden i dialogrutan Bädda in kod.

**Så här kopierar du inbäddningskoden för ett Zoom-visningsprogram:**

1. navigera till resursmappen som innehåller Zoom-visningsprogrammet vars inbäddningskod du vill kopiera i panelen Resursbibliotek på vänster sida.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Välj **[!UICONTROL Grid View]**. Dubbelklicka på en enskild resurs på panelen Resursbläddring för att öppna den i detaljvyn. I panelen URL:er och panelen Bädda in kod till höger väljer du **[!UICONTROL Embed Code]** till höger om det visningsprogram du vill använda.
   * Välj **[!UICONTROL Grid View]**. Markera en resurs i panelen Resurssökning och gå sedan till under miniatyrbilden **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     På sidan Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Embed Code]**.

   * Välj **[!UICONTROL List View]**. Välj en resurs i panelen Resursbläddring och gå sedan till höger om miniatyrbilden till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     På sidan Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Embed Code]**.

   * Välj **[!UICONTROL Grid View]**, **[!UICONTROL List View]**, eller **[!UICONTROL Detail View]**. På samma verktygsfält går du till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     På sidan Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Embed Code]**.

1. I dialogrutan Bädda in kod väljer du **[!UICONTROL Copy to Clipboard]**.

   Det är inte tillåtet att redigera koden i dialogrutan Bädda in kod.

1. Välj **[!UICONTROL Close]**.
