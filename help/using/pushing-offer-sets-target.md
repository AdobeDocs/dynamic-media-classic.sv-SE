---
title: Erbjudandet gäller Adobe Target Standard/Premium
description: Lär dig hur du kan skicka erbjudanden till Adobe Target Standard/Premium från Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
topic: Integrations, Development
level: Experienced
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Erbjudandet gäller Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

När du har skapat eller redigerat ett erbjudande skickar du det till Adobe Target Standard/Premium genom att följa dessa steg:

1. I fönstret Test&amp;Target Offer Set väljer du **[!UICONTROL Push Offers]**.
1. Ange din klientkod och inloggningsuppgifter.
1. Välj **[!UICONTROL Login]**.

Under överföringen till Adobe Target Standard/Premium är prefixet `S7_` bifogas automatiskt till början av erbjudandenamnen. Det här prefixet bifogas för att säkerställa att du enkelt hittar Adobe Dynamic Media Classic-erbjudanden i listan Test&amp;Target. Erbjudandet ser ut som `S7_<name of offer set>_<offer name>`.

Adobe Dynamic Media Classic lanserar widgeten Adobe Target Standard/Premium. Du kan använda Widget-erbjudanden för att lagra ditt eget erbjudna innehåll utanför Adobe Target Standard/Premium. Widgeterbjudanden liknar standarderbjudanden som finns utanför Adobe Target Standard/Premium. De gör att Adobe Target Standard/Premium kan distribuera innehåll som finns på din server, vilket möjliggör mer sofistikerad och dynamisk användning. Widget-erbjudanden kan hämta innehåll från en URL, cachelagra och leverera innehållet i ungefär två timmar. Widgeten innehåller funktioner för att skapa dynamiskt innehåll som inte finns i Adobe Target Standard/Premium. Om rutan som innehåller erbjudandet innehåller mbox-parametrar som `mboxProductID` och `mbox.offerId`, `productId=[PRODUCT_ID]`och `offerID=[OFFERID]` URL-parametrar läggs till den begärda URL:en. Dessa parametrar kan användas av en tjänst som finns på Widget offer URL för att returnera innehåll utanför Adobe Target Standard/Premium som använder produkt- eller orderinformation från dina kartor. Widget-erbjudandet kan också nås via API:t för att skapa erbjudanden utanför Adobe Target Standard/Premium.
