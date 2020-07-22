---
title: Överföra PDF-filer
seo-title: Överföra PDF-filer
description: 'null'
seo-description: Lär dig hur du överför PDF-filer som är kopplade till en e-katalog.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---


# Överföra PDF-filer{#uploading-the-pdf-files}

Vanligtvis är Adobe PDF-filer källan till en e-katalog; dessa filer innehåller all bildinformation samt teckensnitt och vektorgrafik. Du kan även skapa en e-katalog med bilder. När du har förberett PDF-filerna för överföring markerar du knappen Överför i fältet Global navigering för att börja överföra PDF-filerna.

## Förbereda PDF-filer {#preparing-your-pdf-files}

Förbered PDF-filerna innan du överför dem till Dynamic Media Classic:

* Placera alla filer i samma mapp på datorn eller i nätverket så att det blir enklare att överföra filerna.
* Namnge filerna i alfanumerisk ordning per sida. Om du beställer sidorna blir det enklare att placera sidorna i rätt ordning efter att filerna har överförts.
* Granska PDF-sidorna för att se om de innehåller skärmärken, registreringsmål eller färgfält. Dessa märken avgör var papperet ska skäras när dokumenten skrivs ut. måste tas bort innan din eCatalog kan placeras på webben. I Dynamic Media Classic finns alternativ för beskärningsmärken när du överför PDF-filer.
* Om du vill att tittarna ska söka i din e-katalog med nyckelord, ta reda på om PDF-filerna är förenklade. Du kan inte extrahera sökord från förenklade PDF-filer. Om du vill ta reda på om en PDF-fil är förenklad kan du försöka markera text i den. Om du inte kan markera text förenklas PDF-filen och visningsprogrammen kan inte söka efter nyckelord i din eCatalog.
* Eftersom de ska skrivas ut innehåller PDF-filerna vanligtvis CMYK-bilder. Som standard kan Dynamic Media Classic identifiera dessa CMYK-bilder på ett intelligent sätt och konvertera dem med en intern CMYK-färgprofil. Om du vill använda en egen färgprofil för att konvertera CMYK-bilder kan du göra det.

   Se [ICC-profiler](icc-profiles.md#icc_profiles).

## Överföringsalternativ för PDF med bästa praxis {#best-practice-pdf-upload-options}

Mer information om de olika överföringsmetoderna finns i [Överföra filer](uploading-files.md#uploading_your_files).

Markera de filer som du vill överföra och välj sedan följande *bästa* PDF-alternativ:

* **Beskär** Välj Beskär-menyn och välj Manuell om sidorna innehåller skärmärken, passmärken eller andra märken. Ange antalet pixlar att beskära från sidans övre, högra, nedre och vänstra sidor. Skärmärken är vanligtvis inställda på en halv-tumsmarginal. Om du väljer 150 som pixel per tum-upplösning (den rekommenderade inställningen) beskärs en halv tum från marginalerna om du anger 75, 75, 75 i textrutorna Överkant, Höger, Underkant och Vänster (vid 150 ppi, hälften av en tum är lika med 75 pixlar).

* **Bearbetning** Välj Bearbetning och Rastrera. PDF-filen måste rastreras så att alla sidor och bilder kan visas i e-katalogen.

* **Extrahera sökord (valfritt)** Välj det här alternativet om du vill att dina läsare ska kunna söka efter nyckelord i din eCatalog.

* **Skapa e-katalog automatiskt från PDF-fil med flera sidor (valfritt)** Välj det här alternativet om du automatiskt vill skapa en e-katalog när du överför den. Du kan gå direkt till eCatalog-skärmen och börja arbeta med eCatalog utan att först behöva markera PDF-filer och sedan välja kommandot Skapa. eCatalog namnges efter PDF-filen.

* **Upplösning** Dynamic Media Classic rekommenderar 150 pixlar per tum.

* **Färgrymd** Dynamic Media Classic rekommenderar att du väljer Identifiera automatiskt. Vanligtvis är PDF-filer som skapats för utskrift CMYK. PDF-filer för visning online är RGB. Om båda färgrymderna används i en PDF-fil kan du välja en viss färgrymd genom att välja Tvinga som RGB eller Tvinga som CMYK. I PDF-filer används till exempel båda färgmodellerna när sidgrafik använder en CMYK-färgmodell, men bilder använder RGB. Om du överförde en ICC-profil visas dess namn på menyn Färgrymd och du kan välja den där.

   Se [ICC-profiler](icc-profiles.md#icc_profiles).

* **Färgprofil**: Välj ett alternativ för Färgprofil:

* **ConvertTo SRGB** Converts to SRGB (Standard Red Green Blue). SRGB är den rekommenderade färgrymden för visning av bilder på webbsidor.

* **Behåll ursprunglig färgrymd** Behåller den ursprungliga färgrymden.

* **Anpassa från > Till**&#x200B;öppnar menyer så att du kan välja färgmodellen Konvertera från och Konvertera till. Du kan välja en standardfärgmodell för Photoshop eller en färgmodell som du överförde till Dynamic Media Classic.

Se [ICC-profiler](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Mer information om alla PDF-alternativ finns i [PDF-överföringsalternativ](pdfs.md#pdf_upload_options).

