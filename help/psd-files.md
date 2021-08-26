---
title: 'Arbeta med PSD-filer '
description: Lär dig hur du arbetar med PSD-filer.
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 0%

---

# Arbeta med PSD-filer {#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages. -->

PSD (Photoshop Document Files) används oftast i Adobe Dynamic Media Classic för att skapa mallar. När du överför en PSD-fil kan du skapa en Adobe Dynamic Media Classic-mall automatiskt från filen (välj alternativet Skapa mall på överföringsskärmen).

Adobe Dynamic Media Classic skapar flera bilder från en PSD-fil med lager om du använder filen för att skapa en mall; skapas en bild för varje lager.

## PSD-överföringsalternativ {#psd-upload-options}

Alternativ för överföring av PSD-filer finns under Photoshop-alternativ i dialogrutan Alternativ för överföringsjobb. Du kan beskära en fil, välja en färgprofil för den, använda den för att skapa en mall och välja en ankarpunkt.

Dessa alternativ är tillgängliga när du överför PSD-filer:

* **Beskärningsalternativ**  - finns under  **[!UICONTROL Crop Options]**. Välj Trimma om du automatiskt vill beskära tomt utrymme från kanterna på en PSD-fil. klicka på **[!UICONTROL Manual]** för att beskära sidor av PSD-filen:

   * **Trimma** - Markera  **[!UICONTROL Trim Away Based On]** menyn och välj  **[!UICONTROL Color]** eller  **[!UICONTROL Transparency]**.

      Om du väljer alternativet Färg väljer du menyn Hörn och väljer hörnet på PSD-filen med den färg som bäst motsvarar den vitfärgen som du vill beskära.

      Dra skjutreglaget för att ange en tolerans mellan 0 och 1. Om du vill trimma baserat på färg anger du 0 för att beskära pixlar endast om de exakt matchar den färg som du valde i hörnet av PSD:n. Nummer som ligger närmare 1 ger större färgskillnader. Om du vill trimma baserat på genomskinlighet anger du 0 för att beskära pixlar endast om de är genomskinliga. siffror närmare 1 ger större genomskinlighet.

   * **Manuell**  - Ange antalet pixlar att beskära från en sida eller från varje sida av bilden. Hur mycket av bilden som beskärs beror på bildfilens ppi-inställning (pixlar per tum). Om bilden till exempel visar 150 ppi och du anger 75 i textrutorna Överkant, Höger, Underkant och Vänster beskärs en halv tum från varje sida av bilden.

* **Alternativ**  för färgprofil - finns under  **[!UICONTROL Color Profile Options]**.

   * **Standardfärgbevaring**

   * **Behåll ursprunglig färgmodell**  - Behåller bildens ursprungliga färgmodell.

   * **Anpassad från > Till** - Öppnar menyer så att du kan välja färgmodellen Konvertera från och Konvertera till. Du kan välja en standardfärgmodell för Photoshop eller en färgmodell som du har överfört till Adobe Dynamic Media Classic. Se [ICC-profiler](/help/icc-profiles.md).

