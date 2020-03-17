---
title: Skapa mallparametrar
seo-title: Skapa mallparametrar
description: 'null'
seo-description: Lär dig hur du skapar mallparametrar.
uuid: d17168a8-4776-4761-b022-8258d5997604
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: d263f041-5a0d-4c4f-9266-aeff51a5a7e2
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# Skapa mallparametrar{#creating-template-parameters}

Med parametrar kan du använda mallar med maximal flexibilitet; kan du anpassa en mallbild dynamiskt. Du kan bestämma vilka text- och bildlager som ska ingå i mallen och vilka parametrar som ska visas i varje lager. Om du till exempel vill rikta uppmärksamheten mot en produkt som är i rea kan du skapa ett textlager vid försäljning. Du kan senare ta bort det här lagret men behålla resten av mallbilden genom att ta bort parametern Vid försäljning.

När du skapar mallparametrar deklarerar du i själva verket vilka delar av mallen som ska anropas i en URL-sträng. En URL som konstruerats med parametrar visar dessa objekt i URL-strängen. När parametrar visas kan du skapa anpassade resultat utifrån hur mallbilden dynamiskt skapas från Image Server. På så sätt kan du ändra en mall dynamiskt eftersom du kan anropa vissa eller alla dess parametrar i en URL.

I textlagerparametrar kan du också göra textsträngen till ett dynamiskt fält som är länkat till värden i en databas. Att kunna länka text till en databas är användbart i kampanjer. Du kan anpassa mallbilder så att de visar klient- eller kundnamn. Du kan även länka en textlagerparameter till en prisdatabas för att visa priset på ett objekt i en mallbild.

Du kan referera till en parameter mer än en gång. Använd kombinationsrutan för varje kommando i parameterdialogrutan för att välja en parameter som matchar det aktuella kommandot. (Alla storleksparametrar är till exempel tillgängliga för kommandot size=.) Du kan tilldela om parameterreferensen till en parameter som redan finns i kombinationsrutan och ändra namnet till något som inte finns i kombinationsrutan. I det senare fallet måste namnet vara unikt. I annat fall visas ett fel om att parametern redan finns. När du tar bort en parameterreferens tas parametern bort från URL:en om den inte refereras någon annanstans. När du ändrar standardvärdet för en textparameter uppdateras alla referenser till den parametern. Du kan se uppdateringen i lagertabellen, i mallens återgivning och i URL:en. När du ändrar ett lagerattribut genom att ändra storlekshandtag eller skriva värden i egenskapspanelen uppdateras parametervärdet och alla referenser till parameteruppdateringen. Om du till exempel har parametriserat storleken på två lager med en parameter, uppdateras båda lagerstorlekarna när någon av lagerstorlekarna ändras. När du förhandsgranskar en mall och ändrar en parameter uppdateras alla referenser till den parametern.

## Parametrisera ett lager {#parameterizing-a-layer}

Följ de här stegen för att skapa mallparametrar för varje lager i mallen:

1. I listan Lager väljer du knappen Parametrar bredvid namnet på det lager som du vill skapa parametrar för. Skärmen Parametrar öppnas. Den visar namnen på varje parameter i lagret, dess värde och typ.
1. Välj alternativet På bredvid namnet på varje parameter som du vill ta med i mallbilden.
1. Välj **Stäng** för att stänga parameterskärmen.

>[!NOTE]
>
>Du kan byta namn på parametrar på parameterskärmen. Om du byter namn på en parameter blir det enklare att identifiera parametern i URL-strängar och lättare att använda som databasvärde. Om du vill byta namn på en parameter markerar du dess På-alternativ, klickar på dess namn och anger ett nytt namn i fältet Namn.

Om du vill visa en lista över de parametrar du har skapat för mallen väljer du knappen Parametersammanfattning på mallskärmen. Skärmen Parametersammanfattning öppnas. Namnet på varje lager visas och om du har skapat parametrar för ett lager visas parameternamn och värden.

## Skapa dynamiska textparametrar {#creating-dynamic-text-parameters}

För textlager kan du dessutom göra textsträngen till ett dynamiskt fält länkat till ett databasvärde. Följ de här stegen:

1. På mallskärmen väljer du knappen Parametrar bredvid namnet på textlagret som du vill skapa dynamiska textparametrar för. Skärmen Parametrar öppnas.
1. Välj alternativet På bredvid namnet på textattributet (textAttr).
1. Välj fliken Text på skärmen Parametrar.
1. Klicka på knappen Lägg till parameter. Ett standardparameternamn visas. Du kan ersätta det här namnet genom att markera det och skriva över det. Den aktuella textsträngen blir parameterns nya namn.
1. Klicka på knappen Stäng för att stänga skärmen Parametrar.

Om du vill att parameternamnet ska använda ett databasvärde lägger du till följande sträng i mallens URL:

```as3
?$_2(parameter name)=(database value)
```

Parameternamnet ersätts av namn i ett databasfält eller Java-kod som t.ex. anger det aktuella priset för en artikel eller ett kundnamn.
