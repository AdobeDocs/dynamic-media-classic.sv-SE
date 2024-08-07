---
title: Länka URL:er till webbprogrammet
description: Lär dig hur du länkar URL:er till webbprogram från Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
topic: Administration, Content Management, Development
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '814'
ht-degree: 0%

---

# Länka URL:er till webbprogrammet{#linking-urls-to-your-web-application}

Dina webbplatser och program får åtkomst till Dynamic Media Image Server-innehåll via URL-strängar. När du har publicerat en bild aktiverar Adobe Dynamic Media Classic en URL-sträng som refererar till bildförinställningen på Dynamic Media bildservrar. Du kan klistra in dessa URL:er i en webbläsare för testning.

Om du vill montera dessa URL-strängar på webbsidor och i program kopierar du dem från Adobe Dynamic Media Classic. Om du vill hämta en URL-sträng som genererats med en bildförinställning går du till förhandsgranskningsskärmen eller panelen Bläddra (i detaljvyn).

## Hämta en URL för bildförinställning {#obtaining-an-image-preset-url}

Du kan hämta en URL-sträng som genereras av en bildförinställning från förhandsvisningen eller från detaljvyn. När du har kopierat URL:en markeras den i Urklipp så att du kan klistra in den efter behov.

>[!NOTE]
>
>URL:en är inte aktiv förrän du publicerar resursen.

### Hämta en URL för bildförinställning från förhandsvisning {#obtaining-an-image-preset-url-from-preview}

1. Navigera till resursmappen som innehåller bildresursen som du vill förhandsgranska i panelen Resursbibliotek på vänster sida.
1. Gör något av följande:

   * Ovanför Assets-fönstret väljer du **[!UICONTROL Grid View]** till höger om verktygsfältet. I fönstret Resurser väljer du en enda bildresurs och går sedan till **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]** under miniatyrbilden.
   * Ovanför Assets-fönstret väljer du **[!UICONTROL List View]** till höger om verktygsfältet. I fönstret Resurser väljer du en enda bildresurs och går sedan till höger om miniatyrbilden till **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.
   * Ovanför Assets-fönstret väljer du **[!UICONTROL Detail View]** till höger om verktygsfältet. Gå till **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]** i samma verktygsfält.

1. (Valfritt) I listrutan Bildförinställning väljer du den URL-kodning som ska användas för bildresursens URL när den kopieras i URL-kodningslistan för kopiering av URL-generering.
1. Välj **[!UICONTROL Copy URL]** som den valda förinställningstypen i det övre högra hörnet i förhandsgranskningsfönstret i fönstret Bildförinställningslista.
1. I det nedre högra hörnet av fönstret Bildförinställningslista väljer du **[!UICONTROL Close]** om du vill gå tillbaka till Assets-skärmen.

### Hämta en URL för bildförinställning från panelen Bläddra {#obtaining-an-image-preset-url-from-the-browse-panel}

1. Gå till resursmappen som innehåller den bildresurs som du vill förhandsgranska i panelen Resursbibliotek på vänster sida.
1. Ovanför Assets-fönstret väljer du **[!UICONTROL Grid View]** till höger om verktygsfältet. I fönstret Resurser väljer du en enda bildresurs.
1. Ovanför Assets-fönstret väljer du **[!UICONTROL Detail View]** till höger om verktygsfältet.
1. Välj **[!UICONTROL URLs]** på panelen till höger på skärmen så att du kan visa listan med bildförinställningar.
1. Välj länken **[!UICONTROL Copy URL]** bredvid namnet på bildförinställningen med den URL som du vill kopiera till Urklipp.

## Om URL-strängar för bildförinställning {#about-image-preset-url-strings}

Ett URL-anrop för att ändra bildstorlek till Dynamic Media Image Servers har följande grundläggande syntax:

*sökväg*/*namn på bildserver*/*kontonamn*/*bildnamn*?*modifier1*&amp;*modifier2*&amp;...

I en Dynamic Media Image Server-URL visas instruktioner till servern om hur bilden ska visas efter frågetecknet (?). Det här URL-anropet ger t.ex. en bild med namnet &quot;backpack&quot; och bredden 250 pixlar:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250
```

En URL för bildförinställning innehåller alla modifieringsinstruktioner för att visa bilden med rätt storlek och formateringsspecifikationer. Utan en bildförinställning kan du lägga märke till alla modifieringsinstruktioner efter frågetecknet (?) i denna URL-sträng:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250&fmt=jpeg&qlt=80,0&resMode=sharp&op_usm=1.1,0.5,1,0
```

I en URL-sträng som skapas med en bildförinställning visas namnet på bildförinställningen i stället för de instruktioner som definieras av bildförinställningen. Med referens till den långa URL:en ovan är URL-strängen:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?$Large$
```

Namn på bildförinställningar i URL:er omges av dollartecken ($). När en Dynamic Media Image Server stöter på delen Bildförinställning i URL:en (i det här fallet `Large`) och använder de storleks- och formateringsanvisningar som definieras av den stora förinställningen.

## Lägga till dynamiska bilder på webbsidan {#adding-dynamic-images-to-your-web-page}

När du lägger till dynamiska bilder på din webbsida ändras taggen `<IMG>` i HTML-sidkoden vanligtvis med hjälp av Adobe Dynamic Media Classic URL-sträng för att göra en begäran till Dynamic Media Image Servers. Den här strängen skapar bilden med den storlek och formateringsspecifikation som definieras av bildförinställningen.

I stället för det vanliga anropet för att öppna en statisk bild som

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

Du använder nu taggen `<IMG>` för att ersätta referensen till en statisk bild med ett Image Preset-anrop till Adobe Dynamic Media Classic-plattformen. Ett exempelanrop ser ut så här:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$"
```

I det här exemplet söker en Dynamic Media Image Server upp definitionen av `$thumbnail$` och skapar dynamiskt rätt bild med de storleks- och formateringsspecifikationer som definieras av `thumbnail`Image Preset. I en URL-sträng är alla objekt utom produktbildens filnamn ( `backpack_trns` i det här fallet) vanligtvis hårdkopplade för sidmallen. Det enda elementet som infogas automatiskt i sidmallen från e-handelsservern är bildens IPS-ID eller namn.
