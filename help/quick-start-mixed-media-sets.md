---
title: '"Snabbstart: Blandad medieuppsättning"'
description: En introduktion och snabbstart av blandade medieuppsättningar som hjälper dig att komma igång snabbt.
uuid: 0ef033d5-b053-4d7c-b1e1-1980f899fd88
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
discoiquuid: 2708d077-94fc-4045-8992-ad3589ed9cfd
feature: Dynamic Media Classic,visningsprogram,Mix-medieuppsättning
role: User
exl-id: 757893ae-7507-42a0-a67b-f6542e7231c7
source-git-commit: f99832bc9660a16b06e63b19f9ead1267dab0f35
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---

# Snabbstart: Blandade medieuppsättningar{#quick-start-mixed-media-sets}

Mixed Media Sets ger användarna en integrerad visningsupplevelse. Blandade medieuppsättningar kan innehålla bilder, bilduppsättningar, färgruteuppsättningar, snurruppsättningar och videoklipp. Användarna kan klicka på olika flikar i visningsprogrammet för blandade media för att se objekten i olika visningsprogram. Om inga flikar har angetts visas alla resurser tillsammans i färgruteraden.

Förinställningar för visningsprogram för blandade media innehåller communityalternativ för slutanvändare som kan bädda in kod, kopiera URL:er och länka till huvudwebbplatsen. Användare kan använda dessa alternativ för att dela information om produkter på sina personliga webbplatser eller sociala nätverksplatser.

Den här snabbstarten för blandade medieuppsättningar är utformad för att komma igång snabbt med blandad medieuppsättning i Dynamic Media Classic.

## 1. Överföra bilder, färgrutefiler och videoklipp

Börja med att ladda upp bilder, färgrutefiler och videoklipp till dina blandade medieuppsättningar. Eftersom användare kan zooma in bilder i visningsprogrammet för den blandade medieuppsättningen måste du ta hänsyn till den möjligheten när du väljer bilder. Se till att bilderna har en största storlek på minst 2 000 pixlar.

Klicka på **[!UICONTROL Upload]** i fältet Global navigering för att överföra filer från datorn till en mapp i Dynamic Media Classic.

Se [Överföra filer](uploading-files.md#uploading-your-files).

## 2. Skapa medieuppsättningar som ska användas i den blandade medieuppsättningen

Du kan lägga till bilder, bilduppsättningar, färgruteuppsättningar, snurruppsättningar och videoklipp i din uppsättning med blandade media. Förbered medieuppsättningarna innan du lägger till dem i den blandade medieuppsättningen.

Se [Skapa en bilduppsättning](creating-image-set.md#creating-an-image-set), [Skapa en färgruteuppsättning](creating-swatch-set.md#creating-a-swatch-set) och [Skapa en snurruppsättning](creating-spin-set.md#creating-a-spin-set).

## 3. Skapa en blandad medieuppsättning

Klicka på **[!UICONTROL Build]** > **[!UICONTROL Mixed Media Sets]** i fältet Global Navigation. Dra bilder, färgruteuppsättningar, bilduppsättningar och videofilmer till sidan med blandade medieuppsättningar. Om du vill lägga till ett ljudspår drar du en ljudfil till rutan Ljudspår.

Se [Skapa en blandad medieuppsättning](creating-mixed-media-set.md#creating-a-mixed-media-set).

## 4. Konfigurera förinställningar för visningsprogrammet för blandade media

Dynamic Media Classic innehåller standardförinställningar för visningsprogram för blandade medieuppsättningar. Administratörer kan skapa eller ändra förinställningar för visningsprogrammet för blandad medieuppsättning.

När du konfigurerar en visningsförinställning för blandad medieuppsättning lägger du till visningsförinställningarna för alla andra resurser i uppsättningen. Om din uppsättning med blandade media till exempel innehåller videoklipp lägger du till en förinställning för visningsprogrammet för video i förinställningen för visningsprogrammet med blandade media. Du kan också lägga till ett ljudspår i visningsprogrammet. Det här ljudspåret spelas upp när visningsprogrammet är öppet, men spelas inte upp när en video är aktiv.

Se [Konfigurera en visningsförinställning för blandad medieuppsättning](setting-mixed-media-set-viewer.md#setting-up-a-mixed-media-set-viewer-preset) och [Skapa och redigera visningsförinställningar](application-setup.md#adding-and-editing-viewer-presets).

## 5. Förhandsgranska en blandad medieuppsättning

Klicka på knappen **[!UICONTROL Preview]** för den blandade medieuppsättningen. Du kan klicka på miniatyrbilds- och färgruteikonerna för att undersöka den blandade medieuppsättningen i visningsprogrammet för den blandade medieuppsättningen. Du kan välja olika visningsprogram från förinställningsmenyerna.

Se [Förhandsgranska en resurs](previewing-asset.md#previewing-an-asset).

## 6. Publicera en blandad medieuppsättning

När du publicerar en uppsättning med blandade media placeras den på Dynamic Media Classic-servrar och URL-strängen aktiveras.

Blandade medieuppsättningar kräver att du publicerar till **videoserver** och även till **bildserver**. Du använder **Videoserver** för att publicera de faktiska videoklipp som du har markerat för publicering. Du kan också använda **bildserver** för att publicera relaterade resurser, till exempel videominiatyrer, och ange information för alla adaptiva videouppsättningar.

Se [Publicera en blandad medieuppsättning](publishing-mixed-media-set.md#publishing-a-mixed-media-set).

## 7. Länka en uppsättning med blandade media till en webbsida

Dynamic Media Classic aktiverar URL-anrop för blandade medieuppsättningar när du har publicerat dem. Du kan kopiera dessa URL:er från förhandsgranskningssidan.

Markera den blandade medieuppsättningen och klicka sedan på **[!UICONTROL Preview]**. Välj en visningsförinställning för blandad medieuppsättning på sidan Förhandsvisa och klicka sedan på **[!UICONTROL Copy URL]**. Se [Länka en blandad medieuppsättning till en webbsida](linking-mixed-media-set-web.md#linking-a-mixed-media-set-to-a-web-page).
