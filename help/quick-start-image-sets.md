---
title: '"Snabbstart: Bilduppsättningar"'
description: En introduktion och Snabbstart till bilduppsättningar som hjälper dig att komma igång snabbt med hjälp av Image Set-tekniker i Adobe Dynamic Media Classic.
uuid: daf17d13-9c06-41f0-8fc5-2e56d460d341
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 612a425f-2840-46c4-8e5a-c0bc5f738f4e
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
source-git-commit: 92a28b7868e03802f4ef1c113ec3f8b34f57ed56
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# Snabbstart: Bilduppsättningar{#quick-start-image-sets}

Adobe Dynamic Media Classic Image Sets ger användarna en integrerad visningsupplevelse. I visningsprogrammet för den dynamiska bilduppsättningen kan användare visa olika vyer av ett objekt genom att klicka på en miniatyrbild. Med bilduppsättningar kan du visa alternativa högupplösta vyer av ett objekt.

I Image Set Viewer finns zoomningsverktyg som gör att du kan undersöka bilder noggrant. Om du vill kan du göra guidade zoommål och bildscheman till en del av din bilduppsättning. Bilduppsättningar ger en mer samordnad och intimt tittarupplevelse.

Se [Bild- och snurruppsättningar: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) utbildningsvideo.

När du skapar en bilduppsättning rekommenderar Adobe följande metodtips och tillämpar följande begränsningar:

| Begränsningstyp | Bästa praxis | Begränsning har införts |
| --- | --- | --- |
| Antal dubblettresurser per uppsättning | Inga dubbletter | 20 |
| Maximalt antal bilder per uppsättning | 5-10 bilder per uppsättning | 1000 |

Se även [Dynamic Media begränsningar](/help/limitations.md).

Följande snabbstart för bilduppsättningar är utformat för att du snabbt ska komma igång med hjälp av Image Set-tekniker i Adobe Dynamic Media Classic.

## 1. Överför dina primära bilder för flera vyer och färgrutor

Börja med att ladda upp bilderna för dina bilduppsättningar. Eftersom användare kan zooma in på bilder i bilduppsättningsvisningsprogrammet måste du ta hänsyn till den här möjligheten när du väljer bilder. Se till att bilderna har en största storlek på minst 2 000 pixlar. Adobe Dynamic Media Classic har stöd för många bildfilsformat, men förlustfria bilder i TIFF, PNG och EPS rekommenderas.

Välj **[!UICONTROL Upload]** för att överföra filer från datorn till en mapp på Adobe Dynamic Media Classic.

Se [Förbered bilduppsättningsresurser för överföring](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) och [Överför dina filer](uploading-files.md#uploading-your-files).

## 2. Skapa en bilduppsättning

I Bilduppsättningar väljer användare miniatyrbilder i Bilduppsättningsvisningsprogrammet för att visa en bild från en annan sida eller vinkel.

Om du vill skapa en bilduppsättning väljer du **[!UICONTROL Build]** väljer du **[!UICONTROL Image Sets]**. I fönstret Bilduppsättning drar du bilderna till sidan för att komponera bilduppsättningen. Ordna, lägg till och ta bort bilder efter behov.

Se [Skapa en bilduppsättning](creating-image-set.md#creating-an-image-set).

Se även [Inkludera zoommål och bildscheman i bilduppsättningar](/help/including-zoom-targets-image-maps-image-sets.md)

## 3. Förbered bilduppsättningen med visningsförinställningar efter behov

Administratörer kan skapa eller ändra förinställningar för bildspelsvisningsprogrammet. Adobe Dynamic Media Classic levereras med standardförinställningar för visningsprogram för varje multimedietyp. Använda Zoomvisningsprogrammet: **[!UICONTROL Custom]** > **[!UICONTROL Images]** eller **[!UICONTROL Image Sets]**/**[!UICONTROL Multiple Views]** förinställningar för att visa dina bilduppsättningar.

Du kan lägga till eller redigera visningsprogramförinställningar på skärmen Programinställningar.

Se [Skapa och redigera visningsförinställningar](application-setup.md#adding-and-editing-viewer-presets).

## 4. Förhandsvisa en bilduppsättning

Markera bilduppsättningen i panelen Bläddra och välj sedan **[!UICONTROL Preview]**. På sidan Förhandsvisa väljer du miniatyrbildikonerna för att undersöka bilduppsättningen i det valda visningsprogrammet. Du kan välja olika visningsprogram på menyn Förinställningar.

Se [Förhandsgranska en resurs](previewing-asset.md#previewing-an-asset).

## 5. Publicera en bilduppsättning

När du publicerar en bilduppsättning placeras den på Adobe Dynamic Media Classic-servrar och URL-strängen aktiveras.

>[!NOTE]
>
>Detta steg är inte nödvändigt om du har valt **[!UICONTROL Publish after save]** (standard) när du skapade och sparade bilduppsättningen.

Välj **[!UICONTROL Mark for Publish]** till vänster om namnet på panelen Bläddra. Välj sedan **[!UICONTROL Publish]**. På sidan Publicera väljer du **[!UICONTROL Submit Publish]**.

Se [Publicera filer](publishing-files.md#publishing-files).

## 6. Länka en bilduppsättning till din webbplats

Adobe Dynamic Media Classic skapar URL-anrop för bilduppsättningar och aktiverar dem när du har publicerat dem. Du kan kopiera dessa URL:er från förhandsgranskningsskärmen.

Markera bilduppsättningen och välj sedan **[!UICONTROL Preview]**. Välj nu en förinställning för bilduppsättningsvisningsprogrammet och välj sedan **[!UICONTROL Copy URL]**.

Se [Länka en bilduppsättning till en webbsida](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page).
