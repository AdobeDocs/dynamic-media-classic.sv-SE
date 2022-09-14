---
title: Skapa en blandad medieuppsättning
description: Lär dig hur du skapar en uppsättning med blandade media i Adobe Dynamic Media Classic.
uuid: a0c6e5fa-7a85-4376-b9a3-b72ae63d3d95
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0ff9e763-897c-4ba5-b606-a95d5e45f35e
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 18669c65-a1c4-4012-8587-cd5095f4bd4e
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 0%

---

# Skapa en blandad medieuppsättning{#creating-a-mixed-media-set}

Skapa en blandad medieuppsättning när du vill kombinera flera typer av visningsprogram i en presentation. Kontrollera att dina filer, bilduppsättningar, färgruteuppsättningar och snurruppsättningar är klara att publiceras innan du lägger till dem i den blandade medieuppsättningen.

![Blandad medieuppsättning](/help/assets/mm_mixed_media_set.png)

## Skapa en blandad medieuppsättning {#create-a-mixed-media-set}

När du skapar en uppsättning **Publicera efter spara** påverkar uppsättningen och medlemmarna i uppsättningen på följande sätt:

| Alternativet Publicera efter spara är markerat innan du sparar? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
| --- | --- | --- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ange medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här skapar du en blandad medieuppsättning:**

1. Gå till **[!UICONTROL Build]** > **[!UICONTROL Mixed Media Sets]**.
1. Dra videoklipp, bilduppsättningar, snurruppsättningar och färgrutor från resursbiblioteket till skärmen med blandade medieuppsättningar.

   >[!NOTE]
   >
   >En uppsättning med blandade media stöder inte resurser med filnamn som innehåller något av följande tecken: `( ) { }`.

1. Gör något av följande:

   * Om du vill lägga till ett ljudspår drar du en ljudfil från resursbiblioteket till rutan Ljudspår. Ljudspåret spelas upp när bilder visas. Det stoppas när video spelas upp.
   * Om du vill ändra ordningen på uppsättningar drar du dem till nya platser på skärmen med blandade medieuppsättningar. Ordningen på uppsättningarna på skärmen avgör i vilken ordning användarna ser uppsättningar i visningsprogrammet för den blandade medieuppsättningen.
   * (Valfritt) Om du vill lägga till en anpassad miniatyrbild som representerar en video i visningsprogrammet drar du en bildfil från resursbiblioteket till platshållarrutan för miniatyrbilder.

1. I närheten av sidans nedre högra hörn ser du till att **[!UICONTROL Publish after save]** är markerat (standard).
1. Välj **[!UICONTROL Save]**.
1. Välj en mapp för lagring av den blandade medieuppsättningen och ange sedan ett namn för uppsättningen.
1. Välj **[!UICONTROL Save]**.

   Om du vill se hur din kombinationsbilduppsättning ser ut i ett visningsprogram väljer du **[!UICONTROL Preview]**.

## Redigera en blandad medieuppsättning {#edit-a-mixed-media-set}

Du kan redigera en uppsättning med blandade media. Om du vill redigera en uppsättning i en uppsättning med blandade media öppnar du den uppsättningen separat, redigerar den och sparar den. Redigeringarna visas i uppsättningen med blandade media.

Oavsett om du redigerar en publicerad eller opublicerad uppsättning kan du **[!UICONTROL Publish after save]** påverkar uppsättningen och medlemmarna i uppsättningen på följande sätt:

| Har du redan publicerat? | **[!UICONTROL Publish after save]** är du markerad innan du sparar redigeringen? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
| --- |--- |--- |--- |
| Ja | Ja | Publicerad | Publicerad |
| Ja | Nej | Publicerad | Befintliga uppsättningsmedlemmar behåller sin publicerade status. Alla nya uppsättningsmedlemmar som du lägger till under redigeringen behåller sin publicerade eller opublicerade status. |
| Nej | Ja | Publicerad | Publicerad |
| Nej | Nej | Opublicerad | Befintliga uppsättningsmedlemmar och nya uppsättningsmedlemmar som du har lagt till under redigeringen behåller sina publicerade eller opublicerade tillstånd. |

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här redigerar du en blandad medieuppsättning:**

1. Markera den blandade mediauppsättningens överrullning **[!UICONTROL Edit]** -knappen.
1. Gör något av följande:

   * Om du vill ta bort objekt markerar du dem och väljer **[!UICONTROL Delete]**.
   * Om du vill ordna om objekt drar du dem till nya platser.

1. När du är klar med redigeringen av uppsättningen, nära sidans nedre högra hörn, ser du till att **[!UICONTROL Publish after save]** är markerat (standard).
1. Välj **[!UICONTROL Save]** eller **[!UICONTROL Save As]**.

## Ta bort en blandad medieuppsättning {#deleting-a-mixed-media-set}

När du tar bort en uppsättning flyttas själva uppsättningen till papperskorgen. Medlemmarna (eller &quot;barn&quot;) i uppsättningen påverkas dock inte. i stället behåller de sitt befintliga publicerade eller opublicerade läge.

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här tar du bort en blandad medieuppsättning:**

1. I Stödrastervisning, listvy eller detaljvy väljer du en eller flera blandade medieuppsättningar.
1. På det globala navigeringsfältet går du till **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.
