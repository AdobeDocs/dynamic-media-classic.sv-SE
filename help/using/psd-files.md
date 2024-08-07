---
title: Arbeta med PSD-filer
description: Lär dig hur du arbetar med PSD i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
topic: Integrations, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 0%

---

# Arbeta med PSD-filer{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)**: Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on Web pages. -->

PSD (Photoshop Document Files) används oftast i Adobe Dynamic Media Classic för att skapa mallar. När du överför en PSD-fil kan du skapa en Adobe Dynamic Media Classic-mall automatiskt från filen (välj alternativet Skapa mall på överföringsskärmen).

Adobe Dynamic Media Classic skapar flera bilder från en PSD-fil med lager om du använder filen för att skapa en mall. En bild skapas för varje lager.

## Överföringsalternativ för PSD {#psd-upload-options}

Alternativ för att överföra PSD-filer finns under Photoshop-alternativ i dialogrutan Alternativ för överföringsjobb. Du kan beskära en fil, välja en färgprofil för den, använda den för att skapa en mall och välja en ankarpunkt.

De här alternativen är tillgängliga när du överför PSD-filer:

* **Beskärningsalternativ**: Finns under **[!UICONTROL Crop Options]**. Markera **[!UICONTROL Trim]** så att du automatiskt kan beskära tomt utrymme från kanterna på en PSD-fil. Markera **[!UICONTROL Manual]** om du vill beskära sidorna i filen PSD:

   * **[!UICONTROL Trim]**: Välj menyn **[!UICONTROL Trim Away Based On]** och välj **[!UICONTROL Color]** eller **[!UICONTROL Transparency]**.

  Om du väljer alternativet **[!UICONTROL Color]** väljer du menyn Hörn och väljer hörnet på PSD med den färg som bäst motsvarar den vitfärgen som du vill beskära.

  Dra skjutreglaget för att ange en tolerans mellan 0 och 1. Om du vill trimma baserat på färg anger du 0 för att beskära pixlar endast om de exakt matchar färgen som du markerade i hörnet av PSD. Nummer som ligger närmare 1 ger större färgskillnader. Om du vill trimma baserat på genomskinlighet anger du 0 om pixlarna bara ska beskäras om de är genomskinliga. Om du anger värden som är närmare 1 får du mer genomskinlighet.

   * **[!UICONTROL Manual]**: Ange antalet pixlar att beskära från en sida eller från varje sida av bilden. Hur mycket av bilden som beskärs beror på bildfilens ppi-inställning (pixlar per tum). Anta att bilden visar 150 ppi. Sedan anger du 75 i textrutorna Överkant, Höger, Underkant och Vänster. Varje sida av bilden beskärs, 0,5 tum.

* **Alternativ för färgprofil**: Finns under **[!UICONTROL Color Profile Options]**.

   * **[!UICONTROL Default Color Preservation]**

   * **[!UICONTROL Keep Original Color Space]**: Behåller bildens ursprungliga färgrymd.

   * **[!UICONTROL Custom From]** > **[!UICONTROL To]**: Öppnar menyer så att du kan välja färgmodellen Konvertera från och Konvertera till. Du kan välja en standardfärgmodell för Photoshop eller en färgmodell som du har överfört till Adobe Dynamic Media Classic. Se [ICC-profiler](/help/using/icc-profiles.md).

