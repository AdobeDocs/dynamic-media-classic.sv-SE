---
title: '"Definiera variabilitet: Parameterisering kontra DOM-manipulering"'
seo-title: '"Definiera variabilitet: Parameterisering kontra DOM-manipulering"'
description: 'null'
seo-description: Lär dig hur du definierar variabilitet med parameterisering jämfört med DOM-manipulering.
uuid: dce424f2-07d8-4703-aa3a-40d2eee12f74
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: 5b844afe-ac55-4dd2-8fe8-125a9c9af948
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Definiera variabilitet: Parameterisering kontra DOM-manipulering{#defining-variability-parameterization-versus-dom-manipulation}

Dynamic Media Classic erbjuder två tekniker för hantering av variabelt innehåll i en mall. Med båda teknikerna skapar du den ursprungliga mallen i Illustrator, konverterar mallen till det dynamiska Media Classic FXG-filformatet och överför den till SPS. Teknikerna skiljer sig dock åt när det gäller graden av kontroll över variabla element och den skicklighet som krävs för att använda dem:

* **Parameterisering i Scene7 Publishing System** Den här tekniken innebär att du måste definiera variabilitet i mallpubliceringsbygget och förhandsvisningsskärmarna i SPS eller i Adobe Illustrator-plugin-programmet för webb-till-tryck. Båda metoderna innehåller verktygen för att skapa parametrar, tilldela parametervärden och testa resultaten.

* **Använda DOM-manipulering** Med den här tekniken kan du ta kontroll över designen och mallen på XML-nivå. Dynamiska Media Classic FXG-filer är XML. Med den här metoden kan du redigera designmallen direkt med hjälp av dess XML DOM (visningsobjektmodell). I Illustrator kan du markera variabelelement med s7:elementID:n för att ändra dem senare med URL-kommandon.

>[!MORELIKETHIS]
>
>* [Parametrisera en mall i Dynamic Media Classic](parameterizing-template-scene7.md#parameterizing_a_template_in_scene7)
>* [DOM-manipulering](dom-manipulation.md#dom_manipulation)

