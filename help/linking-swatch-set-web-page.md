---
title: Länka en färgruteuppsättning till en webbsida
description: Lär dig hur du länkar en färgruteuppsättning till en webbsida i Adobe Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 8bb1c744-270a-4752-b163-443708fca6c2
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 0%

---

# Länka en färgruteuppsättning till en webbsida{#linking-a-swatch-set-to-a-web-page}

När du har publicerat en färgruteuppsättning kan du använda dess URL-adress eller inbäddningskod på din webbplats eller i ditt program. Sedan kan du distribuera URL-adressen eller inbäddningskoden efter behov så att användarna kan visa färgruteuppsättningen på din webbplats eller i ditt program.

>[!NOTE]
>
>URL:en är inte aktiv förrän du publicerar resursen.

## Kopiera en URL för färgruteuppsättning {#copying-a-swatch-set-url}

1. Välj **[!UICONTROL Swatch Set]** i listrutan Visa i panelen Resurser.
1. navigera till resursmappen som innehåller den färgruteuppsättning vars inbäddningskod du vill kopiera i resurspanelen till vänster.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Välj **[!UICONTROL Grid View]**. Dubbelklicka på en enskild resurs på panelen Resursbläddring för att öppna den i detaljvyn. Välj **[!UICONTROL Copy URL]** till höger om det visningsprogram du vill använda i panelen URL:er och Bädda in kod till höger.
   * Välj **[!UICONTROL Grid View]**. Markera en enskild resurs på panelen Resursbläddring och gå sedan till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** under miniatyrbilden.

      Välj **[!UICONTROL Copy URL]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Välj **[!UICONTROL List View]**. Markera en enskild resurs på panelen Resursbläddring och gå sedan till höger om miniatyrbilden till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Välj **[!UICONTROL Copy URL]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Välj **[!UICONTROL Grid View]**, **[!UICONTROL List View]** eller **[!UICONTROL Detail View]**. Gå till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** på samma verktygsfält.

      Välj **[!UICONTROL Copy URL]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

## Lägg till färgruteuppsättningar av URL:er till din webbsida {#adding-swatch-set-urls-to-your-web-page}

Det vanligaste sättet att distribuera färgruteuppsättningar är att placera en länk (via en navigeringsikon) på webbsidan. När du klickar på länken öppnas en dynamisk sida (ASP eller JSP) som visar uppsättningen med färgrutor i ett popup-fönster för zoomning. Zoomlänken öppnar ett popup-fönster som innehåller den faktiska zoomfunktionen.

Mer information och kodexempel finns i [Bädda in HTML5 Zoom Viewer i referenshandboken för Adobe-visningsprogram](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/zoom/c-html5-20-zoom-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Kopiera inbäddningskoden för ett visningsprogram för färgrutor {#copying-the-embed-code-of-a-swatch-set-viewer}

Med funktionen Bädda in kod kan du granska visningsprogramkoden för den valda uppsättningen med färgrutor. Du kan också kopiera koden till Urklipp så att du kan klistra in den på dina webbsidor för att distribuera visningsprogrammet. Det är inte tillåtet att redigera koden i dialogrutan Bädda in kod.

**Så här kopierar du inbäddningskoden för ett visningsprogram för färgrutor:**

1. Välj **[!UICONTROL Swatch Set]** i listrutan Visa i panelen Resurser.
1. navigera till resursmappen som innehåller den färgruteuppsättning vars inbäddningskod du vill kopiera i resurspanelen till vänster.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Välj **[!UICONTROL Grid View]**. Dubbelklicka på en enskild resurs på panelen Resursbläddring för att öppna den i detaljvyn. Välj **[!UICONTROL Embed Code]** till höger om det visningsprogram du vill använda i panelen URL:er och Bädda in kod till höger.
   * Välj **[!UICONTROL Grid View]**. Markera en enskild resurs på panelen Resursbläddring och gå sedan till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** under miniatyrbilden.

      Välj **[!UICONTROL Embed Code]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Välj **[!UICONTROL List View]**. Markera en enskild resurs på panelen Resursbläddring och gå sedan till höger om miniatyrbilden till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Välj **[!UICONTROL Embed Code]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Välj **[!UICONTROL Grid View]**, **[!UICONTROL List View]** eller **[!UICONTROL Detail View]**. Gå till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** på samma verktygsfält.

      Välj **[!UICONTROL Embed Code]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

1. Välj **[!UICONTROL Copy to Clipboard]** i dialogrutan Bädda in kod.

   Det är inte tillåtet att redigera koden i dialogrutan Bädda in kod.

1. Välj **[!UICONTROL Close]**.

>[!MORELIKETHIS]
>
>* [Publicera](publishing-files.md#publishing_files)

