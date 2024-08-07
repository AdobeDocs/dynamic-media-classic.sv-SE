---
title: Överför mallfiler
description: Lär dig hur du överför mallfiler i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: a105c18a-7e06-43cb-938c-a3bcdc3e9d22
topic: Content Management
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Överför mallfiler{#uploading-template-files}

Överför de filer du behöver för mallen till Adobe Dynamic Media Classic innan du börjar skapa mallen. Du kan skapa mallar från en Adobe® Photoshop®-PSD eller en bildfil. TIFF- och PNG-bilder rekommenderas eftersom de tillåter genomskinlighet.

>[!NOTE]
>
>Adobe Dynamic Media Classic rekommenderar att du använder genomskinliga bilder i TIFF eller PSD i mallarna i exakt den storlek som du vill visa dem på din webbplats. När du publicerar mallen anropar du bilden med en bildförinställning som också har samma storlek. Tänk på storleken för att se till att mallens storlek inte ändras (samplas om) med en storlek som är större eller mindre än den storlek som mallen är avsedd för.

Mallar kan skapas från Adobe Photoshop PSD-filer eller bildfiler.

Detaljerade instruktioner om hur du överför filer finns i [Överför filer](uploading-files.md#uploading_files). Tänk på följande när du överför mallfiler:

* Om du överför en PSD-fil kan du skapa en mall utifrån den. Adobe Dynamic Media Classic skapar en separat bild för varje lager i PSD. I dialogrutan Alternativ för överföring av jobb väljer du **[!UICONTROL Photoshop Options]** och sedan **[!UICONTROL Maintain Layers]** och **[!UICONTROL Create Template]**. Välj sedan ett alternativ i listrutan **[!UICONTROL Layer Naming]** för att namnge de bilder som Adobe Dynamic Media Classic skapar från lager i PSD.
Se [Överföringsalternativ för PSD](psd-files.md#psd_upload_options).
<!-- THERE IS NO LONGER AN IMAGE EDITING OPTIONS MENU * If you are uploading images, you can create a mask from its clipping path. This option applies to images created with image-editing applications in which a clipping path was created. In the Upload Job Options dialog box, select Image Editing Options and select the Create Mask From Clipping Path option. 
See [Image editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload). -->

>[!MORELIKETHIS]
>
>* [Överför dina filer](uploading-files.md#uploading_your_files)
>* [Arbeta med PSD-filer](psd-files.md#working_with_psd_files)
