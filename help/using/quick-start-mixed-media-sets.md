---
title: "Snabbstart: Blandad medieuppsättning"
description: En introduktion och snabbstart av blandade medieuppsättningar som hjälper dig att komma igång snabbt i Adobe Dynamic Media Classic.
uuid: 0ef033d5-b053-4d7c-b1e1-1980f899fd88
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
discoiquuid: 2708d077-94fc-4045-8992-ad3589ed9cfd
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 757893ae-7507-42a0-a67b-f6542e7231c7
topic: Content Management
level: Beginner
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 0%

---

# Snabbstart: Blandade medieuppsättningar{#quick-start-mixed-media-sets}

Mixed Media Sets ger användarna en integrerad visningsupplevelse. Blandade medieuppsättningar kan innehålla bilder, bilduppsättningar, färgruteuppsättningar, snurruppsättningar och videoklipp. Användare kan välja olika flikar i visningsprogrammet för blandade media för att se objekten i olika visningsprogram. Om inga flikar har angetts visas alla resurser tillsammans i färgruteraden.

Förinställningar för visningsprogram för blandade media innehåller communityalternativ för slutanvändare som kan bädda in kod, kopiera URL:er och länka till huvudwebbplatsen. Användare kan använda dessa alternativ för att dela information om produkter på sina personliga webbplatser eller sociala nätverksplatser.

Den här snabbstarten för blandade medieuppsättningar är utformad för att du snabbt ska komma igång med blandad medieuppsättning i Adobe Dynamic Media Classic.

## 1. Överför bilder, färgrutefiler och videoklipp

Börja med att ladda upp bilder, färgrutefiler och videoklipp till dina blandade medieuppsättningar. Eftersom användare kan zooma in bilder i visningsprogrammet för den blandade medieuppsättningen måste du ta hänsyn till den möjligheten när du väljer bilder. Se till att bilderna har en största storlek på minst 2 000 pixlar.

Välj **[!UICONTROL Upload]** för att överföra filer från datorn till en mapp på Adobe Dynamic Media Classic.

Se [Överför dina filer](uploading-files.md#uploading-your-files).

## 2. Skapa medieuppsättningar som ska användas i den blandade medieuppsättningen

Du kan lägga till bilder, bilduppsättningar, färgruteuppsättningar, snurruppsättningar och videoklipp i din uppsättning med blandade media. Förbered medieuppsättningarna innan du lägger till dem i den blandade medieuppsättningen.

Se [Skapa en bilduppsättning](creating-image-set.md#creating-an-image-set), [Skapa en färgruteuppsättning](creating-swatch-set.md#creating-a-swatch-set)och [Skapa en snurruppsättning](creating-spin-set.md#creating-a-spin-set).

## 3. Skapa en blandad medieuppsättning

I fältet Global Navigation går du till **[!UICONTROL Build]** > **[!UICONTROL Mixed Media Sets]**. Dra bilder, färgruteuppsättningar, bilduppsättningar och videoklipp till sidan med blandade medieuppsättningar. Om du vill lägga till ett ljudspår drar du en ljudfil till rutan Ljudspår.

Se [Skapa en blandad medieuppsättning](creating-mixed-media-set.md#creating-a-mixed-media-set).

## 4. Konfigurera förinställningar för visningsprogrammet för blandade media

Adobe Dynamic Media Classic levereras med standardförinställningar för visningsprogram för blandade medieuppsättningar. Administratörer kan skapa eller ändra förinställningar för visningsprogrammet för blandad medieuppsättning.

När du konfigurerar en visningsförinställning för blandad medieuppsättning lägger du till visningsförinställningarna för alla andra resurser i uppsättningen. Om din uppsättning med blandade media innehåller videoklipp lägger du till en förinställning för visningsprogrammet för video i förinställningen för visningsprogrammet för blandade media. Du kan också lägga till ett ljudspår i visningsprogrammet. Det här ljudspåret spelas upp när visningsprogrammet är öppet, men spelas inte upp när en video är aktiv.

Se [Konfigurera en visningsförinställning för blandad medieuppsättning](setting-mixed-media-set-viewer.md#setting-up-a-mixed-media-set-viewer-preset) och [Skapa och redigera visningsförinställningar](application-setup.md#adding-and-editing-viewer-presets).

Se även [Förinställningar för visningsprogram](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) utbildningsvideo.

## 5. Förhandsgranska en uppsättning med blandade media

Välj de blandade mediauppsättningarna **[!UICONTROL Preview]** -knappen. Du kan välja miniatyrbilds- och färgruteikoner för att undersöka den blandade medieuppsättningen i visningsprogrammet för den blandade medieuppsättningen. Du kan välja olika visningsprogram från förinställningsmenyerna.

Se [Förhandsgranska en resurs](previewing-asset.md#previewing-an-asset).

## 6. Publicera en blandad medieuppsättning

När du publicerar en blandad medieuppsättning placeras den på Adobe Dynamic Media Classic-servrar och URL-strängen aktiveras.

Blandade medieuppsättningar kräver att du publicerar till **Videoserver** och även **Bildserver**. Du använder **Videoserver** för att publicera de faktiska videoklipp du har markerat för publicering. Och du använder **Bildserver** för att publicera relaterade resurser, till exempel videominiatyrbilder, och ange information för alla adaptiva videouppsättningar.

Se [Publicera en blandad medieuppsättning](publishing-mixed-media-set.md#publishing-a-mixed-media-set).

## 7. Länka en blandad medieuppsättning till en webbsida

Adobe Dynamic Media Classic aktiverar URL-anrop för blandade medieuppsättningar när du har publicerat dem. Du kan kopiera dessa URL:er från förhandsgranskningssidan.

Markera den blandade medieuppsättningen och välj sedan **[!UICONTROL Preview]**. Välj en visningsförinställning för blandad medieuppsättning på förhandsgranskningssidan och välj sedan en **[!UICONTROL Copy URL]**. Se [Länka en blandad medieuppsättning till en webbsida](linking-mixed-media-set-web.md#linking-a-mixed-media-set-to-a-web-page).
