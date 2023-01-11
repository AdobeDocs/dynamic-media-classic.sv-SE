---
title: Arbeta med PSD-filer
description: Lär dig hur du arbetar med PSD-filer i Adobe Dynamic Media Classic.
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
source-git-commit: dc1ec666b208cec8fffe836d64ed501f6ccf4e7b
workflow-type: tm+mt
source-wordcount: '940'
ht-degree: 0%

---

# Arbeta med PSD-filer{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages. -->

PSD (Photoshop Document Files) används oftast i Adobe Dynamic Media Classic för att skapa mallar. När du överför en PSD-fil kan du skapa en Adobe Dynamic Media Classic-mall automatiskt från filen (välj alternativet Skapa mall på överföringsskärmen).

Adobe Dynamic Media Classic skapar flera bilder från en PSD-fil med lager om du använder filen för att skapa en mall. skapas en bild för varje lager.

## Överföringsalternativ för PSD {#psd-upload-options}

Alternativ för att överföra PSD-filer finns under Photoshop-alternativ i dialogrutan Alternativ för överföringsjobb. Du kan beskära en fil, välja en färgprofil för den, använda den för att skapa en mall och välja en ankarpunkt.

De här alternativen är tillgängliga när du överför PSD-filer:

* **Beskärningsalternativ** - Finns under **[!UICONTROL Crop Options]**. Välj **[!UICONTROL Trim]** att automatiskt beskära tomrum från kanterna av en PSD-fil, välj **[!UICONTROL Manual]** för att beskära sidor av filen PSD:

   * **[!UICONTROL Trim]** - Välj **[!UICONTROL Trim Away Based On]** och väljer **[!UICONTROL Color]** eller **[!UICONTROL Transparency]**.
   Om du väljer **[!UICONTROL Color]** väljer du menyn Hörn och väljer hörnet på PSD med den färg som bäst motsvarar den tomrumsfärg som du vill beskära.

   Dra skjutreglaget för att ange en tolerans mellan 0 och 1. Om du vill trimma baserat på färg anger du 0 för att beskära pixlar endast om de exakt matchar färgen som du markerade i hörnet av PSD. Nummer som ligger närmare 1 ger större färgskillnader. Om du vill trimma baserat på genomskinlighet anger du 0 för att beskära pixlar endast om de är genomskinliga. siffror närmare 1 ger större genomskinlighet.

   * **[!UICONTROL Manual]** - Ange antalet pixlar att beskära från en sida eller från varje sida av bilden. Hur mycket av bilden som beskärs beror på bildfilens ppi-inställning (pixlar per tum). Om bilden till exempel visar 150 ppi och du anger 75 i textrutorna Överkant, Höger, Underkant och Vänster, 0,5 tum. beskärs från varje sida av bilden.


* **Alternativ för färgprofil** - Finns under **[!UICONTROL Color Profile Options]**.

   * **[!UICONTROL Default Color Preservation]**

   * **[!UICONTROL Keep Original Color Space]** - Behåller bildens ursprungliga färgrymd.

   * **[!UICONTROL Custom From]** > **[!UICONTROL To]** - Öppnar menyer så att du kan välja färgmodellen Konvertera från och Konvertera till. Du kan välja en standardfärgmodell för Photoshop eller en färgmodell som du har överfört till Adobe Dynamic Media Classic. Se [ICC-profiler](/help/icc-profiles.md).

