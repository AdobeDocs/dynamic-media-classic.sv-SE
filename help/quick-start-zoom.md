---
title: '"Snabbstart: Zooma"'
seo-title: '"Snabbstart: Zooma"'
description: 'null'
seo-description: En introduktion och Snabbstart till zoom som hjälper dig att komma igång snabbt.
uuid: 31eda632-3469-4f90-885b-e90c6a2e5e75
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 559c986d-313d-46df-a5ff-0b49316ad3a7
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Snabbstart: Zooma{#quick-start-zoom}

Med zoomning kan du interaktivt visa högupplösta detaljer i bilder. Du kan till exempel se färger, alternativ, vinklar och detaljer i en bild i ett dynamiskt, fullständigt konfigurerbart, integrerat visningsprogram. Det här visningsprogrammet kan bäddas in på en webbsida eller visas i ett popup-fönster. Du kan granska bilder i nära intervall och panorera bilder i hög upplösning för att noggrant undersöka dem. Zoomning ger kunderna en engagerande, informativ och interaktiv tittarupplevelse.

Dynamic Media Classic erbjuder även guidad zoomning, ett sätt att framhäva viktiga funktioner i en bild. Om du till exempel vill fokusera tittarnas uppmärksamhet på en logotyp kan du skapa ett zoommål för logotypen. När tittarna klickar på det här zoommålet zoomas de till logotypen.

Alla zoombilder skapas och hanteras från en mallbild, grafik och databasdrivna attribut. Dynamic Media Classic-zoomning minskar tiden och kostnaden för att producera och leverera bilder avsevärt. Du kan använda zoomningsvisningsprogram för att zooma in och ut i bilder. Zoomvisningsprogrammet har knappar som du kan klicka på för att zooma och panorera. Du kan också panorera genom att dra på skärmen. Med förinställningarna för Zoom Viewer kan du konfigurera zoomningsvisningsprogrammet där du zoomar bilder.

**Snabbstart**

Den här snabbstarten för zoomning är utformad för att komma igång snabbt med zoomtekniker i Dynamic Media Classic. Följ steg 1 till 6. Efter varje steg finns en korsreferens till en ämnesrubrik där du kan hitta mer information.

**1. Överför zoombilder**

Börja med att ladda upp dina zoombilder till Scene7 Publishing System. För optimal zoomning rekommenderar Dynamic Media Classic att bilderna har minst 2 000 pixlar i det längsta måttet.

Välj knappen Överför i fältet Global Navigation (Global Navigation) om du vill överföra bilder från datorn eller nätverket till en mapp i Scene7 Publishing System. Se [Överföra zoombilder](uploading-zoom-images.md#uploading_zoom_images).

**2. Skapa zoommål för guidad zoomning**

Zoommål är ett sätt för dig att markera specifika delar av en bild. Du kan till exempel rikta uppmärksamheten mot de delar av en bild som gör den unik eller distinkt. I zoomvisningsfönstret visas zoommål i form av miniatyrbilder på bildens sida. Om du väljer en av dessa zoommålminiatyrer zoomas automatiskt en del av bilden som du anger.

Om du vill skapa ett zoommål klickar du på knappen Redigera överrullning och väljer Zoommål. Du kan också öppna en bild i panelen Bläddra i detaljvyn och klicka på Zoommål. Använd sedan zoomverktygen i zoommålredigeraren för att isolera en del av bilden som ett mål. Se [Skapa zoommål för guidad zoomning](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).

**3. Konfigurera förinställningar för Zoom Viewer**

Förinställningarna för zoomvisningsprogrammet bestämmer hur zoomningsvisningsprogrammen ska se ut och fungera. Om du är administratör kan du konfigurera förinställningar för zoomvisningsprogrammet. Dynamic Media Classic innehåller även förinställningar för zoomningsvisningsprogrammet som är standard.

Om du vill skapa en förinställning för zoomvisningsprogrammet klickar du på knappen Inställningar i det globala navigeringsfältet och väljer Visningsförinställningar. Klicka sedan på knappen Lägg till på skärmen för visningsförinställningar, välj en plattform, välj en zoomningsvisare och klicka på Lägg till. Välj sedan alternativ på skärmen Konfigurera visningsprogram.

I Dynamic Media Classic finns förinställningsalternativ för Zoom Viewer som gör att du kan välja knappstil och visningsprogrammets utseende. Du kan också anpassa zoominställningarna för webbplatsen. Se [Ställa in förinställningar](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets)för zoomvisningsprogrammet.

**4. Förhandsgranska bilder med Zoomvisningsprogrammet**

Du kan förhandsvisa bilder i ett zoomvisningsprogram för att se vad zoomupplevelsen är när bilder zoomas.

Om du vill utforska olika förinställningar för zoomvisning och hur de visar zoomupplevelsen markerar du en bild i panelen Bläddra och klickar på knappen Förhandsvisa. Förhandsgranskningsskärmen öppnas. Välj Förinställningar > Zooma och sedan en förinställning med zoommenyerna.

Zoomknappar visas. Du kan se hur zoombilderna ser ut på webbplatsen. Välj zoomknapparna (och zoommålen) för att testa inställningarna för den förinställning för Zoomvisningsprogram som du har valt. Se [Förhandsvisa bilder med olika zoomvisningsprogram](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

**5. Publicera zoombilder**

När du publicerar dina zoombilder placeras de på dynamiska mediabildsservrar så att de kan levereras till din webbplats och ditt program. Som en del av publiceringsprocessen aktiverar Scene7 Publishing System URL-strängar. Dessa URL-strängar anropar zoombilder från dynamiska mediabildsservrar till din webbplats eller ditt program.

Välj knappen Publicera i fältet Global navigering när du vill initiera en publicering. Välj knappen Starta publicering på skärmen Publicera. Se [Publicera zoombilder](publishing-zoom-images.md#publishing_zoom_images).

**6. Länka zoomningsvisningsprogram till webbsidan**

Dynamic Media Classic skapar de URL-bildtextsträngar som behövs för att zooma bilder och aktiverar dem när du publicerar bilder på dynamiska mediabildsservrar. Du kan kopiera dessa URL-strängar från förhandsgranskningsskärmen. När du har kopierat URL-strängarna är de tillgängliga för dina webbplatser och program. Se [Länka zoomvisningsprogram till webbsidan](linking-zoom-viewers-web-pages.md#linking_zoom_viewers_to_your_web_pages).