---
title: Ladda upp PDF-filerna
description: Lär dig hur du överför PDF-filer som är kopplade till en e-katalog i Adobe Dynamic Media Classic.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
source-git-commit: 8bc49ae3704f0551c70d68a0ddd63725bdcc645c
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# Ladda upp PDF-filerna{#uploading-the-pdf-files}

Vanligtvis är Adobe PDF-filer källa för en e-katalog. Dessa filer innehåller all bildinformation, teckensnitt och vektorgrafik. Du kan även skapa en e-katalog med bilder. När du har förberett dina PDF-filer för överföring väljer du **[!UICONTROL Upload]** i fältet Global Navigation (Global Navigation) för att börja överföra PDF-filerna.

## Förbered PDF-filer {#preparing-your-pdf-files}

Förbered PDF-filerna innan du överför dem till Adobe Dynamic Media Classic:

* Om du vill göra det enklare att överföra filerna placerar du alla filer i samma mapp på datorn eller i nätverket.
* Namnge filerna i alfanumerisk ordning per sida. Om du beställer sidorna blir det enklare att placera sidorna i rätt ordning efter att filerna har överförts.
* Granska sidorna om du vill se om PDF-sidorna innehåller skärmärken, registreringsmål eller färgfält. Dessa märken avgör var papperet ska skäras när dokumenten skrivs ut. måste tas bort innan din eCatalog kan placeras på webben. Adobe Dynamic Media Classic innehåller alternativ för beskärningsmärken när du överför PDF-filer.
* Om du vill att tittarna ska söka i din e-katalog med nyckelord, ta reda på om PDF-filerna är förenklade. Du kan inte extrahera sökord från förenklade PDF-filer. Om du vill ta reda på om en PDF-fil är förenklad kan du försöka markera text i den. Om du inte kan markera text förenklas PDF-filen och visningsprogrammen kan inte söka efter nyckelord i din eCatalog.
* Eftersom de ska skrivas ut innehåller PDF-filerna vanligtvis CMYK-bilder. Som standard kan Adobe Dynamic Media Classic identifiera dessa CMYK-bilder på ett intelligent sätt och konvertera dem med en intern CMYK-färgprofil. Om du vill använda en egen färgprofil för att konvertera CMYK-bilder kan du göra det.

   Se [ICC-profiler (International Color Consortium)](icc-profiles.md#icc_profiles).

## Överföringsalternativ för PDF med bästa praxis {#best-practice-pdf-upload-options}

Mer information om de olika överföringsmetoderna finns i [Överföra filer](uploading-files.md#uploading_your_files).

Markera de filer som du vill överföra och välj sedan följande *metodtips* PDF-alternativ:

* **Beskärningsalternativ**  - Välj  **[!UICONTROL Crop Options]**. Om PDF-sidorna innehåller skärmärken, passmärken eller andra märken väljer du **[!UICONTROL Manual]** i listrutan **[!UICONTROL Crop]**. Ange antalet pixlar att beskära från sidans övre, högra, nedre och vänstra sidor. Skärmärken är ofta inställda på en halv-tumsmarginal. Anta att du väljer **[!UICONTROL 150]** (rekommenderas) som pixel per tum-upplösning och anger 75, 75, 75, 75 i textrutorna Överkant, Höger, Underkant och Vänster. I så fall beskärs en halv tum från marginalerna (vid 150 ppi motsvarar hälften av 1 75 pixlar).

* **Bearbetning**  - I dialogrutan Alternativ för överföringsjobb väljer du  **[!UICONTROL PDF Options]**. Välj **[!UICONTROL Rasterize]** i listrutan **[!UICONTROL Processing]**. PDF-filen måste rastreras så att alla sidor och bilder kan visas i e-katalogen.

* **Extrahera sökord (valfritt)**  - Välj  **[!UICONTROL PDF Options]** i dialogrutan Alternativ för överföringsjobb. Välj **[!UICONTROL Search words]** i listrutan Extract om du vill att dina visningsprogram ska kunna söka efter nyckelord i din eCatalog.

* **Generera eCatalog automatiskt från PDF-fil med flera sidor (valfritt)**  - Välj  **[!UICONTROL PDF Options]** i dialogrutan Alternativ för överföringsjobb. Välj **[!UICONTROL Auto-Generate eCatalog from multiple page PDF]** om du vill skapa en e-katalog automatiskt när du överför. Du kan gå direkt till eCatalog-skärmen och börja arbeta med eCatalog utan att först behöva markera PDF-filer och sedan välja kommandot Skapa. eCatalog namnges efter PDF-filen.

* **Upplösning**  - I dialogrutan Alternativ för överföringsjobb väljer du  **[!UICONTROL PDF Options]**. Ange ett värde i textfältet **[!UICONTROL Resolution]**. Adobe Dynamic Media Classic rekommenderar 150 pixlar per tum.

* **Färgrymd**  - I dialogrutan Alternativ för överföringsjobb väljer du  **[!UICONTROL PDF Options]**. Välj **[!UICONTROL Detect automatically]** i listrutan Färgrymd. Vanligtvis är PDF-filer som skapats för utskrift CMYK. PDF-filer för visning online är RGB. Om båda färgrymderna används i en PDF-fil kan du välja en viss färgrymd genom att välja Använd som RGB eller Använd som CMYK. I PDF-filer används till exempel båda färgmodellerna när sidgrafik använder en CMYK-färgmodell, men bilder använder RGB. Om du överförde en ICC-profil visas dess namn på menyn Färgrymd och du kan välja den där.

   Se [ICC-profiler (International Color Consortium)](/help/icc-profiles.md).

* **Alternativ**  för färgprofil - I dialogrutan Alternativ för överföringsjobb väljer du  **[!UICONTROL Color Profile Options]** och sedan ett färgprofilsalternativ:

   * **Behåll ursprunglig färgmodell**  - Behåller den ursprungliga färgmodellen.

   * **Anpassad från > Till** - Öppnar undermenyer så att du kan välja en  **[!UICONTROL Convert From]** och  **[!UICONTROL Convert To]** en färgrymd. Du kan välja en standardfärgmodell för Photoshop eller en färgmodell som du har överfört till Adobe Dynamic Media Classic.

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

Se [ICC-profiler (International Color Consortium)](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Mer information om alla PDF-alternativ finns i [Alternativ för PDF-överföring](pdfs.md#pdf_upload_options).
