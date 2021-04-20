---
title: Länka URL:er till webbprogrammet
description: Lär dig hur du länkar URL-adresser till webbprogram.
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
feature: Dynamic Media Classic
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---


# Länka URL:er till ditt webbprogram{#linking-urls-to-your-web-application}

Dina webbplatser och program har åtkomst till Dynamic Media Image Server-innehåll via URL-strängar. När du har publicerat en bild aktiverar Dynamic Media Classic en URL-sträng som refererar till bildförinställningen på Dynamic Media bildservrar. Du kan klistra in dessa URL:er i en webbläsare för testning.

Om du vill placera dessa URL-strängar på dina webbsidor och i dina program kopierar du dem från Dynamic Media Classic. Om du vill hämta en URL-sträng som genererats med en bildförinställning går du till förhandsgranskningsskärmen eller panelen Bläddra (i detaljvyn).

## Hämta en URL för bildförinställning {#obtaining-an-image-preset-url}

Du kan hämta en URL-sträng som genereras av en bildförinställning från förhandsvisningen eller från detaljvyn. När du har kopierat URL:en markeras den i Urklipp så att du kan klistra in den efter behov.

***Obs **: URL:en är inte aktiv förrän du publicerar resursen.*

### Hämta en URL för bildförinställning från förhandsvisning {#obtaining-an-image-preset-url-from-preview}

1. Gå till resursmapparna som innehåller den bildresurs som du vill förhandsgranska i panelen Resursbibliotek på vänster sida.
1. Gör något av följande:

   * Klicka på Stödrastervisning ovanför fönstret Resurser, till höger om verktygsfältet. Välj en enda bildresurs i fönstret Resurser och klicka sedan på Förhandsvisa > Lista med bildförinställningar under miniatyrbilden.
   * Ovanför fönstret Resurser klickar du på Listvy till höger om verktygsfältet. Välj en enda bildresurs i fönstret Resurser och klicka sedan på Förhandsvisa > Lista med bildförinställningar till höger om miniatyrbilden.
   * Klicka på Detaljvy ovanför fönstret Resurser, till höger om verktygsfältet. Klicka på Förhandsvisa > Lista med bildförinställningar i samma verktygsfält.

1. (Valfritt) I listrutan URL-kodning för kopiering av URL-generering i fönstret Bildförinställning väljer du den URL-kodning som du vill använda på bildresursens URL när den kopieras.
1. Klicka på Kopiera URL-adress för den valda förinställningstypen i det övre högra hörnet i förhandsgranskningsfönstret.
1. Klicka på Stäng i det nedre högra hörnet av fönstret Bildförinställningslista för att återgå till skärmen Resurser.

### Hämta en URL för bildförinställning från panelen Bläddra {#obtaining-an-image-preset-url-from-the-browse-panel}

1. Gå till resursmapparna som innehåller den bildresurs som du vill förhandsgranska i panelen Resursbibliotek på vänster sida.
1. Klicka på Stödrastervisning ovanför fönstret Resurser, till höger om verktygsfältet. I fönstret Resurser väljer du en enda bildresurs.
1. Klicka på Detaljvy ovanför fönstret Resurser, till höger om verktygsfältet.
1. Klicka på URL:er på panelen till höger på skärmen för att visa listan med bildförinställningar.
1. Klicka på länken Kopiera URL bredvid namnet på bildförinställningen med den URL som du vill kopiera till Urklipp.

## Om URL-strängar för bildförinställning {#about-image-preset-url-strings}

Ett URL-anrop för att ändra bildstorlek till Dynamic Media Image Servers har följande grundläggande syntax:

*sökväg*/*namn för Image Server*/*kontonamn*/*avbildningsnamn*?*modifier1*&amp;*modifier2*&amp;...

I en Dynamic Media Image Server-URL visas instruktioner till servern om hur bilden ska visas efter frågetecknet (?). Det här URL-anropet ger t.ex. en bild med namnet &quot;backpack&quot; och bredden 250 pixlar:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250
```

En URL för bildförinställning innehåller alla modifieringsinstruktioner för att visa bilden med rätt storlek och formateringsspecifikationer. Utan en bildförinställning kan du lägga märke till alla modifieringsinstruktioner efter frågetecknet (?) i den här URL-strängen:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250&fmt=jpeg&qlt=80,0&resMode=sharp&op_usm=1.1,0.5,1,0
```

I en URL-sträng som skapas med en bildförinställning visas namnet på bildförinställningen i stället för de instruktioner som definieras av bildförinställningen. Med referens till den långa URL:en ovan är URL-strängen:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?$Large$
```

Namn på bildförinställningar i URL:er omges av dollartecken ($). När en Dynamic Media Image Server påträffar delen Bildförinställning i URL:en (i det här fallet `Large`) och använder de storleks- och formateringsanvisningar som definieras av den stora bildförinställningen.

## Lägga till dynamiska bilder på webbsidan {#adding-dynamic-images-to-your-web-page}

Om du vill lägga till dynamiska bilder på en webbsida ändras taggen `<IMG>` i HTML-webbsideskoden vanligtvis med URL-strängen för Dynamic Media Classic och en begäran skickas till Dynamic Media Image Servers. Den här strängen skapar bilden med den storlek och formateringsspecifikation som definieras av bildförinställningen.

I stället för det vanliga anropet för att öppna en statisk bild som

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

Du använder nu taggen `<IMG>`för att ersätta referensen till en statisk bild med ett Image Preset-anrop till Dynamic Media Classic-plattformen. Ett exempelanrop ser ut så här:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

I det här exemplet &quot;söker en Dynamic Media Image Server upp&quot; definitionen av `$thumbnail$` och skapar dynamiskt rätt bild med de storleks- och formateringsspecifikationer som definieras av `thumbnail`Image Preset. I en URL-sträng är alla objekt utom produktbildens filnamn ( `backpack_trns` i det här fallet) vanligtvis hårdkopplade för sidmallen. Det enda elementet som infogas automatiskt i sidmallen från e-handelsservern är bildens IPS-ID eller namn.