* **Photoshop-alternativ**

   * **[!UICONTROL Maintain Layers]**: Rippar lagren i PSD, om det finns några, till enskilda resurser. Resurslagren är fortfarande kopplade till PSD. Du kan visa dem genom att öppna filen PSD i detaljvyn och välja lagerpanelen. Se Visa och redigera lager i en PSD-fil.

   * **[!UICONTROL Create Template]**: Skapar en mall från lagren i filen PSD.

   * **[!UICONTROL Extract Text]**: Extraherar texten så att användare kan söka efter text i ett visningsprogram.

   * **[!UICONTROL Extend Layers To Background Size]**: Utökar storleken på rippade bildlager till storleken på bakgrundslagret.

   * **[!UICONTROL Layer Naming]**: Lager i filen PSD överförs som separata bilder. Om du vill namnge bilderna i Adobe Dynamic Media Classic väljer du bland följande alternativ:

      * **[!UICONTROL Layer Name]**: Namnger bilderna efter deras lagernamn i filen PSD. Ett lager med namnet Price Tag i den ursprungliga PSD-filen blir till exempel en bild med namnet Price Tag. Om lagernamnen i filen PSD är Photoshop standardlagernamn (Bakgrund, Lager 1, Lager 2 och så vidare) får bilderna namn efter sina lagernummer i filen PSD. <!-- not their default layer names -->

      * **[!UICONTROL Photoshop and layer number]**: Namnger bilderna efter deras lagernummer i filen PSD och ignorerar de ursprungliga lagernamnen. Bilderna namnges med Photoshop-filnamnet och ett nummer på lagret som läggs till. Det andra lagret i en fil med namnet `Spring Ad.psd` får till exempel namnet `Spring Ad_2` även om det har ett icke-standardnamn i Photoshop.

      * **[!UICONTROL Photoshop and layer name]**: Namnger bilderna efter PSD-filen följt av lagernamnet eller lagernumret. Lagernumret används om lagernamnen i filen PSD är Photoshop standardlagernamn. Ett lager med namnet `Price Tag` i en PSD-fil med namnet `SpringAd` får till exempel namnet `Spring Ad_Price Tag`. Ett lager med standardnamnet Lager2 kallas `Spring Ad_2`.

   * **[!UICONTROL Anchor]**: Ange hur bilder är förankrade i mallar som genereras från lagerkompositionen som skapas från filen PSD. Som standard är ankarpunkten i mitten. Med en central ankarpunkt kan du ersätta bilder som bäst kan fylla samma område, oavsett ersättningsbildens proportioner. Bilder med en annan aspekt som ersätter den här bilden upptar i själva verket samma utrymme när de refererar till mallen och använder parameterersättning. Ändra till en annan inställning om ditt program kräver att ersättningsbilderna fyller ut det tilldelade utrymmet i mallen.

## Visa och redigera lager i en PSD-fil {#viewing-and-editing-layers-in-a-psd-file}

Om du valde alternativet **[!UICONTROL Maintain Layers]** när du överförde PSD, delade Adobe Dynamic Media Classic bort de enskilda lagren i resurser. Du kan visa och redigera de objektlager som hör till en PSD-fil genom att öppna filen i panelen Bläddra i detaljvyn.

>[!NOTE]
>
>Adobe Dynamic Media Classic stöder upp till fem nivåer i en kapslad lagergrupp.

1. Dubbelklicka på den fullständiga PSD-filen på panelen Bläddra. Filen öppnas i detaljvyn.

   >[!NOTE]
   >
   >Se till att du öppnar hela resursen och inte ett av PSD-lagren.

1. Välj **[!UICONTROL Layers]**. Alla lager visas som separata bilder på panelen Lager.
1. Dubbelklicka på ett lager och gör något av följande:

   * Om du vill skapa en bildschema på lagret väljer du ikonen **[!UICONTROL Image Map]** . (Se [Skapa bildscheman](creating-image-maps.md#creating_image_maps).)
   * Om du vill skapa zoommål på lagret väljer du ikonen **[!UICONTROL Zoom Targets]** . (Se [Skapa zoommål för guidad zoomning](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Välj ikonen **[!UICONTROL Crop]** om du vill beskära lagret. (Se [Beskära en bild](cropping-image.md#cropping_an_image).)
   * Markera **[!UICONTROL Sharpen]** om du vill öka skärpan i lagret. (Se [Öka skärpan i en bild](sharpening-image.md#sharpening_an_image).)
   * Om du vill justera lagret väljer du **[!UICONTROL Adjust]**. (Se [Justera en bild](adjusting-image.md#adjusting_an_image).)

1. Välj **[!UICONTROL Save]** eller **[!UICONTROL Save As]**.
1. Om du vill visa eller redigera ett annat lager väljer du en pil längst ned i förhandsgranskningen av lagret.
1. Om du vill stänga lagerdetaljvyn väljer du ikonen **[!UICONTROL Grid View]**.
