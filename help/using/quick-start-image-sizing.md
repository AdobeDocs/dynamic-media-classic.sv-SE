---
title: "Snabbstart: Bildstorlek"
description: En introduktion och Snabbstart till Bildstorlek som hjälper dig att komma igång snabbt med tekniker för bildstorlek i Adobe Dynamic Media Classic.
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
topic: Content Management
level: Beginner
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 0%

---

# Snabbstart: Bildstorlek{#quick-start-image-sizing}

Bildstorlek avser möjligheten för Adobe Dynamic Media Classic att skapa flera bearbetade bilder baserade på en enda högupplöst bild. I stället för att manuellt skapa flera bilder - t.ex. en miniatyrbild och en förstorad bild - för webbplatsen eller programmet kan du skapa en enda primär bild. Adobe Dynamic Media Classic genererar alla ändrade bilder precis som du vill ha dem. Att kunna leverera bilder dynamiskt från en enda primär bild har många fördelar:

* Du behöver inte skapa flera kopior av bilden manuellt i olika storlekar. Du skickar en primär bild till Adobe Dynamic Media Classic, och Adobe Dynamic Media Classic genererar derivat i olika storlekar från den primära bilden.
* Du kan snabbt ändra storlek på en bildtyp på hela webbplatsen eller i programmet. Om du till exempel vill ändra alla miniatyrbilder kan du ändra bildförinställningen&quot;miniatyrbild&quot;. En bildförinställning, som liknar ett makro, är en samling med storleks- och formateringsattribut. Du kan ändra bildförinställningen &quot;miniatyrbild&quot; om du vill ändra storleken på alla miniatyrbilder på hela webbplatsen eller i programmet.
* Ni behöver inte hantera de primära filerna och alla olika derivat i ert innehålls- eller resurshanteringssystem internt eller externt.

![Du kan skapa flera härledda bilder i olika storlekar från samma högupplösta primära fil.](/help/using/assets/is_derivative_sizes_popup.png)

Se [Bildstorlek: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS) utbildningsvideo.

Följande snabbstart för bildstorlekar är utformad för att hjälpa dig att komma igång snabbt med tekniker för bildstorlek i Adobe Dynamic Media Classic. Följ steg 1-5. Efter varje steg finns det en korsreferens där du kan hitta mer information om det behövs.

## 1. Överför primära bilder

Börja med att ladda upp dina primära bilder till Adobe Dynamic Media Classic. När det gäller storlek rekommenderar Adobe Dynamic Media Classic att du använder bilder som är den största storlek du förväntar dig på din webbplats eller i ditt program. Om du till exempel vill att tittarna ska zooma bilder överför du bilder som är minst 2 000 pixlar stora. Adobe Dynamic Media Classic har stöd för många bildfilsformat, men förlustfria TIFF- och PNG-bilder rekommenderas.

Välj **[!UICONTROL Upload]** för att överföra filer från datorn till en mapp på Adobe Dynamic Media Classic. Se [Överför primära bilder](uploading-master-images.md#uploading_master_images).

## 2. Konfigurera bildförinställningar

Precis som ett makro är en bildförinställning en samling fördefinierade storlekar och formateringskommandon som sparas under ett namn. En bildförinställning styr storleken och formateringen som bilder levereras med från Dynamic Media bildservrar. Om du har företagsadministratörsstatus kan du konfigurera bildförinställningar på egen hand. Adobe Dynamic Media Classic innehåller också standardförinställningar för bilder, och du kan använda dem för att dynamiskt leverera bilder.

Om du vill skapa en bildförinställning (om du är administratör) går du till navigeringsfältet Global **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Image Presets]**. Välj sedan **[!UICONTROL Add]** för att skapa en bildförinställning, eller välja **[!UICONTROL Edit]** om du vill ändra en befintlig bildförinställning.

Den bildförinställning du skapar läggs till på menyn Bildförinställning på sidan Förhandsvisa. Du kan använda den nya bildförinställningen för att visa bilder dynamiskt på webbplatser och i program. Se [Konfigurera bildförinställningar](setting-image-presets.md#setting_up_image_presets).

## 3. Förhandsvisa bildförinställningar

Nästa steg är att förhandsvisa de bildförinställningar som administratören har ställt in med olika förinställda storlekar.

Om du vill utforska förinställningarna går du till **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]** och sedan bläddra till en bildförinställning.

Experimentera med olika bildförinställningar. Ta reda på hur bilden ser ut när den levereras dynamiskt till din webbplats eller ditt program i olika storlekar.

Se [Förhandsvisa en bildresurs baserat på dess bildförinställning](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## 4. Publicera dina primära bilder

Publicera dina primära bildfiler för två viktiga syften:

* Publicera dina primära bilder på Dynamic Media Image Servers så att bilderna dynamiskt kan levereras till din webbplats och tillämpning.
* När du publicerar aktiveras URL-strängarna för att anropa bilder från Dynamic Media Image Servers till din webbplats eller ditt program. Efter publiceringen kan du kopiera och placera de URL-adresser som genererats av Adobe Dynamic Media Classic där det behövs på webbplatsen eller i programmet.

Välj **[!UICONTROL Publish]** för att starta ett publiceringsjobb. I dialogrutan Publicera väljer du **[!UICONTROL Submit Publish]**. Se [Publicera primära bilder](publishing-master-images.md#publishing_master_images).

## 5. Länka URL:er till ditt webbprogram

Adobe Dynamic Media Classic skapar URL-bildtextsträngar för bilder. När du publicerar bilder till Dynamic Media Image Servers (Image-servrar) aktiveras URL:erna. Du kan kopiera dessa URL-strängar från panelen Bläddra (i detaljvyn) eller förhandsgranskningsskärmen. När du har kopierat URL-strängarna kan du använda dem på din webbplats och i dina program. URL:en för bildstorlek ersätter referensen till ett statiskt bildnamn i webbsideskoden. URL:en refererar till ett primärt bildnamn som ersätts av databasen för varje ny bild som ska visas.

URL-strängar som skapas med bildförinställningar innehåller namnet på en bildförinställning. Namnet omges av dollartecken (`$`). Till exempel: `$thumbnail$` kan vara den förinställda bilden som är utformad för att visa primära bilder i miniatyrstorlek. Se [Länka URL:er till ditt webbprogram](linking-urls-web-application.md#linking_urls_to_your_web_application).
