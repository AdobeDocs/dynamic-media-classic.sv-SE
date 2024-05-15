---
title: Skapa en bilduppsättning
description: Lär dig hur du skapar en bilduppsättning i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets,Spin Sets
role: User
exl-id: c18bb98c-b087-45d0-a4c9-44f58a3b514f
topic: Content Management
level: Intermediate
source-git-commit: edd893482cbafd9674a44cf9878b8ee3079d98f7
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# Skapa en bilduppsättning{#creating-an-image-set}

Om du vill skapa en bilduppsättning med flera vyer behöver du bilder som visar ett objekt från olika vypunkter eller visar olika aspekter av samma objekt. Målet är att ge tittarna bilder av ett objekt så att de får en bra uppfattning om hur ett objekt ser ut eller gör.

## Skapa en bilduppsättning {#create}

När du skapar en uppsättning **[!UICONTROL Publish after save]** påverkar uppsättningen och medlemmarna i uppsättningen på följande sätt:

| **[!UICONTROL `Publish after save`]** markerat alternativ innan du sparar? | Tillstånd för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
| --- | --- | --- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ställda medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

När du skapar en bilduppsättning rekommenderar Adobe följande metodtips och tillämpar följande begränsningar:

| Begränsningstyp | Bästa praxis | Begränsning har införts |
| --- | --- | --- |
| Antal dubblettresurser per uppsättning | Inga dubbletter | 20‡ |
| Maximalt antal bilder per uppsättning | 5-10 bilder per uppsättning | 1000 |

‡ Bästa praxis är att inte ha duplicerade resurser i en uppsättning. Gränsen är 20 kopior för en enskild resurs. Om du i uppsättningen lägger till en annan dubblett för den resursen returnerar begäran ett fel eller ignorerar dubbletten.

Se även [Dynamic Media begränsningar](/help/using/limitations.md).

**Så här skapar du en bilduppsättning:**

1. Gör något av följande:

   * **Markera bilderna först** - På panelen Bläddra väljer du de bilder du vill använda i din bilduppsättning, går till **[!UICONTROL Build]** > **[!UICONTROL Image Sets]**.

   * **Starta från skärmen Bilduppsättning** - Gå till **[!UICONTROL Build]** > **[!UICONTROL Image Sets]**. Skärmen Bilduppsättning öppnas. Markera en mapp i resursbiblioteket och dra bilderna som du vill använda i bilduppsättningen till skärmen Bilduppsättning.

1. Om du vill ändra bildordningen drar du bilderna till nya platser.
1. I närheten av sidans nedre högra hörn ser du till att **[!UICONTROL Publish after save]** är markerat (standard).
1. Välj **[!UICONTROL Save]**, välj en mapp där bilduppsättningen ska lagras, ange ett namn för uppsättningen och markera sedan **[!UICONTROL Save]**.
1. Om du vill visa din bilduppsättning i bilduppsättningsvisningsprogrammet väljer du **[!UICONTROL Preview]** på skärmen Bilduppsättning. Du kan välja miniatyrbilder för färgrutor i bilduppsättningsvisningsprogrammet för att se hur de fungerar.

## Redigera en bilduppsättning {#editing-an-image-set}

Oavsett om du redigerar en publicerad eller opublicerad uppsättning kan du **[!UICONTROL Publish after save]** påverkar uppsättningen och medlemmarna i uppsättningen på följande sätt:

| Har du redan publicerat? | **[!UICONTROL `Publish after save`]** är du markerad innan du sparar redigeringen? | Tillstånd för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
| --- | --- | --- | --- |
| Ja | Ja | Publicerad | Publicerad |
| Ja | Nej | Publicerad | Befintliga uppsättningsmedlemmar behåller sin publicerade status. Alla nya uppsättningsmedlemmar som du lägger till under redigeringen behåller sin publicerade eller opublicerade status. |
| Nej | Ja | Publicerad | Publicerad |
| Nej | Nej | Opublicerad | Befintliga uppsättningsmedlemmar och nya uppsättningsmedlemmar som du har lagt till under redigeringen behåller sina publicerade eller opublicerade tillstånd. |

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här redigerar du en bilduppsättning:**

1. I stödrastervyn bläddrar du till en ImageSet och väljer sedan under bilden **[!UICONTROL Edit]**.
1. Gör något av följande:

   * Om du vill lägga till en bild (publicerad eller opublicerad) drar du den från en mapp i Lägg till resurser till bilduppsättningens **[!UICONTROL Views]** sida.
   * Om du vill ta bort en bild markerar du den och väljer **[!UICONTROL Delete]** i verktygsfältet.
   * Om du vill ändra ordning på bilderna drar du en bild till en ny plats.

1. När du är klar med redigeringen av uppsättningen, nära sidans nedre högra hörn, ser du till att **[!UICONTROL Publish after save]** är markerat (standard).
1. Välj **[!UICONTROL Save]**, väljer en lagringsmapp för uppsättningen, anger ett namn för uppsättningen och väljer **[!UICONTROL Save]**.

## Ta bort en bilduppsättning

När du tar bort en uppsättning flyttas själva uppsättningen till papperskorgen. Medlemmarna (eller&quot;underordnade&quot;) i uppsättningen påverkas dock inte. De behåller i stället sitt befintliga publicerade eller opublicerade läge.

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här tar du bort en bilduppsättning:**

1. I Stödrastervisning, listvy eller detaljvy väljer du en eller flera bilduppsättningar.
1. På det globala navigeringsfältet går du till **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.
