---
title: 'Snabbstart: Integrering med Adobe Target Standard/Premium'
description: En introduktion och snabbstart till Adobe Target Standard/Premium som hjälper dig att komma igång snabbt med integreringsteknikerna Adobe Target Standard/Premium i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 0%

---

# Snabbstart: Integrering med Adobe Target Standard/Premium{#quick-start-target-integration}

Adobe Target Standard/Premium ger marknadsförarna direkt kontroll. Om du gör det kan du snabbt och kontinuerligt köra flera A/B- och multivariata tester och mäta effektiviteten. Och det kan göra onlinematerialet mer relevant genom segmentering, målinriktning och Automated Personalization.

Med Adobe Dynamic Media Classic kan ni skapa erbjudanden och erbjudanden för Adobe Target Standard/Premium-kampanjer. Du kan till exempel skapa en Erbjudandeuppsättning med tre varianter av samma mediefil. Sedan kan du låta Adobe Target Standard eller Premium avgöra vilken mediefil som ger bättre konverteringshöjning. Du kan skapa erbjudanden och erbjudandeuppsättningar från en grundmall eller från enskilda bilder. När erbjudandeuppsättningen har överförts eller sparats till Adobe Target Standard/Premium, där erbjudandena är kopplade till kartonger och upplevelser, kan Adobe Target Standard/Premium köra kampanjer. Dessa kampanjer avgör vilken typ av webbplats som troligen fungerar bäst för klickningar och konvertering.

Om du vill anpassa dynamiskt Adobe Dynamic Media Classic-innehåll ännu mer kan du använda Adobe Target Standard/Premium HTML. Mer information finns i [produktdokumentationen för Adobe Target Standard/Premium](https://experienceleague.adobe.com/en/docs/target).

>[!NOTE]
>
>Du måste ha ett giltigt Adobe Target Standard-/Premium-konto för att kunna använda Adobe Target Standard/Premium med Adobe Dynamic Media Classic.

Den här snabbstarten är utformad för att du snabbt ska komma igång med Adobe Target Standard/Premium HTML Offer Sets. Följ steg 1 till 3. Efter varje steg finns det en korsreferens till en ämnesrubrik där du kan hitta mer information.

## &#x200B;1. Ange din Adobe Target Standard/Premium-URL på sidan med allmänna inställningar för programmet

Adobe Dynamic Media Classic behöver din Adobe Target Standard/Premium-URL för att kunna integreras med Adobe Target Standard/Premium. Kopiera delen av din Adobe Target Standard/Premium-URL till och med `.com` och ange den på Adobe Dynamic Media Classic **[!UICONTROL Application General Settings]** -sidan i textfältet **[!UICONTROL Servers]** i gruppen **[!UICONTROL Test&Target Server Name]** . Se [Integrera Adobe Dynamic Media Classic med Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## &#x200B;2. Skapa erbjudandeuppsättningen

Använd en parametriserad mall eller bilder för att skapa en erbjudandeuppsättning. Du kan skapa HTML Offer Sets på sidan Test&amp;Target Offer Set. Om du vill öppna den här sidan markerar du mallen eller bilderna och går sedan till **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]** i fältet Global navigering.

Om du vill skapa ett erbjudande med en mall väljer du **[!UICONTROL Add & Preview]**. Ändra parametervärden på sidan Lägg till och förhandsvisa.

Om du vill skapa ett erbjudande med bilder drar du bilderna till sidan Test&amp;Target Offer Set. Välj **[!UICONTROL Preview]** och välj en bildförinställning för en bild eller alla bilder i erbjudandeuppsättningen.

Spara erbjudandeuppsättningen när du har skapat den.

Se [Skapa en erbjudandeuppsättning](creating-offer-set.md#creating_an_offer_set).

## &#x200B;3. Skicka erbjudandet till Adobe Target Standard/Premium

Välj **[!UICONTROL Push Offers]** på sidan Test&amp;Target Offer Set och ange dina inloggningsuppgifter i dialogrutan Test&amp;Target Login. Se [Skicka erbjudanden till Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
