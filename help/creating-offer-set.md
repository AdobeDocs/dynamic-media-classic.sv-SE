---
title: Skapa en erbjudandeuppsättning
seo-title: Skapa en erbjudandeuppsättning
description: 'null'
seo-description: Lär dig hur du skapar en uppsättning erbjudanden.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '1210'
ht-degree: 0%

---


# Skapa en erbjudandeuppsättning{#creating-an-offer-set}

Du kan skapa följande typer av erbjudandeuppsättningar:

* Video
* Parametriserad mall
* Bild

För mallar klickar du på **Lägg till och förhandsgranska** och anger sedan de parametrar du vill använda. De andra typerna av erbjudandeuppsättningar innehåller inga parametrar, men du kan fortfarande anpassa dem genom att klicka på **Förhandsgranska** och ändra de tillgängliga förinställningarna.

I Dynamic Media Classic finns verktyg för redigering och för att skapa erbjudanden.

>[!NOTE]
>
>Innan du skapar en erbjudandeuppsättning måste du publicera alla resurser som du vill använda för uppsättningen till Dynamic Media Classic. Se [Publicera resurser](publishing-files.md#manually_publishing_assets) manuellt och [Avpublicera resurser](publishing-files.md#manually_unpublishing_assets)manuellt.

## Olika typer av uppsättningar erbjudanden {#types-of-offer-sets}

Skapa en erbjudandeuppsättning av följande typer av erbjudanden:

* **Bilder** Du kan sätta ihop bilder för en uppsättning erbjudanden. Varje bild har ett eget erbjudande.

* **Bildmall** Du kan parametrisera bildmallar i Dynamic Media Classic med kommandot Skapa > Mallgrunder. Med hjälp av parametrar kan mallkomponenter - texten i textramar och de olika bilderna - bytas ut och anpassas. För en erbjudandeuppsättning kan du till exempel använda mallparametrar för att skapa varianter på samma bild i din erbjudandeuppsättning. Mer information om hur du skapar och parametriserar bildmallar finns i Skapa mallparametrar.

* **Video** Du kan sätta ihop video för en uppsättning erbjudanden. Varje video är ett separat erbjudande i uppsättningen.

## Skapa en erbjudandeuppsättning med en parametriserad mall {#creating-an-offer-set-with-a-parameterized-template}

När du skapar en erbjudandeuppsättning påverkar alternativet **Publicera efter spara** medlemmarna i uppsättningen och uppsättningen på följande sätt:

| Alternativet Publicera efter spara är markerat innan du sparar? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
|--- |--- |--- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ange medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) manuellt och [Avpublicera resurser](publishing-files.md#manually_unpublishing_assets)manuellt.

**Skapa en erbjudandeuppsättning med en parametriserad mall**

1. Välj mall eller banderoll.
1. Klicka på **Skapa** > **Test&amp;Target Erbjudandeuppsättning**.

   På sidan Test&amp;Target Offer Set listas erbjudanden. Det första objektet i listan är objektet.

1. Markera objektet och klicka på **Lägg till och förhandsgranska**.

   På vänster sida av sidan visas parametrarna i mallen och deras värden.

1. Ändra parametervärden för att skapa erbjudandet. Du kan till exempel ange en annan text i ett textfält, ändra storlek på ett lager, byta ut en bild mot en annan eller välja en annan visningsförinställning.
1. Klicka på **Spara** eller **Spara som** för att spara erbjudandet som en del av erbjudandet.

   På sidan Test&amp;Target Offer Set visas de erbjudanden du har skapat.

1. Upprepa steg 3 till 5 för att skapa fler erbjudanden för uppsättningen.
1. När du är klar ser du till att **Publicera efter spara** är markerat (standard) nära sidans nedre högra hörn.
1. Klicka på **Stäng**, ange ett namn för erbjudandeuppsättningen och klicka sedan på **Spara**.

Innan du stänger sidan Test&amp;Target Offer Set (konfigurera erbjudandet till Target Standard/Premium). Se [Paketera erbjudanden för Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Skapa en erbjudandeuppsättning med bilder eller videor {#creating-an-offer-set-with-images-or-videos}

När du skapar en erbjudandeuppsättning påverkar alternativet **Publicera efter spara** medlemmarna i uppsättningen och uppsättningen på följande sätt:

| Alternativet Publicera efter spara är markerat innan du sparar? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
|--- |--- |--- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ange medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) manuellt och [Avpublicera resurser](publishing-files.md#manually_unpublishing_assets)manuellt.

**Skapa en erbjudandeuppsättning med bilder eller videor**

1. Sammanställ bilder eller videor för uppsättningen. Börja i fönstret Test&amp;Target Offer Set eller i Stödrastervisning eller listvy och använd någon av följande metoder:

   * **Test&amp;Target Offer Set screen** Click **[!UICONTROL Build > Test&Target Offer Set]**. Dra bilder eller videoklipp till skärmen. Om du vill skapa olika storlekar för videoklipp eller bilder drar du i flera kopior av bilden eller videon och anger varje storlek för sig.

   * **Stödraster- eller listvy** Markera bilderna eller videoklippen och klicka sedan på **[!UICONTROL Build > Test&Target Offer Set]**.

1. Du kan också markera en bild eller video och klicka på **Förhandsvisa**. På sidan Förhandsvisningserbjudanden kan du ändra storlek och utseende för den bild eller video som du har valt. Eller så kan du ändra alla bilder eller videor i erbjudandeuppsättningen.

   * Välj en förinställning om du vill ändra utseendet och storleken på bilden eller videon.
   * Klicka på kryssrutan Välj förinställningar för alla för att använda den förinställning du valde på alla erbjudanden i erbjudandeuppsättningen.

   Klicka på **Spara** om du vill spara ändringarna i bild- eller videolösningen. Klicka sedan på **Stäng** för att återgå till sidan Test&amp;Target Offer Set.

1. När du har skapat erbjudanden för erbjudandeuppsättningen och valt Bildförinställningar för olika bilder kontrollerar du att **Publicera efter spara** är markerat (standard).
1. Klicka på **Spara** , ange ett namn för erbjudandeuppsättningen och klicka på **Spara**.

Innan du stänger sidan Test&amp;Target Offer Set (Visa erbjudandet) ska du överföra erbjudandet till Target Standard/Premium. Se [Paketera erbjudanden för Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Redigera en erbjudandeuppsättning {#editing-an-offer-set}

Beroende på om du redigerar en publicerad uppsättning eller en opublicerad uppsättning påverkar alternativet **Publicera efter spara** uppsättningen och ange medlemmar på följande sätt:

| Har du redan publicerat? | Alternativet Publicera efter spara är markerat innan du sparar redigeringen? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
|--- |--- |--- |--- |
| Ja | Ja | Publicerad | Publicerad |
| Ja | Nej | Publicerad | Befintliga uppsättningsmedlemmar behåller sin publicerade status.Alla nya uppsättningsmedlemmar som du lägger till under redigeringen behåller sin publicerade eller opublicerade status. |
| Nej | Ja | Publicerad | Publicerad |
| Nej | Nej | Opublicerad | Befintliga uppsättningsmedlemmar och nya uppsättningsmedlemmar som du har lagt till under redigeringen behåller sina publicerade eller opublicerade tillstånd. |

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) manuellt och [Avpublicera resurser](publishing-files.md#manually_unpublishing_assets)manuellt.

**Redigera en erbjudandeuppsättning**

1. Om du vill redigera en erbjudandeuppsättning visar du erbjudandeuppsättningen i stödrastervyn eller listvyn och klickar sedan på knappen **Redigera** överrullning.
1. Gör något av följande på sidan Test&amp;Target Offer Set:

   * **Ta bort ett erbjudande** Välj erbjudandet och klicka sedan på 
**Ta bort** om du vill ta bort ett erbjudande från uppsättningen.
   * **Lägga till ett erbjudande** Hur du lägger till ett erbjudande beror på vilken typ av erbjudande du arbetar med:
   * **Mallar** Klicka 
**Lägg till och förhandsgranska**, och skapa ett annat erbjudande på sidan Lägg till och förhandsgranska erbjudanden.
   * **Bilder och videor** Dra en bild eller video till sidan Test&amp;Target Offer Set.
   >[!NOTE]
   >
   >Du kan inte ta bort en erbjudandeuppsättning som är associerad med en kampanj. Om du vill ta bort en erbjudandeuppsättning som är associerad med en kampanj loggar du in på Target Standard/Premium och tar bort kampanjassociationerna först. Även efter att en kampanj inte har associerats kan resursen bara tas bort från Dyanmic Media Classic, vilket kräver en inloggning på Target Standard/Premium, och inte från Target Standard/Premium.

1. När du är klar med redigeringen, nära det nedre högra hörnet på sidan, kontrollerar du att **Publicera efter spara** är markerat (standard).
1. Klicka på **Spara**, markera en lagringsmapp, ange ett namn för uppsättningen och klicka sedan på **Spara**.

## Ta bort en erbjudandeuppsättning {#deleting-an-offer-set}

När du tar bort en erbjudandeuppsättning flyttas själva uppsättningen till papperskorgen. Medlemmarna (eller &quot;barn&quot;) i uppsättningen påverkas dock inte. i stället behåller de sitt befintliga publicerade eller opublicerade läge.

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) manuellt och [Avpublicera resurser](publishing-files.md#manually_unpublishing_assets)manuellt.

**Ta bort en erbjudandeuppsättning**

1. Markera en eller flera erbjudandeuppsättningar i Stödrastervisning, listvy eller detaljvy.
1. Klicka på **Arkiv** > **Ta bort** > **Ta bort** i det globala navigeringsfältet.

>[!MORELIKETHIS]
>
>* [Skapa mallparametrar](creating-template-parameters.md#creating_template_parameters)

