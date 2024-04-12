---
title: Arbeta med PDF
description: Lär dig arbeta med PDF i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
topic: Integrations, Development
level: Experienced
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# Arbeta med PDF{#working-with-pdfs}

PDF-filer (Portable Document Format) används oftast i Adobe Dynamic Media Classic för att skapa e-kataloger. När du överför en PDF-fil rastreras eller rips sidorna som standard, så att sidorna kan användas för att skapa multimedia.

När du överför en PDF för sidextrahering använder Adobe följande gräns:

| Begränsningstyp | Begränsning har införts | Ändring till begränsning den 31 december 2022 |
| --- | --- | --- |
| Högsta antal sidor för PDF som ska övervägas för extrahering | 5000 (för nya överföringar) | 100 (för alla PDF) |

Se även [Dynamic Media begränsningar](/help/using/limitations.md).

## Överföringsalternativ för PDF {#pdf-upload-options}

När du överför en PDF-fil kan du formatera den på olika sätt. Du beskär sidorna, extraherar sökord, anger pixlar per tum och väljer en färgrymd. PDF-filer innehåller ofta en ytmarginal, skärmärken, passmärken och andra skrivarmärken. Du kan beskära dessa märken från sidorna när du överför en PDF-fil.

Alternativ för att överföra PDF-filer finns på sidan Överför under Alternativ för PDF.

### Bearbetningsalternativ

**[!UICONTROL Rasterize]** - (Standard) Rippar sidorna i filen PDF och konverterar vektorgrafik till bitmappsbilder. Välj det här alternativet om du vill skapa en e-katalog.

**[!UICONTROL Extract Search Words]** - Extraherar ord från PDF-filen så att filen kan genomsökas efter nyckelord i en eCatalog Viewer.

**[!UICONTROL Extract Links]** - Extraherar länkar från PDF-filerna och konverterar dem till Image Maps som används i en eCatalog Viewer.

**[!UICONTROL Auto-Generate eCatalog With Multi-page PDF]** - Skapar automatiskt en e-katalog från PDF-filen. eCatalog namnges efter den överförda PDF-filen. (Det här alternativet är bara tillgängligt om du rastrerar PDF-filen när du överför den.)

### Upplösning

Anger upplösningsinställningen. Den här inställningen avgör hur många pixlar som visas per tum i filen PDF. Standardvärdet är 150.

### Alternativ för färgrymd

Välj menyn Färgrymd och välj en färgrymd för filen PDF. De flesta PDF-filer har både RGB och CMYK-färgbilder. Färgrymden RGB är att föredra när du vill visa bilden online.

* **[!UICONTROL Detect Automatically]** - Behåller färgrymden för PDF-filen.

* **[!UICONTROL Force As RGB]** - Konverterar till färgmodellen RGB.

* **[!UICONTROL Force As CMYK]** - Konverterar till CMYK-färgmodellen.

* **[!UICONTROL Force As Grayscale]** - Konverterar till färgmodellen Gråskala.

### Alternativ för färgprofil

* **[!UICONTROL Convert To sRGB]** - Konverterar till sRGB (Standard Red Green Blue). sRGB är den rekommenderade färgrymden för visning av bilder på en webbsida.

* **[!UICONTROL Keep Original Color Space]** - Behåller den ursprungliga färgrymden.

* **[!UICONTROL Custom From]** > **[!UICONTROL To]** - Öppnar menyer så att du kan välja färgmodellen Konvertera från och Konvertera till. Du kan välja en standardfärgmodell för Photoshop eller en färgmodell som du har överfört till Adobe Dynamic Media Classic.

Se även [ICC-profiler](/help/using/icc-profiles.md#icc_profiles).

## Beskära tomt utrymme från en PDF-fil {#cropping-white-space-from-a-pdf-file}

1. Om du vill beskära pixlar med tomt utrymme automatiskt från en PDF-fil när du överför den väljer du Beskär-menyn och sedan Beskär.
1. Ange följande alternativ:

   * **[!UICONTROL Trim Away Based On]** - Välj om du vill beskära baserat på färg eller genomskinlighet:

      * **[!UICONTROL Color]** - Välj alternativet Färg. Välj sedan **[!UICONTROL Corner]** och väljer hörnet på PDF med den färg som bäst motsvarar den färgen på tomrummet som du vill beskära.

      * **[!UICONTROL Transparency]** - Välj alternativet Genomskinlighet.

   * **[!UICONTROL Tolerance]** - Dra skjutreglaget för att ange en tolerans mellan 0 och 1.

   * **[!UICONTROL Trimming based on color]** - Ange 0 om du bara vill beskära pixlar om de exakt matchar färgen som du markerade i hörnet av PDF. Nummer som ligger närmare 1 ger större färgskillnader.

   * **[!UICONTROL Trimming based on transparency]** - Ange 0 om du bara vill beskära pixlar om de är genomskinliga. Med siffror närmare 1 får du mer genomskinlighet.

## Beskär från sidorna på PDF {#cropping-from-the-sides-of-pdf-pages}

Du kan ta bort skrivarmärken manuellt från sidorna i en PDF-fil när du överför den.

1. Välj på menyn Beskär **[!UICONTROL Manual]**.
1. Ange pixelinställningar i textrutorna Överkant, Höger, Underkant och Vänster om du vill beskära från sidans överkant, underkant och sidor.

Hur mycket av sidan som beskärs beror på inställningen för Upplösning PX/tum som du anger för PDF-filen. Anta till exempel att du anger 150 (standard) som upplösnings-PX/tum-inställning. Sedan beskär du 75 pixlar från sidorna. I så fall 0,5 tum. beskärs. Vid 150 pixlar per tum är 75 pixlar lika med en halv tum.
