---
title: Hantera innehåll i informationspanelen i e-kataloger
description: Lär dig hur du hanterar innehåll i informationspanelen i e-kataloger i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '852'
ht-degree: 0%

---

# Hantera innehåll i informationspanelen i e-kataloger{#managing-info-panel-content-in-ecatalogs}

Förutom att använda bildschematext för överrullningar i e-kataloger kan du använda en informationspanel för att lägga till större mängder överrullningstext, inklusive länkar. Du kan också hantera InfoPanel genom att använda cachelagring som är tidsbestämd och schemalägga innehållsuppdateringar.

Du kan hantera InfoPanel-konfigurationen och data med följande funktioner i Adobe Dynamic Media Classic:

* På InfoPanel-inställningspanelen kan du ange vilken mall som ska användas för att visa Info-paneltexten, ett standardsvar på fel och det antal timmar som informationen cachelagras. Dessutom kan du ange om e-kataloger ska publiceras automatiskt.
* På dataflödespanelen i InfoPanel kan du ange en CSV-fil som innehåller den text som du vill ska visas i InfoPanel-överrullningstexten och schemalägga tider för uppdatering av informationen.
* I dialogrutan Importera metadata (som du kommer åt från vyn Kartsidor) kan du importera en tabbavgränsad TXT-fil som innehåller överrullningstextinformation. Du kan använda det här TXT-alternativet eller dataflödespanelen med CSV-filalternativet för överrullningstexten.
* I vyn Kartsidor finns ett alternativ för att förhandsgranska XML-filen som visas för specifika bildscheman.

## Konfigurera en svarsmall för e-kataloger {#set-up-a-response-template-for-ecatalogs}

Du kan välja en av tre förinställda svarsmallar för att visa text på en informationspanel. Dessa förinställda svarsmallar avgör hur informationen visas på panelen Info: hur många kolumner och rader, teckenstorlek, teckensnitt osv. Du kan välja en förinställd svarsmall eller skapa en egen.

>[!NOTE]
>
>Du kan också ställa in svarsmallen i visningsförinställningen. Om du vill använda svarsmallen i visningsförinställningen lägger du till `fmt=1` till slutet av informationsserverns URL i visningsförinställningen.
>
>Se [Konfigurera förinställningar för eCatalog Viewer](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).

1. Dubbelklicka på din e-katalog så att den öppnas i detaljvyn.
1. Välj **[!UICONTROL InfoPanel Setup]** -panelen.
1. Välj en svarsmall:

   * Välj en förinställning på menyn Svarsmall. XML-koden för malldesignen visas i rutan Användarmall.
   * Om du vill skapa en egen svarsmall väljer du **[!UICONTROL Custom]**. Skriv XML-malldefinitionen i rutan Användarmall. Du kan använda de förinställda mallarna som bas för dina egna.

1. (Valfritt) I rutan Standardsvar skriver du den text som du vill ska visas om Adobe Dynamic Media Classic stöter på ett fel när information hämtas för en bildschema. Om systemet till exempel tar emot ett företagsnamn och ett eCatalog-namn, men ingen rollover-identifierare, visas det här meddelandet för användaren.
1. I rutan Svarets TTL anger du antalet timmar du vill vänta innan data cachelagras:

   * Ange ett lägre värde om data uppdateras ofta under en dag.
   * Ange ett högre värde om data är relativt stabila och inte behöver uppdateras ofta under dagen. Standardvärdet är tio timmar.

1. Välj **[!UICONTROL Publish]**.

## Importera källinnehåll för Info-panelen i e-kataloger {#import-source-content-for-the-info-panel-in-ecatalogs}

Du kan använda en kommaavgränsad värdefil (CSV) eller tabbavgränsad fil (TXT) för källtexten för en informationspanel för en e-katalog. Tabbavgränsade filer måste använda UTF16-kodning (Unicode). Du kan importera de olika filtyperna på olika sätt.

Tänk på följande när du formaterar källinnehåll:

* Se till att tabb- och kommaavgränsade data innehåller så många kolumner som behövs för överrullningsmallen.
* Se till att det första objektet eller datakolumnen är rollover-identifieraren (associerad med rollover_key-värdet från Image Map-URL:erna).
* Kontrollera att varje tabbavgränsat eller kommaavgränsat objekt efter identifieraren är det objekt som du vill ersätta i svarsmallen. Den första kolumnen ersätts alltså med $1$, den andra kolumnen med $2$ och så vidare.

### Importera CSV-innehåll till e-kataloger från en extern värdplats {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. Dubbelklicka på e-katalogen så att den öppnas i detaljvyn.
1. Välj **[!UICONTROL InfoPanel Data feed]** -panelen.
1. Ange URL:en för CSV-filen i rutan Plats för extern värdbaserad CSV-fil. Du kan klistra in URL-adressen i det här fältet eller skriva den direkt.
1. (Valfritt) Ange en tid för att uppdatera innehållet med hjälp av menyn Schemauppdatering och välj **[!UICONTROL Add]**. Du kan välja flera gånger för uppdatering. Varje uppdateringstid visas i rutan Uppdateringstider. (Om du vill ta bort en tid markerar du den och väljer **[!UICONTROL Delete]**.)
1. (Valfritt) Välj **[!UICONTROL Run Update Now]** så att du kan uppdatera innehållet direkt.

### Importera en tabbavgränsad fil eller CSV-fil {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. Dubbelklicka på e-katalogen så att den öppnas i detaljvyn.
1. Välj **[!UICONTROL InfoPanel Setup]** -panelen.
1. Välj **[!UICONTROL Upload S7Info Content]**.
1. Välj **[!UICONTROL Browse]** markerar du den tabbavgränsade TXT-, CSV- eller SSV-fil som du vill använda och väljer **[!UICONTROL Open]**.
1. Välj **[!UICONTROL Upload]**.

Adobe Dynamic Media Classic skickar ett e-postmeddelande till dig som talar om huruvida överföringen lyckades eller inte.

## Förhandsgranska överrullningsnyckeltext för en bildschema {#preview-rollover-key-text-for-an-image-map}

På skärmen Karta sidor kan du snabbt och enkelt visa text i panelen Info för bildscheman på en viss sida i din eCatalog.

1. Välj katalogens överrullning **[!UICONTROL Edit]** -knappen.
1. Välj **[!UICONTROL Map Pages]**.
1. Överst i tabellen, på skärmens högra sida, väljer du **[!UICONTROL Info Panel]** på menyn Visa.

   Överrullningstexten visas bredvid varje bildschema som innehåller text på informationspanelen.
