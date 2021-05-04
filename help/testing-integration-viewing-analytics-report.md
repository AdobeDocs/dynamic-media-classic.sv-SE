---
title: Testa integrationen genom att visa en Adobe Analytics-rapport
description: Lär dig hur du testar integreringen genom att visa en Adobe Analytics-rapport.
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
translation-type: tm+mt
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---

# Testa integrationen genom att visa en Adobe Analytics-rapport{#testing-the-integration-by-viewing-an-adobe-analytics-report}

När du har skapat de nödvändiga variablerna i Adobe Analytics, länkat dem till Dynamic Media Classic-händelser och slutfört de nödvändiga implementeringsstegen kan du testa konfigurationen. Du kan testa och verifiera att data hämtas, inuti Adobe Analytics. Om installationen fungerar här behövs inga ytterligare steg. Om du följer stegen ovan och länkade dina Dynamic Media Classic-händelsedata till en eller flera anpassade trafikvariabler följer du det här arbetsflödet för att testa data i Adobe Analytics.

**Så här testar du integreringen genom att visa en Adobe Analytics-rapport:**

1. Starta ett Dynamic Media Classic-visningsprogram från ditt konto, särskilt ett som sänder mätvärden som du vill hämta och interagera med det för att skapa vissa händelsedata.

   Om du till exempel vill mäta vanliga alternativa vyer i en bilduppsättning förhandsgranskar du en bilduppsättning och klickar på de olika miniatyrbilderna.

1. I Adobe Analytics går du till **[!UICONTROL Custom Traffic]** > **[!UICONTROL Custom Traffic 1-10]** > [Namn på prop] och väljer trafikproppens namn på menyalternativen.

   Om du till exempel vill komma åt **[!UICONTROL LoadAsset]**-satsen i exempelkontot är det rätta menyalternativet **[!UICONTROL Custom Traffic]** > **[!UICONTROL Custom Traffic 1-10]** > **[!UICONTROL LoadAsset]**. Om du har fler än tio anpassade utkast visas även andra menyalternativ.

1. Visa diagram som skapats av Adobe Analytics. Det här diagrammet är vanligtvis bara data för ett enskilt mått. Om du också vill veta vilken resurs som dessa data är associerade med, kan du hämta resursuppgifter för den här händelsen. Det är till exempel ofta praktiskt att veta vilken video som bara visas till 50 % eller vilken bild i en uppsättning som är populär.

>[!NOTE]
>
>Alla visningsdata för Dynamic Media Classic visas och rapporteras i rapporter om anpassad trafik eller anpassade konverteringsrapporter för Adobe Analytics.

Mer information finns i [Analytics Tutorials](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/overview.html).