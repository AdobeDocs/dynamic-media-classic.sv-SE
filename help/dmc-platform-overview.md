---
title: Adobe Dynamic Media Classic - plattformsöversikt
description: En översikt över Dynamic Media Classic-plattformen och arbetsflödesprocessen.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Administratör,Affärsledare
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---


# Adobe Dynamic Media Classic-plattformen - översikt{#adobe-scene-platform-overview}

Dynamic Media Classic är en integrerad miljö för hantering, publicering och visning av multimedia. Multimedia kan levereras till alla marknadsförings- och säljkanaler, inklusive webben, trycksaker, e-postkampanjer, webbportaler, datorer och enheter.

## Arbetsflödesprocess {#workflow-process}

De viktigaste stegen i Dynamic Media Classic-arbetsflödet är:

* **Överför och hantera dina**
mediefilerÖverför dina mediefiler till Dynamic Media Classic. Du kan ordna, bläddra bland och söka efter resurser i systemet. Du kan också använda metadata för resurser.

* **Skapa**
multimediaSkapa olika konfigurationer av resurser som eCatalogs, Image Sets, Spin Sets, Swatch Sets, Mixed Media Sets, Basic Templates och FXG Templates. Mer information finns i Om multimedia.

* **Publicera och**
administreraPublicera material i Dynamic Media Classic Saas-nätverket samt övervaka status för mediefiler när de publiceras, administrera användarrättigheter och upprätthålla säkerheten.

* ****
ServeLeverera medier från Dynamic Media Classic SaaS-nätverk till webbsidor, tillämpningar och mobila enheter, mediet är prestandaoptimerat och levereras med CDN-cachning. I Dynamic Media Classic finns en URL för varje resurs. När du har publicerat resursen blir URL-adressen aktiv.

![Arbetsflödesprocessen i Dynamic Media Classic](/help/assets/gs_workflow.png)

## Enstaka överordnad bilder och enstaka URL-anrop {#single-master-images-and-single-url-calls}

Dynamic Media Classic skiljer sig i grunden från andra system eftersom du kan använda Dynamic Media Classic för att leverera media dynamiskt från enstaka överordnad resurser och URL-anrop.

De URL-strängar du genererar med Dynamic Media Classic innehåller instruktioner som talar om för servern hur resursen ska visas när den levereras. Samma överordnad bild kan till exempel visas i olika storlekar, format, vikter, färger och zoomningsvyer. När du bygger och publicerar medieresurser med Dynamic Media Classic konfigureras effekterna visuellt. När du gör det skapar du URL-anrop som talar om för servern hur du ska presentera din överordnad resurs för program.

![Dynamic Media Classic kan leverera samma överordnad bild till olika medier i olika storlekar och format.](/help/assets/gs_dynamic_publishing.png)

## Cachelagring av innehåll {#content-caching}

De bilder som Dynamic Media Classic skapar dynamiskt är cachevänliga. I de flesta fall är de JPEG-bilder med unika URL-anrop som identifierar dem. Bilderna levereras i leveransnätverket (CDN), ett system med servrar som är sammankopplade på Internet för att leverera innehåll snabbare. Bilderna distribueras från servrar som finns globalt och sedan till datorer. När du implementerar en cachningsmekanism med en CDN-leverantör ändrar du bara servernamnet så att det pekar på den CDN-aktiverade Dynamic Media Image Server. Alla Dynamic Media Classic-utgåvor innehåller CDN-cachelagring i paket.
