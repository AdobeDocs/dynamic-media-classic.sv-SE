---
title: Skapa en snurruppsättning
seo-title: Skapa en snurruppsättning
description: 'null'
seo-description: Lär dig hur du skapar en snurruppsättning.
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 0%

---


# Skapa en snurruppsättning{#creating-a-spin-set}

Om du vill skapa en effektiv snurra ser du till att du tar bilderna på rätt sätt. Du kan skapa en snurrsuppsättning i Dynamic Media Classic genom att markera knappen Skapa och välja Snurra uppsättningar. Redigera snurruppsättningar på skärmen Snurra uppsättningar.

>[!NOTE]
>
>Tidigare versioner av Dynamic Media Classic hade inte tvådimensionella snurruppsättningar. Om du har skapat en snurra uppsättning i en tidigare version av Dynamic Media Classic kan du inte spara den endimensionella snurra uppsättningen utan att först spara den under ett annat namn. Klicka på Spara som på skärmen med den nya rotationsuppsättningen och ange ett nytt namn så att du kan redigera den i Dynamic Media Classic.

## Riktlinjer för fotografering av snurruppsättningsbilder {#guidelines-for-shooting-spin-set-images}

Ju fler bilder du har i en snurrfunktion, desto bättre blir effekten av att snurra. Om du inkluderar många bilder i uppsättningen ökar dock tiden det tar för bilderna att läsas in. Dynamic Media Classic rekommenderar följande riktlinjer för att ta bilder som ska användas i snurra uppsättningar:

* Använd minst 8-12 bilder i en endimensionell snurra och 16-24 bilder i en tvådimensionell snurra.
* Använd ett förlustfritt format, TIFF och PNG rekommenderas.
* Maskera alla bilder så att objektet visas på en helt vit eller annan bakgrund med hög kontrast. Du kan också lägga till skuggor.
* Se till att produktinformationen är väl belyst och i fokus.
* Ta snurra bilder till modekläder med mannequin eller modell. Ofta är mannequin antingen helt maskerat (med hjälp av en glasmannequin) eller en stiliserad mannequin/form visas i bilden. Du kan skapa en omformningsrotation genom att definiera antalet vinklar. Markera varje vinkel med band på golvet för att vägleda modellen till steg och titta i riktningen för varje tagning.

## Skapa en snurruppsättning {#create}

Tänk på att den ordning i vilken du skapar eller skapar den i Dynamic Media Classic är viktig. Beroende på hur du ordnar resurserna när du drar och släpper bilder i rutnätet på sidan Snurra uppsättning, snurrar den i en viss riktning. Därför är den ordning i vilken resursen visas visuellt i byggaren hur resursen snurras när användaren flyttar muspekaren eller flyttar fingret, från vänster till höger.

När du skapar en uppsättning påverkar alternativet **Publicera efter spara** uppsättningen och anger medlemmar på följande sätt:

| Alternativet Publicera efter spara är markerat innan du sparar? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
|--- |--- |--- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ange medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser](publishing-files.md#manually-publishing-assets) och [Manuellt avpublicera resurser](publishing-files.md#manually-unpublishing-assets).

När du har sparat en snurruppsättning kan du använda Förhandsvisning i Build: På sidan med rotationsuppsättningen ser du hur din snurruppsättning ser ut i standardvisningsprogrammet.

**Skapa en snurruppsättning**

1. I listrutan **Build** klickar du på **Spin Sets**.
1. Ange antalet rader och celler som du vill ha i dialogrutan Ange storlek för snurra.

   Om du vill skapa en endimensionell snurruppsättning markerar du endast en rad.

   Om du vill skapa en tvådimensionell snurra uppsättning markerar du två eller flera rader.

1. Klicka på **OK**.
1. Dra och släpp bilder i rutnätet på skärmen Snurra uppsättning.
1. När du är klar ser du till att **Publicera efter spara** är markerat (standard) nära sidans nedre högra hörn.
1. Klicka på **Spara**.
1. I dialogrutan Spara väljer du en mapp för lagring av din snurruppsättning. I fältet Filnamn anger du namnet på rotationsuppsättningen.
1. Klicka på **Spara**.

## Redigera en snurruppsättning {#editing-a-spin-set}

Beroende på om du redigerar en publicerad eller opublicerad uppsättning påverkar alternativet **Publicera efter spara** uppsättningen och ange medlemmar på följande sätt:

| Har du redan publicerat? | Alternativet Publicera efter spara är markerat innan du sparar redigeringen? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
|--- |--- |--- |--- |
| Ja | Ja | Publicerad | Publicerad |
| Ja | Nej | Publicerad | Befintliga uppsättningsmedlemmar behåller sin publicerade status.Alla nya uppsättningsmedlemmar som du lägger till under redigeringen behåller sin publicerade eller opublicerade status. |
| Nej | Ja | Publicerad | Publicerad |
| Nej | Nej | Opublicerad | Befintliga uppsättningsmedlemmar och nya uppsättningsmedlemmar som du har lagt till under redigeringen behåller sina publicerade eller opublicerade tillstånd. |

Se även [Publicera resurser](publishing-files.md#manually-publishing-assets) och [Manuellt avpublicera resurser](publishing-files.md#manually-unpublishing-assets).

**Redigera en snurruppsättning**

1. Klicka på knappen för rotationsuppsättningens överrullning **Redigera**.
1. Gör något av följande:

   * **Ta bort**
bilderMarkera bilden och klicka sedan på 
**Ta bort**.

   * **Lägga till**
bilderDra bilden till en cell.

   * **Ändra ordning på rader (tvådimensionella snurruppsättningar)**
Klicka i en radväljarruta (till vänster om raden) och klicka sedan på 
**Flytta rad** nedåt eller  **flytta rad uppåt**.

   * **Lägga till rader och**
cellerAnge en siffra i rutorna Rader och Celler för att bestämma antalet rader och antalet celler i varje rad.

1. När du är klar med redigeringen ser du till att **Publicera efter spara** är markerat (standard) nära sidans nedre högra hörn.
1. Klicka på **Spara**, markera en lagringsmapp, ange ett namn för uppsättningen och klicka sedan på **Spara**.

## Tar bort en snurruppsättning {#deleting-a-spin-set}

När du tar bort en uppsättning flyttas själva uppsättningen till papperskorgen. Medlemmarna (eller &quot;barn&quot;) i uppsättningen påverkas dock inte. i stället behåller de sitt befintliga publicerade eller opublicerade läge.

Se även [Publicera resurser](publishing-files.md#manually-publishing-assets) och [Manuellt avpublicera resurser](publishing-files.md#manually-unpublishing-assets).

**Ta bort en snurra uppsättning**

1. I Stödrastervisning, listvy eller detaljvy väljer du en eller flera snurruppsättningar.
1. I det globala navigeringsfältet klickar du på **Arkiv** > **Ta bort** > **Ta bort**.

