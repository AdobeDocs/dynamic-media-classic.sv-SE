---
title: '"Snabbstart: Grundläggande om mallar"'
seo-title: '"Snabbstart: Grundläggande om mallar"'
description: 'null'
seo-description: En introduktion och snabbstart till mallgrunder som hjälper dig att komma igång snabbt.
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
translation-type: tm+mt
source-git-commit: df0c2897b9fceddde648be53b23e25b13388d6b9
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 0%

---


# Snabbstart: Grundläggande om mallar{#quick-start-template-basics}

Grundläggande mallar skapas och adresseras dynamiskt lageruppbyggda bildfiler som lageruppbyggda filer i bildredigeringsprogram som Adobe Photoshop. Till skillnad från en statisk fil som innehåller lager, till exempel en PSD-fil, kan en mall innehålla parametrar. Med hjälp av parametrar kan de olika delarna av bilden hanteras och anpassas.

En mall kan innehålla valfritt antal bildlager och textlager. Du kan konvertera en statisk fil som innehåller lager, till exempel en PSD-fil med lager, till en mall och skapa mallar i Dynamic Media Classic. Du kan skapa textlager i mallar med teckensnitt som du överfört till SPS. När du har lagt till text i en mall kan du formatera den genom att ändra dess justering, teckensnitt, teckenstorlek och färg.

På skärmen Parametrar kan du konvertera alla delar av en mall till adresserbara parametrar. Om du gör det kan du ändra vilken bild i lager som ska användas eller vilket textvärde som ska användas i mallen. Parametrar skickas med URL-strängen så att du kan ändra alla parametrar för att dynamiskt anpassa svarsbilden som genereras från bildservern.

**Snabbstart**

Den här snabbstarten är utformad för att snabbt komma igång med mallgrunderna.

**1. Överför filerna**

Börja med att överföra PSD-filen eller bildfilen för mallen. Dynamic Media Classic stöder många bildfilformat förutom PSD, men förlustfria TIFF- och PNG-bilder rekommenderas för mallar eftersom de möjliggör genomskinlighet.

Om du använder en PSD-fil för att skapa mallen väljer du alternativet Skapa mall i dialogrutan Alternativ för överföringsjobb när du överför PSD-filen. Välj också ett namngivningsalternativ för lager för att tala om för Dynamic Media Classic hur PSD-lager namnges när de överförs till Scene7 Publishing System.

Om du använder bildfiler kan du beskära bilderna och även skapa en mask från urklippsbanor i bilderna när du överför dem.

Välj knappen Överför i fältet Global navigering om du vill överföra en PSD-fil eller andra bildfiler från datorn till en mapp i SPS. Se [Överföra mallfiler](uploading-template-files.md#uploading_template_files).

**2. Skapa en mall**

Om du vill skapa en mall från en PSD-fil väljer du alternativet Skapa mall när du överför filen. Om du vill skapa en mall från bilder väljer du Bygg > Grundläggande om mallar, anger en bredd- och höjdmätning för arbetsytan, väljer antingen Designer eller Utvecklare och drar bilder till mallskärmen. Du kan också markera bilderna innan du väljer Skapa > Grundläggande om mallar. Skärmen Mallar innehåller verktyg för:

* Lägga till bildlager. Om du vill lägga till ett lager drar du en bild till mallskärmen.
* Lägga till textlager. Välj textverktyget och dra för att rita en ruta för textlagret. formatera texten med verktyg på textskärmen.
* Ändra storlek och position för lager.
* Ändra lagerordningen.
* Använda skugg- och glödeffekter på bild- och textlager.

Se [Skapa en mall](creating-template.md#creating_a_template).

**3. Skapa mallparametrar**

Nästa steg är att parametrisera lageregenskaperna för att avgöra vilka lageregenskaper som ingår i URL-strängen. Med parametrar kan du använda mallar med maximal flexibilitet. När du har gjort en lageregenskap till en parameter kan du ändra den dynamiskt.

Om du vill parametrisera ett lager öppnar du mallen på mallskärmen och väljer knappen Parametrar bredvid ett lagernamn. På skärmen Parametrar väljer du alternativet bredvid varje parameter som du vill lägga till. Se [Skapa mallparametrar](creating-template-parameters.md#creating_template_parameters).

**4. Publiceringsmallar**

När du publicerar mallen placeras den på dynamiska mediabildsservrar så att den kan levereras dynamiskt till din webbplats eller ditt program. När du publicerar aktiveras även URL:en så att mallen anropas från dynamiska mediabildsservrar till din webbplats eller ditt program.

Glöm inte att publicera alla bilder som är kopplade till mallen.

Om du vill publicera en mall markerar du den för publicering och väljer knappen Publicera i fältet Global navigering. Välj sedan knappen Starta publicering. Se [Publiceringsmallar](publishing-templates.md#publishing_templates).

**5. Länka en mall till en webbsida**

Dynamic Media Classic skapar URL:er för mallar och aktiverar URL:er när du publicerar mallar till dynamiska mediabildsservrar. Du kan kopiera de här URL-strängarna från skärmen Förhandsgranska mall.

Markera mallen på panelen Bläddra och klicka på knappen Förhandsgranska för att öppna skärmen Förhandsvisa mall. Välj sedan en bildförinställning för mallen och klicka på knappen Kopiera URL. När du har kopierat URL:en från förhandsgranskningsskärmen kan du använda den på din webbplats eller i ditt program. Se [Länka en mall till en webbsida](linking-template-web-page.md#linking_a_template_to_a_web_page).
