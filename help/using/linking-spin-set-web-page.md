---
title: Länka en snurruppsättning till en webbsida
description: Lär dig hur du länkar en snurruppsättning till en webbsida i Adobe Dynamic Media Classic.
uuid: d3c5773e-60c4-4e8b-9c48-e1e3eb8028d0
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 651b21ef-e322-4e6d-8e37-45ffd56f7a58
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 0%

---

# Länka en snurruppsättning till en webbsida{#linking-a-spin-set-to-a-web-page}

Webbplatser och program har åtkomst till Dynamic Media Image Server-innehåll, inklusive snurruppsättningar, via URL-strängar eller inbäddad kod. Dessa URL-strängar aktiveras under publiceringsprocessen. Om du vill placera URL-strängen eller inbäddningskoden för din snurruppsättning på dina webbsidor och i dina program kopierar du den från Adobe Dynamic Media Classic.

>[!NOTE]
>
>URL:en är inte aktiv förrän du publicerar resursen.

## Kopiera en URL för en snurruppsättning {#copying-a-spin-set-url}

1. Välj i listrutan Visa på panelen Resurser **[!UICONTROL Spin Set]**.
1. navigera till resursmappen som innehåller den snurra uppsättning vars inbäddningskod du vill kopiera i resurspanelen till vänster.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Välj **[!UICONTROL Grid View]**. Dubbelklicka på en enskild resurs på panelen Resursbläddring för att öppna den i detaljvyn. I panelen URL:er och panelen Bädda in kod till höger väljer du **[!UICONTROL Copy URL]** till höger om det visningsprogram du vill använda.
   * Välj **[!UICONTROL Grid View]**. Markera en resurs i panelen Resurssökning och gå sedan till under miniatyrbilden **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     På sidan Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Copy URL]**.

   * Välj **[!UICONTROL List View]**. Välj en resurs i panelen Resursbläddring och gå sedan till höger om miniatyrbilden till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     På sidan Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Copy URL]**.

   * Välj **[!UICONTROL Grid View]**, **[!UICONTROL List View]**, eller **[!UICONTROL Detail View]**. På samma verktygsfält går du till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

     På sidan Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Copy URL]**.

## Lägga till URL-adresser för snurruppsättning på webbsidan {#adding-spin-set-urls-to-your-web-page}

Snurra uppsättningar används som alla zoomningsvisningsprogram via en dynamisk sida (ASP eller JSP) som visar snurra uppsättningar i ett zoomfönster. URL-anropet till Adobe Dynamic Media Classic-plattformen följer samma protokoll i zoomvisningsprogrammet. Namnet på visningsförinställningen beror dock på den förinställning som administratören har definierat som förinställning för rotationsuppsättningen. I följande exempel på icke-aktiv URL-syntax finns ett förinställningsnamn med namnet `viewer.jsp` och SKU-parametern är nu Spin Set-namnet:

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

I det här exemplet på URL-syntax (länken är inte live), lägg märke till ett SKU-nummer ( `sku=backpack_spin`). Strängen efter `sku=` är namnet på rotationsuppsättningen ( `backpack spin`).

## Kopiera inbäddningskoden för ett visningsprogram för sned uppsättning {#copying-the-embed-code-of-a-spin-set-viewer}

Med hjälp av funktionen Bädda in kod kan du granska visningsprogramkoden för den valda rotationsuppsättningen. Du kan också kopiera koden till Urklipp så att du kan klistra in den på dina webbsidor för att distribuera visningsprogrammet. Det är inte tillåtet att redigera koden i dialogrutan Bädda in kod.

**Så här kopierar du inbäddningskoden för ett visningsprogram för en sned uppsättning:**

1. Välj i listrutan Visa på panelen Resurser **[!UICONTROL Spin Set]**.
1. navigera till resursmappen som innehåller den snurra uppsättning vars inbäddningskod du vill kopiera i resurspanelen till vänster.
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
