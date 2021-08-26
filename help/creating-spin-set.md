---
title: Skapa en snurruppsättning
description: Lär dig hur du skapar en snurruppsättning i Adobe Dynamic Media Classic.
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '874'
ht-degree: 0%

---

# Skapa en snurruppsättning{#creating-a-spin-set}

Om du vill skapa en effektiv snurra ser du till att du tar bilderna på rätt sätt. Du kan skapa en snurruppsättning i Adobe Dynamic Media Classic genom att markera knappen Skapa och välja Snurra uppsättningar. Redigera snurruppsättningar på skärmen Snurra uppsättningar.

>[!NOTE]
>
>Tidigare versioner av Adobe Dynamic Media Classic hade inte tvådimensionella snurruppsättningar. Om du har skapat en snurra uppsättning i en tidigare version av Adobe Dynamic Media Classic kan du inte spara den endimensionella snurra uppsättningen utan att först spara den under ett annat namn. Välj **[!UICONTROL Save As]** på skärmen för snurruppsättning och ange ett nytt namn så att du kan redigera det i Adobe Dynamic Media Classic.

## Riktlinjer för fotografering av snurra uppsättningsbilder {#guidelines-for-shooting-spin-set-images}

Ju fler bilder du har i en snurrfunktion, desto bättre blir effekten av att snurra. Om du inkluderar många bilder i uppsättningen ökar dock tiden det tar för bilderna att läsas in. Adobe Dynamic Media Classic rekommenderar följande riktlinjer för att ta bilder som ska användas i snurra uppsättningar:

* Använd minst 8-12 bilder i en endimensionell snurra och 16-24 bilder i en tvådimensionell snurra.
* Använd ett förlustfritt format, TIFF och PNG rekommenderas.
* Maskera alla bilder så att objektet visas på en helt vit eller annan bakgrund med hög kontrast. Du kan också lägga till skuggor.
* Se till att produktinformationen är väl belyst och i fokus.
* Ta snurra bilder till modekläder med mannequin eller modell. Ofta är mannequin antingen maskerat (med hjälp av en glasmannequin) eller en stiliserad mannequin/form visas i bilden. Du kan skapa en omformningsrotation genom att definiera antalet vinklar. Markera varje vinkel med band på golvet så att du kan vägleda modellen till steg och titta i riktningen för varje tagning.

## Skapa en snurruppsättning {#create}

Den ordning i vilken du skapar eller skapar den i Adobe Dynamic Media Classic är viktig. Beroende på hur du ordnar resurserna när du drar och släpper bilder i rutnätet på sidan Snurra uppsättning, snurrar den i en viss riktning. Därför är den ordning i vilken resursen visas visuellt i byggaren hur resursen snurras när en användare flyttar muspekaren eller flyttar fingret, från vänster till höger.

När du skapar en uppsättning påverkar **[!UICONTROL Publish after save]**-alternativet mängdmedlemmarna på följande sätt:

| **[!UICONTROL Publish after save]** markerat alternativ innan du sparar? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
| --- | --- | --- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ange medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser](publishing-files.md#manually-publishing-assets) och [Manuellt avpublicera resurser](publishing-files.md#manually-unpublishing-assets).

När du har sparat en snurruppsättning kan du använda Förhandsvisning i Build: På sidan med rotationsuppsättningen ser du hur din snurruppsättning ser ut i standardvisningsprogrammet.

**Så här skapar du en snurra:**

1. Välj **[!UICONTROL Spin Sets]** i listrutan **[!UICONTROL Build]**.
1. Ange antalet rader och celler som du vill ha i dialogrutan Ange storlek för snurra.

   Om du vill skapa en endimensionell snurruppsättning markerar du endast en rad.

   Om du vill skapa en tvådimensionell snurra uppsättning markerar du två eller flera rader.

1. Välj **[!UICONTROL OK]**.
1. Dra och släpp bilder i rutnätet på skärmen Snurra uppsättning.
1. När du är klar ser du till att **Publicera efter spara** är markerat (standard) nära sidans nedre högra hörn.
1. Välj **[!UICONTROL Save]**.
1. I dialogrutan Spara väljer du en mapp för lagring av din snurruppsättning. I fältet Filnamn anger du namnet på rotationsuppsättningen.
1. Välj **[!UICONTROL Save]**.

## Redigera en snurra uppsättning {#editing-a-spin-set}

Oavsett om du redigerar en publicerad eller opublicerad uppsättning påverkar **[!UICONTROL Publish after save]**-alternativet uppsättningen och anger medlemmar på följande sätt:

| Har du redan publicerat? | **[!UICONTROL Publish after save]** är du markerad innan du sparar redigeringen? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
| --- | --- | --- | --- |
| Ja | Ja | Publicerad | Publicerad |
| Ja | Nej | Publicerad | Befintliga uppsättningsmedlemmar behåller sin publicerade status. Alla nya uppsättningsmedlemmar som du lägger till under redigeringen behåller sin publicerade eller opublicerade status. |
| Nej | Ja | Publicerad | Publicerad |
| Nej | Nej | Opublicerad | Befintliga uppsättningsmedlemmar och nya uppsättningsmedlemmar som du har lagt till under redigeringen behåller sina publicerade eller opublicerade tillstånd. |

Se även [Publicera resurser](publishing-files.md#manually-publishing-assets) och [Manuellt avpublicera resurser](publishing-files.md#manually-unpublishing-assets).

**Så här redigerar du en snurra:**

1. Välj knappen för rotationsuppsättningens överrullning **[!UICONTROL Edit]**.
1. Gör något av följande:

   * **Ta bort bilder** - Markera bilden och markera sedan  **[!UICONTROL Delete]**.

   * **Lägga till bilder**  - Dra bilden till en cell.

   * **Ändra ordning på rader (tvådimensionella snurruppsättningar)** - Markera en radväljarruta (till vänster om raden) och markera  **[!UICONTROL Move Row Down]** eller  **[!UICONTROL Move Row Up]**.

   * **Lägga till rader och celler**  - Ange ett värde i rutorna Rader och Celler för att bestämma antalet rader och antalet celler i varje rad.

1. Se till att **[!UICONTROL Publish after save]** är markerat (standard) när du är klar med redigeringen, nära sidans nedre högra hörn.
1. Välj **[!UICONTROL Save]**, markera en lagringsmapp, ange ett namn för uppsättningen och välj sedan **[!UICONTROL Save]**.

## Ta bort en snurruppsättning {#deleting-a-spin-set}

När du tar bort en uppsättning flyttas själva uppsättningen till papperskorgen. Medlemmarna (eller &quot;barn&quot;) i uppsättningen påverkas dock inte. i stället behåller de sitt befintliga publicerade eller opublicerade läge.

Se även [Publicera resurser](publishing-files.md#manually-publishing-assets) och [Manuellt avpublicera resurser](publishing-files.md#manually-unpublishing-assets).

**Så här tar du bort en snurruppsättning:**

1. I Stödrastervisning, listvy eller detaljvy väljer du en eller flera snurruppsättningar.
1. I det globala navigeringsfältet går du till **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.
