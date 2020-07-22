---
title: '"Snabbstart: Integrering av Target Standard/premium"'
seo-title: '"Snabbstart: Integrering av Target Standard/premium"'
description: 'null'
seo-description: En introduktion och snabbstart till Adobe Target Standard/Premium som hjälper dig att komma igång snabbt med Target Standard/Premium-integreringstekniker.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
translation-type: tm+mt
source-git-commit: 38f5cf5264f9775a225d354ed9dc2f6caee236f2
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---


# Snabbstart: Integrering av Target Standard/premium{#quick-start-target-integration}

Med Adobe Target Standard/Premium får marknadsförarna kontroll direkt för att snabbt och kontinuerligt köra flera A/B-tester och multivariata tester, mäta effektiviteten och öka relevansen för onlinematerial genom segmentering, målinriktning och automatiserad personalisering.

Med Dynamic Media Classic kan du skapa erbjudanden och uppsättningar för Target Standard-/Premium-kampanjer. Du kan till exempel skapa en erbjudandeuppsättning med tre varianter av samma mediefil. Sedan kan du låta Target Standard/Premium avgöra vilken resurs som ger bättre konverteringshöjning. Du kan skapa erbjudanden och uppsättningar från en grundmall eller från enskilda bilder. När erbjudandet har skickats vidare eller sparats till Adobe Target Standard/Premium, där erbjudandena är kopplade till kartonger och upplevelser, kan Target Standard/Premium köra kampanjer för att avgöra vilken typ av webbplats som troligen fungerar bäst för klickningar och konverteringar.

Om du vill anpassa dynamiskt Dynamic Media Classic-innehåll mer använder du Target Standard/Premium HTML-erbjudanden. Mer information finns i produktdokumentationen för Target Standard/Premium.

>[!NOTE]
>
>Du måste ha ett giltigt Adobe Target Standard-/Premium-konto för att kunna använda Target Standard/Premium med Dynamic Media Classic.

**Snabbstart**

Den här snabbstarten är utformad för att du snabbt ska komma igång med Target Standard/Premium HTML-erbjudanden. Följ steg 1 till 3. Efter varje steg finns en korsreferens till en ämnesrubrik där du kan hitta mer information.

**1. Ange din Target Standard-/Premium-URL på skärmen för allmänna inställningar för programmet.**

Dynamic Media Classic behöver din Target Standard-/Premium-URL för att kunna integreras med Target Standard/Premium. Kopiera delen av Target Standard-/Premium-URL:en till och med *.com* och ange den på skärmen Allmänna inställningar i Dynamic Media Classic-programmet. Se [Integrera Dynamic Media Classic med Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

**2. Skapa erbjudandeuppsättningen**

Använd en parametriserad mall eller bilder för att skapa en erbjudandeuppsättning. Du skapar uppsättningar med HTML-erbjudanden på skärmen Test&amp;Target Offer Set. Om du vill öppna den här skärmen markerar du mallen eller bilderna och klickar på **Skapa** > **Test&amp;Target-erbjudandeuppsättning**.

Om du vill skapa ett erbjudande med en mall klickar du på **Lägg till och förhandsgranska**. Ändra parametervärden på skärmen Lägg till och förhandsvisa.

Om du vill skapa ett erbjudande med bilder drar du bilder till skärmen Test&amp;Target Offer Set. Klicka på **Förhandsvisa** för att välja en bildförinställning för en bild eller alla bilder i erbjudandeuppsättningen.

Spara erbjudandet när du skapat det.

Se [Skapa en erbjudandeuppsättning](creating-offer-set.md#creating_an_offer_set).

**3. Skicka erbjudandet till Target Standard/Premium**

På skärmen Test&amp;Target Offer Set klickar du på **Push Offers** och anger dina inloggningsuppgifter i dialogrutan Test&amp;Target Login. Se [Paketera erbjudanden för Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
