---
title: Dynamic Media begränsningar
description: Lär dig mer om de effektivaste strategierna och de tvingande gränserna när du skapar en bilduppsättning eller en snurruppsättning, eller överför en PDF. Läs också om webbläsarkombinationer och operativsystemkombinationer som inte stöds för Dynamic Media.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Asset Management,Image Sets,Spin Sets,eCatalog
role: User
exl-id: ee30a2c1-2b26-41bd-8758-e7337a3727bb
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 1%

---

# Dynamic Media-begränsningar

I följande avsnitt beskrivs begränsningar i Dynamic Media.

Det här avsnittet innehåller följande avsnitt:

* [Dynamic Media bästa praxis och tvingande begränsningar för tillgångstyper](#best-practice-enforced-limits)
* [Webbläsare och operativsystem som inte stöds för Dynamic Media](#unsupported-browser-os)

## Dynamic Media bästa praxis och tvingande begränsningar för tillgångstyper {#best-practice-enforced-limits}

När du skapar en snurra uppsättning eller en bilduppsättning, eller överför PDF för sidextrahering, rekommenderar Adobe följande metodtips. Adobe tillämpar även följande begränsningar:

| Tillgång: Begränsningstyp | Bästa praxis | Begränsning har införts |
| --- | --- | --- |
| **Bild**: Antal smarta beskärningar per bild | 5 | 100 |
| **Alla uppsättningar**: Antal dubblettresurser per uppsättning | Inga dubbletter | 20‡ |
| **Alla uppsättningar**: Maximalt antal resurser per uppsättning | 5-10 bilder per uppsättning | 1000 |
| **Snurra uppsättning**: Maximalt antal rader/kolumner per 2D-uppsättning | 12-18 bilder per uppsättning | 1000 |
| **PDF**: Maximalt antal sidor för en PDF som ska tas i beaktande för extrahering |  | 100 (för alla PDF) |

‡ Bästa praxis är att inte ha duplicerade resurser i en uppsättning. Gränsen är 20 kopior för en enskild resurs. Om du lägger till ytterligare en dubblett för den resursen, inom den uppsättningen, returnerar begäran ett fel eller ignorerar dubbletten.

<!-- See also [Dynamic Media limitations](/help/using/assets/limitations.md). -->

## Webbläsare och operativsystem som inte stöds för Dynamic Media {#unsupported-browser-os}

<!-- CQDOC-19433 -->

Adobe Dynamic Media stöder inte följande kombinationer av webbläsare och operativsystem.

* Internet Explorer 11 + Windows 7
* Internet Explorer 11 + Windows 8.1
* Internet Explorer 11 + Windows Phone 8.1
* Internet Explorer 11 + Windows Phone 8.1 - uppdatering
* Safari 6 + iOS 6.0.1
* Safari 7 + iOS 7.1
* Safari 7 + OS X 10.9 Mavericks
* Safari 8 + iOS 8.4
* Safari 8 + OS X 10.10 Yosemite

## Stöd för Secure Socket Layer 2.0 och 3.0 samt Transport Layer Security 1.0 och 1.1 har upphört {#tls}

<!-- CQDOC-19433 (original ticket)
and CQDOC-19792 (removed as per this ticket December 5, 2022) -->

Från och med den 30 april 2024 upphör Adobe Dynamic Media med stödet för följande:

* SSL (Secure Socket Layer) 2.0
* SSL 3.0
* TLS (Transport Layer Security) 1.0 och 1.1
* Följande svaga lärare i TLS 1.2:
   * `TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384`
   * `TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA`
   * `TLS_RSA_WITH_AES_256_GCM_SHA384`
   * `TLS_RSA_WITH_AES_256_CBC_SHA256`
   * `TLS_RSA_WITH_AES_256_CBC_SHA`
   * `TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA256`
   * `TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA`
   * `TLS_RSA_WITH_AES_128_GCM_SHA256`
   * `TLS_RSA_WITH_AES_128_CBC_SHA256`
   * `TLS_RSA_WITH_AES_128_CBC_SHA`
   * `TLS_RSA_WITH_CAMELLIA_256_CBC_SHA`
   * `TLS_RSA_WITH_CAMELLIA_128_CBC_SHA`
   * `TLS_ECDHE_RSA_WITH_3DES_EDE_CBC_SHA`
   * `TLS_RSA_WITH_SDES_EDE_CBC_SHA`

