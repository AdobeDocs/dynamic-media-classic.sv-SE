---
title: Skapa en färgruteuppsättning
description: Lär dig hur du skapar en färgruteuppsättning i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 0%

---

# Skapa en färgruteuppsättning{#creating-a-swatch-set}

Med en uppsättning färgrutor kan användarna visa ett objekt i en annan färg, ett annat mönster eller en annan finish. Om du vill skapa en färgruteuppsättning med färgrutor behöver du en bild för varje färg, mönster eller slut som du vill visa för användarna. Du behöver också en färg-, mönster- eller slutfärgruta för varje färg, mönster eller slut.

Anta till exempel att du vill visa bilder av ändpunkter med olika färgskalor. Bilderna är röda, gröna och blå. I så fall behöver du tre bilder med samma lock. Du behöver en bild med rött, en med grönt och en med blå räkning. Du behöver också en röd, grön och blå färgruta. Färgrutorna fungerar som miniatyrbilder som användarna väljer i Visningsprogrammet för färgrutor för att se den röda, gröna eller blå hatten.

## Skapa en färgruteuppsättning {#create}

När du skapar en uppsättning påverkar alternativet **Publish efter en spara** medlemmarna i uppsättningen och uppsättningen på följande sätt:

| **[!UICONTROL Publish after a save]** alternativ markerat innan du sparar? | Tillstånd för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
| --- | --- | --- |
| Ja | Publicerad | publicerad |
| Nej | Opublicerad | Ställda medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här skapar du en färgruteuppsättning:**

1. Gör något av följande:

   * **Markera först bilderna**: Markera bilderna på panelen Bläddra och gå sedan till **[!UICONTROL Build]** > **[!UICONTROL Swatch Sets]**.

   * **Starta från skärmen för färgruteuppsättningen**: Gå till **[!UICONTROL Build]** > **[!UICONTROL Swatch Sets]**. Markera en mapp i resursbiblioteket och dra bilderna till avsnittet Vyer på sidan Uppsättning med färgrutor.

1. Dra färgrutefärger, mönster eller lapp till platshållarrutan för färgrutor på sidan Uppsättning med färgrutor.

   Se till att färgrutan för färg, mönster eller slut som du drar till varje platshållare motsvarar färgen, mönstret eller slutet på den intilliggande bilden.

1. Om du vill ändra ordningen på bilderna i färgruteuppsättningen drar du bilderna till nya platser.
1. Kontrollera att **[!UICONTROL Publish after a save]** är markerat (standard) nära sidans nedre högra hörn.
1. Välj **[!UICONTROL Save]**, välj en mapp där du vill lagra färgruteuppsättningen, ange ett namn för uppsättningen och välj **[!UICONTROL Submit]**.
1. Om du vill visa färgruteuppsättningen i visningsprogrammet för färgruteuppsättningen väljer du **[!UICONTROL Preview]** på skärmen för färgruteuppsättningen. Du kan välja miniatyrbilder för färgrutor i Visningsprogrammet för färgrutor för att se hur de fungerar.

## Redigera en färgruteuppsättning {#editing-a-swatch-set}

Oavsett om du redigerar en publicerad eller opublicerad uppsättning påverkar alternativet **[!UICONTROL Publish after a save]** medlemmarna i uppsättningen och uppsättningen på följande sätt:

| Har du redan publicerat? | **[!UICONTROL Publish after a save]** sparalternativ är valt innan du sparar redigeringen? | Tillstånd för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
|--- | --- | --- | --- |
| Ja | Ja | Publicerad | Publicerad. |
| Ja | Nej | Publicerad | Befintliga uppsättningsmedlemmar behåller sin publicerade status. Alla nya uppsättningsmedlemmar som du lägger till under redigeringen behåller sin publicerade eller opublicerade status. |
| Nej | Ja | Publicerad | Publicerad. |
| Nej | Nej | Opublicerad | Befintliga uppsättningsmedlemmar och nya uppsättningsmedlemmar som du har lagt till under redigeringen behåller sina publicerade eller opublicerade tillstånd. |

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här redigerar du en färgruteuppsättning:**

1. I stödrastervyn bläddrar du till en SwatchSet och väljer **[!UICONTROL Edit]** nedanför bilden.
1. Gör något av följande:

   * Om du vill lägga till en bild (publicerad eller opublicerad) drar du den från en mapp i Lägg till Assets till sidan **[!UICONTROL Views]** för färgruteuppsättningen.
   * Om du vill ta bort en bild markerar du den och väljer sedan **[!UICONTROL Delete]** i verktygsfältet.
   * Om du vill ändra ordning på bilderna drar du en bild till en ny plats.

1. När du är klar med redigeringen av uppsättningen, nära sidans nedre högra hörn, kontrollerar du att **[!UICONTROL Publish after a save]** är markerat (standard).
1. Välj **[!UICONTROL Save]**, markera en lagringsmapp, ange ett namn för uppsättningen och välj sedan **[!UICONTROL Save]**.

## Ta bort en färgruteuppsättning

När du tar bort en uppsättning flyttas själva uppsättningen till papperskorgen. Medlemmarna (eller&quot;underordnade&quot;) i uppsättningen påverkas dock inte. De behåller i stället sitt befintliga publicerade eller opublicerade läge.

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här tar du bort en färgruteuppsättning:**

1. I Stödrastervisning, listvy eller detaljvy väljer du en färgruteuppsättning eller flera.
1. Gå till **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]** i det globala navigeringsfältet.
