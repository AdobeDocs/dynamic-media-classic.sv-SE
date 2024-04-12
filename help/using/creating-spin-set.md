---
title: Skapa en snurra uppsättning
description: Lär dig hur du skapar en snurruppsättning i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
topic: Content Management
level: Intermediate
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# Skapa en snurra uppsättning{#creating-a-spin-set}

Om du vill skapa en effektiv snurra ser du till att du tar bilderna på rätt sätt. Du kan skapa en snurrsuppsättning i Adobe Dynamic Media Classic genom att markera knappen Skapa och välja Snurra uppsättningar. Redigera snurruppsättningar på skärmen Snurra uppsättningar.

>[!NOTE]
>
>Tidigare versioner av Adobe Dynamic Media Classic hade inte tvådimensionella snurruppsättningar. Om du har skapat en snurra uppsättning i en tidigare version av Adobe Dynamic Media Classic kan du inte spara den endimensionella snurra uppsättningen utan att först spara den under ett annat namn. Välj **[!UICONTROL Save As]** i fönstret för att ange ett nytt namn så att du kan redigera det i Adobe Dynamic Media Classic.

## Riktlinjer för fotografering av snurra uppsättningsbilder {#guidelines-for-shooting-spin-set-images}

Ju fler bilder du har i en snurra desto bättre blir effekten av att snurra. Om du inkluderar många bilder i uppsättningen ökar dock tiden det tar för bilderna att läsas in. Adobe Dynamic Media Classic rekommenderar följande riktlinjer för att ta bilder för användning i snurra uppsättningar:

* Använd minst 8-12 bilder i en endimensionell snurra och 16-24 bilder i en tvådimensionell snurra.
* Använd ett icke-förstörande format; TIFF och PNG rekommenderas.
* Maskera alla bilder så att objektet visas på en helt vit eller annan högkontrastbakgrund. Du kan också lägga till skuggor.
* Se till att produktinformationen är väl belyst och i fokus.
* Ta snurra bilder till modekläder med mannequin eller modell. Ofta är mannequin antingen maskerat (med hjälp av en glasmannequin) eller en stiliserad mannequin/form visas i bilden. Du kan skapa en snurra på modellen genom att definiera antalet vinklar. Markera varje vinkel med band på golvet så att du kan vägleda modellen till steg och titta i riktningen för varje tagning.

## Skapa en snurra uppsättning {#create}

Den ordning i vilken rotationsrutan skapas eller skapas i Adobe Dynamic Media Classic är viktig. Beroende på hur du ordnar resurserna när du drar och släpper bilder i rutnätet på sidan Snurra uppsättning, snurrar den i en viss riktning. Därför är den ordning i vilken resursen visas visuellt i byggaren hur resursen snurras när en användare flyttar muspekaren eller flyttar fingret, från vänster till höger.

När du skapar en uppsättning **[!UICONTROL Publish after save]** påverkar uppsättningen och medlemmarna i uppsättningen på följande sätt:

| **[!UICONTROL Publish after save]** markerat alternativ innan du sparar? | Tillstånd för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
| --- | --- | --- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ställda medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser manuellt](publishing-files.md#manually-publishing-assets) och [Avpublicera resurser manuellt](publishing-files.md#manually-unpublishing-assets).

När du skapar en snurrsuppsättning rekommenderar Adobe följande bästa praxis och tillämpar följande gräns:

| Begränsningstyp för snurra uppsättning | Bästa praxis | Begränsning har införts |
| --- | --- | --- |
| Maximalt antal rader/kolumner per 2D-uppsättning | 12-18 bilder per uppsättning | 1000 |

Se även [Dynamic Media begränsningar](/help/using/limitations.md).

När du har sparat en snurruppsättning kan du använda Förhandsvisning på sidan Skapa: snurra uppsättning för att se hur din snurra uppsättning ser ut i standardvisningsprogrammet.

**Så här skapar du en snurra:**

1. På **[!UICONTROL Build]** nedrullningsbar meny, välja **[!UICONTROL Spin Sets]**.
1. Ange antalet rader och celler som du vill ha i dialogrutan Ange storlek för snurra.

   Om du vill skapa en endimensionell snurruppsättning markerar du endast en rad.

   Om du vill skapa en tvådimensionell snurra uppsättning markerar du två eller flera rader.

1. Välj **[!UICONTROL OK]**.
1. Dra och släpp bilder i rutnätet på skärmen Snurra uppsättning.
1. När du är klar ser du till att du ser till att **Publicera efter spara** är markerat (standard).
1. Välj **[!UICONTROL Save]**.
1. I dialogrutan Spara väljer du en mapp för lagring av din snurruppsättning. I fältet Filnamn anger du namnet på rotationsuppsättningen.
1. Välj **[!UICONTROL Save]**.

## Redigera en snurra uppsättning {#editing-a-spin-set}

Oavsett om du redigerar en publicerad uppsättning eller en opublicerad uppsättning kan du **[!UICONTROL Publish after save]** påverkar uppsättningen och medlemmarna i uppsättningen på följande sätt:

| Har du redan publicerat? | **[!UICONTROL Publish after save]** är du markerad innan du sparar redigeringen? | Tillstånd för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
| --- | --- | --- | --- |
| Ja | Ja | Publicerad | Publicerad |
| Ja | Nej | Publicerad | Befintliga uppsättningsmedlemmar behåller sin publicerade status. Alla nya uppsättningsmedlemmar som du lägger till under redigeringen behåller sin publicerade eller opublicerade status. |
| Nej | Ja | Publicerad | Publicerad |
| Nej | Nej | Opublicerad | Befintliga uppsättningsmedlemmar och nya uppsättningsmedlemmar som du har lagt till under redigeringen behåller sina publicerade eller opublicerade tillstånd. |

Se även [Publicera resurser manuellt](publishing-files.md#manually-publishing-assets) och [Avpublicera resurser manuellt](publishing-files.md#manually-unpublishing-assets).

**Så här redigerar du en snurra:**

1. Markera rotationslistens överrullning **[!UICONTROL Edit]** -knappen.
1. Gör något av följande:

   * **Ta bort bilder** - Markera bilden och välj sedan **[!UICONTROL Delete]**.

   * **Lägga till bilder** - Dra bilden till en cell.

   * **Ändra ordning på rader (tvådimensionella snurruppsättningar)** - Markera en radväljarruta (till vänster om raden) och markera sedan **[!UICONTROL Move Row Down]** eller **[!UICONTROL Move Row Up]**.

   * **Lägga till rader och celler** - Ange en siffra i rutorna Rader och Celler för att bestämma antalet rader och antalet celler i varje rad.

1. När du är klar med redigeringen, nära det nedre högra hörnet på sidan, ser du till att **[!UICONTROL Publish after save]** är markerat (standard).
1. Välj **[!UICONTROL Save]**, väljer en lagringsmapp, anger ett namn för uppsättningen och väljer sedan **[!UICONTROL Save]**.

## Ta bort en snurruppsättning

När du tar bort en uppsättning flyttas själva uppsättningen till papperskorgen. Medlemmarna (eller&quot;underordnade&quot;) i uppsättningen påverkas dock inte. De behåller i stället sitt befintliga publicerade eller opublicerade läge.

Se även [Publicera resurser manuellt](publishing-files.md#manually-publishing-assets) och [Avpublicera resurser manuellt](publishing-files.md#manually-unpublishing-assets).

**Så här tar du bort en snurruppsättning:**

1. I Stödrastervisning, listvy eller detaljvy väljer du en eller flera snurruppsättningar.
1. På det globala navigeringsfältet går du till **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.
