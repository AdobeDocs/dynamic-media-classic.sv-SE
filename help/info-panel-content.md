---
title: Hantera innehåll i informationspanelen i e-kataloger
description: Lär dig hur du hanterar innehåll i panelen Info i e-kataloger.
uuid: 5aa634f9-0874-4bb5-a3d9-8ce4d5577941
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: be277831-77cc-4011-ae30-e75c18eec99b
feature: Dynamic Media Classic,Visningsprogram,eCatalog
role: User
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 2%

---

# Hantera innehåll i informationspanelen i e-kataloger{#managing-info-panel-content-in-ecatalogs}

Förutom att använda bildschematext för överrullningar i e-kataloger kan du använda en informationspanel för att lägga till större mängder överrullningstext, inklusive länkar. Du kan också hantera InfoPanel med hjälp av tidsbestämd cachning och schemaläggning av innehållsuppdateringar.

Du kan hantera InfoPanel-inställningar och data med följande funktioner i Dynamic Media Classic:

* I inställningspanelen i InfoPanel kan du ange vilken mall som ska användas för att visa Info-paneltexten, ett standardsvar på fel och det antal timmar som informationen cachelagras. Dessutom kan du ange om e-kataloger ska publiceras automatiskt.
* Med InfoPanel-datafeed-panelen kan du ange en CSV-fil som innehåller den text som du vill ska visas i InfoPanel-överrullningstexten och schemalägga tider för uppdatering av informationen.
* I dialogrutan Importera metadata (hämtas från vyn Kartsidor) kan du importera en tabbavgränsad TXT-fil som innehåller överrullningstextinformation. Du kan använda det här TXT-alternativet eller Datafeed-panelen med CSV-filalternativet för överrullningstexten.
* Vyn Kartsidor innehåller ett alternativ för att förhandsgranska XML-filen som visas för specifika bildscheman.

## Konfigurera en svarsmall för e-kataloger {#set-up-a-response-template-for-ecatalogs}

Du kan välja en av tre förinställda svarsmallar för att visa text på en informationspanel. De här förinställda svarsmallarna avgör hur informationen visas på panelen Info: hur många kolumner och rader, teckenstorlek, teckensnitt och så vidare. Du kan välja en förinställd svarsmall eller skapa en egen.

>[!NOTE]
>
>Du kan också ställa in svarsmallen i visningsförinställningen. Om du vill använda svarsmallen i visningsförinställningen i stället lägger du till `fmt=1` i slutet av informationsserverns URL i visningsförinställningen.
>
>Se [Konfigurera eCatalog Viewer-förinställningar](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).

1. Dubbelklicka på din e-katalog för att öppna den i detaljvyn.
1. Klicka på panelen InfoPanel-inställningar.
1. Välj en svarsmall:

   * Välj en förinställning på menyn Svarsmall. XML-koden för malldesignen visas i rutan Användarmall.
   * Om du vill skapa en egen svarsmall väljer du **[!UICONTROL Custom]**. Skriv XML-malldefinitionen i rutan Användarmall. Du kan använda de förinställda mallarna som bas för dina egna.

1. (Valfritt) I rutan Standardsvar skriver du den text som du vill ska visas om Dynamic Media Classic stöter på ett fel när information hämtas för ett bildschema. Om systemet till exempel tar emot ett företagsnamn och ett eCatalog-namn, men ingen rollover-identifierare, visas det här meddelandet för användaren.
1. I rutan Svarets TTL anger du antalet timmar du vill vänta innan data cachelagras:

   * Ange ett lägre värde om data uppdateras ofta under en dag.
   * Ange ett högre värde om data är relativt stabila och inte behöver uppdateras ofta under dagen. Standardvärdet är tio timmar.

1. Klicka på **[!UICONTROL Publish]**.

## Importera källinnehåll för Info-panelen i e-kataloger {#import-source-content-for-the-info-panel-in-ecatalogs}

Du kan använda en kommaavgränsad värdefil (CSV) eller tabbavgränsad fil (TXT) för källtexten för en informationspanel för en e-katalog. Tabbavgränsade filer måste använda UTF16-kodning (Unicode). Du importerar de olika filtyperna på olika sätt.

Tänk på följande när du formaterar källinnehåll:

* Se till att tabb- och kommaavgränsade data innehåller så många kolumner som behövs för överrullningsmallen.
* Se till att det första objektet eller datakolumnen är rollover-identifieraren (associerad med rollover_key-värdet från URL:erna för bildschemat).
* Kontrollera att varje tabbavgränsat eller kommaavgränsat objekt efter identifieraren är det objekt som du vill ersätta i svarsmallen. Den första kolumnen ersätts alltså med $1$, den andra kolumnen med $2$ och så vidare.

### Importera CSV-innehåll till e-kataloger från en externt värdbaserad plats {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. Dubbelklicka på e-katalogen för att öppna den i detaljvyn.
1. Klicka på panelen Datafeed i InfoPanel.
1. Ange URL:en för CSV-filen i rutan Plats för extern värdbaserad CSV-fil. Du kan klistra in URL-adressen i det här fältet eller skriva den direkt.
1. (Valfritt) Ange en tid för att uppdatera innehållet med hjälp av menyerna Schemauppdatering och klicka på Lägg till. Du kan välja flera gånger för uppdatering. Varje uppdateringstid visas i rutan Uppdateringstider. (Om du vill ta bort en tid markerar du den och klickar på Ta bort.)
1. (Valfritt) Klicka på Kör uppdatering nu för att omedelbart uppdatera innehållet.

### Importera en tabbavgränsad fil eller CSV-fil {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. Dubbelklicka på e-katalogen för att öppna den i detaljvyn.
1. Klicka på panelen InfoPanel-inställningar.
1. Klicka på **[!UICONTROL Upload S7Info Content]**.
1. Klicka på **[!UICONTROL Browse]**, markera den tabbavgränsade TXT-, CSV- eller SSV-filen som du vill använda och klicka sedan på **[!UICONTROL Open]**.
1. Klicka på **[!UICONTROL Upload]**.

Dynamic Media Classic skickar ett e-postmeddelande till dig med information om överföringen lyckades eller inte.

## Förhandsgranska överrullningsnyckeltext för en bildschema {#preview-rollover-key-text-for-an-image-map}

På skärmen Karta sidor kan du snabbt och enkelt visa text i panelen Info för bildscheman på en viss sida i din eCatalog.

1. Klicka på Katalogens överrullningsknapp **[!UICONTROL Edit]**.
1. Klicka på **[!UICONTROL Map Pages]**.
1. Överst i tabellen till höger på skärmen väljer du **[!UICONTROL Info Panel]** på menyn Visa.

   Övergångstexten visas bredvid alla bildscheman som innehåller text på informationspanelen.
