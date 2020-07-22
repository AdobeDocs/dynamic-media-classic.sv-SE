---
title: Överför mallfiler
seo-title: Överför mallfiler
description: 'null'
seo-description: Lär dig hur du överför mallfiler.
uuid: e19979b5-3f41-49c5-99aa-107ede3be98c
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 75658717-5c39-473e-9d32-718d00706310
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 1%

---


# Överför mallfiler{#uploading-template-files}

Överför de filer du behöver för mallen till Dynamic Media Classic innan du börjar skapa mallen. Du kan skapa mallar från en Adobe® Photoshop® PSD-fil eller en bildfil. TIFF- och PNG-bilder rekommenderas eftersom de tillåter genomskinlighet.

>[!NOTE]
>
>Dynamic Media Classic rekommenderar att du använder genomskinliga TIFF- eller PSD-bilder i mallarna med exakt den storlek som du vill visa dem på webbplatsen. När du publicerar mallen anropar du bilden med en bildförinställning som också har samma storlek. Tänk på storleken för att se till att mallens storlek inte ändras (samplas om) med en storlek som är större eller mindre än den storlek som mallen är avsedd för.

Mallar kan skapas från Adobe Photoshop PSD-filer eller bildfiler.

Detaljerade instruktioner om hur du överför filer finns i [Överföra filer](uploading-files.md#uploading_files). Tänk på följande när du överför mallfiler:

* Om du överför en PSD-fil kan du skapa en mall utifrån den. I Dynamic Media Classic skapas en separat bild för varje lager i PSD-filen. I dialogrutan Alternativ för överföringsjobb väljer du Photoshop-alternativ, markerar alternativet Behåll lager och väljer alternativet Skapa mall. Välj sedan ett alternativ på menyn Lagernamn för att namnge bilderna som skapas i Dynamic Media Classic från lager i PSD-filen. Se [PSD-överföringsalternativ](psd-files.md#psd_upload_options).
* Om du överför bilder kan du skapa en mask från urklippsbanan. Det här alternativet gäller bilder som skapats med bildredigeringsprogram där en urklippsbana har skapats. I dialogrutan Alternativ för överföringsjobb väljer du Bildredigeringsalternativ och väljer alternativet Skapa mask från urklippsbana. Se [Bildredigeringsalternativ vid överföring](image-editing-options-upload.md#image-editing-options-at-upload).

>[!MORELIKETHIS]
>
>* [Överför filer](uploading-files.md#uploading_your_files)
>* [Arbeta med PSD-filer ](psd-files.md#working_with_psd_files)

