---
title: '"Snabbstart: Zooma"'
description: En introduktion och Snabbstart till zoom som hjälper dig att komma igång snabbt.
uuid: 31eda632-3469-4f90-885b-e90c6a2e5e75
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 559c986d-313d-46df-a5ff-0b49316ad3a7
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: eae35207-000c-4ced-b9ab-714c2384a9e7
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 0%

---

# Snabbstart: Zooma{#quick-start-zoom}

Med zoomning kan du interaktivt visa högupplösta detaljer i bilder. Du kan till exempel se färger, alternativ, vinklar och detaljer i en bild i ett dynamiskt, fullständigt konfigurerbart, integrerat visningsprogram. Det här visningsprogrammet kan bäddas in på en webbsida eller visas i ett popup-fönster. Du kan granska bilder i nära intervall och panorera bilder i hög upplösning för att noggrant granska dem. Zoomning ger kunderna en engagerande, informativ och interaktiv tittarupplevelse.

Adobe Dynamic Media Classic erbjuder även guidad zoomning, ett sätt att framhäva viktiga funktioner i en bild. Om du till exempel vill fokusera tittarnas uppmärksamhet på en logotyp kan du skapa ett zoommål för logotypen. När tittarna klickar på det här zoommålet zoomas de till logotypen.

Alla zoombilder skapas och hanteras av enstaka överordnad bilder, grafik och databasdrivna attribut. Zoomning i Adobe Dynamic Media Classic minskar tiden och kostnaden för att producera och leverera bilder avsevärt. Du kan använda zoomningsvisningsprogram för att zooma in och ut i bilder. Zoomvisningsprogrammet har knappar som du kan klicka på för att zooma och panorera. Du kan också panorera genom att dra på skärmen. Med förinställningarna för Zoom Viewer kan du konfigurera zoomningsvisningsprogrammet där du zoomar bilder.

Snabbstart för zoomning är utformat för att komma igång snabbt med zoomtekniker i Adobe Dynamic Media Classic. Följ steg 1 till 6. Efter varje steg finns en korsreferens till en ämnesrubrik där du kan hitta mer information.

## 1. Överför zoombilder

Börja med att överföra dina zoombilder till Adobe Dynamic Media Classic. För optimal zoomning rekommenderar Adobe Dynamic Media Classic att bilderna har minst 2 000 pixlar i den längsta storleken.

Klicka på **[!UICONTROL Upload]** i fältet Global navigering för att överföra bilder från datorn eller nätverket till en mapp på Adobe Dynamic Media Classic. Se [Överföra zoombilder](uploading-zoom-images.md#uploading_zoom_images).

## 2. Skapa zoommål för guidad zoomning

Zoommål är ett sätt för dig att markera specifika delar av en bild. Du kan till exempel rikta uppmärksamheten mot de delar av en bild som gör den unik eller distinkt. I zoomvisningsfönstret visas zoommål i form av miniatyrbilder på bildens sida. Om du väljer en av dessa zoommålminiatyrer zoomas automatiskt en del av bilden som du anger.

Om du vill skapa ett zoommål klickar du på **[!UICONTROL Edit]** och väljer Zoommål. Du kan också öppna en bild i panelen Bläddra i detaljvyn och klicka på **[!UICONTROL Zoom Targets]**. Använd sedan zoomverktygen på sidan Zoommålredigerare så att du kan isolera en del av bilden som ett mål. Se [Skapa zoommål för guidad zoomning](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).

## 3. Konfigurera förinställningar för Zoom Viewer

Förinställningarna för zoomvisningsprogrammet bestämmer hur zoomningsvisningsprogrammen ska se ut och fungera. Om du är administratör kan du konfigurera förinställningar för zoomvisningsprogrammet. Adobe Dynamic Media Classic innehåller även förinställningar för zoomvisning som är standard.

Om du vill skapa en förinställning för zoomvisningsprogrammet klickar du på **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]** i fältet Global navigering. Klicka på **[!UICONTROL Add]** på sidan Visningsförinställningar, välj en plattform och ett zoomvisningsprogram och klicka sedan på **[!UICONTROL Add]**. Välj sedan alternativ på sidan Konfigurera visningsprogram.

I Adobe Dynamic Media Classic finns **[!UICONTROL Zoom Viewer Preset]** alternativ som gör att du kan välja knappstil och visningsprogrammets utseende. Du kan också anpassa zoominställningarna för webbplatsen. Se [Konfigurera förinställningar för zoomvisningsprogrammet](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## 4. Förhandsgranska bilder med Zoomvisningsprogrammet

Du kan förhandsvisa bilder i ett zoomvisningsprogram för att se vad zoomupplevelsen är när bilder zoomas.

Om du vill utforska olika förinställningar för zoomvisning och hur de visar zoomupplevelsen markerar du en bild i panelen Bläddra och klickar på **[!UICONTROL Preview]**. Klicka på **[!UICONTROL Presets]** > **[!UICONTROL Zoom]** och välj sedan en förinställning med zoommenyerna.

Zoomknappar visas. Du kan se hur zoombilderna ser ut på webbplatsen. Klicka på zoomknapparna (och zoomverktygen) så att du kan testa inställningarna för den förinställning för Zoomvisning som du har valt. Se [Förhandsvisa bilder med olika zoomningsvisningsprogram](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

## 5. Publicera zoombilder

När du publicerar dina zoombilder placeras de på Dynamic Media bildservrar så att de kan levereras till din webbplats och tillämpning. Som en del av publiceringsprocessen aktiverar Adobe Dynamic Media Classic URL-strängar. Dessa URL-strängar anropar zoombilder från Dynamic Media Image Servers till din webbplats eller ditt program.

Klicka på **[!UICONTROL Publish]** i fältet Global navigering. Klicka på **[!UICONTROL Submit Publish]** i dialogrutan Publicera. Se [Publicera zoombilder](publishing-zoom-images.md#publishing_zoom_images).

## 6. Länka zoomningsvisningsprogram till webbsidan

Adobe Dynamic Media Classic skapar de URL-bildtextsträngar som behövs för att zooma bilder och aktiverar dem när du publicerar bilder på Dynamic Media bildservrar. Du kan kopiera dessa URL-strängar från sidan **[!UICONTROL Preview]**. När du har kopierat URL-strängarna är de tillgängliga för dina webbplatser och program. Se [Länka zoomningsvisningsprogram till din webbsida](linking-zoom-viewers-web-pages.md#linking_zoom_viewers_to_your_web_pages).
