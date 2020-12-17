---
title: Skapa en bilduppsättning
seo-title: Skapa en bilduppsättning
description: 'null'
seo-description: Lär dig hur du skapar en bilduppsättning.
uuid: 689fdc14-4f51-4c94-8515-cd8551e101d8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 3f356410-b30e-4870-ad95-6e5a9dc126c8
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---


# Skapa en bilduppsättning{#creating-an-image-set}

Om du vill skapa en bilduppsättning med flera vyer behöver du bilder som visar ett objekt från olika vypunkter eller visar olika aspekter av samma objekt. Målet är att ge tittarna bilder av ett objekt så att de får en bra uppfattning om hur ett objekt ser ut eller gör.

## Skapa en bilduppsättning {#create}

När du skapar en uppsättning påverkar alternativet **Publicera efter spara** uppsättningen och anger medlemmar på följande sätt:

| Alternativet Publicera efter spara är markerat innan du sparar? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
|:--- |:--- |:--- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ange medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

**Skapa en bilduppsättning**

1. Gör något av följande:

   **Markera bilderna** förstMarkera de bilder du vill använda i bilduppsättningen i panelen Bläddra och klicka sedan på Skapa > Bilduppsättningar.

   **Starta från** skärmen BilduppsättningKlicka på Skapa > Bilduppsättningar. Skärmen Bilduppsättning öppnas. Markera en mapp i resursbiblioteket och dra bilderna som du vill använda i bilduppsättningen till skärmen Bilduppsättning.

1. Om du vill ändra bildordningen drar du bilderna till nya platser.
1. Kontrollera att **Publicera efter spara** är markerat i sidans nedre högra hörn (standard).
1. Klicka på **Spara**, välj en mapp där du vill spara din bilduppsättning, ange ett namn för uppsättningen och klicka sedan på **Spara**.
1. Om du vill visa din bilduppsättning i bilduppsättningsvisningsprogrammet klickar du på **Förhandsvisa** på skärmen Bilduppsättning. Du kan klicka på miniatyrbilderna för färgrutor i bilduppsättningsvisningsprogrammet för att se hur de beter sig.

## Redigera en bilduppsättning {#editing-an-image-set}

Beroende på om du redigerar en publicerad eller opublicerad uppsättning påverkar alternativet **Publicera efter spara** uppsättningen och ange medlemmar på följande sätt:

| Har du redan publicerat? | Alternativet Publicera efter spara är markerat innan du sparar redigeringen? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
|--- |--- |--- |--- |
| Ja | Ja | Publicerad | Publicerad |
| Ja | Nej | Publicerad | Befintliga uppsättningsmedlemmar behåller sin publicerade status.Alla nya uppsättningsmedlemmar som du lägger till under redigeringen behåller sin publicerade eller opublicerade status. |
| Nej | Ja | Publicerad | Publicerad |
| Nej | Nej | Opublicerad | Befintliga uppsättningsmedlemmar och nya uppsättningsmedlemmar som du har lagt till under redigeringen behåller sina publicerade eller opublicerade tillstånd. |

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

**Redigera en bilduppsättning**

1. I stödrastervyn bläddrar du till en ImageSet och klickar sedan under bilden på **Redigera**.
1. Gör något av följande:

   * Om du vill lägga till en bild (publicerad eller opublicerad) drar du den från en mapp i Lägg till resurser till sidan **Vyer** i bilduppsättningen.
   * Om du vill ta bort en bild markerar du den och klickar sedan på **Ta bort** i verktygsfältet.
   * Om du vill ändra ordning på bilderna drar du en bild till en ny plats.

1. När du är klar med redigeringen av uppsättningen, nära sidans nedre högra hörn, kontrollerar du att **Publicera efter spara** är markerat (standard).
1. Klicka på **Spara**, välj en lagringsmapp för uppsättningen, ange ett namn för uppsättningen och klicka sedan på **Spara**.

## Ta bort en bilduppsättning {#deleting-an-image-set}

När du tar bort en uppsättning flyttas själva uppsättningen till papperskorgen. Medlemmarna (eller &quot;barn&quot;) i uppsättningen påverkas dock inte. i stället behåller de sitt befintliga publicerade eller opublicerade läge.

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

**Ta bort en bilduppsättning**

1. Markera en eller flera bilduppsättningar i Stödrastervisning, listvy eller detaljvy.
1. I det globala navigeringsfältet klickar du på **Arkiv** > **Ta bort** > **Ta bort**.

