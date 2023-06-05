---
title: Länka en bilduppsättning till en webbsida
description: Lär dig hur du länkar en bilduppsättning till en webbsida i Adobe Dynamic Media Classic.
uuid: 8153a228-b2ec-4bc2-8996-266113a83df5
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 40f4abab-9059-4d92-a761-f6d573b42e00
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: df4e5218-2a66-413c-b247-b2a16d884041
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 0%

---

# Länka en bilduppsättning till en webbsida{#linking-an-image-set-to-a-web-page}

När du har publicerat en bilduppsättning kan du kopiera dess URL eller dess inbäddningskod för användning på din webbplats eller i ditt program. Sedan kan du distribuera URL:en eller klistra in inbäddningskoden om det behövs så att användarna kan visa bilduppsättningen på din webbplats eller i ditt program.

>[!NOTE]
>
>URL:en är inte aktiv förrän du publicerar resursen.

## Kopiera en URL för bilduppsättning {#copying-an-image-set-url}

1. Välj i listrutan Visa på panelen Resurser **[!UICONTROL Image Set]**.
1. navigera till resursmappen som innehåller den bilduppsättning vars inbäddningskod du vill kopiera i panelen Resursbibliotek på vänster sida.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Välj **[!UICONTROL Grid View]**. Dubbelklicka på en enskild resurs på panelen Resursbläddring för att öppna den i detaljvyn. I panelen URL:er och panelen Bädda in kod till höger väljer du **[!UICONTROL Copy URL]** till höger om det visningsprogram du vill använda.
   * Välj **[!UICONTROL Grid View]**. Markera en resurs i panelen Resurssökning och gå sedan till under miniatyrbilden **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      På sidan Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Copy URL]**.

   * Välj **[!UICONTROL List View]**. Välj en resurs i panelen Resursbläddring och gå sedan till höger om miniatyrbilden till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      På sidan Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Copy URL]**.

   * Välj **[!UICONTROL Grid View]**, **[!UICONTROL List View]**, eller **[!UICONTROL Detail View]**. På samma verktygsfält går du till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      På sidan Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Copy URL]**.

## Lägga till URL:er för bilduppsättning på webbsidan {#adding-image-set-urls-to-your-web-page}

Det vanligaste sättet att distribuera bilduppsättningar är att placera en länk (via en navigeringsikon) på webbsidan. När du klickar på länken öppnas en dynamisk sida (JSP) som visar bilduppsättningen i ett popup-fönster för zoomning. Zoomlänken öppnar ett popup-fönster som innehåller den faktiska zoomfunktionen.

Mer information och kodexempel finns i [Bädda in HTML5 Zoom Viewer i referenshandboken för visningsprogrammen för Adobe](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/zoom/c-html5-20-zoom-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Kopiera inbäddningskoden för ett visningsprogram för bilduppsättning {#copying-the-embed-code-of-an-image-set-viewer}

Med funktionen Bädda in kod kan du granska visningsprogramkoden för den valda bilduppsättningen. Du kan också kopiera koden till Urklipp så att du kan klistra in den på dina webbsidor för att distribuera visningsprogrammet. Det är inte tillåtet att redigera koden i dialogrutan Bädda in kod.

**Så här kopierar du inbäddningskoden för ett visningsprogram för bilduppsättning:**

1. Välj i listrutan Visa på panelen Resurser **[!UICONTROL Image Set]**.
1. navigera till resursmappen som innehåller den bilduppsättning vars inbäddningskod du vill kopiera i panelen Resursbibliotek på vänster sida.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Välj **[!UICONTROL Grid View]**. Dubbelklicka på en enskild resurs på panelen Resursbläddring för att öppna den i detaljvyn. På panelen URL:er till höger väljer du **[!UICONTROL Embed Code]**.
   * Välj **[!UICONTROL Grid View]**. Markera en resurs i panelen Resurssökning och gå sedan till under miniatyrbilden **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      På sidan Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Embed Code]**.

   * Välj **[!UICONTROL List View]**. Välj en resurs i panelen Resursbläddring och gå sedan till höger om miniatyrbilden till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      På sidan Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Embed Code]**.

   * Välj **[!UICONTROL Grid View]**, **Listvy**, eller **Detaljvy**. På samma verktygsfält går du till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      På sidan Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Embed Code]**.

1. I dialogrutan Bädda in kod väljer du **[!UICONTROL Copy to Clipboard]**.

   Det är inte tillåtet att redigera koden i dialogrutan Bädda in kod.

1. Välj **[!UICONTROL Close]**.

>[!MORELIKETHIS]
>
>* [Publicera](publishing-files.md#publishing_files)

