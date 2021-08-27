---
title: Arbeta med PDF-filer
description: Lär dig hur du arbetar med PDF-filer i Adobe Dynamic Media Classic.
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
source-git-commit: 3185824deca4d4b3c5549bda2e47f179094110e7
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Arbeta med PDF-filer{#working-with-pdfs}

PDF-filer (Portable Document Format) används oftast i Adobe Dynamic Media Classic för att skapa e-kataloger. När du överför en PDF-fil rastreras eller rips Adobe Dynamic Media Classic, så att sidorna kan användas för att skapa multimedia.

## Alternativ för PDF-överföring {#pdf-upload-options}

När du överför en PDF-fil kan du formatera den på olika sätt. Du beskär sidorna, extraherar sökord, anger en pixel per tum-upplösning och väljer en färgrymd. PDF-filer innehåller ofta en ytmarginal, skärmärken, passmärken och andra skrivarmärken. Du kan beskära dessa märken från sidorna när du överför en PDF-fil.

Alternativ för att överföra PDF-filer finns på sidan Överför under PDF-alternativ.

### Bearbetningsalternativ

**[!UICONTROL Rasterize]** - (Standard) Rippar ned sidorna i PDF-filen och konverterar vektorgrafik till bitmappsbilder. Välj det här alternativet om du vill skapa en e-katalog.

**[!UICONTROL Extract Search Words]** - Extraherar ord från PDF-filen så att filen kan genomsökas efter nyckelord i en eCatalog Viewer.

**[!UICONTROL Extract Links]** - Extraherar länkar från PDF-filerna och konverterar dem till bildscheman som används i en eCatalog Viewer.

**[!UICONTROL Auto-Generate eCatalog With Multi-page PDF]** - Skapar automatiskt en e-katalog från PDF-filen. eCatalog namnges efter den PDF-fil du överförde. (Det här alternativet är bara tillgängligt om du rastrerar PDF-filen när du överför den.)

### Upplösning

Anger upplösningsinställningen. Den här inställningen avgör hur många pixlar som visas per tum i PDF-filen. Standardvärdet är 150.

### Alternativ för färgrymd

Välj menyn Färgrymd och välj en färgrymd för PDF-filen. De flesta PDF-filer har både RGB- och CMYK-färgbilder. RGB-färgmodellen är att föredra när du vill visa bilden online.

* **[!UICONTROL Detect Automatically]** - Behåller PDF-filens färgrymd.

* **[!UICONTROL Force As RGB]** - Konverterar till RGB-färgmodellen.

* **[!UICONTROL Force As CMYK]** - Konverterar till CMYK-färgmodellen.

* **[!UICONTROL Force As Grayscale]** - Konverterar till färgmodellen Gråskala.

### Alternativ för färgprofil

* **[!UICONTROL Convert To sRGB]** - Konverterar till sRGB (Standard Red Green Blue). sRGB är den rekommenderade färgrymden för visning av bilder på webbsidor.

* **[!UICONTROL Keep Original Color Space]** - Behåller den ursprungliga färgrymden.

* **[!UICONTROL Custom From]** >  **[!UICONTROL To]** - Öppnar menyer så att du kan välja färgmodellen Konvertera från och Konvertera till. Du kan välja en standardfärgmodell för Photoshop eller en färgmodell som du har överfört till Adobe Dynamic Media Classic.

Se även [ICC-profiler](/help/icc-profiles.md#icc_profiles).

## Beskära tomt utrymme från en PDF-fil {#cropping-white-space-from-a-pdf-file}

1. Om du vill beskära pixlar med tomt utrymme automatiskt från en PDF-fil när du överför den väljer du Beskär-menyn och sedan Beskär.
1. Ange följande alternativ:

   * **[!UICONTROL Trim Away Based On]** - Välj om du vill beskära baserat på färg eller genomskinlighet:

      * **[!UICONTROL Color]** - Välj alternativet Färg. Välj sedan menyn **[!UICONTROL Corner]** och välj hörnet av PDF-filen med den färg som bäst motsvarar den tomrumsfärg som du vill beskära.

      * **[!UICONTROL Transparency]** - Välj alternativet Genomskinlighet.
   * **[!UICONTROL Tolerance]** - Dra skjutreglaget för att ange en tolerans mellan 0 och 1.

   * **[!UICONTROL Trimming based on color]** - Ange 0 om du bara vill beskära pixlar om de exakt matchar färgen som du valde i PDF-filens hörn. Nummer som ligger närmare 1 ger större färgskillnader.

   * **[!UICONTROL Trimming based on transparency]** - Ange 0 om pixlarna bara ska beskäras om de är genomskinliga. siffror närmare 1 ger större genomskinlighet.


## Beskära från sidorna på PDF-sidorna {#cropping-from-the-sides-of-pdf-pages}

Du kan ta bort skrivarmärken manuellt från sidorna i en PDF-fil när du överför den.

1. Välj **[!UICONTROL Manual]** på menyn Beskär.
1. Ange pixelinställningar i textrutorna Överkant, Höger, Underkant och Vänster om du vill beskära från sidans överkant, underkant och sidor.

Hur mycket av sidan som beskärs beror på inställningen för upplösning PX/tum som du anger för PDF-filen. Om du t.ex. anger 150 (standardvärdet) som inställningen Upplösning PX/tum och beskär 75 pixlar från sidorna beskärs en halv tum. vid 150 pixlar per tum är 75 pixlar lika med en halv tum.
