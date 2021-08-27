---
title: Arbeta med PSD-filer
description: Lär dig hur du arbetar med PSD-filer i Adobe Dynamic Media Classic.
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# Arbeta med PSD-filer{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages. -->

PSD (Photoshop Document Files) används oftast i Adobe Dynamic Media Classic för att skapa mallar. När du överför en PSD-fil kan du skapa en Adobe Dynamic Media Classic-mall automatiskt från filen (välj alternativet Skapa mall på överföringsskärmen).

Adobe Dynamic Media Classic skapar flera bilder från en PSD-fil med lager om du använder filen för att skapa en mall; skapas en bild för varje lager.

## PSD-överföringsalternativ {#psd-upload-options}

Alternativ för överföring av PSD-filer finns under Photoshop-alternativ i dialogrutan Alternativ för överföringsjobb. Du kan beskära en fil, välja en färgprofil för den, använda den för att skapa en mall och välja en ankarpunkt.

Dessa alternativ är tillgängliga när du överför PSD-filer:

* **Beskärningsalternativ**  - finns under  **[!UICONTROL Crop Options]**. Välj **[!UICONTROL Trim]** om du automatiskt vill beskära tomt utrymme från kanterna i en PSD-fil; välj **[!UICONTROL Manual]** för att beskära sidor av PSD-filen:

   * **[!UICONTROL Trim]** - Markera  **[!UICONTROL Trim Away Based On]** menyn och välj  **[!UICONTROL Color]** eller  **[!UICONTROL Transparency]**.

      Om du väljer alternativet **[!UICONTROL Color]** väljer du menyn Hörn och väljer hörnet på PSD-filen med den färg som bäst motsvarar den tomrumsfärg som du vill beskära.

      Dra skjutreglaget för att ange en tolerans mellan 0 och 1. Om du vill trimma baserat på färg anger du 0 för att beskära pixlar endast om de exakt matchar den färg som du valde i hörnet av PSD:n. Nummer som ligger närmare 1 ger större färgskillnader. Om du vill trimma baserat på genomskinlighet anger du 0 för att beskära pixlar endast om de är genomskinliga. siffror närmare 1 ger större genomskinlighet.

   * **[!UICONTROL Manual]** - Ange antalet pixlar att beskära från en sida eller från varje sida av bilden. Hur mycket av bilden som beskärs beror på bildfilens ppi-inställning (pixlar per tum). Om bilden till exempel visar 150 ppi och du anger 75 i textrutorna Överkant, Höger, Underkant och Vänster beskärs en halv tum från varje sida av bilden.

* **Alternativ**  för färgprofil - finns under  **[!UICONTROL Color Profile Options]**.

   * **[!UICONTROL Default Color Preservation]**

   * **[!UICONTROL Keep Original Color Space]** - Behåller bildens ursprungliga färgrymd.

   * **[!UICONTROL Custom From]** >  **[!UICONTROL To]** - Öppnar menyer så att du kan välja färgmodellen Konvertera från och Konvertera till. Du kan välja en standardfärgmodell för Photoshop eller en färgmodell som du har överfört till Adobe Dynamic Media Classic. Se [ICC-profiler](/help/icc-profiles.md).

