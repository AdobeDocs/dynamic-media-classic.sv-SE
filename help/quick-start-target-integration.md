---
title: '"Snabbstart: Integrering med Adobe Target Standard/Premium"'
description: En introduktion och snabbstart till Adobe Target Standard/Premium som hjälper dig att komma igång snabbt med integreringsteknikerna Adobe Target Standard/Premium.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# Snabbstart: Integrering med Adobe Target Standard/Premium{#quick-start-target-integration}

Med Adobe Target Standard/Premium får marknadsförarna kontroll direkt för att snabbt och kontinuerligt köra flera A/B-tester och multivariata tester, mäta effektiviteten och öka relevansen av onlinematerial genom segmentering, målinriktning och automatiserad personalisering.

Med Dynamic Media Classic kan du skapa erbjudanden och uppsättningar för Adobe Target Standard/Premium-kampanjer. Du kan till exempel skapa en erbjudandeuppsättning med tre varianter av samma mediefil. Sedan kan du låta Adobe Target Standard/Premium avgöra vilken mediefil som ger bättre konverteringshöjning. Du kan skapa erbjudanden och uppsättningar från en grundmall eller från enskilda bilder. När erbjudandet har skickats vidare eller sparats till Adobe Target Standard/Premium, där erbjudandena är kopplade till kartonger och upplevelser, kan Adobe Target Standard/Premium köra kampanjer. Dessa kampanjer avgör vilken typ av webbplats som troligen fungerar bäst för klickningar och konvertering.

Om du vill anpassa dynamiskt Dynamic Media Classic-innehåll ännu mer använder du Adobe Target Standard/Premium HTML. Mer information finns i [Adobe Target Standard/Premium produktdokumentation](https://experienceleague.adobe.com/docs/target.html).

>[!NOTE]
>
>Du måste ha ett giltigt Adobe Target Standard-/Premium-konto för att kunna använda Adobe Target Standard/Premium med Dynamic Media Classic.

Den här snabbstarten är utformad för att du snabbt ska komma igång med Adobe Target Standard/Premium HTML. Följ steg 1 till 3. Efter varje steg finns en korsreferens till en ämnesrubrik där du kan hitta mer information.

## 1. Ange din Adobe Target Standard/Premium-URL på sidan med allmänna inställningar för programmet

Dynamic Media Classic behöver din Adobe Target Standard/Premium-URL för att kunna integreras med Adobe Target Standard/Premium. Kopiera delen av din Adobe Target Standard/Premium-URL till och med `.com` och ange den på sidan Dynamic Media Classic **[!UICONTROL Application General Settings]** i gruppen **[!UICONTROL Servers]** i textfältet **[!UICONTROL Test&Target Server Name]**. Se [Integrera Dynamic Media Classic med Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2. Skapa erbjudandeuppsättningen

Använd en parametriserad mall eller bilder för att skapa en erbjudandeuppsättning. Du skapar uppsättningar med HTML-erbjudanden på sidan Test&amp;Target-erbjudanden. Om du vill öppna den här sidan markerar du mallen eller bilderna och klickar sedan på **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]** i fältet Global navigering.

Om du vill skapa ett erbjudande med en mall klickar du på **[!UICONTROL Add & Preview]**. Ändra parametervärden på sidan Lägg till och förhandsvisa.

Om du vill skapa ett erbjudande med bilder drar du bilderna till sidan Test&amp;Target Offer Set. Klicka på **[!UICONTROL Preview]** och välj en bildförinställning för en bild eller alla bilder i erbjudandeuppsättningen.

Spara erbjudandet när du skapat det.

Se [Skapa en erbjudandeuppsättning](creating-offer-set.md#creating_an_offer_set).

## 3. Skicka erbjudandet till Adobe Target Standard/Premium

Klicka på **[!UICONTROL Push Offers]** på sidan Test&amp;Target Offer Set och ange dina inloggningsuppgifter i dialogrutan Test&amp;Target Login. Se [Paketera erbjudanden till Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
