---
title: '"Snabbstart: eCatalogs"'
description: En introduktion och snabbstart till e-kataloger som hjälper dig att komma igång snabbt med eCatalog-tekniker.
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '1425'
ht-degree: 0%

---


# Snabbstart: eCatalogs{#quick-start-ecatalogs}

En e-katalog är en digital webbversion av trycksaker, till exempel en katalog, broschyr, flygblad, produkthandbok eller reklamcirkel. En e-katalog visas i ett eCatalog-visningsprogram på en webbplats. Det här visningsprogrammet simulerar upplevelsen av att läsa tryckt material. Beroende på vilka inställningar du väljer för din eCatalog kan du göra följande med visningsprogrammet:

* Sök i katalogen efter nyckelord eller nyckelord. Sökresultaten visas som en lista med miniatyrbilder i en sökpanel till vänster i katalogen. Varje klickbar miniatyrbild representerar ett kataloguppslag där den markerade söktermen hittades.

* Dela katalogen via sociala medier, ladda ned katalogen för att visa den offline, aktivera Favoriter för att markera objekt som du snabbt vill återgå till eller skriva ut katalogen.
* Navigera i katalogen med hjälp av innehållsförteckningen eller sidstödrastervyn. sida framåt eller bakåt genom att klicka på en sidas mittersta kant.
* Zooma in, zooma ut och panorera för att undersöka objekt på en sida.
* Flytta pekaren över ett sidområde (kallas bildschema) för att visa ett popup-fönster med information om ett objekt.
* Klicka på ett sidområde för att öppna en ny webbsida med mer information om ett objekt.
* Skriv en anteckning och bifoga den till en eCatalog-sida.
* Tryck på ikoner för bildschema för att öppna relaterade webbsidor eller infopaneler i sitt sammanhang.
* Använd gester, till exempel nypa för att zooma och svepa för att vända sidor.
* Sök efter objekt med nyckelord.

![eCatalog som den ser ut för användarna. A) Öppningssida för e-katalog. B) eCatalog har skickats till sidan 2.](/help/assets/ec_cat_viewer_popup.png)

Om du vill skapa en e-katalog använder du vanligtvis högupplösta PDF-filer som skapats i Adobe® Acrobat® eller något annat utskriftsprogram, men du kan också skapa en e-katalog från bildfiler.

När du skapar en e-katalog kan du ordna sidorna eller uppslagen i den ordning du vill. Du kan också deklarera om du vill ha enstaka sidor, dubbelsidiga uppslag eller flersidiga uppslag. Du kan skapa bildscheman för sidområden så att de som tittar kan klicka på ett område på sidan och öppna en ny sida på webbplatsen. Du kan hantera den överrullningstext som visas med InfoPanel-inställningarna på eCatalog-skärmen. Du kan också konfigurera eCatalog Viewer genom att välja bland fler än 100 olika konfigurationsalternativ. Du kan anpassa funktionerna och utseendet på visningsprogrammet för just din publik.

>[!NOTE]
>
>Om du använder läget AEM Dynamic Media - Scene7 och vill använda e-kataloger måste du redigera `pdfbrochure`-värdet i CRXDE Lite. Om du vill göra det AEM du på **[!UICONTROL Tools > General > CRXDE Lite]**. Navigera till `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf` i det vänstra panelnavigeringsträdet.
>
>Markera raden `jobParam` på fliken **[!UICONTROL Properties]** i den nedre högra rutan. Ange värdet för `pdfbrochure` från `false` till `true`. Som i `pdfbrochure=true`
>
>Klicka på **[!UICONTROL Save All]** i det övre vänstra hörnet på CRXDE Lite-sidan.
>
>Nu kan du skapa e-kataloger i Dynamic Media Classic.

**Snabbstart**

Den här eCatalog-snabbstarten är utformad för att hjälpa dig komma igång snabbt med e-kataloger. Följ steg 1 till 7. Efter varje steg finns en korsreferens till en ämnesrubrik där du kan hitta mer information.

**1. Överföra PDF-filer**

Adobe PDF-filer är vanligtvis källan till en e-katalog. Eftersom de ska skrivas ut innehåller PDF-filerna vanligtvis CMYK-bilder. Dynamic Media Classic identifierar dessa bilder och konverterar dem med en CMYK-standardfärgprofil. Du kan dock behöva överföra och använda en anpassad färgprofil.

Klicka på Överför i fältet Global navigering för att börja överföra PDF-filer eller bilder för din eCatalog. Du kan överföra filer från skrivbordet eller via FTP; FTP rekommenderas om du överför många filer eller filer som är större än 100 MB.

Under PDF-alternativ innehåller skärmen Överför alternativ för att överföra PDF-filer med rätt upplösning och rätt färgrymd. En upplösning på 150 pixlar per tum rekommenderas. Du kan välja alternativet Generera eCatalog automatiskt för att skapa en e-katalog när du överför en PDF-fil.

