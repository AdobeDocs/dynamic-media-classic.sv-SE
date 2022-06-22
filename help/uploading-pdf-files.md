---
title: Överför PDF-filer
description: Lär dig hur du överför PDF-filer som är kopplade till en e-katalog i Adobe Dynamic Media Classic.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
source-git-commit: d5293a2983e1105c65005634e7eb4147e17e8328
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 0%

---

# Överför PDF-filer{#uploading-the-pdf-files}

Vanligtvis är Adobe PDF-filer källa för en e-katalog. Dessa filer innehåller all bildinformation, teckensnitt och vektorgrafik. Du kan även skapa en e-katalog med bilder. När du har förberett dina PDF-filer för överföring väljer du **[!UICONTROL Upload]** för att börja ladda upp PDF.

När du överför en PDF för sidextrahering använder Adobe följande gräns:

| Begränsningstyp för PDF | Implementerad gräns | Ändringar av begränsningen 31 december 2022 |
| --- | --- | --- |
| Högsta antal sidor för PDF som ska övervägas för extrahering | 5000 (för nya överföringar) | 100 |

<!-- 
>[!NOTE]
>
>When you upload a PDF for page extraction, Adobe imposes the following best practice guideline and enforced limit.d
>
>* Maximum page size of a PDF to be considered for extraction
>   * Best practice: 100
>   * Enforced limit: 1000 (for refresh uploads) -->

## Förbered dina PDF-filer {#preparing-your-pdf-files}

Förbered dina PDF-filer innan du överför dem till Adobe Dynamic Media Classic:

* Om du vill göra det enklare att överföra filerna placerar du alla filer i samma mapp på datorn eller i nätverket.
* Namnge filerna i alfanumerisk ordning per sida. Om du beställer sidorna blir det enklare att placera sidorna i rätt ordning efter att filerna har överförts.
* Granska sidorna om du vill se om PDF-sidor innehåller skärmärken, registreringsmål eller färgfält. Dessa märken avgör var papperet ska skäras när dokumenten skrivs ut. måste tas bort innan din eCatalog kan placeras på webben. I Adobe Dynamic Media Classic finns alternativ för beskärningsmärken när du överför PDF-filer.
* Om du vill att tittarna ska söka i din e-katalog med nyckelord, ta reda på om dina PDF-filer är förenklade. Du kan inte extrahera sökord från sammanslagna PDF-filer. Om du vill ta reda på om en PDF är förenklad kan du försöka markera text i den. Om du inte kan markera text förenklas PDF och visningsprogrammen kan inte söka efter nyckelord i din eCatalog.
* Eftersom de ska skrivas ut innehåller PDF vanligtvis CMYK-bilder. Som standard kan Adobe Dynamic Media Classic identifiera dessa CMYK-bilder på ett intelligent sätt och konvertera dem med en intern CMYK-färgprofil. Om du vill använda en egen färgprofil för att konvertera CMYK-bilder kan du göra det.

   Se [ICC-profiler (International Color Consortium)](icc-profiles.md#icc_profiles).

## Överföringsalternativ för PDF {#best-practice-pdf-upload-options}

Mer information om de olika överföringsmetoderna finns i [Överför filer](uploading-files.md#uploading_your_files).

Markera de filer som du vill överföra och välj sedan dessa *bästa praxis* Alternativ för PDF:

* **Beskärningsalternativ** - I dialogrutan Alternativ för överföring av jobb väljer du **[!UICONTROL Crop Options]**. Om PDF-sidorna innehåller skärmärken, passmärken eller andra märken finns det **[!UICONTROL Crop]** nedrullningsbar lista, välja **[!UICONTROL Manual]**. Ange antalet pixlar att beskära från sidans övre, högra, nedre och vänstra sidor. Skärmärken är ofta inställda på en halv-tumsmarginal. Anta att du väljer **[!UICONTROL 150]** (rekommenderas) som pixelupplösning och anger 75, 75, 75, 75, 75 i textrutorna Överkant, Höger, Underkant och Vänster. I så fall beskärs en halv tum från marginalerna (vid 150 ppi motsvarar hälften av 1 75 pixlar).

* **Bearbetar** - I dialogrutan Alternativ för överföring av jobb väljer du **[!UICONTROL PDF Options]**. I **[!UICONTROL Processing]** nedrullningsbar lista, välja **[!UICONTROL Rasterize]**. PDF måste rastreras så att alla sidor och bilder kan visas i eCatalog.

* **Extrahera sökord (valfritt)** - I dialogrutan Alternativ för överföring av jobb väljer du **[!UICONTROL PDF Options]**. Välj **[!UICONTROL Search words]** om du vill att tittarna ska kunna söka efter nyckelord i din eCatalog.

* **Generera eCatalog automatiskt från PDF med flera sidor (valfritt)** - I dialogrutan Alternativ för överföring av jobb väljer du **[!UICONTROL PDF Options]**. Välj **[!UICONTROL Auto-Generate eCatalog from multiple page PDF]** för att automatiskt skapa en e-katalog när du överför den. Du kan gå direkt till eCatalog-skärmen och börja arbeta med din eCatalog utan att först behöva markera PDF-filer och sedan välja kommandot Skapa. eCatalog får ett namn efter filen PDF.

* **Upplösning** - I dialogrutan Alternativ för överföring av jobb väljer du **[!UICONTROL PDF Options]**. I **[!UICONTROL Resolution]** anger du ett värde i textfältet. Adobe Dynamic Media Classic rekommenderar 150 pixlar per tum.

* **Färgrymd** - I dialogrutan Alternativ för överföring av jobb väljer du **[!UICONTROL PDF Options]**. Välj **[!UICONTROL Detect automatically]**. PDF som skapas för utskrift är vanligtvis i CMYK. PDF för onlinevisning är RGB. Om båda färgmodellerna används i ett PDF kan du välja en viss färgmodell genom att välja Använd som RGB eller Använd som CMYK. PDF använder båda färgmodellerna, till exempel när sidgrafik använder en CMYK-färgmodell, men RGB används i bilderna. Om du överförde en ICC-profil visas dess namn på menyn Färgrymd och du kan välja den där.

   Se [ICC-profiler (International Color Consortium)](/help/icc-profiles.md).

* **Alternativ för färgprofil** - I dialogrutan Alternativ för överföring av jobb väljer du **[!UICONTROL Color Profile Options]** och välj sedan ett färgprofilsalternativ:

   * **Behåll ursprunglig färgmodell** - Behåller den ursprungliga färgrymden.

   * **Anpassa från > Till** - Öppnar undermenyer så att du kan välja en **[!UICONTROL Convert From]** och **[!UICONTROL Convert To]** färgrymd. Du kan välja en standardfärgmodell för Photoshop eller en färgmodell som du har överfört till Adobe Dynamic Media Classic.

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

Se [ICC-profiler (International Color Consortium)](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Mer information om alla alternativ för PDF finns i [Överföringsalternativ för PDF](pdfs.md#pdf_upload_options).
