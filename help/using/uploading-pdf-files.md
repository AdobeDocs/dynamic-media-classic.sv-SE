---
title: Överför PDF-filer
description: Lär dig hur du överför PDF-filer som är kopplade till en e-katalog i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
topic: Integrations, Development
level: Experienced
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 0%

---

# Överför PDF-filer{#uploading-the-pdf-files}

Vanligtvis är Adobe PDF-filer källa för en e-katalog. Dessa filer innehåller all bildinformation, teckensnitt och vektorgrafik. Du kan även skapa en e-katalog med bilder. När du har förberett dina PDF-filer för överföring väljer du **[!UICONTROL Upload]** i fältet Global navigering för att börja överföra PDF.

När du överför en PDF för sidextrahering använder Adobe följande gräns:

| Begränsningstyp för PDF | Begränsning har införts | Ändring till begränsning den 31 december 2022 |
| --- | --- | --- |
| Högsta antal sidor för PDF som ska övervägas för extrahering | 5000 (för nya överföringar) | 100 (för alla PDF) |

Se även [Dynamic Media-begränsningar](/help/using/limitations.md).

## Förbered dina PDF-filer

Förbered dina PDF-filer innan du överför dem till Adobe Dynamic Media Classic:

* Om du vill göra det enklare att överföra filerna placerar du alla filer i samma mapp på datorn eller i nätverket.
* Namnge filerna i alfanumerisk ordning per sida. Om du beställer sidorna blir det enklare att placera sidorna i rätt ordning efter att filerna har överförts.
* Granska sidorna om du vill se om PDF-sidor innehåller skärmärken, registreringsmål eller färgfält. Dessa märken avgör var papperet ska skäras ut när dokument skrivs ut. De måste tas bort innan e-katalogen kan placeras på webben. I Adobe Dynamic Media Classic finns alternativ för beskärningsmärken när du överför PDF-filer.
* Om du vill att tittarna ska söka i din e-katalog med nyckelord, ta reda på om dina PDF-filer är förenklade. Du kan inte extrahera sökord från sammanslagna PDF-filer. Om du vill ta reda på om ett PDF är förenklat kan du försöka markera texten i det. Om du inte kan markera text förenklas PDF och visningsprogrammen kan inte söka efter nyckelord i din eCatalog.
* Eftersom de ska skrivas ut innehåller PDF vanligtvis CMYK-bilder. Som standard kan Adobe Dynamic Media Classic identifiera dessa CMYK-bilder på ett intelligent sätt och konvertera dem med en intern CMYK-färgprofil. Om du vill använda en egen färgprofil för att konvertera CMYK-bilder kan du göra det.

  Se [ICC-profiler (International Color Consortium)](icc-profiles.md#icc_profiles).

## Överföringsalternativ för PDF {#best-practice-pdf-upload-options}

Mer information om de olika överföringsmetoderna finns i [Överföra filer](uploading-files.md#uploading_your_files).

Markera de filer som du vill överföra och välj sedan följande *bästa praxis*-alternativ för PDF:

* **Beskärningsalternativ**: Välj **[!UICONTROL Crop Options]** i dialogrutan Alternativ för överföringsjobb. Om PDF-sidorna innehåller skärmärken, passmärken eller andra märken väljer du **[!UICONTROL Manual]** i listrutan **[!UICONTROL Crop]**. Ange antalet pixlar att beskära från sidans övre, högra, nedre och vänstra sidor. Skärmärken är ofta inställda på en halv-tumsmarginal. Anta att du väljer **[!UICONTROL 150]** (rekommenderas) som pixel per tum-upplösning. Sedan anger du 75, 75, 75, 75 i textrutorna Överkant, Höger, Underkant och Vänster. I så fall beskärs en halv tum från marginalerna (vid 150 ppi motsvarar hälften av 1 75 pixlar).

* **Bearbetar**: Välj **[!UICONTROL PDF Options]** i dialogrutan Alternativ för överföringsjobb. Välj **[!UICONTROL Rasterize]** i listrutan **[!UICONTROL Processing]**. PDF måste rastreras så att alla sidor och bilder kan visas i eCatalog.

* **Extrahera sökord (valfritt)**: Välj **[!UICONTROL PDF Options]** i dialogrutan Alternativ för överföringsjobb. Välj **[!UICONTROL Search words]** i den nedrullningsbara listan Extract om du vill att dina visningsprogram ska kunna söka efter nyckelord i din eCatalog.

* **Skapa eCatalog automatiskt från flera sidor PDF (valfritt)**: I dialogrutan Alternativ för överföringsjobb väljer du **[!UICONTROL PDF Options]**. Klicka på **[!UICONTROL Auto-Generate eCatalog from multiple page PDF]** så att du automatiskt kan skapa en e-katalog när du överför den. Du kan gå direkt till eCatalog-skärmen och börja arbeta med din eCatalog utan att först behöva markera PDF-filer och sedan välja kommandot Skapa. eCatalog får ett namn efter filen PDF.

* **Upplösning**: Välj **[!UICONTROL PDF Options]** i dialogrutan Alternativ för överföringsjobb. Ange ett värde i textfältet **[!UICONTROL Resolution]**. Adobe Dynamic Media Classic rekommenderar 150 pixlar per tum.

* **Färgrymd**: Välj **[!UICONTROL PDF Options]** i dialogrutan Alternativ för överföringsjobb. Välj **[!UICONTROL Detect automatically]** i listrutan Färgrymd. PDF som skapas för utskrift är normalt i CMYK, medan PDF för visning online är RGB. Om båda färgmodellerna används i ett PDF kan du välja en viss färgmodell genom att välja Använd som RGB eller Använd som CMYK. PDF använder båda färgmodellerna, till exempel när sidgrafik använder en CMYK-färgmodell, men RGB används i bilderna. Om du överförde en ICC-profil visas dess namn på menyn Färgrymd och du kan välja den där.

  Se [ICC-profiler (International Color Consortium)](/help/using/icc-profiles.md).

* **Alternativ för färgprofil**: I dialogrutan Alternativ för överföringsjobb väljer du **[!UICONTROL Color Profile Options]** och sedan ett alternativ för färgprofil:

   * **Behåll ursprunglig färgmodell**: Behåller den ursprungliga färgmodellen.

   * **Anpassad från > Till**: Öppnar undermenyer så att du kan välja en **[!UICONTROL Convert From]** - och **[!UICONTROL Convert To]**-färgrymd. Du kan välja en standardfärgmodell för Photoshop eller en färgmodell som du har överfört till Adobe Dynamic Media Classic.

<!-- * **Convert To SRGB**: Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on Web pages. -->

Se [ICC-profiler (International Color Consortium)](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Mer information om alla överföringsalternativ för PDF finns i [PDF](pdfs.md#pdf_upload_options).
