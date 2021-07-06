---
title: Skapa en erbjudandeuppsättning
description: Lär dig hur du skapar en uppsättning erbjudanden.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '1156'
ht-degree: 0%

---

# Skapa en erbjudandeuppsättning{#creating-an-offer-set}

Du kan skapa följande typer av erbjudandeuppsättningar:

* Video
* Parametriserad mall
* Bild

För mallar klickar du på **[!UICONTROL Add and Preview]** och anger sedan de parametrar du väljer. De andra erbjudandetyperna innehåller inga parametrar, men du kan fortfarande anpassa dem genom att klicka på **[!UICONTROL Preview]** och ändra de tillgängliga förinställningarna.

I Dynamic Media Classic finns verktyg för redigering och för att skapa erbjudanden.

>[!NOTE]
>
>Innan du skapar en erbjudandeuppsättning måste du publicera alla resurser som du vill använda för uppsättningen till Dynamic Media Classic. Se [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

## Olika typer av uppsättningar erbjudanden {#types-of-offer-sets}

Skapa en erbjudandeuppsättning av följande typer av erbjudanden:

* **Bilder**  - Du kan sätta ihop bilder för en uppsättning erbjudanden. Varje bild har ett eget erbjudande.

* **Bildmall**  - Du kan parametrisera bildmallar i Dynamic Media Classic med kommandot Skapa > Mallgrunder. Med hjälp av parametrar kan mallkomponenter - texten i textramar och de olika bilderna - bytas ut och anpassas. För en erbjudandeuppsättning kan du till exempel använda mallparametrar för att skapa varianter på samma bild i din erbjudandeuppsättning. Mer information om hur du skapar och parametriserar bildmallar finns i Skapa mallparametrar.

* **Video**  - Du kan sammanställa video för en uppsättning erbjudanden. Varje video är ett separat erbjudande i uppsättningen.

## Skapa en erbjudandeuppsättning med en parametriserad mall {#creating-an-offer-set-with-a-parameterized-template}

När du skapar en erbjudandeuppsättning påverkar **[!UICONTROL Publish after save]**-alternativet uppsättningen och anger medlemmar på följande sätt:

| Alternativet Publicera efter spara är markerat innan du sparar? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
|--- |--- |--- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ange medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

**Så här skapar du en erbjudandeuppsättning med en parametriserad mall:**

1. Välj mall eller banderoll.
1. Klicka på **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**.

   På sidan Test&amp;Target Offer Set listas erbjudanden i uppsättningen. Det första objektet i listan är objektet.

1. Markera objektet och klicka på **[!UICONTROL Add & Preview]**.

   På vänster sida av sidan visas parametrarna i mallen och deras värden.

1. Ändra parametervärden för att skapa erbjudandet. Du kan till exempel ange en annan text i ett textfält, ändra storlek på ett lager, byta ut en bild mot en annan eller välja en annan visningsförinställning.
1. Klicka på **[!UICONTROL **Save]** eller **[!UICONTROL Save As**]** för att spara erbjudandet som en del av erbjudandeuppsättningen.

   På sidan Test&amp;Target Offer Set (Ange erbjudanden) visas de erbjudanden du har skapat.

1. Upprepa steg 3 till 5 för att skapa fler erbjudanden för uppsättningen.
1. När du är klar ser du till att **[!UICONTROL Publish after save*]** är markerat (standard) nära sidans nedre högra hörn.
1. Klicka på **[!UICONTROL Close]**, ange ett namn för erbjudandeuppsättningen och klicka sedan på **[!UICONTROL Save]**.

Innan du stänger sidan Test&amp;Target Offer Set (Ange erbjudanden) ska du överföra erbjudandet till Adobe Target Standard/Premium. Se [Paketera erbjudanden till Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Skapa en erbjudandeuppsättning med bilder eller videor {#creating-an-offer-set-with-images-or-videos}

När du skapar en erbjudandeuppsättning påverkar **[!UICONTROL Publish after save]**-alternativet uppsättningen och anger medlemmar på följande sätt:

| **[!UICONTROL Publish after save]** markerat alternativ innan du sparar? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
|--- |--- |--- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ange medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

**Så här skapar du en erbjudandeuppsättning med bilder eller videor:**

1. Sammanställ bilder eller videor för uppsättningen. Starta i fönstret Test&amp;Target Offer Set eller i Stödrastervisning eller listvy och använd någon av följande metoder:

   * **Test&amp;Target Offer Set screen**  - Click  **[!UICONTROL Build]** >  **[!UICONTROL Test&Target Offer Set]**. Dra bilder eller videoklipp till skärmen. Om du vill skapa olika storlekar för videoklipp eller bilder drar du i flera kopior av bilden eller videon och anger varje storlek för sig.

   * **Stödrastervisning eller listvy** - Markera bilderna eller videoklippen och klicka sedan på  **[!UICONTROL Build]** >  **[!UICONTROL Test&Target Offer Set]**.

1. Du kan också markera en bild eller video och klicka på **[!UICONTROL Preview]**. På sidan Förhandsvisningserbjudanden kan du ändra storlek och utseende för den bild eller video som du har valt. Eller så kan du ändra alla bilder eller videor i erbjudandeuppsättningen.

   * Välj en förinställning om du vill ändra utseendet och storleken på bilden eller videon.
   * Klicka i kryssrutan **[!UICONTROL Select Presets to All]** för att använda den förinställning du valt på alla erbjudanden i erbjudandeuppsättningen.

   Klicka på **[!UICONTROL Save]** om du vill spara ändringarna i bild- eller videorbjudandet. Klicka sedan på **[!UICONTROL Close]** för att återgå till sidan Test&amp;Target Offer Set.

1. När du har skapat erbjudanden för erbjudandeuppsättningen och valt Bildförinställningar för olika bilder kontrollerar du att **[!UICONTROL Publish after save]** är valt (standard).
1. Klicka på **[!UICONTROL Save]** och ange ett namn för erbjudandeuppsättningen och klicka på **[!UICONTROL Save]**.

Innan du stänger sidan Test&amp;Target Offer Set (Ange erbjudandet) ska du överföra erbjudandet till Adobe Target Standard/Premium. Se [Paketera erbjudanden till Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Redigera en erbjudandeuppsättning {#editing-an-offer-set}

Oavsett om du redigerar en publicerad eller opublicerad uppsättning påverkar **[!UICONTROL Publish after save]**-alternativet uppsättningen och anger medlemmar på följande sätt:

| Har du redan publicerat? | **[!UICONTROL Publish after save]** är du markerad innan du sparar redigeringen? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
|--- |--- |--- |--- |
| Ja | Ja | Publicerad | Publicerad |
| Ja | Nej | Publicerad | Befintliga uppsättningsmedlemmar behåller sin publicerade status. Alla nya uppsättningsmedlemmar som du lägger till under redigeringen behåller sin publicerade eller opublicerade status. |
| Nej | Ja | Publicerad | Publicerad |
| Nej | Nej | Opublicerad | Befintliga uppsättningsmedlemmar och nya uppsättningsmedlemmar som du har lagt till under redigeringen behåller sina publicerade eller opublicerade tillstånd. |

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

**Så här redigerar du en erbjudandeuppsättning:**

1. Om du vill redigera en erbjudandeuppsättning visar du erbjudandeuppsättningen i stödrastervyn eller listvyn och klickar sedan på överrullningsknappen **[!UICONTROL Edit]**.
1. Gör något av följande på sidan Test&amp;Target Offer Set:

   * **Ta bort ett erbjudande** - Välj erbjudandet och klicka sedan på  **[!UICONTROL Delete]** för att ta bort ett erbjudande från uppsättningen.
   * **Lägg till ett erbjudande** - Hur du lägger till ett erbjudande beror på vilken typ av erbjudande du arbetar med:
      * **Mallar**  - Klicka  **[!UICONTROL Add & Preview]** och skapa ett annat erbjudande på sidan Lägg till och förhandsgranska erbjudanden.
      * **Bilder och videor**  - Dra en bild eller video till sidan Test&amp;Target Offer Set.

   >[!NOTE]
   >
   >Du kan inte ta bort en erbjudandeuppsättning som är associerad med en kampanj. Om du vill ta bort en erbjudandeuppsättning som är associerad med en kampanj loggar du in på Adobe Target Standard/Premium och tar bort kampanjassociationerna först. Även om du avassocierar från en kampanj kan resursen bara tas bort från Dynamic Media Classic, vilket kräver att du loggar in på Adobe Target Standard/Premium och inte från Adobe Target Standard/Premium.

1. När du är klar med redigeringen, nära det nedre högra hörnet på sidan, kontrollerar du att **[!UICONTROL Publish after save]** är markerat (standard).
1. Klicka på **[!UICONTROL Save]**, markera en lagringsmapp, ange ett namn för uppsättningen och klicka sedan på **[!UICONTROL Save]**.

## Ta bort en erbjudandeuppsättning {#deleting-an-offer-set}

När du tar bort en erbjudandeuppsättning flyttas själva uppsättningen till papperskorgen. Medlemmarna (eller &quot;barn&quot;) i uppsättningen påverkas dock inte. i stället behåller de sitt befintliga publicerade eller opublicerade läge.

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

**Så här tar du bort en erbjudandeuppsättning:**

1. Markera en eller flera erbjudandeuppsättningar i Stödrastervisning, listvy eller detaljvy.
1. Klicka på **[!UICONTROL File]** > **[!UICONTROL Delete]** > **Ta bort** i det globala navigeringsfältet.

>[!MORELIKETHIS]
>
>* [Skapa mallparametrar](creating-template-parameters.md#creating_template_parameters)

