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
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Adobe Dynamic Media Classic - programöversikt{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic är en integrerad miljö för hantering, publicering och hantering av multimedia. Multimedia kan levereras till alla marknadsförings- och säljkanaler. Dessa kanaler omfattar webben, trycksaker, e-postkampanjer, webbportaler, datorer och enheter.

Se även utbildningsvideon [Plattformsöversikt](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS).

## Arbetsflödesprocess {#workflow-process}

De viktigaste stegen i Adobe Dynamic Media Classic arbetsflöde är:

* **Överför och hantera dina mediefiler**: Överför dina mediefiler till Adobe Dynamic Media Classic. Du kan ordna, bläddra bland och söka efter resurser i systemet. Du kan också använda metadata för resurser.

* **Skapa multimedia**: Skapa olika konfigurationer av dina resurser, till exempel eCatalogs, Image Sets, Spin Sets, Swatch Sets, Mixed Media Sets, Basic Templates och FXG Templates.

* **Publicera och administrera**: Publicera resurser i Adobe Dynamic Media Classic SaaS-nätverket. Övervaka status för resurser när de publiceras. Administrera användarrättigheter och bevara säkerheten.

* **Server**: Leverera media från Adobe Dynamic Media Classic SaaS-nätverk till webbsidor, program och mobila enheter. Mediet är prestandaoptimerat och levereras med CDN-cachning. Adobe Dynamic Media Classic tillhandahåller en URL för varje resurs. När du har publicerat resursen blir URL-adressen aktiv.

![Adobe Dynamic Media Classic arbetsflödesprocess](/help/using/assets/gs_workflow.png)

## Enstaka primära bilder och enstaka URL-anrop {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic skiljer sig i grunden från andra system eftersom du kan använda Adobe Dynamic Media Classic för att leverera media dynamiskt från enskilda primära resurser och URL-anrop.

De URL-strängar som du har skapat med Adobe Dynamic Media Classic innehåller instruktioner som talar om för servern hur resursen ska visas när den levereras. Samma primära bild kan till exempel visas i olika storlekar, format, vikter, färger och zoomningsvyer. Som en del av arbetet med att skapa och publicera medieresurser med Adobe Dynamic Media Classic kan du visuellt konfigurera effekterna. När du gör det skapar du URL-anrop som talar om för servern hur den primära resursen ska visas för program.

![Adobe Dynamic Media Classic kan leverera samma primära bild till olika medier i olika storlekar och format.](/help/using/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic ser till att enhetliga upplevelser av hög kvalitet levereras till alla skärmar, oavsett storlek och bandbredd.*

## Cachelagring av innehåll {#content-caching}

De bilder som Adobe Dynamic Media Classic genererar dynamiskt är cachelagrade, vanligtvis JPEG-bilder med unika URL-anrop som identifierar dem. Bilderna levereras i leveransnätverket (CDN), ett system med servrar som är sammankopplade på Internet för att leverera innehåll snabbare. Bilderna distribueras från servrar som finns globalt och sedan till datorer. När du implementerar en cachningsmekanism med valfri CDN-leverantör ändrar du bara servernamnet så att det pekar på den CDN-aktiverade Dynamic Media Image-servern. Alla Adobe Dynamic Media Classic-utgåvor innehåller CDN-cache.
