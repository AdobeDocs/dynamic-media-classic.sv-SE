---
title: Konfigurera bildförinställningar
description: Lär dig hur du ställer in bildförinställningar i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Image Presets
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 1%

---

# Konfigurera bildförinställningar{#setting-up-image-presets}

Precis som ett makro är en bildförinställning en fördefinierad samling kommandon för storleksändring och formatering som sparats under ett namn. Om du vill förstå hur bildförinställningar fungerar kan du anta att webbplatsen kräver att varje produktbild ska ha två olika storlekar: 500 × 500 pixlar och 150 × 150 pixlar. Du skapar två bildförinställningar, en som kallas&quot;Förstora&quot; om du vill visa bilder med 500 × 500 pixlar och en som kallas&quot;Miniatyrbild&quot; om du vill visa bilder med 150 × 150 pixlar. För att leverera bilder i storleken &quot;Förstora&quot; och &quot;Miniatyrbild&quot;, söker en Dynamic Media Image Server upp definitionen av &quot;Förstora bildförinställning&quot; och &quot;Förinställning för miniatyrbild&quot;. Sedan genererar servern dynamiskt en bild med samma storlek och formateringsspecifikationer som varje bildförinställning.

Adobe Dynamic Media Classic innehåller flera &quot;bästa praxis&quot;-förinställningar som du redan har ställt in för att använda. Administratörer kan även skapa bildförinställningar. Om du vill skapa en bildförinställning kan du börja från början eller så kan du börja från en befintlig och spara den under ett nytt namn.

Bilder som minskar i storlek när de levereras dynamiskt från en server kan förlora i skärpa och detaljer. Därför innehåller varje bildförinställning formateringskontroller för optimering av en bild när den levereras i en viss storlek. Med dessa kontroller ser du till att bilderna är skarpa och tydliga när de levereras till din webbplats eller ditt program.

## Skapa en bildförinställning {#creating-an-image-preset}

Du kan skapa egna bildförinställningar om du är företagsadministratör. Du kan skapa bildförinställningar eller börja med en standardförinställning som finns i Adobe Dynamic Media Classic, redigera den och spara den med ett nytt namn.

**Så här skapar du en bildförinställning:**

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]**.

   Du kan bläddra till namnet på en bildförinställning på den här skärmen om du vill förhandsgranska en befintlig bildförinställning. När du väljer namnet på en bildförinställning ändras storleken och utseendet på exempelbilden i förhandsvisningsfönstret.

1. Gör något av följande:

   * **Skapa en bildförinställning**: Välj **[!UICONTROL Add]**.
   * **Redigera en bildförinställning**: Bläddra till den bildförinställning som är mest lik den som du vill skapa och välj sedan **[!UICONTROL Edit]**.

1. Ange ett namn för bildförinställningen.
1. Ange mått för bredd och höjd i pixlar. Dessa mått bestämmer storleken som bilderna levereras med.
1. Fyll i skärmen Lägg till förinställning eller Redigera förinställning. Mer information finns i [Alternativ för bildförinställning](application-setup.md#image_preset_options).

   Adobe Dynamic Media Classic rekommenderar att du börjar med följande alternativ:

   * **[!UICONTROL Format]**: Välj JPEG eller ett annat format som uppfyller dina krav. Alla webbläsare har stöd för bildformatet JPEG, vilket ger en bra balans mellan små filstorlekar och bildkvalitet. JPEG-bilder använder dock ett förlustgivande komprimeringsschema som kan ge upphov till oönskade bildartefakter om komprimeringsinställningen är för låg. Därför rekommenderar Adobe Dynamic Media Classic att du ställer in komprimeringskvaliteten (på skjutreglaget) på 75. Den här inställningen ger en bra balans mellan bildkvalitet och liten filstorlek.

   * **[!UICONTROL Sharpening]**: Välj inte Skärpa (det här skärpefiltret ger mindre kontroll än **[!UICONTROL Unsharp Masking]** inställningar).

   * **[!UICONTROL Resample Mode]**: Välj **[!UICONTROL Bi-Cubic]**.

   * **[!UICONTROL Unsharp Masking]** (USM): Ange följande inställningar:

   | Förinställningstyp | Storlek | USM: Belopp | USM: Radie | USM: Tröskelvärde |
   | --- | --- | --- | --- | --- |
   | Korsförsäljning (miniatyrbild) | 75 × 75 | 1,5 | 0,8 | 5 |
   | Miniatyrbild | 150 × 150 | 1,1 | 1 | 5 |
   | Huvud | 350 × 350 | 1 | 1 | 6 |
   | Förstora | 500 × 500 | 1,2 | 1,2 | 5 |

1. Välj **[!UICONTROL Save]**.

Adobe Dynamic Media Classic&quot;best practice&quot;-alternativ för att skapa bildförinställningar som listas här är allmänna rekommendationer. Skärpeinställningen är mycket subjektiv. Inställningarna för&quot;bästa praxis&quot; baserades på en primär bild på 2 000 × 2 000. Inställningarna för större eller mindre primärfiler kan vara olika. Om du vill justera inställningarna för Oskarp mask rekommenderar Adobe Dynamic Media Classic följande intervall:

* **[!UICONTROL Amount]**: Mellan `.8` och `1.5`.

* **[!UICONTROL Radius]**: Mellan `.6` och `2`.

* **[!UICONTROL Threshold]**: Från `1` via `6`.

Om du vill ta bort en bildförinställning markerar du den på skärmen Bildförinställningar och väljer sedan **[!UICONTROL Delete]**.

>[!MORELIKETHIS]
>
>* [Skapa och redigera bildförinställningar](application-setup.md#creating_and_editing_image_presets)
>* [Alternativ för bildförinställning](application-setup.md#image_preset_options)
>* [Förhandsvisa en bildresurs baserat på dess bildförinställning](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)
