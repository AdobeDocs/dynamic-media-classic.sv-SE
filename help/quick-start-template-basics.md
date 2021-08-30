---
title: '"Snabbstart: Grundläggande om mallar"'
description: En introduktion och snabbstart till mallgrunder som hjälper dig att komma igång snabbt i Adobe Dynamic Media Classic.
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
source-git-commit: 36f9aa3c2b4dc66e4cb851c2ce6837ae0ad4f64c
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 0%

---

# Snabbstart: Grundläggande om mallar{#quick-start-template-basics}

Mallgrunder skapas dynamiskt och adresserbara bildfiler i lager, som lageruppbyggda filer i bildredigeringsprogram som Adobe Photoshop. Till skillnad från en statisk fil som innehåller lager, till exempel en PSD-fil, kan en mall innehålla parametrar. Med hjälp av parametrar kan de olika delarna av bilden hanteras och anpassas.

En mall kan innehålla valfritt antal bildlager och textlager. Du kan konvertera en statisk fil som innehåller lager, till exempel en PSD-fil med lager, till en mall och skapa mallar i Adobe Dynamic Media Classic. Du kan skapa textlager i mallar med teckensnitt som du överfört till Adobe Dynamic Media Classic. När du har lagt till text i en mall kan du formatera den genom att ändra dess justering, teckensnitt, teckenstorlek och färg.

På sidan Parametrar kan du konvertera alla delar av en mall till adresserbara parametrar. Om du gör det kan du ändra vilken bild i lager som ska användas eller vilket textvärde som ska användas i mallen. Parametrar skickas med URL-strängen så att du kan ändra alla parametrar för att dynamiskt anpassa svarsbilden som genereras från bildservern.

Den här snabbstarten är utformad för att snabbt komma igång med mallgrunderna.

## 1. Överför filerna

Börja med att överföra PSD-filen eller bildfilen för mallen. Adobe Dynamic Media Classic stöder många bildfilsformat förutom PSD, men förlustfria TIFF- och PNG-bilder rekommenderas för mallar eftersom de möjliggör genomskinlighet.

Om du använder en PSD-fil för att skapa mallen väljer du **[!UICONTROL Create Template]** i dialogrutan **[!UICONTROL Upload Job Options]** när du överför PSD-filen. Välj också ett **[!UICONTROL Layer Naming]**-alternativ så att Adobe Dynamic Media Classic kan namnge PSD-lager när de överförs till Adobe Dynamic Media Classic.

Om du använder bildfiler kan du beskära bilderna och även skapa en mask från urklippsbanor i bilderna när du överför dem.

I det globala navigeringsfältet väljer du **[!UICONTROL Upload]** om du vill överföra en PSD-fil eller andra bildfiler från datorn till en mapp på Adobe Dynamic Media Classic. Se [Överför mallfiler](uploading-template-files.md#uploading_template_files).

## 2. Skapa en mall

Om du vill skapa en mall från en PSD-fil väljer du **[!UICONTROL Create Template]** när du överför filen. Om du vill skapa en mall från bilder går du till **[!UICONTROL Build]** > **[!UICONTROL Template Basics]** i fältet Global navigering och anger mått för bredd och höjd för arbetsytan. I det övre högra hörnet av sidan väljer du antingen **[!UICONTROL Designer]** eller **[!UICONTROL Developer]** och drar bilder till mallsidan. Du kan också markera bilderna *innan* du går till **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**. På mallsidan finns verktyg för:

* Lägga till bildlager. Om du vill lägga till ett lager drar du en bild till mallsidan.
* Lägga till textlager. Välj ikonen **[!UICONTROL Text tool]**. Dra pekaren för att skapa en ruta för textlagret; formatera texten med verktyg på textsidan.
* Ändra storlek och position för lager.
* Ändra lagerordningen.
* Använda skugg- och glödeffekter på bild- och textlager.

Se [Skapa en mall](creating-template.md#creating_a_template).

## 3. Skapa mallparametrar

Nästa steg är att parametrisera lageregenskaperna för att avgöra vilka lageregenskaper som ingår i URL-strängen. Med parametrar kan du använda mallar med maximal flexibilitet. När du har gjort en lageregenskap till en parameter kan du ändra den dynamiskt.

Om du vill parametrisera ett lager öppnar du mallen på mallsidan och väljer sedan **[!UICONTROL Parameters]** bredvid ett lagernamn. På sidan Parametrar väljer du alternativet bredvid varje parameter som du vill lägga till. Se [Skapa mallparametrar](creating-template-parameters.md#creating_template_parameters).

## 4. Publiceringsmallar

När du publicerar mallen placeras den på Dynamic Media Image-servrar så att den kan levereras dynamiskt till din webbplats eller ditt program. När du publicerar aktiveras även URL:en så att mallen anropas från Dynamic Media Image Servers till din webbplats eller ditt program.

Glöm inte att publicera alla bilder som är kopplade till mallen.

Om du vill publicera en mall markerar du den för publicering och väljer **[!UICONTROL Publish]** i fältet Global navigering. Välj sedan **[!UICONTROL Submit Publish]**. Se [Publicera mallar](publishing-templates.md#publishing_templates).

## 5. Länka en mall till en webbsida

Dynamic Media Classic skapar URL:er för mallar och aktiverar URL:er när du publicerar mallar på Dynamic Media Image Servers. Du kan kopiera dessa URL-strängar från sidan Förhandsvisa mall.

Markera mallen i panelen Bläddra och välj sedan **[!UICONTROL Preview]** för att öppna sidan Mallförhandsvisning. Välj en bildförinställning för mallen och välj sedan **[!UICONTROL Copy URL]**. När du har kopierat URL-adressen från förhandsgranskningssidan kan du använda den på din webbplats eller i ditt program. Se [Länka en mall till en webbsida](linking-template-web-page.md#linking_a_template_to_a_web_page).
