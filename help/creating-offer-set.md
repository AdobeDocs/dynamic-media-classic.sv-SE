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
source-git-commit: 4819803428adee539e46498c73e5f2ba6a952693
workflow-type: tm+mt
source-wordcount: '1210'
ht-degree: 0%

---


# Skapa en erbjudandeuppsättning{#creating-an-offer-set}

Du kan skapa följande typer av erbjudandeuppsättningar:

* Video
* Parametriserad mall
* Bild

För mallar klickar du på **Lägg till och förhandsgranska** och anger sedan de parametrar du vill använda. De andra erbjudandetyperna innehåller inga parametrar, men du kan fortfarande anpassa dem genom att klicka på **Förhandsgranska** och ändra de tillgängliga förinställningarna.

I Dynamic Media Classic finns verktyg för redigering och för att skapa erbjudanden.

>[!NOTE]
>
>Innan du skapar en erbjudandeuppsättning måste du publicera alla resurser som du vill använda för uppsättningen till Dynamic Media Classic. Se [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

## Olika typer av uppsättningar {#types-of-offer-sets}

Skapa en erbjudandeuppsättning av följande typer av erbjudanden:

* ****
BilderDu kan sätta ihop bilder för en uppsättning erbjudanden. Varje bild har ett eget erbjudande.

* **BildmallDu**
kan parametrisera bildmallar i Dynamic Media Classic med kommandot Skapa > Mallgrunder. Med hjälp av parametrar kan mallkomponenter - texten i textramar och de olika bilderna - bytas ut och anpassas. För en erbjudandeuppsättning kan du till exempel använda mallparametrar för att skapa varianter på samma bild i din erbjudandeuppsättning. Mer information om hur du skapar och parametriserar bildmallar finns i Skapa mallparametrar.

* ****
VideoDu kan sätta ihop video för ett erbjudande. Varje video är ett separat erbjudande i uppsättningen.

## Skapa en erbjudandeuppsättning med en parametriserad mall {#creating-an-offer-set-with-a-parameterized-template}

När du skapar en erbjudandeuppsättning påverkar alternativet **Publicera efter spara** uppsättningen och ange medlemmar på följande sätt:

| Alternativet Publicera efter spara är markerat innan du sparar? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
|--- |--- |--- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ange medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

**Skapa en erbjudandeuppsättning med en parametriserad mall**

1. Välj mall eller banderoll.
1. Klicka på **Build** > **Test&amp;Target Offer Set**.

   På sidan Test&amp;Target Offer Set listas erbjudanden i uppsättningen. Det första objektet i listan är objektet.

1. Markera objektet och klicka på **Lägg till och förhandsgranska**.

   På vänster sida av sidan visas parametrarna i mallen och deras värden.

1. Ändra parametervärden för att skapa erbjudandet. Du kan till exempel ange en annan text i ett textfält, ändra storlek på ett lager, byta ut en bild mot en annan eller välja en annan visningsförinställning.
1. Klicka på **Spara** eller **Spara som** för att spara erbjudandet som en del av erbjudandeuppsättningen.

   På sidan Test&amp;Target Offer Set (Ange erbjudanden) visas de erbjudanden du har skapat.

1. Upprepa steg 3 till 5 för att skapa fler erbjudanden för uppsättningen.
1. När du är klar ser du till att **Publicera efter spara** är markerat (standard) nära sidans nedre högra hörn.
1. Klicka på **Stäng**, ange ett namn för erbjudandeuppsättningen och klicka sedan på **Spara**.

Innan du stänger sidan Test&amp;Target Offer Set (Ange erbjudanden) ska du överföra erbjudandet till Target Standard/Premium. Se [Paketera erbjudanden till Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Skapa en erbjudandeuppsättning med bilder eller videoklipp {#creating-an-offer-set-with-images-or-videos}

När du skapar en erbjudandeuppsättning påverkar alternativet **Publicera efter spara** uppsättningen och ange medlemmar på följande sätt:

| Alternativet Publicera efter spara är markerat innan du sparar? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
|--- |--- |--- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ange medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

**Skapa en erbjudandeuppsättning med bilder eller videor**

1. Sammanställ bilder eller videor för uppsättningen. Starta i fönstret Test&amp;Target Offer Set eller i Stödrastervisning eller listvy och använd någon av följande metoder:

   * **Test&amp;Target Offer Set** screenClick  **[!UICONTROL Build > Test&Target Offer Set]**. Dra bilder eller videoklipp till skärmen. Om du vill skapa olika storlekar för videoklipp eller bilder drar du i flera kopior av bilden eller videon och anger varje storlek för sig.

   * **Stödraster- eller** listvyMarkera bilderna eller videoklippen och klicka sedan på  **[!UICONTROL Build > Test&Target Offer Set]**.

1. Du kan också markera en bild eller video och klicka på **Förhandsgranska**. På sidan Förhandsvisningserbjudanden kan du ändra storlek och utseende för den bild eller video som du har valt. Eller så kan du ändra alla bilder eller videor i erbjudandeuppsättningen.

   * Välj en förinställning om du vill ändra utseendet och storleken på bilden eller videon.
   * Klicka på kryssrutan Välj förinställningar för alla för att använda den förinställning du valde på alla erbjudanden i erbjudandeuppsättningen.

   Klicka på **Spara** om du vill spara ändringarna i bilden eller videopresentationen. Klicka sedan på **Stäng** för att återgå till sidan Test&amp;Target Offer Set.

1. När du har skapat erbjudanden för erbjudandeuppsättningen och valt Bildförinställningar för olika bilder kontrollerar du att **Publicera när du har sparat** är markerat (standard).
1. Klicka på **Spara** och ange ett namn för erbjudandeuppsättningen. Klicka sedan på **Spara**.

Innan du stänger sidan Test&amp;Target Offer Set (Ange erbjudandet) ska du överföra erbjudandet till Target Standard/Premium. Se [Paketera erbjudanden till Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Redigera en erbjudandeuppsättning {#editing-an-offer-set}

Beroende på om du redigerar en publicerad eller opublicerad uppsättning påverkar alternativet **Publicera efter spara** uppsättningen och ange medlemmar på följande sätt:

| Har du redan publicerat? | Alternativet Publicera efter spara är markerat innan du sparar redigeringen? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
|--- |--- |--- |--- |
| Ja | Ja | Publicerad | Publicerad |
| Ja | Nej | Publicerad | Befintliga uppsättningsmedlemmar behåller sin publicerade status.Alla nya uppsättningsmedlemmar som du lägger till under redigeringen behåller sin publicerade eller opublicerade status. |
| Nej | Ja | Publicerad | Publicerad |
| Nej | Nej | Opublicerad | Befintliga uppsättningsmedlemmar och nya uppsättningsmedlemmar som du har lagt till under redigeringen behåller sina publicerade eller opublicerade tillstånd. |

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

**Redigera en erbjudandeuppsättning**

1. Om du vill redigera en erbjudandeuppsättning visar du erbjudandeuppsättningen i stödrastervyn eller listvyn och klickar sedan på knappen **Redigera**.
1. Gör något av följande på sidan Test&amp;Target Offer Set:

   * **Ta bort ett**
erbjudandeVälj erbjudandet och klicka sedan på 
**Ta** bort ett erbjudande från uppsättningen.
   * **Lägg till ett**
erbjudandeHur du lägger till ett erbjudande beror på vilken typ av erbjudande du arbetar med:
   * ****
MallarKlicka 
**Lägg till och förhandsgranska**, och skapa ett annat erbjudande på sidan Lägg till och förhandsgranska erbjudanden.
   * **Bilder och**
videorDra en bild eller video till sidan Test&amp;Target Offer Set.
   >[!NOTE]
   >
   >Du kan inte ta bort en erbjudandeuppsättning som är associerad med en kampanj. Om du vill ta bort en erbjudandeuppsättning som är associerad med en kampanj loggar du in på Target Standard/Premium och tar bort kampanjassociationerna först. Även efter det att du har tagit bort kopplingen från en kampanj kan resursen bara tas bort från Dyanmic Media Classic, vilket kräver en inloggning på Target Standard/Premium, och inte från Target Standard/Premium.

1. När du är klar med redigeringen, nära det nedre högra hörnet på sidan, kontrollerar du att **Publicera efter spara** är markerat (standard).
1. Klicka på **Spara**, markera en lagringsmapp, ange ett namn för uppsättningen och klicka sedan på **Spara**.

## Ta bort en erbjudandeuppsättning {#deleting-an-offer-set}

När du tar bort en erbjudandeuppsättning flyttas själva uppsättningen till papperskorgen. Medlemmarna (eller &quot;barn&quot;) i uppsättningen påverkas dock inte. i stället behåller de sitt befintliga publicerade eller opublicerade läge.

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

**Ta bort en erbjudandeuppsättning**

1. Markera en eller flera erbjudandeuppsättningar i Stödrastervisning, listvy eller detaljvy.
1. I det globala navigeringsfältet klickar du på **Arkiv** > **Ta bort** > **Ta bort**.

>[!MORELIKETHIS]
>
>* [Skapa mallparametrar](creating-template-parameters.md#creating_template_parameters)

