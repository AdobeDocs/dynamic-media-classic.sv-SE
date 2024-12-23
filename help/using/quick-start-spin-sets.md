---
title: 'Snabbstart: Snurra uppsättningar'
description: En introduktion och Snabb start till snurra uppsättning som hjälper dig att komma igång snabbt i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
topic: Content Management
level: Beginner
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 0%

---

# Snabbstart: Snurra uppsättningar{#quick-start-spin-sets}

Med en snurra uppsättning kan du simulera hur det ser ut när du vrider ett objekt för att undersöka det. Med snurra uppsättningar kan du visa objekt från vilken vinkel som helst och få fram viktiga visuella detaljer från vilken vinkel som helst. Med en snurra uppsättning simuleras en 360-graders visningsupplevelse. Adobe Dynamic Media Classic erbjuder endimensionella snurruppsättningar där tittarna kan rotera ett objekt och tvådimensionella snurruppsättningar där tittarna kan rotera och vända objektet. Dessutom kan man zooma och panorera med ett par musklick. På så sätt kan användare undersöka ett objekt närmare från en viss betraktningsvinkel.

![Bilder för en snurruppsättning.](/help/using/assets/spin_set.png)

Du kan även använda snurruppsättningar för bildscheman. En bildschema är ett område i en bild i den snurrande uppsättningen som visar en överrullningspanel med text. När användaren väljer en bildschema utlöses en åtgärd av något slag. En webbsida startas till exempel så att användaren kan lära sig mer om en produkt. Om du vill peka ut en bildschema i en snurruppsättning visas en kontur runt själva bildschemat när användaren flyttar muspekaren över den.

Se [Skapa bildscheman](creating-image-maps.md).

Se [Bild- och snurruppsättningar: utbildningsvideon Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS).

När du skapar en snurrsuppsättning rekommenderar Adobe följande bästa praxis och tillämpar följande begränsningar:

| Begränsningstyp för snurra uppsättning | Bästa praxis | Begränsning har införts |
| --- | --- | --- |
| Maximalt antal rader/kolumner per 2D-uppsättning | 12-18 bilder per uppsättning | 1000 |

Se även [Dynamic Media-begränsningar](/help/using/limitations.md).

Snabbstart för den här snurruppsättningen är utformad för att du snabbt ska komma igång med Spin Set-teknik i Adobe Dynamic Media Classic. Följ steg 1 till 7. I slutet av varje steg kan du välja en ämneslänk och lära dig mer.

## 1. Skapa och överföra bilderna

Du behöver minst 8-12 tagningar av ett objekt för en endimensionell snurra och 16-24 för en tvådimensionell snurra uppsättning. Fotografierna måste tas med jämna mellanrum för att ge intryck av att objektet roteras och vändas. Om en endimensionell snurra t.ex. innehåller 12 tagningar roterar du objektet 30° (360/12) för varje tagning.

I fältet Global navigering väljer du **[!UICONTROL Upload]** om du vill överföra snurrbilder från datorn eller nätverket till Adobe Dynamic Media Classic.

Se [Riktlinjer för fotografering av snurrbilder](creating-spin-set.md#guidelines-for-shooting-spin-set-images).

## 2. Skapa en snurruppsättning

Om du vill skapa en snurruppsättning går du till **[!UICONTROL Build]** > **[!UICONTROL Spin Sets]** i fältet Global navigering. I dialogrutan Ange storlek för snurra väljer du hur många rader och celler du vill ha och väljer **[!UICONTROL OK]**. Dra sedan bilderna till rutnätet på sidan Snurra uppsättning.

Se [Skapa en snurruppsättning](creating-spin-set.md#creating-a-spin-set).

## 3. Redigera en snurruppsättning

Om du vill redigera en snurruppsättning går du till **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]** i fältet Global navigering. Välj en snurruppsättning och välj sedan **[!UICONTROL Edit]**. Lägg till, ta bort och ändra placeringen av bilder. Du kan ändra radplaceringen i tvådimensionella snurruppsättningar.

Se [Redigera en snurruppsättning](creating-spin-set.md#editing-a-spin-set).

## 4. Konfigurera förinställningar för Snurra uppsättning för visningsprogram

Administratörer kan skapa förinställningar för Snurra uppsättning för visningsprogram. De här förinställningarna bestämmer hur visningsprogrammet för snurra uppsättning ser ut. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]** om du vill konfigurera en ny visningsförinställning för rotationsuppsättning i fältet Global navigering.

Välj **[!UICONTROL Add]** på sidan Visningsförinställningar, välj **[!UICONTROL Spin Set Viewer]** i listrutan och välj sedan **[!UICONTROL Add]**. Välj alternativ på sidan `Configure Viewer` och välj sedan **[!UICONTROL Save]**.

Se [Ställ in förinställningar för Rotation av uppsättning för visningsprogram](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets).

## 5. Förhandsgranska en snurruppsättning

Välj din snurruppsättning på panelen Bläddra och välj sedan **[!UICONTROL Preview]**. Håll ned musknappen på förhandsgranskningssidan och dra pekaren åt vänster eller höger för att se objektet&quot;snurra&quot; visuellt.

Se [Förhandsgranska en snurruppsättning](previewing-spin-set.md#previewing-a-spin-set).

## 6. Publish a Spin Set

När du publicerar en snurruppsättning placeras den på Adobe Dynamic Media Classic-servrar så att den kan levereras dynamiskt till din webbplats eller ditt program. Den aktiverar även URL-strängen som anropar den nya uppsättningen från Dynamic Media Image Servers till din webbplats eller ditt program.

Om du vill publicera en snurruppsättning markerar du den för publicering genom att markera ikonen **[!UICONTROL Mark for Publish]** bredvid namnet på bläddringspanelen. Välj **[!UICONTROL Publish]** i fältet Global navigering för att initiera en publicering. Välj **[!UICONTROL Submit Publish]** på publiceringssidan.

Se [Publish a Spin Set](publishing-spin-set.md#publishing-a-spin-set).

## 7. Länka en snurruppsättning till en webbsida

Adobe Dynamic Media Classic skapar URL-bildtextsträngar för Spin Sets och aktiverar dem när du har publicerat dem. Du kan kopiera dessa URL:er från förhandsgranskningssidan.

Markera rotationsuppsättningen och välj sedan **[!UICONTROL Preview]**. Välj en förinställning för Snurra uppsättning för visning. Välj sedan **[!UICONTROL Copy URL]**.

Se [Länka en snurruppsättning till en webbsida](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page).
