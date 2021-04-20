---
title: Länka en mall till en webbsida
description: Lär dig hur du länkar en mall till en webbsida.
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
feature: Dynamic Media Classic
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---


# Länka en mall till en webbsida{#linking-a-template-to-a-web-page}

Dina webbplatser och program har åtkomst till Dynamic Media Image Server-innehåll via URL-strängar. När du har publicerat en mall aktiverar Dynamic Media Classic en URL-sträng som refererar till mallen på Dynamic Media Image-servrar. Du kan klistra in den här URL:en i en webbläsare för testning.

Om du vill placera URL-strängar på webbsidor och i program kopierar du dem från Dynamic Media Classic. Om du vill hämta en mall-URL-sträng som genererats med en bildförinställning går du till förhandsgranskningsskärmen eller panelen Bläddra (i detaljvyn). Välj sedan en bildförinställning och klicka på knappen Kopiera URL.

>[!NOTE]
>
>URL:en är inte aktiv förrän du publicerar resursen.

## Hämta en mall-URL {#obtaining-a-template-url}

Du kan hämta en mall-URL-sträng som genereras av en bildförinställning från skärmen Förhandsvisa mall. När du har kopierat URL:en markeras den i Urklipp så att du kan klistra in den efter behov. Följ de här stegen för att hämta en mall-URL-sträng som genereras med en bildförinställning från skärmen Förhandsvisa mall:

1. Klicka på mallens förhandsgranskningsknapp eller välj Arkiv > Förhandsgranska. Förhandsgranskningsskärmen öppnas.
1. Använd förinställningens menyer och välj den bildförinställning som du vill leverera mallbilden med. På förhandsgranskningsskärmen visas hur mallen ser ut när den levereras från servern.
1. Klicka på knappen Kopiera URL för att kopiera URL-adressen till Urklipp.

## Lägga till mall-URL:er på webbsidan {#adding-template-urls-to-your-web-page}

Om du vill lägga till en mall på en webbsida ska du rådfråga webbsidans utvecklingsteam och ändra taggen `<IMG>` i HTML-webbsideskoden med hjälp av URL-strängen för Dynamic Media Classic och göra en förfrågan till Dynamic Media Image Servers. Handelsmotorn eller den dynamiska webbsideskoden infogar mallbilden med den storlek och formateringsspecifikation som definieras av den bildförinställning som du väljer för mallen.

>[!MORELIKETHIS]
>
>* [Lägga till dynamiska bilder på webbsidan](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

