---
title: Arbeta med PDF-filer
seo-title: Arbeta med PDF-filer
description: 'null'
seo-description: Lär dig hur du arbetar med PDF-filer i Dynamic Media Classic.
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Arbeta med PDF-filer{#working-with-pdfs}

PDF-filer (Portable Document Format) används oftast i Dynamic Media Classic för att skapa e-kataloger. När du överför en PDF-fil rastreras eller rips sidorna som standard så att sidorna kan användas för att skapa multimedia.

## Alternativ för PDF-överföring {#pdf-upload-options}

När du överför en PDF-fil kan du formatera den på olika sätt. Du beskär sidorna, extraherar sökord, anger en pixel per tum-upplösning och väljer en färgrymd. PDF-filer innehåller ofta en ytmarginal, skärmärken, passmärken och andra skrivarmärken. Du kan beskära dessa märken från sidorna när du överför en PDF-fil.

Alternativ för att överföra PDF-filer finns på skärmen Överför under PDF-alternativ.

**Bearbetar**

Bearbetningsalternativen är följande:

**Rastrera** (standard) Rippar sidorna i PDF-filen och konverterar vektorgrafik till bitmappsbilder. Välj det här alternativet om du vill skapa en e-katalog.

**Extrahera sökord** Extraherar ord från PDF-filen så att filen kan genomsökas efter nyckelord i en eCatalog Viewer.

**Extrahera länkar** extraherar länkar från PDF-filerna och konverterar dem till bildscheman som används i en eCatalog Viewer.

**Skapa automatiskt en eCatalog med PDF** med flera sidor skapar automatiskt en e-katalog från PDF-filen. eCatalog namnges efter den PDF-fil du överförde. (Det här alternativet är bara tillgängligt om du rastrerar PDF-filen när du överför den.)

**Upplösning**

Anger upplösningsinställningen. Den här inställningen avgör hur många pixlar som visas per tum i PDF-filen. Standardvärdet är 150.

**Färgmodell**

Välj menyn Färgrymd och välj en färgrymd för PDF-filen. De flesta PDF-filer har både RGB- och CMYK-färgbilder. RGB-färgmodellen är att föredra när du vill visa bilden online.

**Identifiera automatiskt** Behåller PDF-filens färgrymd.

**Tvinga som RGB** Konverterar till RGB-färgrymden.

**Använd som CMYK** Konverterar till CMYK-färgmodellen.

**Använd som gråskala** Konverterar till färgrymden Gråskala.

**Färgprofil**

Välj ett färgprofilsalternativ:

**Konvertera till sRGB** Konverterar till sRGB (röd standardgrön blå). sRGB är den rekommenderade färgrymden för visning av bilder på webbsidor.

**Behåll ursprunglig färgrymd** Behåller den ursprungliga färgrymden.

**Anpassad från > Till** öppnar menyer så att du kan välja färgmodellen Konvertera från och Konvertera till. Du kan välja en Photoshop-standardfärgmodell eller en färgmodell som du överförde till SPS.

Se [ICC-profiler](icc-profiles.md#icc_profiles).

## Beskära tomt utrymme från en PDF-fil {#cropping-white-space-from-a-pdf-file}

1. Om du vill beskära pixlar med tomt utrymme automatiskt från en PDF-fil när du överför den väljer du Beskär-menyn och sedan Beskär.
1. Ange följande alternativ:

   **Rensa bortBaserat på** Välj om du vill beskära baserat på färg eller genomskinlighet:

   **Färg** Välj alternativet Färg. Välj sedan menyn Hörn och välj hörnet av PDF-filen med den färg som bäst motsvarar den tomrumsfärg som du vill beskära.

   **Genomskinlighet** Välj alternativet Genomskinlighet.

   **Tolerans** Dra skjutreglaget för att ange en tolerans mellan 0 och 1:

   **Trimma baserat på färg** Ange 0 om du bara vill beskära pixlar om de exakt matchar färgen som du valde i PDF-filens hörn. Nummer som ligger närmare 1 ger större färgskillnader.

   **Trimma baserat på genomskinlighet** Ange 0 om pixlarna bara ska beskäras om de är helt genomskinliga. siffror närmare 1 ger större genomskinlighet.

## Beskära från sidorna på PDF-sidor {#cropping-from-the-sides-of-pdf-pages}

Du kan ta bort skrivarmärken manuellt från sidorna i en PDF-fil när du överför den.

1. Välj menyn Beskär och välj Manuell.
1. Ange pixelinställningar i textrutorna Överkant, Höger, Underkant och Vänster om du vill beskära från sidans överkant, underkant och sidor.

Hur mycket av sidan som beskärs beror på inställningen för upplösning PX/tum som du anger för PDF-filen. Om du t.ex. anger 150 (standardvärdet) som inställningen Upplösning PX/tum och beskär 75 pixlar från sidorna beskärs en halv tum eftersom 75 pixlar är lika med en halv tum vid 150 pixlar per tum.
