---
title: '"Snabbstart: Blandade medieuppsättningar"'
seo-title: '"Snabbstart: Blandade medieuppsättningar"'
description: 'null'
seo-description: En introduktion och snabbstart av blandade medieuppsättningar som hjälper dig att komma igång snabbt.
uuid: 0ef033d5-b053-4d7c-b1e1-1980f899fd88
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
discoiquuid: 2708d077-94fc-4045-8992-ad3589ed9cfd
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Snabbstart: Blandade medieuppsättningar{#quick-start-mixed-media-sets}

Mixed Media Sets ger användarna en integrerad visningsupplevelse. Blandade medieuppsättningar kan innehålla bilder, bilduppsättningar, färgruteuppsättningar, snurruppsättningar och videoklipp. Användarna kan klicka på olika flikar i visningsprogrammet för blandade media för att se objekten i olika visningsprogram. Om inga flikar har angetts visas alla resurser tillsammans i färgruteraden.

Förinställningar för visningsprogram för blandade media innehåller communityalternativ för slutanvändare som kan bädda in kod, kopiera URL:er och länka till huvudwebbplatsen. Användare kan använda dessa alternativ för att dela information om produkter på sina personliga webbplatser eller sociala nätverksplatser.

**Snabbstart**

Den här snabbstarten för blandade medieuppsättningar är utformad för att komma igång snabbt med blandad mediauppsättning i Dynamic Media Classic.

**1. Överföra bilder, färgrutefiler och videoklipp**

Börja med att ladda upp bilder, färgrutefiler och videoklipp till dina blandade medieuppsättningar. Eftersom användare kan zooma in bilder i visningsprogrammet för uppsättningen med blandade medier bör du ta hänsyn till zoomningen när du väljer bilder. Se till att bilderna har minst 2 000 pixlar i den största dimensionen.

Klicka på Överför i det globala navigeringsfältet för att överföra filer från datorn till en mapp i Scene7 Publishing System.

Se [Överföra filer](uploading-files.md#uploading-your-files).

**2. Skapa medieuppsättningar som ska användas i den blandade medieuppsättningen**

Du kan lägga till bilder, bilduppsättningar, färgruteuppsättningar, snurruppsättningar och videoklipp i din uppsättning med blandade media. Förbered medieuppsättningarna innan du lägger till dem i den blandade medieuppsättningen.

Se [Skapa en bilduppsättning](creating-image-set.md#creating-an-image-set), [Skapa en uppsättning](creating-swatch-set.md#creating-a-swatch-set)med färgrutor och [Skapa en uppsättning](creating-spin-set.md#creating-a-spin-set)med snurra.

**3. Skapa en blandad medieuppsättning**

Klicka på knappen Skapa och välj Blandade medieuppsättningar. Dra bilder, färgruteuppsättningar, bilduppsättningar och videofilmer till skärmen med blandade medieuppsättningar. Om du vill lägga till ett ljudspår drar du en ljudfil till rutan Ljudspår.

Se [Skapa en blandad medieuppsättning](creating-mixed-media-set.md#creating-a-mixed-media-set).

**4. Konfigurera förinställningar för visningsprogrammet för blandade media**

Dynamic Media Classic levereras med standardförinställningar för visningsprogram för blandade medieuppsättningar. Administratörer kan skapa eller ändra förinställningar för visningsprogrammet för blandad medieuppsättning.

När du konfigurerar en visningsförinställning för blandad medieuppsättning lägger du till visningsförinställningarna för alla andra resurser i uppsättningen. Om din uppsättning med blandade media innehåller videoklipp lägger du till en förinställning för visningsprogrammet för video i förinställningen för visningsprogrammet för blandade media. Du kan också lägga till ett ljudspår i visningsprogrammet. Det här ljudspåret spelas upp när visningsprogrammet är öppet, men spelas inte upp när en video är aktiv.

Se [Konfigurera en visningsförinställning](setting-mixed-media-set-viewer.md#setting-up-a-mixed-media-set-viewer-preset) för en blandad medieuppsättning och [Skapa och redigera visningsförinställningar](application-setup.md#adding-and-editing-viewer-presets).

**5. Förhandsgranska en blandad medieuppsättning**

Klicka på knappen Förhandsvisa överrullning för den blandade medieuppsättningen. Den blandade medieuppsättningen visas. Du kan klicka på miniatyrbilds- och färgruteikonerna för att undersöka den blandade medieuppsättningen i visningsprogrammet för den blandade medieuppsättningen. Du kan välja olika visningsprogram från förinställningsmenyerna.

Se [Förhandsvisa en resurs](previewing-asset.md#previewing-an-asset).

**6. Publicera en blandad medieuppsättning**

När du publicerar en uppsättning med blandade media placeras den på dynamiska Media Classic-servrar och URL-strängen aktiveras.

Blandade medieuppsättningar kräver att du publicerar till **videoservern** och även till **bildservern**. Du använder **Video Server** för att publicera de faktiska videoklippen som du har markerat för publicering. Och du kan använda **Image Server** för att publicera relaterade resurser, till exempel videominiatyrer, och ange information för alla adaptiva videouppsättningar.

Se [Publicera en blandad medieuppsättning](publishing-mixed-media-set.md#publishing-a-mixed-media-set).

**7. Länka en uppsättning med blandade media till en webbsida**

Dynamic Media Classic aktiverar URL-anrop för blandade medieuppsättningar när du har publicerat dem. Du kan kopiera dessa URL:er från förhandsgranskningsskärmen.

Markera den blandade medieuppsättningen och klicka på Förhandsgranska. Välj en visningsförinställning för blandad medieuppsättning på förhandsgranskningsskärmen och klicka på knappen Kopiera URL. Se [Länka en uppsättning med blandade media till en webbsida](linking-mixed-media-set-web.md#linking-a-mixed-media-set-to-a-web-page).
