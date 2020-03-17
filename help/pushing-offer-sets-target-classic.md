---
title: Paketera erbjudanden till Adobe Target Classic
seo-title: Paketera erbjudanden till Adobe Target Classic
description: 'null'
seo-description: Lär dig hur du kan skicka erbjudanden till Adobe Target Classic.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Paketera erbjudanden till Adobe Target Classic{#pushing-offer-sets-to-adobe-target-classic}

När du har skapat eller redigerat en erbjudandeuppsättning skickar du den till Target Classic genom att följa de här stegen:

1. Klicka på knappen Push Offers (Skjut erbjudanden) i fönstret för Classic-erbjudanden.
1. Ange dina inloggningsuppgifter.
1. Klicka på knappen Inloggning.

Under överföringen till Target Classic kopplas prefixet S7_ automatiskt till början av erbjudandenamnen. Det här prefixet bifogas för att säkerställa att du enkelt hittar erbjudanden för Dynamic Media Classic i listan över erbjudanden för Target Classic. Erbjudandet visas till exempel som S7_&lt;erbjudandeuppsättningens namn>_&lt;erbjudandenamn>.

SPS tar steget in i Target Classic-widgeten. Du kan använda Widget-erbjudanden för att lägga upp ditt eget erbjudandeinnehåll utanför Target Classic. Widgeterbjudanden liknar standarderbjudanden som ligger utanför Target Classic. De gör att Target Classic kan distribuera erbjudandeinnehåll som lagras på servern, vilket möjliggör mer sofistikerad och dynamisk användning. Widgeten erbjuder hämtning av innehåll från en URL, cachelagring och leverans av innehållet i ungefär två timmar. Widgeten innehåller funktioner för generering av dynamiskt innehåll som andra erbjudanden utanför Target Classic inte har. Om rutan som innehåller erbjudandet innehåller mbox-parametrar som `mboxProductID` och `mbox.offerId`, läggs parametrarna `productId=[PRODUCT_ID]`och `offerID=[OFFERID]` URL till i den begärda URL:en. De här parametrarna kan användas av en tjänst som finns på Widget offer URL för att returnera innehåll utanför Target Classic som använder produkt- eller orderinformation från dina kryssrutor. Widget-erbjudandet kan också nås via API:t för att programmässigt skapa erbjudanden utanför Target Classic.