* **Photoshop-alternativ**

   * **[!UICONTROL Maintain Layers]** - Rippar lagren i PSD-filen, om sådana finns, till enskilda resurser. Resurslagren förblir kopplade till PSD-filen. Du kan visa dem genom att öppna PSD-filen i detaljvyn och välja lagerpanelen. Se Visa och redigera lager i en PSD-fil.

   * **[!UICONTROL Create Template]** - Skapar en mall från lagren i PSD-filen.

   * **[!UICONTROL Extract Text]** - Extraherar texten så att användare kan söka efter text i ett visningsprogram.

   * **[!UICONTROL Extend Layers To Background Size]** - Utökar storleken på överlappade bildlager till storleken på bakgrundslagret.

   * **[!UICONTROL Layer Naming]** - Lager i PSD-filen överförs som separata bilder. Om du vill namnge bilderna i Adobe Dynamic Media Classic väljer du bland följande alternativ:

      * **[!UICONTROL Layer Name]** - Namnger bilderna efter deras lagernamn i PSD-filen. Ett lager med namnet Price Tag i den ursprungliga PSD-filen blir till exempel en bild med namnet Price Tag. Om lagernamnen i PSD-filen däremot är Photoshop standardlagernamn (Bakgrund, Lager 1, Lager 2 och så vidare) får bilderna namn efter sina lagernummer i PSD-filen. <!-- not their default layer names -->

      * **[!UICONTROL Photoshop and layer number]** - Namnger bilderna efter deras lagernummer i PSD-filen och ignorerar de ursprungliga lagernamnen. Bilderna får samma namn som Photoshop-filnamnet och ett nummer i det tillagda lagret. Det andra lagret i en fil med namnet `Spring Ad.psd` får till exempel namnet `Spring Ad_2` även om det har ett icke-standardnamn i Photoshop.

      * **[!UICONTROL Photoshop and layer name]** - Namnger bilderna efter PSD-filen följt av lagernamnet eller lagernumret. Lagernumret används om lagernamnen i PSD-filen är Photoshop standardlagernamn. Ett lager med namnet `Price Tag` i en PSD-fil med namnet `SpringAd` har till exempel namnet `Spring Ad_Price Tag`. Ett lager med standardnamnet Lager2 kallas `Spring Ad_2`.
   * **[!UICONTROL Anchor]** - Ange hur bilder ska förankras i mallar som genereras från lagerkompositionen som skapas från PSD-filen. Som standard är ankarpunkten i mitten. Med en central ankarpunkt kan ersättningsbilder bäst fylla samma område, oavsett ersättningsbildens proportioner. Bilder med en annan aspekt som ersätter den här bilden upptar i själva verket samma utrymme när de refererar till mallen och använder parameterersättning. Ändra till en annan inställning om ditt program kräver att ersättningsbilderna fyller ut det tilldelade utrymmet i mallen.


## Visa och redigera lager i en PSD-fil {#viewing-and-editing-layers-in-a-psd-file}

Om du valde alternativet Behåll lager när du överförde PSD-filen, delade Adobe Dynamic Media Classic de enskilda lagren i resurser. Du kan visa och redigera de objektlager som tillhör en PSD-fil genom att öppna filen i panelen Bläddra i detaljvyn.

1. Dubbelklicka på den fullständiga PSD-filen i panelen Bläddra. Filen öppnas i detaljvyn.

   >[!NOTE]
   >
   >Se till att du öppnar hela resursen och inte något av PSD-lagren.

1. Välj **[!UICONTROL Layers]**. Alla lager visas som separata bilder på panelen Lager.
1. Dubbelklicka på ett lager och gör något av följande:

   * Om du vill skapa ett bildschema på lagret väljer du **[!UICONTROL Image Map]**-ikonen. (Se [Skapa bildscheman](creating-image-maps.md#creating_image_maps).)
   * Om du vill skapa zoommål på lagret väljer du **[!UICONTROL Zoom Targets]**-ikonen. (Se [Skapa zoommål för guidad zoomning](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Om du vill beskära lagret väljer du **[!UICONTROL Crop]**-ikonen. (Se [Beskära en bild](cropping-image.md#cropping_an_image).)
   * Om du vill öka skärpan i lagret väljer du **[!UICONTROL Sharpen]**. (Se [Öka skärpan i en bild](sharpening-image.md#sharpening_an_image).)
   * Om du vill justera lagret väljer du **[!UICONTROL Adjust]**. (Se [Justera en bild](adjusting-image.md#adjusting_an_image).)

1. Välj **[!UICONTROL Save]** eller **[!UICONTROL Save As]**.
1. Om du vill visa eller redigera ett annat lager väljer du en pil längst ned i förhandsgranskningen av lagret.
1. Om du vill stänga lagerdetaljvyn väljer du ikonen **[!UICONTROL Grid View]**.
