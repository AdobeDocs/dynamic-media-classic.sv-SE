---
title: Skapa en erbjudandeuppsättning
description: Lär dig hur du skapar en offertuppsättning i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
topic: Integrations, Development
level: Experienced
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '1159'
ht-degree: 0%

---

# Skapa en erbjudandeuppsättning {#creating-an-offer-set}

Du kan skapa följande typer av erbjudandeuppsättningar:

* Video
* Parametriserad mall
* Bild

Välj för mallar **[!UICONTROL Add and Preview]** anger du sedan de parametrar du vill använda. Andra objekttyper innehåller inga parametrar, men du kan fortfarande anpassa dem genom att välja **[!UICONTROL Preview]** och ändra de tillgängliga förinställningarna.

Adobe Dynamic Media Classic har verktyg för redigering och framtagning av erbjudandeuppsättningar.

>[!NOTE]
>
>Innan du skapar en erbjudandeuppsättning måste du se till att publicera alla resurser som du vill använda för uppsättningen till Adobe Dynamic Media Classic. Se [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

## Olika typer av erbjudandeuppsättningar {#types-of-offer-sets}

Skapa en erbjudandeuppsättning av följande typer av erbjudandeuppsättningar:

* **Bilder**: Du kan sätta ihop bilder för en erbjudandeuppsättning. Varje bild har ett eget erbjudande.

* **Bildmall**: Du kan parametrisera bildmallar i Adobe Dynamic Media Classic med **[!UICONTROL Build]** > Mallgrunder. Med hjälp av parametrar kan mallkomponenter, text i textramar och olika bilder bytas ut och anpassas. För en erbjudandeuppsättning kan du till exempel använda mallparametrar för att skapa variationer på samma bild i din erbjudandeuppsättning. Mer information om hur du skapar och parametriserar bildmallar finns i [Skapa mallparametrar](creating-template-parameters.md#creating_template_parameters).

Se även [Grundläggande om mallar](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) utbildningsvideo.

* **Video**: Du kan sammanställa video för en erbjudandeuppsättning. Varje video är ett separat erbjudande i uppsättningen.

## Skapa en erbjudandeuppsättning med en parametriserad mall {#creating-an-offer-set-with-a-parameterized-template}

När du skapar en erbjudandeuppsättning **[!UICONTROL Publish after a save]** påverkar uppsättningen och medlemmarna i uppsättningen på följande sätt:

| **[!UICONTROL Publish after a save]** markerat alternativ innan du sparar? | Tillstånd för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
| --- | --- | --- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ställda medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här skapar du en erbjudandeuppsättning med en parametriserad mall:**

1. Välj mall eller banderoll.
1. Gå till **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**.

   På sidan Test&amp;Target Offer Set visas erbjudanden i erbjudandeuppsättningen. Det första objektet i listan är objektet.

1. Markera objektet och markera **[!UICONTROL Add & Preview]**.

   På vänster sida av sidan visas parametrarna i mallen och deras värden.

1. Ändra parametervärden för att skapa erbjudandet. Du kan till exempel ange en annan text i ett textfält, ändra storlek på ett lager, byta ut en bild mot en annan eller välja en annan visningsförinställning.
1. Välj **[!UICONTROL Save]** eller **[!UICONTROL Save As**]** för att spara erbjudandet som en del av erbjudandeuppsättningen.

   På sidan Test&amp;Target Offer Set (Ange erbjudanden) visas de erbjudanden du har skapat.

1. Upprepa steg 3 till 5 för att skapa fler erbjudanden för uppsättningen.
1. När du är klar, nära det nedre högra hörnet på sidan, ser du till att **[!UICONTROL Publish after a save*]** är markerat (standard).
1. Välj **[!UICONTROL Close]**, ange ett namn för erbjudandeuppsättningen och välj **[!UICONTROL Save]**.

Innan du stänger sidan Test&amp;Target Offer Set (Erbjudandeuppsättning) ska du trycka på Adobe Target Standard/Premium. Se [Push Offer Sets to Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Skapa en erbjudandeuppsättning med bilder eller videor {#creating-an-offer-set-with-images-or-videos}

När du skapar en erbjudandeuppsättning **[!UICONTROL Publish after a save]** påverkar uppsättningen och medlemmarna i uppsättningen på följande sätt:

| **[!UICONTROL Publish after a save]** markerat alternativ innan du sparar? | Tillstånd för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
| --- | --- | --- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ställda medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här skapar du en erbjudandeuppsättning med bilder eller videoklipp:**

1. Sammanställ bilder eller videor till erbjudandeuppsättningen. Starta i fönstret Test&amp;Target Offer Set eller i Stödrastervisning eller listvy och använd någon av följande metoder:

   * **Test&amp;Target Offer Set screen**: Gå till **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**. Dra bilder eller videoklipp till skärmen. Om du vill skapa olika storlekar för videoklipp eller bilder drar du i flera kopior av bilden eller videon och anger varje storlek för sig.

   * **Stödrastervisning eller listvy**: Välj bilder eller videoklipp och gå sedan till **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**.

1. Du kan också markera en bild eller video och välja **[!UICONTROL Preview]**. På sidan Förhandsvisningserbjudanden kan du ändra storlek och utseende för den bild eller video som du har valt. Du kan också ändra alla bilder eller videor i erbjudandeuppsättningen.

   * Välj en förinställning om du vill ändra utseendet och storleken på bilden eller videon.
   * Om du vill använda den förinställning du valde på alla erbjudanden i erbjudandeuppsättningen väljer du **[!UICONTROL Select Presets to All]** kryssruta.

   Välj **[!UICONTROL Save]** för att spara ändringar i bild- eller videopresentationen. Välj sedan **[!UICONTROL Close]** för att återgå till sidan Test&amp;Target Offer Set.

1. När du har skapat erbjudanden för erbjudandeuppsättningen och valt Bildförinställningar för olika bilder kontrollerar du att **[!UICONTROL Publish after a save]** är markerat (standard).
1. Välj **[!UICONTROL Save]** och ange ett namn för erbjudandeuppsättningen och markera **[!UICONTROL Save]**.

Innan du stänger sidan Test&amp;Target Offer Set (Erbjudandeuppsättning) ska du trycka på Adobe Target Standard/Premium. Se [Push Offer Sets to Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Redigera en erbjudandeuppsättning {#editing-an-offer-set}

Oavsett om du redigerar en publicerad uppsättning eller en opublicerad uppsättning kan du **[!UICONTROL Publish after a save]** påverkar uppsättningen och medlemmarna i uppsättningen på följande sätt:

| Har du redan publicerat? | **[!UICONTROL Publish after a save]** är du markerad innan du sparar redigeringen? | Tillstånd för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
| --- | --- | --- | --- |
| Ja | Ja | Publicerad | Publicerad |
| Ja | Nej | Publicerad | Befintliga uppsättningsmedlemmar behåller sin publicerade status. Alla nya uppsättningsmedlemmar som du lägger till under redigeringen behåller sin publicerade eller opublicerade status. |
| Nej | Ja | Publicerad | Publicerad |
| Nej | Nej | Opublicerad | Befintliga uppsättningsmedlemmar och nya uppsättningsmedlemmar som du har lagt till under redigeringen behåller sina publicerade eller opublicerade tillstånd. |

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här redigerar du en erbjudandeuppsättning:**

1. Om du vill redigera en erbjudandeuppsättning visar du den i Stödrastervisning eller listvy och markerar sedan den **[!UICONTROL Edit]** överrullningsknapp.
1. Gör något av följande på sidan Test&amp;Target Offer Set:

   * **Ta bort ett erbjudande**: Välj erbjudandet och välj sedan **[!UICONTROL Delete]** för att ta bort ett erbjudande från uppsättningen.
   * **Lägga till ett erbjudande**: Hur du lägger till ett erbjudande beror på vilken typ av erbjudandeuppsättning du arbetar med:
      * **Mallar**: Välj **[!UICONTROL Add & Preview]** och på sidan Lägg till och förhandsgranska erbjudanden skapar du ett annat erbjudande.
      * **Bilder och videor**: Dra en bild eller video till sidan Test&amp;Target Offer Set.

   >[!NOTE]
   >
   >Du kan inte ta bort en erbjudandeuppsättning som är associerad med en kampanj. Om du vill ta bort en erbjudandeuppsättning som är associerad med en kampanj loggar du in på Adobe Target Standard/Premium och tar bort kampanjassociationerna först. Även om du avassocierar från en kampanj kan resursen bara tas bort från Adobe Dynamic Media Classic, vilket kräver en inloggning till Adobe Target Standard/Premium, och inte från Adobe Target Standard/Premium.

1. När du är klar med redigeringen, nära det nedre högra hörnet på sidan, ser du till att **[!UICONTROL Publish after a save]** är markerat (standard).
1. Välj **[!UICONTROL Save]**, väljer en lagringsmapp, anger ett namn för uppsättningen och väljer sedan **[!UICONTROL Save]**.

## Ta bort en erbjudandeuppsättning {#delet-an-offer-set}

När du tar bort en erbjudandeuppsättning flyttas själva uppsättningen till papperskorgen. Medlemmarna (eller&quot;underordnade&quot;) i uppsättningen påverkas dock inte. De behåller i stället sitt befintliga publicerade eller opublicerade läge.

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här tar du bort en erbjudandeuppsättning:**

1. I Stödrastervisning, listvy eller detaljvy väljer du en eller flera erbjudanden.
1. På det globala navigeringsfältet går du till **[!UICONTROL File]** > **[!UICONTROL Delete]** > **Ta bort**.

>[!MORELIKETHIS]
>
>* [Skapa mallparametrar](creating-template-parameters.md#creating_template_parameters)
