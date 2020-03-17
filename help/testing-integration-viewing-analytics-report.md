---
title: Testa integreringen genom att visa en Adobe Analytics-rapport
seo-title: Testa integreringen genom att visa en Adobe Analytics-rapport
description: 'null'
seo-description: Lär dig hur du testar integreringen genom att visa en Adobe Analytics-rapport.
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Testa integreringen genom att visa en Adobe Analytics-rapport{#testing-the-integration-by-viewing-an-adobe-analytics-report}

När du har skapat de nödvändiga variablerna i Adobe Analytics, länkat dem till Dynamic Media Classic-händelser och slutfört de nödvändiga implementeringsstegen bör du testa konfigurationen. Ni kan testa och verifiera att data hämtas, inifrån själva Adobe Analytics. Om installationen fungerar här behövs inga ytterligare steg. Förutsatt att du följde stegen ovan och länkade dina Dynamic Media Classic-händelsedata till en eller flera anpassade trafikvariabler följer du det här arbetsflödet för att testa data i Adobe Analytics.

**Testa integreringen genom att visa en Adobe Analytics-rapport**

1. Starta en Dynamic Media Classic-läsare från ditt konto, särskilt en som visar mätvärden som du vill hämta och interagera med den för att skapa händelsedata.

   Om du till exempel vill mäta de mest populära alternativa vyerna i en bilduppsättning förhandsgranskar du en bilduppsättning och klickar på de olika miniatyrbilderna.

1. I Adobe Analytics går du till Anpassad trafik > Anpassad trafik 1-10 > [Namn på prop]och väljer trafikproppens namn i menyalternativen.

   Om du till exempel vill få åtkomst till LoadAsset-beställningen i vårt exempelkonto är rätt menyval Anpassad trafik > Anpassad trafik 1-10 > LoadAsset. Om du har fler än tio anpassade utkast kan du se fler menyalternativ.

1. Visa det diagram som skapats med Adobe Analytics. Observera att detta vanligtvis bara är data för ett enskilt mått. Om du också vill veta vilken resurs som dessa data är associerade med (till exempel vilken video som bara bevakas till 50 % eller vilken bild i en uppsättning som är populärast), ska du även se till att samla in resursdata för den här händelsen.

>[!NOTE]
>
>Alla visningsdata för Dynamic Media Classic visas och rapporteras i rapporter om anpassad trafik eller anpassade konverteringsrapporter för Adobe Analytics.

Mer information finns i [www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en).
