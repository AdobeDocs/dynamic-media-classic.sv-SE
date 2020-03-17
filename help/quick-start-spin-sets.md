---
title: '"Snabbstart: Snurra uppsättningar"'
seo-title: '"Snabbstart: Snurra uppsättningar"'
description: 'null'
seo-description: En introduktion och Snabb start till snurra uppsättning som hjälper dig att komma igång snabbt.
uuid: d0af9db6-cb6f-48f0-89f6-f3ab2da0659f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 282b8e83-b20f-43f7-b9f8-6eebd5b1c5a7
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Snabbstart: Snurra uppsättningar{#quick-start-spin-sets}

Med en snurra uppsättning kan du simulera hur det ser ut när du vrider ett objekt för att undersöka det. Med snurra uppsättningar kan du visa objekt från vilken vinkel som helst och få fram de viktigaste visuella detaljerna från vilken vinkel som helst. Med en snurra uppsättning simuleras en 360-graders visningsupplevelse. Dynamic Media Classic erbjuder endimensionella snurpuppsättningar där tittarna kan rotera ett objekt och tvådimensionella snurpuppar där tittarna kan rotera och vända objektet. Dessutom kan man zooma och panorera med några enkla musklick. På så sätt kan användare undersöka ett objekt närmare från en viss betraktningsvinkel.

![Bilder för en snurra uppsättning.](/help/assets/spin_set.png)

Du kan även använda snurruppsättningar för bildscheman. En bildschema är ett område i en bild i den snurrande uppsättningen som visar en överrullningspanel med text. När användaren klickar på en bildschema utlöses en åtgärd av något slag. En webbsida startas till exempel så att användaren kan lära sig mer om en produkt. Om du vill rikta uppmärksamheten mot användningen av ett bildschema i en snurruppsättning, visas en kontur runt själva bildschemat när användaren flyttar muspekaren över den.

Se [Skapa bildscheman](creating-image-maps.md).

**Snabbstart**

Snabbstart för den här snurruppsättningen är utformad för att komma igång snabbt med Spin Set-teknik i Dynamic Media Classic. Följ steg 1 till 7. I slutet av varje steg finns en korsreferens till en ämnesrubrik där du kan hitta mer information om det behövs.

**1. Skapa och överföra bilder**

Du behöver minst 8-12 tagningar av ett objekt för en endimensionell snurra och 16-24 för en tvådimensionell snurra uppsättning. Fotografierna måste tas med jämna mellanrum för att ge intryck av att objektet roteras och vändas. Om en endimensionell snurra t.ex. innehåller 12 tagningar roterar du objektet 30 grader (360/12) för varje tagning.

Välj knappen Överför i fältet Global Navigation (Global Navigation) om du vill överföra snurrbilder från datorn eller nätverket till Scene7 Publishing System.

Se [Riktlinjer för fotografering av snurra uppsättningsbilder](creating-spin-set.md#guidelines-for-shooting-spin-set-images).

**2. Skapa en snurruppsättning**

Om du vill skapa en snurrsuppsättning klickar du på knappen Skapa och väljer Snurra uppsättningar. Välj hur många rader och celler du vill ha i dialogrutan Ange storlek för snurra och klicka sedan på OK. Dra sedan bilder till rutnätet på skärmen för snurra uppsättning.

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

**3. Redigera en snurra uppsättning**

Om du vill redigera en snurruppsättning väljer du knappen Redigera överrullning. Skärmen med snurra uppsättning öppnas. Lägg till, ta bort och ändra placeringen av bilder. Du kan ändra placeringen av rader i tvådimensionella snurruppsättningar.

Se [Redigera en snurruppsättning](creating-spin-set.md#editing-a-spin-set).

**4. Konfigurera förinställningar för Snurra uppsättningar för visningsprogram**

Administratörer kan skapa förinställningar för Snurra uppsättning för visningsprogram. De här förinställningarna bestämmer hur visningsprogrammet för snurra uppsättning ser ut. Om du vill konfigurera en ny förinställning för Snurra uppsättning för visningsprogram väljer du knappen Inställningar i fältet Global navigering. Visa programinställningsalternativ på skärmen Konfigurera och välj sedan Visningsförinställningar.

På skärmen Förinställningar för visningsprogram väljer du menyn Lägg till och väljer Snurra uppsättning för visningsprogram i dialogrutan Lägg till visningsförinställning. Välj sedan alternativ på skärmen Konfigurera visningsprogram.

Se [Ställa in visningsförinställningar för](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets)snurra uppsättningar.

**5. Förhandsgranska en snurra uppsättning**

Markera din snurruppsättning på panelen Bläddra och klicka på knappen Förhandsvisa överrullning. Håll ned musknappen på förhandsgranskningsskärmen och dra pekaren åt vänster eller höger för att visuellt&quot;snurra&quot; objektet.

Se [Förhandsvisa en snurra](previewing-spin-set.md#previewing-a-spin-set).

**6. Publicera en snurruppsättning**

När du publicerar en snurruppsättning placeras den på Dynamic Media Classic-servrar så att den kan levereras dynamiskt till din webbplats eller ditt program. Den aktiverar även URL-strängen som anropar den snurra uppsättningen från dynamiska mediabildsservrar till din webbplats eller ditt program.

Om du vill publicera en snurruppsättning markerar du den för publicering genom att markera ikonen **Markera för publicering** bredvid namnet på bläddringspanelen. Klicka på **Publicera** i fältet Global navigering för att starta en publicering. På skärmen Publicera klickar du på **Starta publicering**.

Se [Publicera en snurruppsättning](publishing-spin-set.md#publishing-a-spin-set).

**7. Länka en snurruppsättning till en webbsida**

Dynamic Media Classic skapar URL-bildtextssträngar för snurruppsättningar och aktiverar dem när du har publicerat dem. Du kan kopiera dessa URL:er från förhandsgranskningsskärmen.

Markera rotationsuppsättningen och klicka sedan på **Förhandsgranska**. Förhandsgranskningsskärmen öppnas. Välj en förinställning för Snurra uppsättning för visningsprogram. Klicka sedan på **Kopiera URL**.

Se [Länka en snurruppsättning till en webbsida](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page).
