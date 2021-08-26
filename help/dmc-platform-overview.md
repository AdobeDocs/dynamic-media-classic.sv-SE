---
title: Adobe Dynamic Media Classic - programöversikt
description: Översikt över programmet och arbetsflödet i Adobe Dynamic Media Classic.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Adobe Dynamic Media Classic - programöversikt{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic är en integrerad miljö för hantering, publicering och visning av multimedia. Multimedia kan levereras till alla marknadsförings- och säljkanaler, inklusive webben, trycksaker, e-postkampanjer, webbportaler, datorer och enheter.

## Arbetsflödesprocess {#workflow-process}

De viktigaste stegen i arbetsflödet för Adobe Dynamic Media Classic är:

* **Överför och hantera mediefiler**  - Överför mediefiler till Adobe Dynamic Media Classic. Du kan ordna, bläddra bland och söka efter resurser i systemet. Du kan också använda metadata för resurser.

* **Skapa multimedia** - Skapa olika konfigurationer av dina resurser, t.ex. eCatalogs, Image Sets, Spin Sets, Swatch Sets, Mixed Media Sets, Basic Templates och FXG Templates.

* **Publicera och administrera**  - Publicera material i Adobe Dynamic Media Classic SaaS-nätverket samt övervaka status för resurser när de publiceras, administrera användarrättigheter och upprätthålla säkerheten.

* **Serve** - Leverera media från Adobe Dynamic Media Classic SaaS-nätverk till webbsidor, tillämpningar och mobila enheter. mediet är prestandaoptimerat och levereras med CDN-cachning. I Adobe Dynamic Media Classic finns en URL för varje resurs. När du har publicerat resursen blir URL-adressen aktiv.

![Arbetsflödet i Adobe Dynamic Media Classic](/help/assets/gs_workflow.png)

## Enstaka överordnad bilder och enstaka URL-anrop {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic skiljer sig i grunden från andra system eftersom du kan använda Adobe Dynamic Media Classic för att leverera media dynamiskt från enstaka överordnad resurser och URL-anrop.

De URL-strängar som du genererar med Adobe Dynamic Media Classic innehåller instruktioner som talar om för servern hur resursen ska visas när den levereras. Samma överordnad bild kan till exempel visas i olika storlekar, format, vikter, färger och zoomningsvyer. När du bygger och publicerar medieresurser med Adobe Dynamic Media Classic konfigureras effekterna visuellt. När du gör det skapar du URL-anrop som talar om för servern hur du ska presentera din överordnad resurs för program.

![Adobe Dynamic Media Classic kan leverera samma överordnad bild till olika medier i olika storlekar och format.](/help/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic säkerställer att enhetliga upplevelser av hög kvalitet levereras till alla skärmar, oavsett storlek och bandbredd.*

## Cachelagring av innehåll {#content-caching}

De bilder som Adobe Dynamic Media Classic genererar dynamiskt är cachevänliga. oftast är de JPEG-bilder med unika URL-anrop som identifierar dem. Bilderna levereras i leveransnätverket (CDN), ett system med servrar som är sammankopplade på Internet för att leverera innehåll snabbare. Bilderna distribueras från servrar som finns globalt och sedan till datorer. När du implementerar en cachningsmekanism med en CDN-leverantör ändrar du bara servernamnet så att det pekar på den CDN-aktiverade Dynamic Media Image Server. Alla utgåvor av Adobe Dynamic Media Classic innehåller CDN-cachelagring.