* **Photoshop-alternativ**

   * **[!UICONTROL Maintain Layers]** - Rippar lagren i PSD, om det finns några, till enskilda resurser. Resurslagren förblir kopplade till PSD. Du kan visa dem genom att öppna filen PSD i detaljvyn och välja lagerpanelen. Se Visa och redigera lager i en PSD-fil.

   * **[!UICONTROL Create Template]** - Skapar en mall från lagren i filen PSD.

   * **[!UICONTROL Extract Text]** - Extraherar texten så att användare kan söka efter text i ett visningsprogram.

   * **[!UICONTROL Extend Layers To Background Size]** - Utökar storleken på överlappade bildlager till storleken på bakgrundslagret.

   * **[!UICONTROL Layer Naming]** - Lager i filen PSD överförs som separata bilder. Om du vill namnge bilderna i Adobe Dynamic Media Classic väljer du bland följande alternativ:

      * **[!UICONTROL Layer Name]** - Namnger bilderna efter deras lagernamn i filen PSD. Ett lager med namnet Price Tag i den ursprungliga PSD-filen blir till exempel en bild med namnet Price Tag. Om lagernamnen i filen PSD är Photoshop standardlagernamn (Bakgrund, Lager 1, Lager 2 och så vidare) får bilderna namn efter sina lagernummer i filen PSD. <!-- not their default layer names -->

      * **[!UICONTROL Photoshop and layer number]** - Namnger bilderna efter deras lagernummer i filen PSD och ignorerar de ursprungliga lagernamnen. Bilderna får samma namn som Photoshop-filnamnet och ett nummer i det tillagda lagret. Det andra lagret i en fil med namnet `Spring Ad.psd` är namngiven `Spring Ad_2` även om det har ett icke-standardnamn i Photoshop.

      * **[!UICONTROL Photoshop and layer name]** - Namnger bilderna efter PSD-filen följt av lagernamnet eller lagernumret. Lagernumret används om lagernamnen i filen PSD är Photoshop standardlagernamn. Ett lager med namnet `Price Tag` i en PSD-fil med namnet `SpringAd` är namngiven `Spring Ad_Price Tag`. Ett lager med standardnamnet Lager2 anropas `Spring Ad_2`.
   * **[!UICONTROL Anchor]** - Ange hur bilder är förankrade i mallar som genereras från lagerkompositionen som skapas från filen PSD. Som standard är ankarpunkten i mitten. Med en central ankarpunkt kan ersättningsbilder bäst fylla samma område, oavsett ersättningsbildens proportioner. Bilder med en annan aspekt som ersätter den här bilden upptar i själva verket samma utrymme när de refererar till mallen och använder parameterersättning. Ändra till en annan inställning om ditt program kräver att ersättningsbilderna fyller ut det tilldelade utrymmet i mallen.


## Visa och redigera lager i en PSD-fil {#viewing-and-editing-layers-in-a-psd-file}

Om du valde alternativet Behåll lager när du överförde PSD, delade Adobe Dynamic Media Classic bort de enskilda lagren i resurser. Du kan visa och redigera de objektlager som tillhör en PSD-fil genom att öppna filen i panelen Bläddra i detaljvyn.

>[!NOTE]
>
>Adobe Dynamic Media Classic har stöd för upp till fem nivåer i en kapslad lagergrupp.

1. Dubbelklicka på den fullständiga PSD-filen på panelen Bläddra. Filen öppnas i detaljvyn.

   >[!NOTE]
   >
   >Se till att du öppnar hela resursen och inte ett av PSD-lagren.

1. Välj **[!UICONTROL Layers]**. Alla lager visas som separata bilder på panelen Lager.
1. Dubbelklicka på ett lager och gör något av följande:

   * Om du vill skapa ett bildschema på lagret väljer du **[!UICONTROL Image Map]** ikon. (Se [Skapa bildscheman](creating-image-maps.md#creating_image_maps).)
   * Om du vill skapa zoommål på lagret väljer du **[!UICONTROL Zoom Targets]** ikon. (Se [Skapa zoommål för guidad zoomning](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Beskär lagret genom att markera **[!UICONTROL Crop]** ikon. (Se [Beskära en bild](cropping-image.md#cropping_an_image).)
   * Om du vill öka skärpan i lagret markerar du **[!UICONTROL Sharpen]**. (Se [Öka skärpan i en bild](sharpening-image.md#sharpening_an_image).)
   * Justera lagret genom att markera **[!UICONTROL Adjust]**. (Se [Justera en bild](adjusting-image.md#adjusting_an_image).)

1. Välj **[!UICONTROL Save]** eller **[!UICONTROL Save As]**.
1. Om du vill visa eller redigera ett annat lager väljer du en pil längst ned i förhandsgranskningen av lagret.
1. Om du vill stänga lagerdetaljvyn väljer du **[!UICONTROL Grid View]** ikon.
