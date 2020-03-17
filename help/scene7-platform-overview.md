---
title: Adobe Dynamic Media Classic - plattformsöversikt
seo-title: Adobe Dynamic Media Classic - plattformsöversikt
description: 'null'
seo-description: En översikt över den dynamiska Media Classic-plattformen och arbetsflödesprocessen.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Adobe Dynamic Media Classic - plattformsöversikt{#adobe-scene-platform-overview}

Dynamic Media Classic är en integrerad miljö för hantering, publicering och service av multimedia. Multimedia kan levereras till alla marknadsförings- och säljkanaler, inklusive webben, trycksaker, e-postkampanjer, webbportaler, datorer och enheter.

## Arbetsflödesprocess {#workflow-process}

De viktigaste stegen i det dynamiska arbetsflödet är:

* **Överför och hantera dina mediefiler**&#x200B;Överför dina mediefiler till SPS. Du kan ordna, bläddra bland och söka efter resurser i systemet. Du kan också använda metadata för resurser. Om du installerar skrivbordsprogrammet Adobe Scene7 Publishing System kan du överföra filer och mappar genom att dra dem från skrivbordet till en överföringsmapp.

* **Skapa multimedia** Skapa olika konfigurationer av dina resurser som eCatalogs, Image Sets, Spin Sets, Swatch Sets, Mixed Media Sets, Basic Templates och FXG Templates. Mer information finns i Om multimedia.

* **Publicera och administrera** publiceringsresurser i Dynamic Media Classic Saas-nätverket samt övervaka status för resurser när de publiceras, administrera användarrättigheter och upprätthålla säkerheten.

* **Leverera** media från Dynamic Media Classic SaaS-nätverk till webbsidor, tillämpningar och mobila enheter. mediet är prestandaoptimerat och levereras med CDN-cachning. I Dynamic Media Classic finns en URL för varje resurs. När du har publicerat resursen blir URL-adressen aktiv.

![Arbetsflödet i Dynamic Media Classic](/help/assets/gs_workflow.png)

## Enstaka mallbilder och enstaka URL-anrop {#single-master-images-and-single-url-calls}

Dynamic Media Classic skiljer sig i grunden från andra system eftersom du kan använda Dynamic Media Classic för att leverera media dynamiskt från en huvudresurs och URL-anrop.

De URL-strängar du genererar med Dynamic Media Classic innehåller instruktioner som talar om för servern hur resursen ska visas när den levereras. Samma mallbild kan till exempel visas i olika storlekar, format, vikter, färger och zoomningsvyer. Som en del av arbetet med att bygga och publicera medieresurser med Dynamic Media Classic konfigurerar du effekterna visuellt. När du gör det skapar du URL-anrop som talar om för servern hur huvudresursen ska visas för program.

![Dynamic Media Classic kan leverera samma huvudbild till olika medier i olika storlekar och format.](/help/assets/gs_dynamic_publishing.png)

## Cachelagring av innehåll {#content-caching}

De bilder som Dynamic Media Classic genererar dynamiskt är cachevänliga. I de flesta fall är de JPEG-bilder med unika URL-anrop som identifierar dem. Bilderna levereras i leveransnätverket (CDN), ett system med servrar som är sammankopplade på Internet för att leverera innehåll snabbare. Bilderna distribueras från servrar som finns globalt och sedan till datorer. När du implementerar en cachningsmekanism med valfri CDN-leverantör ändrar du bara servernamnet så att det pekar på den CDN-aktiverade Dynamic Media Image-servern. Alla Dynamic Media Classic-utgåvor innehåller CDN-cachelagring i paket.
