---
title: Skapa en färgruteuppsättning
description: Lär dig hur du skapar en färgruteuppsättning.
uuid: 250b3525-310d-4481-b0bc-f9057e823e0b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
discoiquuid: 631d2b2d-9e69-4b96-8392-17e00a1a8de0
feature: Dynamic Media Classic,Viewers
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 0%

---


# Skapa en färgruteuppsättning{#creating-a-swatch-set}

Med en uppsättning färgrutor kan användarna visa ett objekt i en annan färg, ett annat mönster eller en annan finish. Om du vill skapa en färgruteuppsättning med färgrutor behöver du en bild för varje färg, mönster eller slut som du vill visa för användarna. Du behöver också en färg-, mönster- eller slutfärgruta för varje färg, mönster eller slut.

Anta till exempel att du vill visa bilder med olika färgskalor; räkningarna är röda, gröna och blå. I så fall behöver du tre bilder med samma lock. Du behöver en bild med rött, en med grönt och en med blå räkning. Du behöver också en röd, grön och blå färgruta. Färgrutorna fungerar som miniatyrbilder som användare klickar på i visningsprogrammet för färgrutor för att visa den röda, gröna eller blå hatten.

## Skapa en färgruteuppsättning {#create}

När du skapar en uppsättning påverkar alternativet **Publicera efter spara** uppsättningen och anger medlemmar på följande sätt:
| Alternativet Publicera efter spara markerat innan du sparar?|Tillstånd för uppsättningen när den sparats|Tillstånd för angivna medlemmar efter sparande|
|— |— |— |
|Ja|Publicerad|Publicerad|
|No|Unpublished|Ange att medlemmarna behåller sitt publicerade eller opublicerade tillstånd.|

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

**Skapa en färgruteuppsättning**

1. Gör något av följande:

   **Markera bilderna** förstMarkera bilderna på panelen Bläddra och klicka sedan på Skapa > Färgruteuppsättningar.

   **Starta från** skärmen Uppsättning med färgrutorKlicka på Skapa > Uppsättningar med färgrutor. Markera en mapp i resursbiblioteket och dra bilderna till avsnittet Vyer på sidan Uppsättning med färgrutor.

1. Dra färgrutefärger, mönster eller lapp till platshållarrutan för färgrutor på sidan Uppsättning med färgrutor.

   Se till att färgrutan för färg, mönster eller slut som du drar till varje platshållare motsvarar färgen, mönstret eller slutet på den intilliggande bilden.

1. Om du vill ändra ordningen på bilderna i färgruteuppsättningen drar du bilderna till nya platser.
1. Kontrollera att **Publicera efter spara** är markerat i sidans nedre högra hörn (standard).
1. Klicka på **Spara**, välj en mapp där du vill spara färgruteuppsättningen, ange ett namn för uppsättningen och klicka på Skicka.
1. Klicka på **Förhandsgranska** på skärmen för färgruteuppsättningen om du vill visa din uppsättning i visningsprogrammet för färgrutor. Du kan klicka på miniatyrbilderna för färgrutor i Visningsprogrammet för färgrutor för att se hur de beter sig.

## Redigera en färgruteuppsättning {#editing-a-swatch-set}

Beroende på om du redigerar en publicerad eller opublicerad uppsättning påverkar alternativet **Publicera efter spara** uppsättningen och ange medlemmar på följande sätt:

| Har du redan publicerat? | Alternativet Publicera efter spara är markerat innan du sparar redigeringen? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
|--- |--- |--- |--- |
| Ja | Ja | Publicerad | Publicerad |
| Ja | Nej | Publicerad | Befintliga uppsättningsmedlemmar behåller sin publicerade status.Alla nya uppsättningsmedlemmar som du lägger till under redigeringen behåller sin publicerade eller opublicerade status. |
| Nej | Ja | Publicerad | Publicerad |
| Nej | Nej | Opublicerad | Befintliga uppsättningsmedlemmar och nya uppsättningsmedlemmar som du har lagt till under redigeringen behåller sina publicerade eller opublicerade tillstånd. |

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

**Redigera en färgruteuppsättning**

1. I stödrastervyn bläddrar du till en färgruteuppsättning och klickar sedan under bilden på **Redigera**.
1. Gör något av följande:

   * Om du vill lägga till en bild (publicerad eller opublicerad) drar du den från en mapp i Lägg till resurser till **Vyer** på sidan för färgruteuppsättningen.
   * Om du vill ta bort en bild markerar du den och klickar sedan på **Ta bort** i verktygsfältet.
   * Om du vill ändra ordning på bilderna drar du en bild till en ny plats.

1. När du är klar med redigeringen av uppsättningen, nära sidans nedre högra hörn, kontrollerar du att **Publicera efter spara** är markerat (standard).
1. Klicka på **Spara**, markera en lagringsmapp, ange ett namn för uppsättningen och klicka sedan på **Spara**.

## Ta bort en färgruteuppsättning {#deleting-a-swatch-set}

När du tar bort en uppsättning flyttas själva uppsättningen till papperskorgen. Medlemmarna (eller &quot;barn&quot;) i uppsättningen påverkas dock inte. i stället behåller de sitt befintliga publicerade eller opublicerade läge.

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

**Ta bort en färgruteuppsättning**

1. Markera en eller flera färgruteuppsättningar i Stödrastervisning, listvy eller detaljvy.
1. I det globala navigeringsfältet klickar du på **Arkiv** > **Ta bort** > **Ta bort**.

