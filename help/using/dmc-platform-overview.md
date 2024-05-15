---
title: Adobe Dynamic Media Classic - programöversikt
description: En översikt över Adobe Dynamic Media Classic och hela arbetsflödesprocessen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
topic: Administration
level: Beginner
source-git-commit: edd893482cbafd9674a44cf9878b8ee3079d98f7
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Adobe Dynamic Media Classic - programöversikt{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic är en integrerad miljö för hantering, publicering och hantering av multimedia. Multimedia kan levereras till alla marknadsförings- och säljkanaler. Dessa kanaler omfattar webben, trycksaker, e-postkampanjer, webbportaler, datorer och enheter.

Se även [Plattformsöversikt](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS) utbildningsvideo.

## Arbetsflödesprocess {#workflow-process}

De viktigaste stegen i Adobe Dynamic Media Classic arbetsflöde är:

* **Överför och hantera dina resurser** - Överför mediefiler till Adobe Dynamic Media Classic. Du kan ordna, bläddra bland och söka efter resurser i systemet. Du kan också använda metadata för resurser.

* **Skapa multimedia** - Skapa olika konfigurationer av dina resurser, t.ex. eCatalogs, Image Sets, Spin Sets, Swatch Sets, Mixed Media Sets, Basic Templates och FXG Templates.

* **Publicera och administrera** - Publicera material i Adobe Dynamic Media Classic SaaS-nätverket. Övervaka status för resurser när de publiceras. Administrera användarrättigheter och bevara säkerheten.

* **Serva** - Leverera media från Adobe Dynamic Media Classic SaaS-nätverk till webbsidor, applikationer och mobila enheter. Medierna är prestandaoptimerade och levereras med CDN-cachning. Adobe Dynamic Media Classic tillhandahåller en URL för varje resurs. När du har publicerat resursen blir URL-adressen aktiv.

![Adobe Dynamic Media Classic arbetsflöde](/help/using/assets/gs_workflow.png)

## Enstaka primära bilder och enstaka URL-anrop {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic skiljer sig i grunden från andra system eftersom du kan använda Adobe Dynamic Media Classic för att leverera media dynamiskt från enskilda primära resurser och URL-anrop.

De URL-strängar som du har skapat med Adobe Dynamic Media Classic innehåller instruktioner som talar om för servern hur resursen ska visas när den levereras. Samma primära bild kan till exempel visas i olika storlekar, format, vikter, färger och zoomningsvyer. Som en del av arbetet med att skapa och publicera medieresurser med Adobe Dynamic Media Classic kan du visuellt konfigurera effekterna. När du gör det skapar du URL-anrop som talar om för servern hur den primära resursen ska visas för program.

![Adobe Dynamic Media Classic kan leverera samma primära bild till olika medier i olika storlekar och format.](/help/using/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic ser till att enhetliga upplevelser av hög kvalitet levereras till alla skärmar, oavsett storlek och bandbredd.*

## Cachelagring av innehåll {#content-caching}

De bilder som Adobe Dynamic Media Classic genererar dynamiskt är cachelagrade, vanligen JPEG-bilder med unika URL-anrop som identifierar dem. Bilderna levereras i leveransnätverket (CDN), ett system med servrar som är sammankopplade på Internet för att leverera innehåll snabbare. Bilderna distribueras från servrar som finns globalt och sedan till datorer. När du implementerar en cachningsmekanism med en CDN-leverantör ändrar du bara servernamnet så att det pekar på den CDN-aktiverade Dynamic Media Image Server. Alla Adobe Dynamic Media Classic-utgåvor innehåller CDN-cache.
