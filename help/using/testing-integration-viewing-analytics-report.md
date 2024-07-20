---
title: Testa integrationen genom att visa en Adobe Analytics-rapport
description: Lär dig hur du testar integreringen i Adobe Dynamic Media Classic genom att visa en Adobe Analytics-rapport.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
topic: Integrations, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---

# Testa integrationen genom att visa en Adobe Analytics-rapport{#testing-the-integration-by-viewing-an-adobe-analytics-report}

När du har skapat de nödvändiga variablerna i Adobe Analytics, länkat dem till Adobe Dynamic Media Classic-händelser och slutfört de nödvändiga implementeringsstegen kan du testa konfigurationen. Du kan testa och verifiera att data hämtas inuti Adobe Analytics. Om installationen fungerar här behövs inga ytterligare steg. Förutsatt att du följde stegen ovan och länkade dina Adobe Dynamic Media Classic-händelsedata till en eller flera anpassade trafikvariabler följer du det här arbetsflödet för att testa data i Adobe Analytics.

**Så här testar du integreringen genom att visa en Adobe Analytics-rapport:**

1. Starta ett Adobe Dynamic Media Classic-visningsprogram från ditt konto, särskilt ett som sänder mätvärden som du vill ha och interagera med det för att skapa vissa händelsedata.

   Om du till exempel vill mäta vanliga alternativa vyer i en bilduppsättning förhandsgranskar du en bilduppsättning och klickar på de olika miniatyrbilderna.

1. I Adobe Analytics går du till **[!UICONTROL Custom Traffic]** > **[!UICONTROL Custom Traffic 1-10]** > [Namn på erbjudande] och väljer ditt trafikproppsnamn i menyalternativen.

   Om du till exempel vill få åtkomst till **[!UICONTROL LoadAsset]**-satsen i exempelkontot är rätt menyval **[!UICONTROL Custom Traffic]** > **[!UICONTROL Custom Traffic 1-10]** > **[!UICONTROL LoadAsset]**. Om du har fler än tio anpassade utkast visas även andra menyalternativ.

1. Visa diagram som skapats av Adobe Analytics. Det här diagrammet är vanligtvis bara data för ett enskilt mått. Om du också vill veta vilken resurs som dessa data är associerade med, kan du hämta resursuppgifter för den här händelsen. Det är till exempel ofta praktiskt att veta vilken video som bara visas till 50 % eller vilken bild i en uppsättning som är populär.

>[!NOTE]
>
>Alla Adobe Dynamic Media Classic-visningsprogramdata visas och rapporteras i rapporter om anpassad trafik eller anpassade konverteringsrapporter för Adobe Analytics.

Mer information finns i [Analytics Tutorials](https://experienceleague.adobe.com/en/docs/analytics-learn/tutorials/overview).