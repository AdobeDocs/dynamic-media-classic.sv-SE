---
title: Paketera erbjudanden för Adobe Target Standard/Premium
seo-title: Paketera erbjudanden för Adobe Target Standard/Premium
description: 'null'
seo-description: Lär dig hur du kan skicka erbjudanden till Adobe Target Standard/Premium.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---


# Paketera erbjudanden för Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

När du har skapat eller redigerat ett erbjudande skickar du det till Target Standard/Premium genom att följa dessa steg:

1. Klicka på i fönstret Test&amp;Target Offer Set **[!UICONTROL Push Offers]**.
1. Ange din klientkod och inloggningsuppgifter.
1. Klicka på **[!UICONTROL Login]**.

Under överföringen till Target Standard/Premium kopplas prefixet S7_ automatiskt till början av erbjudandenamnen. Det här prefixet bifogas för att säkerställa att du enkelt hittar erbjudanden för Dynamic Media Classic i Test&amp;Target. Erbjudandet visas till exempel som S7_&lt;erbjudandeuppsättningens namn>_&lt;erbjudandenamn>.

Dynamic Media Classic utnyttjar Target Standard-/Premium-widgeten. Du kan använda Widget-erbjudanden för att lägga upp ditt eget erbjudandeinnehåll utanför Target Standard/Premium. Widgeterbjudanden liknar standarderbjudanden som tillhandahålls utanför Target Standard/Premium. De gör det möjligt för Target Standard/Premium att driftsätta erbjudandeinnehåll som lagras på din server, vilket möjliggör mer sofistikerad och dynamisk användning. Widgeten erbjuder hämtning av innehåll från en URL, cachelagring och leverans av innehållet i ungefär två timmar. Widgeten innehåller funktioner för att skapa dynamiskt innehåll som andra erbjudanden utanför Target Standard/Premium inte har. Om rutan som innehåller erbjudandet innehåller mbox-parametrar som `mboxProductID` och `mbox.offerId`, läggs parametrarna `productId=[PRODUCT_ID]`och `offerID=[OFFERID]` URL till i den begärda URL:en. De här parametrarna kan användas av en tjänst som finns på Widget offer URL för att returnera innehåll utanför Target Standard/Premium som använder produkt- eller orderinformation från dina lådor. Widget-erbjudandet kan också nås via API:t för att skapa erbjudanden utanför Target Standard/Premium.