---
title: 'Snabbstart: Blandad medieuppsättning'
description: En introduktion och snabbstart av blandade medieuppsättningar som hjälper dig att komma igång snabbt i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 757893ae-7507-42a0-a67b-f6542e7231c7
topic: Content Management
level: Beginner
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Snabbstart: Blandade medieuppsättningar{#quick-start-mixed-media-sets}

Mixed Media Sets ger användarna en integrerad visningsupplevelse. Blandade medieuppsättningar kan innehålla bilder, bilduppsättningar, färgruteuppsättningar, snurruppsättningar och videoklipp. Användare kan välja olika flikar i visningsprogrammet för blandade media för att se objekten i olika visningsprogram. Om inga flikar har angetts visas alla resurser tillsammans i färgruteraden.

Förinställningar för visningsprogram för blandad media innehåller communityalternativ för slutanvändare så att de kan bädda in kod, kopiera URL:er och länka till huvudwebbplatsen. Användare kan använda dessa alternativ för att dela information om produkter på sina egna webbplatser eller sociala nätverk.

Den här snabbstarten för blandade medieuppsättningar är utformad för att du snabbt ska komma igång med blandad medieuppsättning i Adobe Dynamic Media Classic.

## &#x200B;1. Överför bilder, färgrutefiler och videofilmer

Börja med att ladda upp bilder, färgrutefiler och videoklipp till dina blandade medieuppsättningar. Eftersom användare kan zooma in bilder i visningsprogrammet för den blandade medieuppsättningen måste du ta hänsyn till den möjligheten när du väljer bilder. Se till att bilderna har en största storlek på minst 2 000 pixlar.

I fältet Global navigering väljer du **[!UICONTROL Upload]** om du vill överföra filer från datorn till en mapp på Adobe Dynamic Media Classic.

Se [Överför filer](uploading-files.md#uploading-your-files).

## &#x200B;2. Skapa medieuppsättningar för användning i den blandade medieuppsättningen

Du kan lägga till bilder, bilduppsättningar, färgruteuppsättningar, snurruppsättningar och videoklipp i den blandade medieuppsättningen. Förbered medieuppsättningarna innan du lägger till dem i den blandade medieuppsättningen.

Se [Skapa en bilduppsättning](creating-image-set.md#creating-an-image-set), [Skapa en färgruteuppsättning](creating-swatch-set.md#creating-a-swatch-set) och [Skapa en snurruppsättning](creating-spin-set.md#creating-a-spin-set).

## &#x200B;3. Skapa en blandad medieuppsättning

Gå till **[!UICONTROL Build]** > **[!UICONTROL Mixed Media Sets]** i fältet Global navigering. Dra bilder, färgruteuppsättningar, bilduppsättningar och videofilmer till sidan med blandade medieuppsättningar. Om du vill lägga till ett ljudspår drar du en ljudfil till rutan Ljudspår.

Se [Skapa en blandad medieuppsättning](creating-mixed-media-set.md#creating-a-mixed-media-set).

## &#x200B;4. Konfigurera förinställningar för blandad medievisning

Adobe Dynamic Media Classic levereras med standardförinställningar för visningsprogram för blandade medieuppsättningar. Administratörer kan skapa eller ändra visningsförinställningar för blandad medieuppsättning.

När du konfigurerar en visningsförinställning för en blandad medieuppsättning lägger du till visningsförinställningarna för alla andra resurser i uppsättningen. Om din uppsättning med blandade media till exempel innehåller videoklipp lägger du till en visningsförinställning för Videovisning i visningsförinställningen för den blandade medieuppsättningen. Du kan också lägga till ett ljudspår i visningsprogrammet. Det här ljudspåret spelas upp när visningsprogrammet är öppet, men spelas inte upp när en video är aktiv.

Se [Konfigurera en visningsförinställning för en blandad medieuppsättning](setting-mixed-media-set-viewer.md#setting-up-a-mixed-media-set-viewer-preset) och [Skapa och redigera visningsförinställningar](application-setup.md#adding-and-editing-viewer-presets).

Se även utbildningsvideon [Visningsförinställningar](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS).

## &#x200B;5. Förhandsgranska en uppsättning med blandade media

Välj knappen **[!UICONTROL Preview]** för den blandade medieuppsättningen. Du kan välja miniatyrbilds- och färgruteikoner för att undersöka den blandade medieuppsättningen i visningsprogrammet för den blandade medieuppsättningen. Du kan välja olika visningsprogram från förinställningsmenyerna.

Se [Förhandsgranska en resurs](previewing-asset.md#previewing-an-asset).

## &#x200B;6. Publicera en blandad medieuppsättning

När du publicerar en blandad medieuppsättning placeras den på Adobe Dynamic Media Classic-servrar och URL-strängen aktiveras.

Blandade medieuppsättningar kräver att du publicerar till **videoservern** och även till **bildservern**. Använd **videoservern** för att publicera de faktiska videoklippen som du har markerat för publicering. Och du använder **bildservern** för att publicera relaterade resurser, till exempel videominiatyrer, och ange information för alla adaptiva videouppsättningar.

Se [Publicera en blandad medieuppsättning](publishing-mixed-media-set.md#publishing-a-mixed-media-set).

## &#x200B;7. Länka en blandad medieuppsättning till en webbsida

Adobe Dynamic Media Classic aktiverar URL-anrop för blandade medieuppsättningar när du har publicerat dem. Du kan kopiera dessa URL:er från förhandsgranskningssidan.

Markera den blandade medieuppsättningen och välj sedan **[!UICONTROL Preview]**. Välj en visningsförinställning för blandad medieuppsättning på förhandsgranskningssidan och välj sedan **[!UICONTROL Copy URL]**. Se [Länka blandade medieuppsättningar till webbsidor](linking-mixed-media-set-web.md#linking-a-mixed-media-set-to-a-web-page).
