---
title: Länka en mall till en webbsida
description: Lär dig hur du länkar en mall till en webbsida i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
topic: Administration, Content Management, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Länka en mall till en webbsida{#linking-a-template-to-a-web-page}

Dina webbplatser och program får åtkomst till Dynamic Media Image Server-innehåll via URL-strängar. När du har publicerat en mall aktiverar Adobe Dynamic Media Classic en URL-sträng som refererar till mallen på dynamiska mediabildsservrar. Du kan klistra in den här URL:en i en webbläsare för testning.

Om du vill placera URL-strängar på webbsidor och i program kopierar du dem från Adobe Dynamic Media Classic. Om du vill hämta en mall-URL-sträng som genererats med en bildförinställning går du till förhandsgranskningsskärmen eller panelen Bläddra (i detaljvyn). Välj sedan en bildförinställning och klicka på knappen Kopiera URL.

>[!NOTE]
>
>URL:en är inte aktiv förrän du publicerar resursen.

## Hämta en mall-URL {#obtaining-a-template-url}

Du kan hämta en mall-URL-sträng som genereras av en bildförinställning från skärmen Förhandsvisa mall. När du har kopierat URL:en markeras den i Urklipp så att du kan klistra in den efter behov. Så här hämtar du en mall-URL-sträng som genererats med en bildförinställning från sidan Förhandsvisa mall:

1. Välj mallens överrullningsknapp **[!UICONTROL Preview]** eller gå till **[!UICONTROL File]** > **[!UICONTROL Preview]**.
1. Använd förinställningens menyer och välj den bildförinställning som du vill leverera mallbilden med. På sidan Förhandsgranska visas hur mallen ser ut när den levereras från servern.
1. Välj **[!UICONTROL Copy URL]** så att du kan kopiera URL:en till Urklipp.

## Lägga till mall-URL:er på webbsidan {#adding-template-urls-to-your-web-page}

Om du vill lägga till en mall på din webbsida kontaktar du webbsidans utvecklingsteam för att ändra taggen `<IMG>` i HTML webbsideskod. Använd Adobe Dynamic Media Classic URL-sträng för att göra en begäran till dynamiska mediabildsservrar. Handelsmotorn eller den dynamiska webbsideskoden infogar mallbilden med den storlek och formateringsspecifikation som definieras av den bildförinställning som du väljer för mallen.

>[!MORELIKETHIS]
>
>* [Lägg till dynamiska bilder på din webbsida](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
