---
title: Länka en e-katalog till en webbsida
description: Lär dig hur du länkar en e-katalog till en webbsida i Adobe Dynamic Media Classic.
uuid: 90098a90-180b-477a-8533-24a52a93200b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 140640f2-3ca4-4b6c-a240-5f01be87fa9c
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: aee72576-1e3e-401c-953d-cc2be27f7dfd
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 0%

---

# Länka en e-katalog till en webbsida{#linking-an-ecatalog-to-a-web-page}

Dina webbplatser och program har åtkomst till Dynamic Media Image Server-innehåll, inklusive e-kataloger, via URL-strängar eller inbäddad kod. Dessa URL-strängar aktiveras under publiceringsprocessen. Om du vill placera URL-strängen eller den inbäddade koden för din eCatalog på dina webbsidor och i dina program kopierar du den från Adobe Dynamic Media Classic.

>[!NOTE]
>
>URL:en är inte aktiv förrän du publicerar resursen.

## Kopiera en eCatalog-URL {#copying-an-ecatalog-url}

1. Välj i listrutan Visa på panelen Resurser **[!UICONTROL Catalog]**.
1. navigera till resursmappen som innehåller den eCatalog vars inbäddningskod du vill kopiera i panelen Resursbibliotek på vänster sida.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Välj **[!UICONTROL Grid View]**. Dubbelklicka på en enskild resurs på panelen Resursbläddring för att öppna den i detaljvyn. I panelen URL:er och panelen Bädda in kod till höger väljer du **[!UICONTROL Copy URL]** till höger om det visningsprogram du vill använda.
   * Välj **[!UICONTROL Grid View]**. Markera en resurs i panelen Resurssökning och gå sedan till under miniatyrbilden **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      På sidan Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Copy URL]**.

   * Välj **[!UICONTROL List View]**. Välj en resurs i panelen Resursbläddring och gå sedan till höger om miniatyrbilden till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      På sidan Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Copy URL]**.

   * Välj **[!UICONTROL Grid View]**, **[!UICONTROL List View]**, eller **[!UICONTROL Detail View]**. På samma verktygsfält går du till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      På sidan Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **Kopiera URL**.

## Lägga till eCatalog-URL:er på din webbsida {#adding-ecatalog-urls-to-your-web-page}

Det vanligaste sättet att distribuera en e-katalog är att placera en länk i form av en försättssida med en eCatalog-miniatyrbild på webbsidan. Samarbeta med IT-avdelningen för att säkerställa att e-katalogen öppnas i ett rent, centrerat popup-fönster. Be IT-avdelningen att inte visa verktygsfältet och adressfältet i webbläsaren.

Mer information och kodexempel finns i [Bädda in HTML5 eCatalog Viewer i referenshandboken för Adobe Viewer](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/ecatalog/c-html5-20-ecatalog-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Kopiera inbäddningskoden för ett eCatalog-visningsprogram {#copying-the-embed-code-of-an-ecatalog-viewer}

Med funktionen Bädda in kod kan du granska visningsprogramkoden för den valda e-katalogen. Du kan också kopiera koden till Urklipp så att du kan klistra in den på dina webbsidor för att distribuera visningsprogrammet. Det är inte tillåtet att redigera koden i dialogrutan Bädda in kod.

**Så här kopierar du inbäddningskoden för ett eCatalog-visningsprogram:**

1. Välj i listrutan Visa på panelen Resurser **[!UICONTROL Catalog]**.
1. navigera till resursmappen som innehåller den eCatalog vars inbäddningskod du vill kopiera i panelen Resursbibliotek på vänster sida.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Välj **[!UICONTROL Grid View]**. Dubbelklicka på en enskild resurs på panelen Resursbläddring för att öppna den i detaljvyn. På panelen URL:er till höger väljer du **[!UICONTROL Embed Code]**.
   * Välj **[!UICONTROL Grid View]**. Markera en resurs i panelen Resurssökning och gå sedan till under miniatyrbilden **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      På sidan Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Embed Code]**.

   * Välj **[!UICONTROL List View]**. Välj en resurs i panelen Resursbläddring och gå sedan till höger om miniatyrbilden till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      På sidan Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Embed Code]**.

   * Välj **[!UICONTROL Grid View]**, **[!UICONTROL List View]**, eller **[!UICONTROL Detail View]**. På samma verktygsfält går du till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      På sidan Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Embed Code]**.

1. I dialogrutan Bädda in kod väljer du **[!UICONTROL Copy to Clipboard]**.

   Det är inte tillåtet att redigera koden i dialogrutan Bädda in kod.

1. Välj **[!UICONTROL Close]**.
