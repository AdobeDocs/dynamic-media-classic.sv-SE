---
title: Hantera innehåll i informationspanelen i bilduppsättningar
seo-title: Hantera innehåll i informationspanelen i bilduppsättningar
description: 'null'
seo-description: Lär dig hur du hanterar innehåll i panelen Info i Bilduppsättningar.
uuid: ed7b4344-f180-41fc-a95a-62a9767dc056
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: ba5d1fb1-af54-471c-a471-853ace7f72fd
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---


# Hantera innehåll i informationspanelen i bilduppsättningar{#managing-info-panel-content-in-image-sets}

Förutom att använda bildschematext för överrullningar i bilduppsättningar kan du använda en informationspanel för att lägga till större mängder överrullningstext, inklusive länkar. Du kan också hantera InfoPanel med hjälp av tidsbestämd cachning och schemaläggning av innehållsuppdateringar.

Du kan hantera InfoPanel-inställningarna och data med följande funktioner i Dynamic Media Classic:

* I inställningspanelen i InfoPanel kan du ange den mall som används för att visa informationspanelens text, ett standardsvar på fel och det antal timmar som informationen cachelagras. Dessutom kan du ange om bilduppsättningen ska publiceras automatiskt.
* Med InfoPanel-datafeed-panelen kan du ange en CSV-fil som innehåller den text som du vill ska visas i informationspanelens överrullningstext, samt schemaläggningstider för uppdatering av informationen.
* I dialogrutan Importera metadata kan du importera en tabbavgränsad TXT-fil som innehåller överrullningstextinformation. Du kan använda det här TXT-alternativet eller InfoPanel-datafeed-panelen med CSV-filalternativet för överrullningstexten.

## Konfigurera en svarsmall för bilduppsättningar {#set-up-a-response-template-for-image-sets}

Du kan välja en av tre förinställda svarsmallar för att visa text på en informationspanel. De här förinställda svarsmallarna avgör hur informationen visas på panelen Info: hur många kolumner och rader, teckenstorlek, teckensnitt och så vidare. Du kan välja en förinställd svarsmall eller skapa en egen.

**Ställa in en svarsmall**

1. Dubbelklicka på bilduppsättningen för att öppna den i detaljvyn.
1. Klicka på **InfoPanel Setup** för att visa panelen.
1. Gör något av följande i listrutan Svarsmall:

   * Välj Standard om du vill använda standardsvaret. XML-koden för malldesignen visas nedtonad i textrutan Användarmall.
   * Välj Anpassad om du vill skapa en egen svarsmall. Skriv XML-malldefinitionen i textrutan Användarmall. Du kan använda standardmallen som redan är definierad i textrutan som bas för ditt eget svar.

1. (Valfritt) I rutan Standardsvar skriver du den text som du vill ska visas om Dynamic Media Classic stöter på ett fel när information hämtas för ett bildschema. Om systemet till exempel får ett företagsnamn och ett bilduppsättningsnamn, men ingen rollover-identifierare, visas det här meddelandet för användaren.
1. Ange i textfältet Svarets TTL antalet timmar som du vill vänta innan du cachelagrar data.

   * Ange ett lägre värde om data uppdateras ofta under dagen.
   * Ange ett högre värde om data är relativt stabila och inte behöver uppdateras ofta under dagen. Standardvärdet är tio timmar.

1. Klicka på **Överför** för att överföra innehåll i informationspanelen, baserat på rollover_key-värden, till s7info.
1. I dialogrutan S7Info Upload bläddrar du till filen som du vill använda och klickar sedan på **Upload**.

   Filformat som stöds är TAB-avgränsade filer med UTF-16-kodning och CSV-filer med ASCII-kodning. För CSV-filer måste icke-ASCII-tecken vara HTML-kodade.

1. Klicka på **Publicera** på inställningspanelen i InfoPanel.

## Importera källinnehåll för Info-panelen i Bilduppsättningar {#import-source-content-for-the-info-panel-in-image-sets}

Du kan använda en CSV-fil (kommaseparerat värde) med ASCII-kodning (icke-ASCII-tecken måste vara HTML-kodade) eller en tabbavgränsad fil för källtexten för en informationspanel för en bilduppsättning. Tabbavgränsade filer måste använda UTF-16-kodning (Unicode). Du importerar de olika filtyperna på olika sätt.

Tänk på följande när du formaterar källinnehåll:

* Tabb- och kommaavgränsade data ska innehålla så många kolumner som behövs för rollover-mallen.
* Det första objektet eller datakolumnen ska vara rollover-identifieraren (associerad med rollover_key-värdet från URL:erna för bildschemat).
* Kontrollera att varje tabb- eller kommaavgränsat objekt efter identifieraren är det objekt som du vill ersätta i svarsmallen (den första kolumnen ersätts alltså till $1$, den andra kolumnen till $2$ och så vidare).

### Importera CSV-innehåll till bilduppsättningar från en extern värdplats {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Dubbelklicka på bilduppsättningen för att öppna den i detaljvyn.
1. Klicka på **InfoPanel-datafeed** för att visa panelen.
1. I textfältet Externt hosted CSV file location (HTTP) anger du URL:en till CSV-filen.
1. (Valfritt) I fälten Schemalägg uppdatering anger du en tid för att uppdatera innehållet och klickar sedan på **Lägg till**.

   Du kan välja flera gånger för uppdatering. Varje uppdateringstid visas i textrutan Uppdateringstider. Om du vill ta bort en schemalagd tid markerar du den och klickar sedan på **Ta bort**.

1. (Valfritt) Klicka på **Kör uppdatering** för att omedelbart uppdatera innehållet.

