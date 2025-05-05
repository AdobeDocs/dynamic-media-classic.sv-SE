---
title: Länka en bilduppsättning till en webbsida
description: Lär dig hur du länkar en bilduppsättning till en webbsida i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: df4e5218-2a66-413c-b247-b2a16d884041
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---

# Länka en bilduppsättning till en webbsida{#linking-an-image-set-to-a-web-page}

När du har publicerat en bilduppsättning kan du kopiera dess associerade URL eller dess inbäddade kod för användning på din webbplats eller i ditt program. Sedan kan du distribuera URL:en eller klistra in den inbäddade koden så att användarna kan se bilduppsättningen på webbplatsen eller i programmet.

>[!NOTE]
>
>URL:en är inte aktiv förrän du publicerar resursen.

## Kopiera en URL för bilduppsättning {#copying-an-image-set-url}

1. Välj **[!UICONTROL Image Set]** i listrutan Visa på panelen Resursbläddring.
1. navigera till resursmappen som innehåller den bilduppsättning vars inbäddade kod du vill kopiera i panelen Resursbibliotek på vänster sida.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Välj **[!UICONTROL Grid View]**. Dubbelklicka på en enskild resurs på panelen Resursbläddring för att öppna den i detaljvyn. I panelen URL:er och panelen Bädda in kod till höger väljer du **[!UICONTROL Copy URL]** till höger om det visningsprogram du vill använda.
   * Välj **[!UICONTROL Grid View]**. Markera en enskild resurs på panelen Resursbläddring och gå sedan till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** under miniatyrbilden.

     Välj **[!UICONTROL Copy URL]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Välj **[!UICONTROL List View]**. Markera en enskild resurs på panelen Resursbläddring och gå sedan till höger om miniatyrbilden till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Välj **[!UICONTROL Copy URL]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Välj **[!UICONTROL Grid View]**, **[!UICONTROL List View]** eller **[!UICONTROL Detail View]**. Gå till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** i samma verktygsfält.

     Välj **[!UICONTROL Copy URL]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

## Lägga till URL:er för bilduppsättning på webbsidan {#adding-image-set-urls-to-your-web-page}

Det vanligaste sättet att distribuera bilduppsättningar är att placera en länk (via en navigeringsikon) på webbsidan. När du väljer det här alternativet öppnas en dynamisk sida (JSP) som visar bilduppsättningen i ett popup-fönster för zoomning. Zoomlänken öppnar ett popup-fönster som innehåller den faktiska zoomfunktionen.

Mer information och kodexempel finns i [Embed HTML5 Zoom Viewer (Bädda in zoom Viewer) i referenshandboken för Adobe Viewer](https://experienceleague.adobe.com/sv/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/zoom/c-html5-20-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Kopiera inbäddningskoden för en bilduppsättningsvisare {#copying-the-embed-code-of-an-image-set-viewer}

Med funktionen Bädda in kod kan du granska visningsprogramkoden för den valda bilduppsättningen. Du kan också kopiera koden till Urklipp så att du kan klistra in den på webbsidorna för att distribuera visningsprogrammet. Det är inte tillåtet att redigera koden i dialogrutan Bädda in kod.

**Så här kopierar du inbäddningskoden för ett visningsprogram för bilduppsättning:**

1. Välj **[!UICONTROL Image Set]** i listrutan Visa på panelen Resursbläddring.
1. navigera till resursmappen som innehåller den bilduppsättning vars inbäddade kod du vill kopiera i panelen Resursbibliotek på vänster sida.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Välj **[!UICONTROL Grid View]**. Dubbelklicka på en enskild resurs på panelen Resursbläddring för att öppna den i detaljvyn. Välj **[!UICONTROL Embed Code]** på panelen URL:er till höger.
   * Välj **[!UICONTROL Grid View]**. Markera en enskild resurs på panelen Resursbläddring och gå sedan till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** under miniatyrbilden.

     Välj **[!UICONTROL Embed Code]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Välj **[!UICONTROL List View]**. Markera en enskild resurs på panelen Resursbläddring och gå sedan till höger om miniatyrbilden till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Välj **[!UICONTROL Embed Code]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Välj **[!UICONTROL Grid View]**, **listvy** eller **detaljvy**. Gå till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** i samma verktygsfält.

     Välj **[!UICONTROL Embed Code]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

1. Välj **[!UICONTROL Copy to Clipboard]** i dialogrutan Bädda in kod.

   Det är inte tillåtet att redigera koden i dialogrutan Bädda in kod.

1. Välj **[!UICONTROL Close]**.

>[!MORELIKETHIS]
>
>* [Publish](publishing-files.md#publishing_files)
