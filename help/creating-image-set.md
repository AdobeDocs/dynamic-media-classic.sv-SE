---
title: Skapa en bilduppsättning
description: Lär dig hur du skapar en bilduppsättning i Adobe Dynamic Media Classic.
uuid: 689fdc14-4f51-4c94-8515-cd8551e101d8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 3f356410-b30e-4870-ad95-6e5a9dc126c8
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: c18bb98c-b087-45d0-a4c9-44f58a3b514f
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 0%

---

# Skapa en bilduppsättning{#creating-an-image-set}

Om du vill skapa en bilduppsättning med flera vyer behöver du bilder som visar ett objekt från olika vypunkter eller visar olika aspekter av samma objekt. Målet är att ge tittarna bilder av ett objekt så att de får en bra uppfattning om hur ett objekt ser ut eller gör.

## Skapa en bilduppsättning {#create}

När du skapar en uppsättning påverkar **[!UICONTROL Publish after save]**-alternativet mängdmedlemmarna på följande sätt:

| **[!UICONTROL Publish after save]** markerat alternativ innan du sparar? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
| --- | --- | --- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ange medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

**Så här skapar du en bilduppsättning:**

1. Gör något av följande:

   * **Markera bilderna först**  - I panelen Bläddra väljer du de bilder du vill använda i bilduppsättningen, går till  **[!UICONTROL Build]** >  **[!UICONTROL Image Sets]**.

   * **Starta från skärmen**  Bilduppsättning - Gå till  **[!UICONTROL Build]** >  **[!UICONTROL Image Sets]**. Skärmen Bilduppsättning öppnas. Markera en mapp i resursbiblioteket och dra bilderna som du vill använda i bilduppsättningen till skärmen Bilduppsättning.

1. Om du vill ändra bildordningen drar du bilderna till nya platser.
1. Kontrollera att **[!UICONTROL Publish after save]** är markerat (standard) nära sidans nedre högra hörn.
1. Välj **[!UICONTROL Save]**, välj en mapp där du vill lagra din bilduppsättning, ange ett namn för uppsättningen och välj sedan **[!UICONTROL Save]**.
1. Om du vill visa din bilduppsättning i bilduppsättningsvisningsprogrammet väljer du **[!UICONTROL Preview]** på skärmen Bilduppsättning. Du kan välja miniatyrbilder för färgrutor i bilduppsättningsvisningsprogrammet för att se hur de fungerar.

## Redigera en bilduppsättning {#editing-an-image-set}

Oavsett om du redigerar en publicerad eller opublicerad uppsättning påverkar alternativet **[!UICONTROL Publish after save]** uppsättningen och anger medlemmar på följande sätt:

| Har du redan publicerat? | **[!UICONTROL Publish after save]** är du markerad innan du sparar redigeringen? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
| --- | --- | --- | --- |
| Ja | Ja | Publicerad | Publicerad |
| Ja | Nej | Publicerad | Befintliga uppsättningsmedlemmar behåller sin publicerade status. Alla nya uppsättningsmedlemmar som du lägger till under redigeringen behåller sin publicerade eller opublicerade status. |
| Nej | Ja | Publicerad | Publicerad |
| Nej | Nej | Opublicerad | Befintliga uppsättningsmedlemmar och nya uppsättningsmedlemmar som du har lagt till under redigeringen behåller sina publicerade eller opublicerade tillstånd. |

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

**Så här redigerar du en bilduppsättning:**

1. I stödrastervyn bläddrar du till en ImageSet och väljer **[!UICONTROL Edit]** nedanför bilden.
1. Gör något av följande:

   * Om du vill lägga till en bild (publicerad eller opublicerad) drar du den från en mapp i Lägg till resurser till **[!UICONTROL Views]**-sidan för bilduppsättningen.
   * Om du vill ta bort en bild markerar du den och väljer **[!UICONTROL Delete]** i verktygsfältet.
   * Om du vill ändra ordning på bilderna drar du en bild till en ny plats.

1. När du är klar med redigeringen av uppsättningen, nära sidans nedre högra hörn, kontrollerar du att **[!UICONTROL Publish after save]** är markerat (standard).
1. Välj **[!UICONTROL Save]**, markera en lagringsmapp för uppsättningen, ange ett namn för uppsättningen och välj sedan **[!UICONTROL Save]**.

## Ta bort en bilduppsättning {#deleting-an-image-set}

När du tar bort en uppsättning flyttas själva uppsättningen till papperskorgen. Medlemmarna (eller &quot;barn&quot;) i uppsättningen påverkas dock inte. i stället behåller de sitt befintliga publicerade eller opublicerade läge.

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

**Så här tar du bort en bilduppsättning:**

1. I Stödrastervisning, listvy eller detaljvy väljer du en eller flera bilduppsättningar.
1. I det globala navigeringsfältet går du till **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.
