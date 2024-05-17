---
title: Skapa en blandad medieuppsättning
description: Lär dig hur du skapar en uppsättning med blandade media i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 18669c65-a1c4-4012-8587-cd5095f4bd4e
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Skapa en blandad medieuppsättning{#creating-a-mixed-media-set}

Skapa en blandad medieuppsättning när du vill kombinera flera typer av visningsprogram i en presentation. Kontrollera att dina filer, bilduppsättningar, färgruteuppsättningar och snurruppsättningar är klara att publiceras innan du lägger till dem i den blandade medieuppsättningen.

![Blandad medieuppsättning](/help/using/assets/mm_mixed_media_set.png)

## Skapa en blandad medieuppsättning {#create-a-mixed-media-set}

När du skapar en uppsättning **Publicera efter spara** påverkar uppsättningen och medlemmarna i uppsättningen på följande sätt:

| Vill du publicera efter att ha sparat innan du sparar? | Tillstånd för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
| --- | --- | --- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ställda medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här skapar du en blandad medieuppsättning:**

1. Gå till **[!UICONTROL Build]** > **[!UICONTROL Mixed Media Sets]**.
1. Dra videoklipp, bilduppsättningar, snurruppsättningar och färgrutor från resursbiblioteket till skärmen med blandade medieuppsättningar.

   >[!NOTE]
   >
   >En uppsättning med blandade media stöder inte resurser med filnamn som innehåller något av följande tecken: `( ) { }`.

1. Gör något av följande:

   * Om du vill lägga till ett ljudspår drar du en ljudfil från resursbiblioteket till rutan Ljudspår. Ljudspåret spelas upp när bilder visas. Den stoppas när en video spelas upp.
   * Om du vill ändra ordningen på uppsättningar drar du dem till nya platser på skärmen med blandade medieuppsättningar. Ordningen på uppsättningarna på skärmen avgör i vilken ordning användarna ser uppsättningar i visningsprogrammet för den blandade medieuppsättningen.
   * (Valfritt) Om du vill lägga till en anpassad miniatyrbild som representerar en video i visningsprogrammet drar du en bildfil från resursbiblioteket till platshållarrutan för miniatyrbilder.

1. I närheten av sidans nedre högra hörn ser du till att **[!UICONTROL Publish after a save]** är markerat (standard).
1. Välj **[!UICONTROL Save]**.
1. Välj en mapp för lagring av den blandade medieuppsättningen och ange sedan ett namn för uppsättningen.
1. Välj **[!UICONTROL Save]**.

   Om du vill se hur din kombinationsbilduppsättning ser ut i ett visningsprogram väljer du **[!UICONTROL Preview]**.

## Redigera en blandad medieuppsättning {#edit-a-mixed-media-set}

Du kan redigera en uppsättning med blandade media. Om du vill redigera en uppsättning i en uppsättning med blandade media öppnar du den uppsättningen separat, redigerar den och sparar den. Redigeringarna visas i den blandade medieuppsättningen.

Oavsett om du redigerar en publicerad eller opublicerad uppsättning kan du **[!UICONTROL Publish after a save]** påverkar uppsättningen och medlemmarna i uppsättningen på följande sätt:

| Har du redan publicerat? | **[!UICONTROL Publish after a save]** är du markerad innan du sparar redigeringen? | Tillstånd för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
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
   * Om du vill ändra ordning på objekten drar du dem till nya platser.

1. När du är klar med redigeringen av uppsättningen, nära sidans nedre högra hörn, ser du till att **[!UICONTROL Publish after a save]** är markerat (standard).
1. Välj **[!UICONTROL Save]** eller **[!UICONTROL Save As]**.

## Ta bort en blandad medieuppsättning

När du tar bort en uppsättning flyttas själva uppsättningen till papperskorgen. Medlemmarna (eller&quot;underordnade&quot;) i uppsättningen påverkas dock inte. De behåller i stället sitt befintliga publicerade eller opublicerade läge.

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här tar du bort en blandad medieuppsättning:**

1. I Stödrastervisning, listvy eller detaljvy väljer du en eller flera blandade medieuppsättningar.
1. På det globala navigeringsfältet går du till **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.
