---
title: Adobe Dynamic Media Classic - programöversikt
description: En översikt över Adobe Dynamic Media Classic och hela arbetsflödesprocessen.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
source-git-commit: 2616c067215196e8145043ba57fba1e3a5667cdc
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---

# Adobe Dynamic Media Classic - programöversikt{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic är en integrerad miljö för hantering, publicering och hantering av multimedia. Multimedia kan levereras till alla marknadsförings- och säljkanaler, inklusive webben, trycksaker, e-postkampanjer, webbportaler, datorer och enheter.

Se även [Plattformsöversikt](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS) utbildningsvideo.

## Arbetsflödesprocess {#workflow-process}

De viktigaste stegen i Adobe Dynamic Media Classic arbetsflöde är:

* **Överför och hantera mediefiler**  - Överför mediefiler till Adobe Dynamic Media Classic. Du kan ordna, bläddra bland och söka efter resurser i systemet. Du kan också använda metadata för resurser.

* **Skapa multimedia** - Skapa olika konfigurationer av dina resurser, t.ex. eCatalogs, Image Sets, Spin Sets, Swatch Sets, Mixed Media Sets, Basic Templates och FXG Templates.

* **Publicera och administrera**  - Publicera material i Adobe Dynamic Media Classic SaaS-nätverket. Övervaka status för resurser när de publiceras. Administrera användarrättigheter och bevara säkerheten.

* **Serve** - Leverera media från Adobe Dynamic Media Classic SaaS-nätverk till webbsidor, tillämpningar och mobila enheter. mediet är prestandaoptimerat och levereras med CDN-cachning. Adobe Dynamic Media Classic tillhandahåller en URL för varje resurs. När du har publicerat resursen blir URL-adressen aktiv.

![Adobe Dynamic Media Classic arbetsflöde](/help/assets/gs_workflow.png)

## Enstaka överordnad bilder och enstaka URL-anrop {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic skiljer sig i grunden från andra system eftersom du kan använda Adobe Dynamic Media Classic för att leverera media dynamiskt från enstaka överordnad resurser och URL-anrop.

De URL-strängar du skapar med Adobe Dynamic Media Classic innehåller instruktioner som talar om för servern hur resursen ska visas när den levereras. Samma överordnad bild kan till exempel visas i olika storlekar, format, vikter, färger och zoomningsvyer. Som en del av arbetet med att skapa och publicera mediematerial med Adobe Dynamic Media Classic kan du visuellt konfigurera effekterna. När du gör det skapar du URL-anrop som talar om för servern hur du ska presentera din överordnad resurs för program.

![Adobe Dynamic Media Classic kan leverera samma överordnad bild till olika medier i olika storlekar och format.](/help/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic ser till att enhetliga upplevelser av hög kvalitet levereras till alla skärmar, oavsett storlek och bandbredd.*

## Cachelagring av innehåll {#content-caching}

De bilder som Adobe Dynamic Media Classic genererar dynamiskt är cachevänliga. oftast är de bilder i JPEG med unika URL-anrop som identifierar dem. Bilderna levereras i leveransnätverket (CDN), ett system med servrar som är sammankopplade på Internet för att leverera innehåll snabbare. Bilderna distribueras från servrar som finns globalt och sedan till datorer. När du implementerar en cachningsmekanism med en CDN-leverantör ändrar du bara servernamnet så att det pekar på den CDN-aktiverade Dynamic Media Image Server. Alla Adobe Dynamic Media Classic-utgåvor innehåller CDN-cache.
