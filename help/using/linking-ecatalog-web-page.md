---
title: Länka en e-katalog till en webbsida
description: Lär dig hur du länkar en e-katalog till en webbsida i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: aee72576-1e3e-401c-953d-cc2be27f7dfd
topic: Integrations, Development
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 0%

---

# Länka en e-katalog till en webbsida{#linking-an-ecatalog-to-a-web-page}

Dina webbplatser och tillämpningar har åtkomst till innehåll från Dynamic Media Image Server, inklusive e-kataloger, via URL-strängar eller inbäddad kod. Dessa URL-strängar aktiveras under publiceringsprocessen. Om du vill placera URL-strängen eller den inbäddade koden för din eCatalog på dina webbsidor och i dina webbprogram kopierar du den från Adobe Dynamic Media Classic.

>[!NOTE]
>
>URL:en är inte aktiv förrän du publicerar resursen.

## Kopiera en eCatalog-URL {#copying-an-ecatalog-url}

1. Välj **[!UICONTROL Catalog]** i listrutan Visa på panelen Resursbläddring.
1. navigera till resursmappen som innehåller den eCatalog vars inbäddningskod du vill kopiera i panelen Resursbibliotek på vänster sida.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Välj **[!UICONTROL Grid View]**. Dubbelklicka på en enskild resurs på panelen Resursbläddring för att öppna den i detaljvyn. I panelen URL:er och panelen Bädda in kod till höger väljer du **[!UICONTROL Copy URL]** till höger om det visningsprogram du vill använda.
   * Välj **[!UICONTROL Grid View]**. Markera en enskild resurs på panelen Resursbläddring och gå sedan till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** under miniatyrbilden.

     Välj **[!UICONTROL Copy URL]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Välj **[!UICONTROL List View]**. Markera en enskild resurs på panelen Resursbläddring och gå sedan till höger om miniatyrbilden till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Välj **[!UICONTROL Copy URL]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Välj **[!UICONTROL Grid View]**, **[!UICONTROL List View]** eller **[!UICONTROL Detail View]**. Gå till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** i samma verktygsfält.

     Välj **Kopiera URL** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

## Lägga till eCatalog-URL:er på webbsidan {#adding-ecatalog-urls-to-your-web-page}

Det vanligaste sättet att distribuera en e-katalog är att placera en länk i form av en försättssida med en eCatalog-miniatyrbild på webbsidan. Samarbeta med IT-avdelningen för att säkerställa att e-katalogen öppnas i ett rent, centrerat popup-fönster. Be IT-avdelningen att inte visa verktygsfältet och adressfältet i webbläsaren.

Mer information och kodexempel finns i [Bädda in HTML5 eCatalog Viewer i referenshandboken för Adobe Viewer](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/ecatalog/c-html5-20-ecatalog-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Kopiera inbäddningskoden för ett eCatalog-visningsprogram {#copying-the-embed-code-of-an-ecatalog-viewer}

Med funktionen Bädda in kod kan du granska visningsprogramkoden för den valda e-katalogen. Du kan också kopiera koden till Urklipp så att du kan klistra in den på webbsidorna för att distribuera visningsprogrammet. Det är inte tillåtet att redigera koden i dialogrutan Bädda in kod.

**Så här kopierar du den inbäddade koden för ett eCatalog-visningsprogram:**

1. Välj **[!UICONTROL Catalog]** i listrutan Visa på panelen Resursbläddring.
1. navigera till resursmappen som innehåller den eCatalog vars inbäddningskod du vill kopiera i panelen Resursbibliotek på vänster sida.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Välj **[!UICONTROL Grid View]**. Dubbelklicka på en enskild resurs på panelen Resursbläddring för att öppna den i detaljvyn. Välj **[!UICONTROL Embed Code]** på panelen URL:er till höger.
   * Välj **[!UICONTROL Grid View]**. Markera en enskild resurs på panelen Resursbläddring och gå sedan till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** under miniatyrbilden.

     Välj **[!UICONTROL Embed Code]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Välj **[!UICONTROL List View]**. Markera en enskild resurs på panelen Resursbläddring och gå sedan till höger om miniatyrbilden till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     Välj **[!UICONTROL Embed Code]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Välj **[!UICONTROL Grid View]**, **[!UICONTROL List View]** eller **[!UICONTROL Detail View]**. Gå till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** i samma verktygsfält.

     Välj **[!UICONTROL Embed Code]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

1. Välj **[!UICONTROL Copy to Clipboard]** i dialogrutan Bädda in kod.

   Det är inte tillåtet att redigera koden i dialogrutan Bädda in kod.

1. Välj **[!UICONTROL Close]**.
