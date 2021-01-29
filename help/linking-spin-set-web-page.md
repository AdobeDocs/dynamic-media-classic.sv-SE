---
title: Länka en snurruppsättning till en webbsida
description: Lär dig hur du länkar en snurruppsättning till en webbsida.
uuid: d3c5773e-60c4-4e8b-9c48-e1e3eb8028d0
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 651b21ef-e322-4e6d-8e37-45ffd56f7a58
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---


# Länka en snurruppsättning till en webbsida{#linking-a-spin-set-to-a-web-page}

Webbplatser och program har åtkomst till Dynamic Media Image Server-innehåll, inklusive snurruppsättningar, via URL-strängar eller inbäddad kod. Dessa URL-strängar aktiveras under publiceringsprocessen. Om du vill placera URL-strängen eller inbäddningskoden för din snurruppsättning på dina webbsidor och i dina program kopierar du den från Dynamic Media Classic.

>[!NOTE]
>
>URL:en är inte aktiv förrän du publicerar resursen.

## Kopiera en URL för snurruppsättning {#copying-a-spin-set-url}

1. Klicka på **Snurra uppsättning** i listrutan Visa på panelen Resurser.
1. navigera till resursmappen som innehåller den snurra uppsättning vars inbäddningskod du vill kopiera i resurspanelen till vänster.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Klicka på **Stödrastervisning**. Dubbelklicka på en enskild resurs på panelen Resursbläddring för att öppna den i detaljvyn. Klicka på **Kopiera URL** till höger om det visningsprogram du vill använda i panelen URL:er och Bädda in kod till höger.
   * Klicka på **Stödrastervisning**. Markera en enskild resurs på panelen Resursbläddring och klicka sedan under miniatyrbilden på **Förhandsvisa** > **Visningsprogramlista**.

      Klicka på **Kopiera URL** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Klicka på **Listvy**. Markera en enskild resurs på panelen Resursbläddring och klicka sedan på **Förhandsvisa** > **Visningsprogramlista** till höger om miniatyrbilden.

      Klicka på **Kopiera URL** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Klicka på **Stödrastervisning**, **Listvy** eller **Detaljvy**. Klicka på **Förhandsgranska** > **Visningsprogramlista** i samma verktygsfält.

      Klicka på **Kopiera URL** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

## Lägga till URL:er för snurruppsättning på webbsidan {#adding-spin-set-urls-to-your-web-page}

Snurra uppsättningar används som alla zoomningsvisningsprogram via en dynamisk sida (ASP eller JSP) som visar snurra uppsättningar i ett zoomfönster. URL-anropet till Dynamic Media Classic-plattformen följer samma protokoll i zoomvisningsprogrammet. Namnet på visningsförinställningen beror dock på den förinställning som administratören har definierat som förinställning för rotationsuppsättningen. I följande exempel på icke-aktiv URL-syntax finns ett förinställningsnamn med namnet `viewer.jsp` och SKU-parametern är nu namnet på den aktiva uppsättningen:

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

Lägg märke till ett SKU-nummer ( `sku=backpack_spin`) i det här exemplet på URL-syntax (länken är inte aktiv). Strängen efter `sku=` är namnet på den tomma uppsättningen ( `backpack spin`).

## Kopiera inbäddningskoden för ett visningsprogram för sned uppsättning {#copying-the-embed-code-of-a-spin-set-viewer}

Med hjälp av funktionen Bädda in kod kan du granska visningsprogramkoden för den valda rotationsuppsättningen. Du kan också kopiera koden till Urklipp så att du kan klistra in den på dina webbsidor för att distribuera visningsprogrammet. Det är inte tillåtet att redigera koden i dialogrutan Bädda in kod.

**Så här kopierar du inbäddningskoden för ett visningsprogram för sned uppsättning**

1. Klicka på **Snurra uppsättning** i listrutan Visa på panelen Resurser.
1. navigera till resursmappen som innehåller den snurra uppsättning vars inbäddningskod du vill kopiera i resurspanelen till vänster.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Klicka på **Stödrastervisning**. Dubbelklicka på en enskild resurs på panelen Resursbläddring för att öppna den i detaljvyn. Klicka på **Bädda in kod** till höger om det visningsprogram du vill använda i panelen URL:er och Bädda in kod till höger.
   * Klicka på **Stödrastervisning**. Markera en enskild resurs på panelen Resursbläddring och klicka sedan under miniatyrbilden på **Förhandsvisa** > **Visningsprogramlista**.

      Klicka på **Bädda in kod** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Klicka på **Listvy**. Markera en enskild resurs på panelen Resursbläddring och klicka sedan på **Förhandsvisa** > **Visningsprogramlista** till höger om miniatyrbilden.

      Klicka på **Bädda in kod** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

   * Klicka på **Stödrastervisning**, **Listvy** eller **Detaljvy**. Klicka på **Förhandsgranska** > **Visningsprogramlista** i samma verktygsfält.

      Klicka på **Bädda in kod** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista.

1. I dialogrutan Bädda in kod klickar du på **Kopiera till Urklipp**.

   Det är inte tillåtet att redigera koden i dialogrutan Bädda in kod.

1. Klicka på Stäng.

