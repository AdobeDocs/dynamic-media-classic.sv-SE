---
title: Hantera innehåll i informationspanelen i bilduppsättningar
description: Lär dig hur du hanterar innehåll i panelen Info i Bilduppsättningar i Adobe Dynamic Media Classic.
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 09fafdb4-51e2-4719-83b6-056f79d1ba9e
topic: Content Management
level: Intermediate
source-git-commit: 5b5dcd1199bd51ec987b5673fce75bc86baad55b
workflow-type: tm+mt
source-wordcount: '755'
ht-degree: 0%

---

# Hantera innehåll i informationspanelen i bilduppsättningar{#managing-info-panel-content-in-image-sets}

Förutom att använda bildschematext för överrullningar i bilduppsättningar kan du använda en informationspanel för att lägga till större mängder överrullningstext, inklusive länkar. Du kan också hantera InfoPanel med hjälp av tidscachning och schemaläggning av innehållsuppdateringar.

Du kan hantera InfoPanel-konfigurationen och data med följande funktioner i Adobe Dynamic Media Classic:

* I inställningspanelen i InfoPanel kan du ange den mall som används för att visa informationspanelens text, ett standardsvar på fel och det antal timmar som informationen cachelagras. Dessutom kan du ange om bilduppsättningen ska publiceras automatiskt.
* Med dataflödespanelen i InfoPanel kan du ange en CSV-fil som innehåller den text som du vill ska visas i informationspanelens överrullningstext och schemalägga tider för uppdatering av informationen.
* I dialogrutan Importera metadata kan du importera en tabbavgränsad TXT-fil som innehåller överrullningstextinformation. Du kan använda det här TXT-alternativet eller InfoPanel Data feed-panelen med CSV-filalternativet för överrullningstexten.

## Konfigurera en svarsmall för bilduppsättningar {#set-up-a-response-template-for-image-sets}

Du kan välja en av tre förinställda svarsmallar för att visa text på en informationspanel. Dessa förinställda svarsmallar avgör hur informationen visas på panelen Info: hur många kolumner och rader, teckenstorlek, teckensnitt osv. Du kan välja en förinställd svarsmall eller skapa en egen.

**Så här ställer du in en svarsmall för bilduppsättningar:**

1. Dubbelklicka på din bilduppsättning så att den öppnas i detaljvyn.
1. Välj **[!UICONTROL InfoPanel Setup]**.
1. Gör något av följande i listrutan Svarsmall:

   * Välj om du vill använda standardsvaret **[!UICONTROL Default]**. XML-koden för malldesignen visas nedtonad i textrutan Användarmall.
   * Om du vill skapa en egen svarsmall väljer du **[!UICONTROL Custom]**. Skriv XML-malldefinitionen i textrutan Användarmall. Du kan använda standardmallen som redan är definierad i textrutan som bas för ditt eget svar.

1. (Valfritt) I rutan Standardsvar skriver du den text som du vill ska visas om Adobe Dynamic Media Classic stöter på ett fel när information hämtas för ett bildschema. Om systemet till exempel får ett företagsnamn och ett bilduppsättningsnamn, men ingen rollover-identifierare, visas det här meddelandet för användaren.
1. Ange i textfältet Svarets TTL antalet timmar som du vill vänta innan du cachelagrar data.

   * Ange ett lägre värde om data uppdateras ofta under dagen.
   * Ange ett högre värde om data är relativt stabila och inte behöver uppdateras ofta under dagen. Standardvärdet är tio timmar.

1. Välj **[!UICONTROL Upload]** om du vill överföra innehåll i informationspanelen, baserat på rollover_key-värdet, till s7info.
1. I dialogrutan S7Info Upload bläddrar du till filen som du vill använda och väljer sedan **[!UICONTROL Upload]**.

   Filformat som stöds är TAB-avgränsade filer med UTF-16-kodning och CSV-filer med ASCII-kodning. För CSV-filer måste tecken som inte är ASCII-tecken vara HTML-kodade.

1. På panelen InfoPanel Setup väljer du **[!UICONTROL Publish]**.

## Importera källinnehåll för Info-panelen i Bilduppsättningar {#import-source-content-for-the-info-panel-in-image-sets}

Du kan använda en CSV-fil (kommaseparerat värde) med ASCII-kodning (icke-ASCII-tecken måste vara HTML-kodade) eller en tabbavgränsad fil för källtexten för en informationspanel för en bilduppsättning. Tabbavgränsade filer måste använda UTF-16-kodning (Unicode). Du importerar de olika filtyperna på olika sätt.

Tänk på följande när du formaterar källinnehåll:

* Tabb- och kommaavgränsade data kan innehålla så många kolumner som behövs för rollover-mallen.
* Det första objektet eller datakolumnen är rollover-identifieraren (associerad med rollover_key-värdet från URL:erna för bildschemat).
* Kontrollera att varje tabbavgränsat eller kommaavgränsat objekt efter identifieraren är det objekt som du vill ersätta i svarsmallen. Den första kolumnen ersätts alltså med $1$, den andra kolumnen med $2$ och så vidare).

### Importera CSV-innehåll till bilduppsättningar från en extern värdplats {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Dubbelklicka på bilduppsättningen så att den öppnas i detaljvyn.
1. Välj **[!UICONTROL InfoPanel Data feed]**.
1. I textfältet Externt hosted CSV file location (HTTP) anger du URL:en till CSV-filen.
1. (Valfritt) I fältet Schemalägg uppdatering anger du en tid för att uppdatera innehållet och väljer sedan **[!UICONTROL Add]**.

   Du kan välja flera gånger för uppdatering. Varje uppdateringstid visas i textrutan Uppdateringstider. Om du vill ta bort en schemalagd tid markerar du den och väljer **[!UICONTROL Delete]**.

1. (Valfritt) Välj **[!UICONTROL Run Update]** för att uppdatera innehållet omedelbart.
