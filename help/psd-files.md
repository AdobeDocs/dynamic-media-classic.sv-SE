---
title: 'Arbeta med PSD-filer '
seo-title: 'Arbeta med PSD-filer '
description: 'null'
seo-description: Lär dig hur du arbetar med PSD-filer.
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1030'
ht-degree: 1%

---


# Arbeta med PSD-filer {#working-with-psd-files}

PSD (Photoshop Document files) används oftast i Dynamic Media Classic för att skapa mallar. När du överför en PSD-fil kan du skapa en dynamisk Media Classic-mall automatiskt från filen (välj alternativet Skapa mall på överföringsskärmen).

Dynamic Media Classic skapar flera bilder från en PSD-fil med lager om du använder filen för att skapa en mall; skapas en bild för varje lager.

## PSD-överföringsalternativ {#psd-upload-options}

Alternativ för överföring av PSD-filer finns under Photoshop-alternativ i Alternativ för överföringsjobb. Du kan beskära en fil, välja en färgprofil för den, använda den för att skapa en mall och välja en ankarpunkt.

Dessa alternativ är tillgängliga när du överför PSD-filer:

**Beskär** (finns under Beskärningsalternativ.) Välj Trimma om du automatiskt vill beskära tomt utrymme från kanterna på en PSD-fil. Välj Manuell för att beskära sidor av PSD-filen:

**Rensa** Välj menyn Beskär bort baserat på och välj Färg eller Genomskinlighet.

Om du väljer alternativet Färg väljer du menyn Hörn och väljer hörnet på PSD-filen med den färg som bäst motsvarar den vitfärgen som du vill beskära.

Dra skjutreglaget för att ange en tolerans mellan 0 och 1:

Om du vill trimma baserat på färg anger du 0 för att beskära pixlar endast om de exakt matchar den färg som du valde i hörnet av PSD:n. Nummer som ligger närmare 1 ger större färgskillnader.

Om du vill trimma baserat på genomskinlighet anger du 0 för att beskära pixlar endast om de är helt genomskinliga. siffror närmare 1 ger större genomskinlighet.

**Manuell** Ange antalet pixlar som ska beskäras från en sida eller från varje sida av bilden. Hur mycket av bilden som beskärs beror på bildfilens ppi-inställning (pixlar per tum). Om bilden till exempel visar 150 ppi och du anger 75 i textrutorna Överkant, Höger, Underkant och Vänster beskärs en halv tum från varje sida av bilden.

**Färgprofil** (finns under Alternativ för färgprofil.) Välj ett alternativ:

**Konvertera till sRGB (standard)** Konverterar till sRGB (standard röd grön blå). sRGB är den rekommenderade färgrymden för visning av bilder på webbsidor.

**Behåll ursprunglig färgmodell** Behåller bildens ursprungliga färgmodell.

**Anpassad från > Till** öppnar menyer så att du kan välja färgmodellen Konvertera från och Konvertera till. Du kan välja en standardfärgmodell för Photoshop eller en färgmodell som du överfört till Dynamic Media Classic. Se ICC-profiler.

**Med Behåll lager** rippar du lagren i PSD-filen, om det finns några, till enskilda resurser. Resurslagren förblir kopplade till PSD-filen. Du kan visa dem genom att öppna PSD-filen i detaljvyn och välja lagerpanelen. Se Visa och redigera lager i en PSD-fil.

**Skapa mall** Skapar en mall från lagren i PSD-filen.

**Extrahera text** Extraherar texten så att användare kan söka efter text i ett visningsprogram.

**Utöka lager till bakgrundsstorlek** Utökar storleken på överlappade bildlager till storleken på bakgrundslagret.

**Lager för namngivning** av lager i PSD-filen överförs som separata bilder. Välj ett alternativ för att namnge dessa bilder i Dynamic Media Classic:

**Lagernamn** Namnger bilderna efter deras lagernamn i PSD-filen. Ett lager med namnet Price Tag i den ursprungliga PSD-filen blir till exempel en bild med namnet Price Tag. Om lagernamnen i PSD-filen däremot är Photoshop standardlagernamn (Bakgrund, Lager 1, Lager 2 och så vidare) får bilderna namn efter sina lagernummer i PSD-filen, inte efter deras standardlagernamn.

**Photoshop och Lagernummer** Namnger bilderna efter deras lagernummer i PSD-filen och ignorerar de ursprungliga lagernamnen. Bilderna får samma namn som Photoshop-filnamnet och ett nummer i det tillagda lagret. Det andra lagret i en fil som heter Spring Ad.psd får till exempel namnet Spring Ad_2 även om det har ett icke-standardnamn i Photoshop.

**Photoshop och Lagernamn** Namnger bilderna efter PSD-filen följt av lagernamnet eller lagernumret. Lagernumret används om lagernamnen i PSD-filen är Photoshop standardlagernamn. Ett lager med namnet Price Tag i en PSD-fil med namnet SpringAd får till exempel namnet Spring Ad_Price Tag. Ett lager med standardnamnet Lager2 kallas Spring Ad_2.

**Ankarpunkt** Ange hur bilder ska förankras i mallar som genereras från lagerkompositionen som skapas från PSD-filen. Som standard är ankarpunkten i mitten. Med en central ankarpunkt kan ersättningsbilder bäst fylla samma område, oavsett ersättningsbildens proportioner. Bilder med en annan aspekt som ersätter den här bilden upptar i själva verket samma utrymme när de refererar till mallen och använder parameterersättning. Ändra till en annan inställning om ditt program kräver att ersättningsbilderna fyller ut det tilldelade utrymmet i mallen.

## Visa och redigera lager i en PSD-fil {#viewing-and-editing-layers-in-a-psd-file}

Om du valde alternativet Behåll lager när du överförde din PSD-fil, delade Dynamic Media Classic de enskilda lagren i resurser. Du kan visa och redigera de objektlager som tillhör en PSD-fil genom att öppna filen i panelen Bläddra i detaljvyn.

1. Dubbelklicka på den fullständiga PSD-filen i panelen Bläddra för att öppna den i vyn Detalj.

   ***Obs **! Se till att du öppnar hela resursen och inte något av PSD-lagren.*

1. Klicka på Lager för att öppna lagerpanelen. Alla lager visas som separata bilder på panelen Lager.
1. Dubbelklicka på ett lager för att öppna det och gör något av följande:

   * Klicka på ikonen Bildschema för att skapa ett bildschema på lagret. (Se [Skapa bildscheman](creating-image-maps.md#creating_image_maps).)
   * Klicka på ikonen Zoommål för att skapa zoommål på lagret. (Se [Skapa zoommål för guidad zoomning](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Klicka på ikonen Beskär för att beskära lagret. (Se [Beskära en bild](cropping-image.md#cropping_an_image).)
   * Klicka på Skärpa om du vill öka skärpan i lagret. (Se [Skärpa en bild](sharpening-image.md#sharpening_an_image).)
   * Justera lagret genom att klicka på Justera. (Se [Justera en bild](adjusting-image.md#adjusting_an_image).)

1. Klicka på Spara eller Spara som.
1. Om du vill visa eller redigera ett annat lager klickar du på en pil längst ned i förhandsgranskningen av lagret.
1. Om du vill stänga lagerdetaljvyn klickar du på ikonen för stödrastervyn.

