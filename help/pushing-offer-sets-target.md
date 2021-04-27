---
title: Paketera erbjudanden för Adobe Target Standard/Premium
description: Lär dig hur du kan skicka erbjudanden till Adobe Target Standard/Premium.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
translation-type: tm+mt
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Paketera erbjudanden till Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

När du har skapat eller redigerat ett erbjudande skickar du det till Adobe Target Standard/Premium genom att följa dessa steg:

1. Klicka på **[!UICONTROL Push Offers]** på skärmen Test&amp;Target Offer Set.
1. Ange din klientkod och inloggningsuppgifter.
1. Klicka på **[!UICONTROL Login]**.

Under överföringen till Adobe Target Standard/Premium kopplas prefixet `S7_` automatiskt till början av erbjudandenamnen. Det här prefixet bifogas för att säkerställa att du enkelt hittar erbjudanden för Dynamic Media Classic i listan Test&amp;Target. Erbjudandet visas till exempel som `S7_<name of offer set>_<offer name>`.

Dynamic Media Classic utnyttjar Adobe Target Standard/Premium-widgeten. Du kan använda Widget-erbjudanden för att lägga upp ditt eget erbjudandeinnehåll utanför Adobe Target Standard/Premium. Widgeterbjudanden liknar standarderbjudanden som finns utanför Adobe Target Standard/Premium. De gör att Adobe Target Standard/Premium kan distribuera innehåll som finns på din server, vilket möjliggör mer sofistikerad och dynamisk användning. Widgeten erbjuder hämtning av innehåll från en URL, cachelagring och leverans av innehållet i ungefär två timmar. Widgeten innehåller funktioner för att skapa dynamiskt innehåll som inte finns i Adobe Target Standard/Premium. Om den ruta som innehåller erbjudandet innehåller mbox-parametrar som `mboxProductID` och `mbox.offerId`, läggs URL-parametrarna `productId=[PRODUCT_ID]`och `offerID=[OFFERID]` till i den begärda URL:en. Dessa parametrar kan användas av en tjänst som finns på Widget offer URL för att returnera innehåll utanför Adobe Target Standard/Premium som använder produkt- eller orderinformation från dina kartor. Widget-erbjudandet kan också nås via API:t för att skapa erbjudanden utanför Adobe Target Standard/Premium.