Se [Överföra PDF-filer](uploading-pdf-files.md#uploading_the_pdf_files).

**2. Skapa en e-katalog**

Skapa din e-katalog genom att välja PDF eller bildfiler i panelen Bläddra och sedan klicka på knappen Skapa och välja e-kataloger. eCatalog-skärmen öppnas.

På fliken Ordna sidor väljer du en layoutknapp - 1 upp, 2 upp eller anpassad - för att välja om du vill ha enkla, dubbla eller anpassade siduppslag. Du kan ordna om sidor eller uppslag genom att dra dem eller, i en stor e-katalog, genom att välja ett sidnamn på menyn Flytta till.

Om du vill lägga till sidor markerar du en mapp i resursbiblioteket och drar PDF- eller bildfiler från till skärmen Ordna sidor. I stället för standardsidnummer kan du ange egna sidnamn eller importera ett stort antal sidnamn.

Klicka på **[!UICONTROL Save]**, ange ett namn för din e-katalog, välj en Dynamic Media Classic-mapp att lagra den i och klicka på **[!UICONTROL Save]**. Varje gång du ändrar sidordningen eller redigerar din e-katalog sparar du ändringarna genom att klicka på **[!UICONTROL Save]**.

Se [Skapa en e-katalog](creating-ecatalog.md).

**3. Skapa bildscheman**

Bildscheman lägger till ytterligare en dimension till eCatalog-sidor. En bildschema är ett område på en sida som innehåller mer information om ett objekt. När visningsprogram rullar pekaren över en bildschema visas en beskrivning av objektet. När du klickar på en bildschema aktiveras en extern referens som öppnar en ny webbsida där du kan lära dig mer om ett objekt.

Om du vill skapa en bildschema öppnar du skärmen för eCatalog. Gå sedan till fliken **[!UICONTROL Map Pages]** på skärmen eCatalog och rita kartan med verktyget Rektangelbildschema eller verktyget Polygonbildschema. Du kan justera placering och storlek för bildscheman genom att dra kartkanterna med panoreringsverktyget.

När du har ritat bildschemat anger du den URL-adress du vill gå till när du klickar på bildschemat. Du kan också ange den överrullningstext som visas när du flyttar pekaren över bildschemat.

Se [Skapa eCatalog-bildscheman](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Se [Använda bildscheman för att bädda in multimedia i en eCatalog](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Du kan ställa in och hantera bildschematexten med hjälp av inställningarna i panelen Info på eCatalog-skärmen.

Se [Hantera innehåll i informationspanelen](info-panel-content.md#managing-info-panel-content).

**4. Konfigurera eCatalog Viewer-förinställningar**

Slutanvändarna ser din eCatalog i eCatalog Viewer. Om du är administratör kan du konfigurera eCatalog Viewer. Du kan ändra dess konturfärg och välja ett nytt&quot;skal&quot; för att märka upp din eCatalog. Dynamic Media Classic innehåller flera förinställningar för eCatalog Viewer. Du kan välja en av dessa förinställningar för att visa dina e-kataloger. Om du är administratör kan du även skapa en egen visningsförinställning för eCatalog.

Om du vill skapa en förinställning för eCatalog-visningsprogrammet klickar du på **[!UICONTROL Setup]** i fältet Global navigering och väljer **[!UICONTROL Viewer Presets]**. Klicka sedan på **[!UICONTROL Add]**, välj en plattform och klicka sedan på **[!UICONTROL eCatalog > Viewer]**.

Se [Konfigurera eCatalog Viewer-förinställningar](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

**5. Förhandsgranska e-kataloger i eCatalog Viewer**

Förinställningarna för eCatalog-visningsprogrammet avgör formatet och beteendet för eCatalog-visningsprogrammen.

Om du vill ta reda på hur eCatalog-visningsförinställningarna visar din eCatalog väljer du din eCatalog på panelen Bläddra och klickar på **[!UICONTROL Preview]**. Förhandsgranskningsskärmen öppnas i standardvisningsprogrammet.

Lägg märke till orientering, färgschema, hur kontrollerna för att ändra sidor ser ut och hur sidorna ser ut när de vrids.

Se [Förhandsgranska e-kataloger i eCatalog Viewer](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

**6. Publicera e-katalog och tillhörande PDF-filer**

När du publicerar din e-katalog och tillhörande PDF-filer placeras den på Dynamic Media Image-servrar så att den kan levereras till din webbplats och ditt program. Som en del av publiceringsprocessen aktiverar Dynamic Media Classic URL-strängen för din eCatalog. Använd den här URL:en för att anropa eCatalog från Dynamic Media Image Servers till din webbplats eller ditt program.

När du har markerat din e-katalog och PDF-fil för publicering i panelen Bläddra väljer du knappen Publicera i fältet Global navigering för att initiera en publicering. Klicka på **[!UICONTROL Start Publish]** på skärmen Publicera.

Se [Publicera e-kataloger och tillhörande PDF-filer](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

**7. Länka en e-katalog till en webbsida**

Dynamic Media Classic aktiverar den URL-bildtextsträng som krävs för att visa din e-katalog när du publicerar den på Dynamic Media Image Servers. Du kan kopiera den här URL-strängen från förhandsgranskningsskärmen och panelen Bläddra (i detaljvyn) genom att välja URL-adresser i panelen. När du har kopierat URL-strängen är den tillgänglig för dina webbplatser och program.

Samarbeta med IT-avdelningen och placera länken till e-katalogen på rätt plats på din webbsida. När användarna klickar på länken visas eCatalog Viewer och användarna kan bläddra i din eCatalog.

Se [Länka en e-katalog till en webbsida](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