* **Photoshop-alternativ**

   * **Behåll lager**  - Rippar lagren i PSD-filen, om det finns några, till enskilda resurser. Resurslagren förblir kopplade till PSD-filen. Du kan visa dem genom att öppna PSD-filen i detaljvyn och välja lagerpanelen. Se Visa och redigera lager i en PSD-fil.

   * **Skapa mall**  - Skapar en mall från lagren i PSD-filen.

   * **Extrahera text**  - Extraherar texten så att användare kan söka efter text i ett visningsprogram.

   * **Utöka lager till bakgrundsstorlek**  - Utökar storleken på överlappade bildlager till storleken på bakgrundslagret.

   * **Namnge**  lager - Lager i PSD-filen överförs som separata bilder. Om du vill namnge bilderna i Adobe Dynamic Media Classic väljer du bland följande alternativ:

      * **Lagernamn**  - Namnger bilderna efter deras lagernamn i PSD-filen. Ett lager med namnet Price Tag i den ursprungliga PSD-filen blir till exempel en bild med namnet Price Tag. Om lagernamnen i PSD-filen däremot är Photoshop standardlagernamn (Bakgrund, Lager 1, Lager 2 och så vidare) får bilderna namn efter sina lagernummer i PSD-filen, inte efter deras standardlagernamn.

      * **Photoshop och lagernummer**  - Namnger bilderna efter deras lagernummer i PSD-filen och ignorerar de ursprungliga lagernamnen. Bilderna får samma namn som Photoshop-filnamnet och ett nummer i det tillagda lagret. Det andra lagret i en fil med namnet `Spring Ad.psd` får till exempel namnet `Spring Ad_2` även om det har ett icke-standardnamn i Photoshop.

      * **Photoshop och lagernamn**  - Namnger bilderna efter PSD-filen följt av lagernamnet eller lagernumret. Lagernumret används om lagernamnen i PSD-filen är Photoshop standardlagernamn. Ett lager med namnet `Price Tag` i en PSD-fil med namnet `SpringAd` har till exempel namnet `Spring Ad_Price Tag`. Ett lager med standardnamnet Lager2 kallas `Spring Ad_2`.
   * **Fästpunkt**  - Ange hur bilder ska förankras i mallar som genereras från lagerkompositionen som skapas från PSD-filen. Som standard är ankarpunkten i mitten. Med en central ankarpunkt kan ersättningsbilder bäst fylla samma område, oavsett ersättningsbildens proportioner. Bilder med en annan aspekt som ersätter den här bilden upptar i själva verket samma utrymme när de refererar till mallen och använder parameterersättning. Ändra till en annan inställning om ditt program kräver att ersättningsbilderna fyller ut det tilldelade utrymmet i mallen.


## Visa och redigera lager i en PSD-fil {#viewing-and-editing-layers-in-a-psd-file}

Om du valde alternativet Behåll lager när du överförde PSD-filen, delade Adobe Dynamic Media Classic de enskilda lagren i resurser. Du kan visa och redigera de objektlager som tillhör en PSD-fil genom att öppna filen i panelen Bläddra i detaljvyn.

1. Dubbelklicka på den fullständiga PSD-filen i panelen Bläddra. Filen öppnas i detaljvyn.

   >[!NOTE]
   >
   >Se till att du öppnar hela resursen och inte något av PSD-lagren.

1. Klicka på **[!UICONTROL Layers]**. Alla lager visas som separata bilder på panelen Lager.
1. Dubbelklicka på ett lager och gör något av följande:

   * Om du vill skapa ett bildschema på lagret klickar du på ikonen **[!UICONTROL Image Map]**. (Se [Skapa bildscheman](creating-image-maps.md#creating_image_maps).)
   * Om du vill skapa zoommål på lagret klickar du på ikonen **[!UICONTROL Zoom Targets]**. (Se [Skapa zoommål för guidad zoomning](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Klicka på ikonen **[!UICONTROL Crop]** om du vill beskära lagret. (Se [Beskära en bild](cropping-image.md#cropping_an_image).)
   * Om du vill öka skärpan i lagret klickar du på **[!UICONTROL Sharpen]**. (Se [Öka skärpan i en bild](sharpening-image.md#sharpening_an_image).)
   * Om du vill justera lagret klickar du på **[!UICONTROL Adjust]**. (Se [Justera en bild](adjusting-image.md#adjusting_an_image).)

1. Klicka på **[!UICONTROL Save]** eller **[!UICONTROL Save As]**.
1. Om du vill visa eller redigera ett annat lager klickar du på en pil längst ned i förhandsgranskningen av lagret.
1. Klicka på ikonen **[!UICONTROL Grid View]** för att stänga lagerdetaljvyn.
