---
title: 'Snabbstart: Bilduppsättningar'
description: En introduktion och Snabbstart till bilduppsättningar som hjälper dig att komma igång snabbt med hjälp av Image Set-tekniker i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
topic: Content Management
level: Beginner
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Snabbstart: Bilduppsättningar{#quick-start-image-sets}

Adobe Dynamic Media Classic Image Sets ger användarna en integrerad visningsupplevelse. I visningsprogrammet för den dynamiska bilduppsättningen kan användarna se olika vyer av ett objekt genom att välja en miniatyrbild. Med bilduppsättningar kan du visa alternativa högupplösta vyer av ett objekt.

I Image Set Viewer finns zoomningsverktyg som gör att du kan undersöka bilder noggrant. Om du vill kan du göra guidade zoommål och bildscheman till en del av din bilduppsättning. Bilduppsättningar ger en mer samordnad och intimt tittarupplevelse.

Se [Bild- och snurruppsättningar: utbildningsvideon för Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/556_Image%20&%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS).

När du skapar en bilduppsättning rekommenderar Adobe följande metodtips och tillämpar följande begränsningar:

| Begränsningstyp | Bästa praxis | Begränsning har införts |
| --- | --- | --- |
| Antal dubblettresurser per uppsättning | Inga dubbletter | 20‡ |
| Maximalt antal bilder per uppsättning | 5-10 bilder per uppsättning | 1000 |

‡ Bästa praxis är att inte ha duplicerade resurser i en uppsättning. Gränsen är 20 kopior för en enskild resurs. Om du lägger till ytterligare en dubblett för den resursen, inom den uppsättningen, returnerar begäran ett fel eller ignorerar dubbletten.

Se även [Dynamiska mediebegränsningar](/help/using/limitations.md).

Följande snabbstart för bilduppsättningar är utformat för att du snabbt ska komma igång med hjälp av Image Set-tekniker i Adobe Dynamic Media Classic.

## &#x200B;1. Överför dina primära bilder för flera vyer och färgrutor

Börja med att ladda upp bilderna för dina bilduppsättningar. Eftersom användare kan zooma in på bilder i bilduppsättningsvisningsprogrammet måste du ta hänsyn till den här möjligheten när du väljer bilder. Se till att bilderna har en största storlek på minst 2 000 pixlar. Adobe Dynamic Media Classic har stöd för många bildfilsformat, men förlustfria TIFF-, PNG- och EPS-bilder rekommenderas.

I fältet Global navigering väljer du **[!UICONTROL Upload]** om du vill överföra filer från datorn till en mapp på Adobe Dynamic Media Classic.

Se [Förbered bilduppsättningsresurser för överföring](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) och [Överför filer](uploading-files.md#uploading-your-files).

## &#x200B;2. Skapa en bilduppsättning

I Bilduppsättningar väljer användare miniatyrbilder i Bilduppsättningsvisningsprogrammet för att visa en bild från en annan sida eller vinkel.

Om du vill skapa en bilduppsättning väljer du **[!UICONTROL Build]** i fältet Global navigering och sedan **[!UICONTROL Image Sets]**. I fönstret Bilduppsättning drar du bilderna till sidan för att komponera bilduppsättningen. Ordna, lägg till och ta bort bilder efter behov.

Se [Skapa en bilduppsättning](creating-image-set.md#creating-an-image-set).

Se även [Inkludera zoommål och bildscheman i bilduppsättningar](/help/using/including-zoom-targets-image-maps-image-sets.md)

## &#x200B;3. Förbered visningsförinställningar för bilduppsättning efter behov

Administratörer kan skapa eller ändra förinställningar för bildspelsvisningsprogrammet. Adobe Dynamic Media Classic levereras med standardförinställningar för visningsprogram för varje multimedietyp. Använd zoomvisningsprogrammet: **[!UICONTROL Custom]** > **[!UICONTROL Images]** eller **[!UICONTROL Image Sets]**/**[!UICONTROL Multiple Views]** förinställningar för att visa dina bilduppsättningar.

Du kan lägga till eller redigera visningsprogramförinställningar på skärmen Programinställningar.

Se [Skapa och redigera visningsförinställningar](application-setup.md#adding-and-editing-viewer-presets).

## &#x200B;4. Förhandsvisa en bilduppsättning

Markera bilduppsättningen på panelen Bläddra och välj sedan **[!UICONTROL Preview]**. På sidan Förhandsvisa väljer du miniatyrbildikonerna för att undersöka bilduppsättningen i det valda visningsprogrammet. Du kan välja olika visningsprogram på menyn Förinställningar.

Se [Förhandsgranska en resurs](previewing-asset.md#previewing-an-asset).

## &#x200B;5. Publicera en bilduppsättning

När du publicerar en bilduppsättning placeras den på Adobe Dynamic Media Classic-servrar och URL-strängen aktiveras.

>[!NOTE]
>
>Det här steget är inte nödvändigt om du valde **[!UICONTROL Publish after a save]** (standard) när du skapade och sparade bilduppsättningen.

Välj ikonen **[!UICONTROL Mark for Publish]** till vänster om namnet på panelen Bläddra. Välj sedan **[!UICONTROL Publish]**. Välj **[!UICONTROL Submit Publish]** på publiceringssidan.

Se [Publicera filer](publishing-files.md#publishing-files).

## &#x200B;6. Länka en bilduppsättning till din webbplats

Adobe Dynamic Media Classic skapar URL-anrop för bilduppsättningar och aktiverar dem när du har publicerat dem. Du kan kopiera dessa URL:er från förhandsgranskningsskärmen.

Markera bilduppsättningen och välj sedan **[!UICONTROL Preview]**. Välj nu en förinställning för bilduppsättningsvisningsprogrammet och klicka sedan på knappen **[!UICONTROL Copy URL]**.

Se [Länka bilduppsättningen till en webbsida](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page).
