---
title: Skapa mallparametrar
description: Lär dig skapa mallparametrar i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 118806ea-c8a7-4aaf-9ae3-739c6b04ea77
topic: Development
level: Experienced
source-git-commit: 00591bdbe721035e25d3dea245a2110f978d19aa
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 0%

---

# Skapa mallparametrar{#creating-template-parameters}

Med parametrar kan du använda mallar med maximal flexibilitet. Du kan anpassa en mallbild dynamiskt. Du kan bestämma vilka text- och bildlager som ska ingå i mallen och vilka parametrar som ska visas i varje lager. Om du till exempel vill rikta uppmärksamheten mot en produkt som är på rea kan du skapa ett textlager som är på rea. Du kan senare ta bort det här lagret men behålla resten av mallbilden genom att ta bort parametern Vid försäljning.

När du skapar mallparametrar deklarerar du i själva verket vilka delar av mallen som ska anropas i en URL-sträng. En URL som konstruerats med parametrar visar dessa objekt i URL-strängen. När parametrar visas kan du skapa anpassade resultat utifrån hur mallbilden dynamiskt skapas från Image Server. På så sätt kan du ändra en mall dynamiskt eftersom du kan anropa vissa eller alla dess parametrar i en URL.

I textlagerparametrar kan du också göra textsträngen till ett dynamiskt fält som är länkat till värden i en databas. Att kunna länka text till en databas är användbart i kampanjer. Du kan anpassa mallbilder så att de visar klient- eller kundnamn. Du kan även länka en textlagerparameter till en prisdatabas för att visa priset på ett objekt i en mallbild.

Du kan referera till en parameter mer än en gång. Använd kombinationsrutan för varje kommando i parameterdialogrutan för att välja en parameter som matchar det aktuella kommandot. Alla storleksparametrar är till exempel tillgängliga för kommandot `size=`. Du kan tilldela om parameterreferensen till en parameter som redan finns i kombinationsrutan och ändra namnet till något som inte finns i kombinationsrutan. I det senare fallet måste namnet vara unikt. I annat fall visas ett fel om att parametern finns. När du tar bort en parameterreferens tas parametern bort från URL:en om den inte refereras någon annanstans. När du ändrar standardvärdet för en textparameter uppdateras alla referenser till den parametern. Uppdateringen visas i lagertabellen, i mallåtergivningen och i URL:en. När du ändrar ett lagerattribut genom att ändra storlekshandtag eller ange värden i egenskapspanelen uppdateras parametervärdet och alla referenser till parametern uppdateras. Om du till exempel har parametriserat storleken på två lager med en parameter, uppdateras båda lagerstorlekarna när någon av lagerstorlekarna ändras. När du förhandsgranskar en mall och ändrar en parameter uppdateras alla referenser till den parametern.

Se även utbildningsvideon [Mallgrunder](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS).

## Parametrisera ett lager {#parameterizing-a-layer}

Följ de här stegen för att skapa mallparametrar för varje lager i mallen:

1. I listan Lager väljer du knappen Parametrar bredvid namnet på det lager som du vill skapa parametrar för. Skärmen Parametrar öppnas. Den visar namnet på varje parameter i lagret, dess värde och typ.
1. Välj alternativet På bredvid namnet på varje parameter som du vill ta med i mallbilden.
1. Välj **[!UICONTROL Close]** om du vill stänga parameterskärmen.

>[!NOTE]
>
>Du kan byta namn på parametrar på parameterskärmen. Om du byter namn på en parameter blir det enklare att identifiera parametern i URL-strängar och lättare att använda som databasvärde. Om du vill byta namn på en parameter markerar du dess **[!UICONTROL On]**-alternativ, markerar dess namn och anger ett nytt namn i fältet Namn.

Om du vill visa en lista över de parametrar som du har skapat för mallen väljer du knappen Parametersammanfattning på mallskärmen. På skärmen Parametersammanfattning visas namnet på varje lager. Om du har skapat parametrar för ett lager visas parameternamn och värden.

## Skapa dynamiska textparametrar {#creating-dynamic-text-parameters}

För textlager kan du också göra textsträngen till ett dynamiskt fält länkat till ett databasvärde. Följ de här stegen:

1. På mallskärmen väljer du knappen Parametrar bredvid namnet på textlagret som du vill skapa dynamiska textparametrar för. Sidan Parametrar öppnas.
1. Välj alternativet **[!UICONTROL On]** bredvid textattributets namn (textAttr).
1. Välj fliken **[!UICONTROL Text]** på skärmen Parametrar.
1. Välj **[!UICONTROL Add Parameter]**. Ett standardparameternamn visas. Du kan ersätta det här namnet genom att markera det och skriva över det. Den aktuella textsträngen blir parameterns nya namn.
1. Välj **[!UICONTROL Close]** för att stänga sidan Parametrar.

Om du vill att parameternamnet ska använda ett databasvärde lägger du till följande sträng i mallens URL:

```as3
?$_2(parameter name)=(database value)
```

Namnen i ett databasfält eller Java™-koden ersätter parameternamnen. Den här funktionaliteten anger till exempel det aktuella priset på en artikel eller ett kundnamn.
