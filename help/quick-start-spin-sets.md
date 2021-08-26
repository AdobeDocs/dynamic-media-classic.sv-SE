---
title: '"Snabbstart: Snurra uppsättningar"'
description: En introduktion och Snabb start till snurra uppsättning som hjälper dig att komma igång snabbt.
uuid: d0af9db6-cb6f-48f0-89f6-f3ab2da0659f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 282b8e83-b20f-43f7-b9f8-6eebd5b1c5a7
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 0%

---

# Snabbstart: Snurra uppsättningar{#quick-start-spin-sets}

Med en snurra uppsättning kan du simulera hur det ser ut när du vrider ett objekt för att undersöka det. Med snurra uppsättningar kan du visa objekt från vilken vinkel som helst och få fram de viktigaste visuella detaljerna från vilken vinkel som helst. Med en snurra uppsättning simuleras en 360-graders visningsupplevelse. Adobe Dynamic Media Classic har endimensionella snurruppsättningar där visningsprogram kan rotera ett objekt och tvådimensionella snurpuppar där visningsprogram kan rotera och vända objektet. Dessutom kan man zooma och panorera med några enkla musklick. På så sätt kan användare undersöka ett objekt närmare från en viss betraktningsvinkel.

![Bilder för en snurra uppsättning.](/help/assets/spin_set.png)

Du kan även använda snurruppsättningar för bildscheman. En bildschema är ett område i en bild i den snurrande uppsättningen som visar en överrullningspanel med text. När användaren klickar på en bildschema utlöses en åtgärd av något slag. En webbsida startas till exempel så att användaren kan lära sig mer om en produkt. Om du vill peka ut ett bildschema i en snurruppsättning visas en kontur runt själva bildschemat när användaren flyttar muspekaren över den.

Se [Skapa bildscheman](creating-image-maps.md).

Snabbstart för den här snurruppsättningen är utformad för att komma igång snabbt med Spin Set-teknik i Adobe Dynamic Media Classic. Följ steg 1 till 7. I slutet av varje steg kan du klicka på en ämneslänk om du vill veta mer.

## 1. Skapa och överföra bilder

Du behöver minst 8-12 tagningar av ett objekt för en endimensionell snurra och 16-24 för en tvådimensionell snurra uppsättning. Fotografierna måste tas med jämna mellanrum för att ge intryck av att objektet roteras och vändas. Om en endimensionell snurra t.ex. innehåller 12 tagningar roterar du objektet 30° (360/12) för varje tagning.

Klicka på **[!UICONTROL Upload]** i fältet Global navigering för att överföra snurrbilder från datorn eller nätverket till Adobe Dynamic Media Classic.

Se [Riktlinjer för fotografering av uppsättningsbilder för snurra](creating-spin-set.md#guidelines-for-shooting-spin-set-images).

## 2. Skapa en snurruppsättning

Om du vill skapa en snurruppsättning klickar du på **[!UICONTROL Build]** > **[!UICONTROL Spin Sets]** i fältet Global navigering. Välj hur många rader och celler du vill ha i dialogrutan Ange storlek för snurra och klicka sedan på **[!UICONTROL OK]**. Dra sedan bilderna till rutnätet på sidan Snurra uppsättning.

Se [Skapa en snurruppsättning](creating-spin-set.md#creating-a-spin-set).

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>See <a href="#UnresolvedLink-sc7_spinsets_sp.xml#WS98ca2e6790647c06-245331fc135ab744793-8000">Including Image Maps in Spin Sets</a> to add clickable, hotspot regions, known as Image Maps, to images in a Spin Set. </p>

 -->

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>See also <a href="#UnresolvedLink-sc7_spinsets_sp.xml#WS98ca2e6790647c06229f600f135ab7cc461-8000">Managing InfoPanel content</a>.</p>

 -->

## 3. Redigera en snurra uppsättning

Om du vill redigera en snurruppsättning klickar du på **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]** i fältet Global navigering. Välj en snurra och klicka sedan på **[!UICONTROL Edit]**. Lägg till, ta bort och ändra placeringen av bilder. Du kan ändra placeringen av rader i tvådimensionella snurruppsättningar.

Se [Redigera en snurruppsättning](creating-spin-set.md#editing-a-spin-set).

## 4. Konfigurera förinställningar för Snurra uppsättningar för visningsprogram

Administratörer kan skapa förinställningar för Snurra uppsättning för visningsprogram. De här förinställningarna bestämmer hur visningsprogrammet för snurra uppsättning ser ut. Om du vill konfigurera en ny förinställning för Snurra uppsättning för visningsprogram klickar du på **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]** i fältet Global navigering.

Klicka på **[!UICONTROL Add]** på sidan Visningsförinställningar, välj **[!UICONTROL Spin Set Viewer]** i listrutan och klicka sedan på **[!UICONTROL Add]**. Välj alternativ på sidan Konfigurera visningsprogram och klicka sedan på **[!UICONTROL Save]**.

Se [Konfigurera förinställningar för Snurra uppsättning för visningsprogram](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets).

## 5. Förhandsgranska en snurra uppsättning

Välj din snurruppsättning på panelen Bläddra och klicka sedan på **[!UICONTROL Preview]**. Håll ned musknappen på förhandsgranskningssidan och dra pekaren åt vänster eller höger för att se objektet&quot;snurra&quot; visuellt.

Se [Förhandsgranska en snurruppsättning](previewing-spin-set.md#previewing-a-spin-set).

## 6. Publicera en snurruppsättning

När du publicerar en snurruppsättning placeras den på Adobe Dynamic Media Classic-servrar så att den kan levereras dynamiskt till din webbplats eller ditt program. Den aktiverar även URL-strängen som anropar den nya uppsättningen från Dynamic Media Image-servrar till din webbplats eller ditt program.

Om du vill publicera en snurruppsättning markerar du den för publicering genom att markera ikonen **[!UICONTROL Mark for Publish]** bredvid namnet på panelen Bläddra. Klicka på **[!UICONTROL Publish]** i fältet Global navigering för att starta en publicering. Klicka på **[!UICONTROL Submit Publish]** på skärmen Publicera.

Se [Publicera en snurruppsättning](publishing-spin-set.md#publishing-a-spin-set).

## 7. Länka en snurruppsättning till en webbsida

Adobe Dynamic Media Classic skapar URL-bildtextssträngar för snurruppsättningar och aktiverar dem när du har publicerat dem. Du kan kopiera dessa URL:er från förhandsgranskningssidan.

Markera rotationsuppsättningen och klicka sedan på **[!UICONTROL Preview]**. Välj en förinställning för Snurra uppsättning för visningsprogram. Klicka sedan på **[!UICONTROL Copy URL]**.

Se [Länka en snurruppsättning till en webbsida](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page).
