---
title: Skapa en blandad medieuppsättning
seo-title: Skapa en blandad medieuppsättning
description: 'null'
seo-description: Lär dig hur du skapar en uppsättning med blandade media.
uuid: a0c6e5fa-7a85-4376-b9a3-b72ae63d3d95
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0ff9e763-897c-4ba5-b606-a95d5e45f35e
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 0%

---


# Skapa en blandad medieuppsättning{#creating-a-mixed-media-set}

Skapa en blandad medieuppsättning när du vill kombinera flera typer av visningsprogram i en presentation. Kontrollera att dina filer, bilduppsättningar, färgruteuppsättningar och snurruppsättningar är klara att publiceras innan du lägger till dem i den blandade medieuppsättningen.

![Blandad medieuppsättning](/help/assets/mm_mixed_media_set.png)

## Skapa en blandad medieuppsättning {#create-a-mixed-media-set}

När du skapar en uppsättning påverkar alternativet **Publicera efter spara** den och anger medlemmar på följande sätt:

| Alternativet Publicera efter spara är markerat innan du sparar? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
|--- |--- |--- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ange medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) manuellt och [Avpublicera resurser](publishing-files.md#manually_unpublishing_assets)manuellt.

**Skapa en blandad medieuppsättning**

1. Klicka på **Skapa** > **Blandade medieuppsättningar**.
1. Dra videoklipp, bilduppsättningar, snurruppsättningar och färgrutor från resursbiblioteket till skärmen med blandade medieuppsättningar.

   >[!NOTE]
   >
   >Blandade medieuppsättningar stöder inte resurser med filnamn som innehåller något av följande tecken: ( ) { }.

1. Gör något av följande:

   * Om du vill lägga till ett ljudspår drar du en ljudfil från resursbiblioteket till rutan Ljudspår. Ljudspåret spelas upp när bilder visas. Det stoppas när video spelas upp.
   * Om du vill ändra ordningen på uppsättningar drar du dem till nya platser på skärmen med blandade medieuppsättningar. Ordningen på uppsättningarna på skärmen avgör i vilken ordning användarna ser uppsättningar i visningsprogrammet för den blandade medieuppsättningen.
   * (Valfritt) Om du vill lägga till en anpassad miniatyrbild som representerar en video i visningsprogrammet drar du en bildfil från resursbiblioteket till platshållarrutan för miniatyrbilder.

1. Kontrollera att **Publicera efter spara** är markerat i sidans nedre högra hörn (standard).
1. Klicka på **Spara**, välj en mapp där den blandade medieuppsättningen ska lagras, ange ett namn för uppsättningen och klicka på **Spara**.

   Klicka på **Förhandsgranska** för att se hur din kombinationsbilduppsättning ser ut i en visningsprogram för bilduppsättning.

## Redigera en blandad medieuppsättning {#edit-a-mixed-media-set}

Du kan redigera en uppsättning med blandade media. Om du vill redigera en uppsättning i en uppsättning med blandade media öppnar du den uppsättningen separat, redigerar den och sparar den. Redigeringarna visas i uppsättningen med blandade media.

Beroende på om du redigerar en publicerad eller opublicerad uppsättning påverkar alternativet **Publicera efter sparande** medlemmarna i uppsättningen och uppsättningen på följande sätt:

| Har du redan publicerat? | Alternativet Publicera efter spara är markerat innan du sparar redigeringen? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
|--- |--- |--- |--- |
| Ja | Ja | Publicerad | Publicerad |
| Ja | Nej | Publicerad | Befintliga uppsättningsmedlemmar behåller sin publicerade status.Alla nya uppsättningsmedlemmar som du lägger till under redigeringen behåller sin publicerade eller opublicerade status. |
| Nej | Ja | Publicerad | Publicerad |
| Nej | Nej | Opublicerad | Befintliga uppsättningsmedlemmar och nya uppsättningsmedlemmar som du har lagt till under redigeringen behåller sina publicerade eller opublicerade tillstånd. |

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) manuellt och [Avpublicera resurser](publishing-files.md#manually_unpublishing_assets)manuellt.

**Redigera en blandad medieuppsättning**

1. Klicka på knappen **Redigera** överrullning för den blandade medieuppsättningen.
1. Gör något av följande:

   * Om du vill ta bort objekt markerar du dem och klickar på **Ta bort**.
   * Om du vill ordna om objekt drar du dem till nya platser.

1. När du är klar med redigeringen av uppsättningen, nära sidans nedre högra hörn, kontrollerar du att **Publicera efter spara** är markerat (standard).
1. Klicka på **Spara** eller **Spara som**.

## Ta bort en blandad medieuppsättning {#deleting-a-mixed-media-set}

När du tar bort en uppsättning flyttas själva uppsättningen till papperskorgen. Medlemmarna (eller &quot;barn&quot;) i uppsättningen påverkas dock inte. i stället behåller de sitt befintliga publicerade eller opublicerade läge.

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) manuellt och [Avpublicera resurser](publishing-files.md#manually_unpublishing_assets)manuellt.

**Ta bort en blandad medieuppsättning**

1. I Stödrastervisning, listvy eller detaljvy väljer du en eller flera blandade medieuppsättningar.
1. Klicka på **Arkiv** > **Ta bort** > **Ta bort** i det globala navigeringsfältet.

