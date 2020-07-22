---
title: '"Snabbstart: Bildstorlek"'
seo-title: '"Snabbstart: Bildstorlek"'
description: 'null'
seo-description: En introduktion och Snabbstart till Bildstorlek som hjälper dig att komma igång snabbt med tekniker för bildstorlek.
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 0%

---


# Snabbstart: Bildstorlek{#quick-start-image-sizing}

Bildstorlek avser möjligheten för Dynamic Media Classic att skapa flera bearbetade bilder baserade på en enda högupplöst bild. I stället för att manuellt skapa flera bilder - t.ex. en miniatyrbild och en förstorad bild - för webbplatsen eller programmet kan du skapa en enda överordnad bild. I Dynamic Media Classic skapas alla ändrade bilder precis som du vill ha dem. Att kunna leverera bilder dynamiskt från en enda överordnad bild har många fördelar:

* Du behöver inte skapa flera kopior av bilden manuellt i olika storlekar. Om du anger en överordnad bild för Dynamic Media Classic genereras varianter från den överordnad bilden i Dynamic Media Classic.
* Du kan snabbt ändra storlek på en bildtyp på hela webbplatsen eller i programmet. Om du till exempel vill ändra alla miniatyrbilder kan du ändra bildförinställningen&quot;miniatyrbild&quot;. En bildförinställning, som liknar ett makro, är en samling med storleks- och formateringsattribut. Du kan ändra bildförinställningen &quot;miniatyrbild&quot; om du vill ändra storleken på alla miniatyrbilder på hela webbplatsen eller i programmet.
* Ni behöver inte hantera mallarna och alla olika derivat i ert innehålls- eller resurshanteringssystem internt eller externt.

![Du kan skapa flera variantbilder med olika storlek från samma högupplösta överordnad fil.](/help/assets/is_derivative_sizes_popup.png)

**Snabbstart**

Den här snabbstarten för bildstorlek är utformad för att hjälpa dig att komma igång snabbt med hjälp av tekniker för bildstorlek i Dynamic Media Classic. Följ steg 1-5. Efter varje steg finns en korsreferens där du kan hitta mer information om det behövs.

**1. Överför överordnad bilder**

Börja med att överföra dina överordnad bilder till Dynamic Media Classic. När det gäller storlek rekommenderar Dynamic Media Classic att du använder bilder med den största storlek som du förväntar dig på din webbplats eller i ditt program. Om du till exempel vill att tittarna ska zooma bilder överför du bilder som är minst 2 000 pixlar i den största dimensionen. Dynamic Media Classic stöder många bildfilsformat, men förlustfria TIFF- och PNG-bilder rekommenderas.

Klicka på knappen Överför i fältet Global navigering om du vill överföra filer från datorn till en mapp i Dynamic Media Classic. Se [Överföra överordnad bilder](uploading-master-images.md#uploading_master_images).

**2. Konfigurera bildförinställningar**

Precis som ett makro är en bildförinställning en samling fördefinierade storlekar och formateringskommandon som sparas under ett namn. En bildförinställning styr storleken och formateringen som bilder levereras med från Dynamic Media bildservrar. Om du har företagsadministratörsstatus kan du konfigurera bildförinställningar på egen hand. Dynamic Media Classic innehåller även standardförinställningar för bilder, och du kan använda dem för att dynamiskt leverera bilder.

Om du vill skapa en bildförinställning (om du är administratör) väljer du Konfigurera > Programinställningar. Visa programinställningsalternativen på skärmen Konfigurera och välj Bildförinställningar. Klicka sedan på **Lägg till** eller **Redigera** för att skapa en bildförinställning.

Den bildförinställning du skapar läggs till på menyn Bildförinställning på förhandsvisningsskärmen. Du kan använda den nya bildförinställningen för att visa bilder dynamiskt på webbplatser och i program. Se [Konfigurera bildförinställningar](setting-image-presets.md#setting_up_image_presets).

**3. Förhandsgranska förinställningar**

Nästa steg är att förhandsvisa de bildförinställningar som administratören har ställt in med olika förinställda storlekar.

Om du vill utforska bildförinställningar klickar du på **Inställningar** > **Bildförinställningar** och bläddrar sedan till en bildförinställning.

Experimentera med olika bildförinställningar. Ta reda på hur bilden ser ut när den levereras dynamiskt till din webbplats eller ditt program i olika storlekar.

Se [Förhandsvisa en bildresurs baserat på bildförinställningen](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

**4. Publicera dina överordnad bilder**

Publicera dina överordnad bildfiler i två viktiga syften:

* Publicera dina överordnad bilder på Dynamic Media Image Servers så att bilderna dynamiskt kan levereras till din webbplats och ditt program.
* När du publicerar aktiveras URL-strängarna för att anropa bilder från Dynamic Media Image Servers till din webbplats eller ditt program. Efter publiceringen kan du kopiera och placera de Dynamic Media Classic-genererade URL:erna där det behövs på webbplatsen eller i programmet.

Välj knappen Publicera i fältet Global navigering när du vill initiera en publicering. Välj knappen Starta publicering på skärmen Publicera. Se [Publicera överordnad bilder](publishing-master-images.md#publishing_master_images).

**5. Länka URL:er till webbprogrammet**

Dynamic Media Classic skapar URL-bildtextsträngar för bilder. När du publicerar bilder till Dynamic Media Image Servers (-bildservrar) aktiveras URL:erna. Du kan kopiera dessa URL-strängar från panelen Bläddra (i detaljvyn) eller förhandsgranskningsskärmen. När du har kopierat URL-strängarna kan du använda dem på din webbplats och i dina program. URL:en för bildstorlek ersätter referensen till ett statiskt bildnamn i webbsideskoden. URL:en refererar till ett överordnad bildnamn som ersätts av databasen för varje ny bild som ska visas.

URL-strängar som skapas med bildförinställningar innehåller namnet på en bildförinställning. Namnet omges av dollartecken (`$`). Du kan till exempel `$thumbnail$` använda bildförinställningen som är utformad för att visa överordnad bilder i miniatyrstorlek. Se [Länka URL:er till ditt webbprogram](linking-urls-web-application.md#linking_urls_to_your_web_application).
