---
title: Video SEO (sökmotoroptimering)
description: Lär dig hur du konfigurerar SEO-inställningar för video.
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
feature: Dynamic Media Classic
role: Administrator
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
translation-type: tm+mt
source-git-commit: 06bd65c92c88595786b14213944a7cebd0d2590b
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 0%

---

# Video SEO (sökmotoroptimering){#video-seo-search-engine-optimization}

SEO är processen att förbättra trafiken till en webbplats från sökmotorer. Sökmotorer är utmärkta på att samla in information om textbaserat innehåll, men de kan inte hämta in information om video på ett adekvat sätt om de inte får den här informationen.

Med hjälp av Dynamic Media Classic Video SEO kan du använda videometadata för att ge sökmotorer beskrivningar av videoklipp. Med Dynamic Media Classic kan du skapa webbplatskartor för video och mRSS-flöden. Dessa XML-filer används för att skicka videoinformation till sökmotorer:

* **Webbplatskarta**  för video - Informerar Google om exakt var och vad videomaterialet finns på en webbplats. Så videor är helt sökbara på Google. En webbplatskarta för video kan till exempel ange körningstid och videokategorier. Mer information om webbplatskartor för video finns i [Alternativ för webbplatskartor för video](https://developers.google.com/search/docs/advanced/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

* **mRSS-feed (Media Really Simple Syndication)**  - Används av utgivare för att skicka mediefiler till Yahoo! Videosökning. Mer information om mRSS-flöden finns i [Webbplatskartor för video och alternativ för videowebbplatskarta](https://developers.google.com/search/docs/advanced/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

>[!NOTE]
>
>Google stöder både Video Sitemap- och mRSS-feed-protokollet för att skicka information till sökmotorer.

Dynamic Media Classic kan generera videosemappningar och mRSS-flöden från metadata som lagras med varje video. När du skapar videosemappningar och mRSS-flöden bestämmer du vilka metadatafält från videofiler som ska inkluderas. På det här sättet beskriver du dina videoklipp för sökmotorer så att sökmotorer kan dirigera trafik till videoklipp på din webbplats mer exakt

>[!NOTE]
>
>Innan du skapar en webbplatskarta för video eller RSS-feed bör du ta reda på vilka fält sökmotorn behöver i XML-filen och hur du strukturerar dessa fält. Om du vill skapa en lyckad webbplatskarta för video eller mRSS-feed måste den uppfylla kraven i sökmotorn.

I Dynamic Media Classic skapas rapporter om webbplatskartor för video och mRSS-flöden när du har genererat dem. Rapporterna finns på sidan Video SEO Report.

>[!NOTE]
>
>För Video Sitemaps och mRSS-flöden hämtar Dynamic Media Classic endast metadata från videoklipp som har markerats för publicering. Markera videoklipp för publicering för att inkludera deras metadata i webbplatskartor för video och mRSS-flöden.

## Välja SEO-inställningar för video {#choosing-video-seo-settings}

Klicka på SEO-inställningar för video för webbplatskartor och mRSS-flöden på sidan **[!UICONTROL Video Search Engine Optimization Settings]**. Om du vill öppna den här sidan klickar du på **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Settings]** i fältet Global Navigation.

I **[!UICONTROL General Setting]**-området väljer du om du vill generera webbplatskartor för video, mRSS-flöden eller både och. Mappa metadatafält till indatafält i **[!UICONTROL Generation Settings]**-området.

När du har valt inställningar klickar du på **[!UICONTROL Save]** (eller **[!UICONTROL Save & Generate]**) för att skapa videosemap, mRSS-flöden eller båda.

### Välj allmänna inställningar {#choosing-general-settings}

Välj ett rapportläge i listrutan **[!UICONTROL Generation Mode]**:

* **Webbplatskarta**  för video - Skapa en webbplatskarta för video.

* **mRSS-feed**  - Skapa en mRSS-feed (Media RSS).

* **Båda**  - Skapa båda typerna av XML-filer.

* **Av** - Välj det här alternativet om du vill sluta generera video-platskartor och media-RSS-flöden (mRSS).

I listrutan **[!UICONTROL Automatic/Manual Mode]** väljer du om du vill generera automatiskt eller manuellt:

* **Automatiskt läge**  - Dynamic Media Classic genererar automatiskt en video-platskarta, en media-RSS-matning (mRSS) eller båda, varje dag. Välj alternativet Markera för publicering om du automatiskt vill markera XML-filen som genereras i Dynamic Media Classic för publicering.

   * **Markera för** PublishMarks för att publicera XML-filen som genereras.

* **Manuellt läge**  - Dynamic Media Classic genererar videowebbplatskartan, Media RSS-matningen (mRSS) eller både och när du klickar på Generera eller Spara och generera på skärmen Optimeringsinställningar för videosökning. Välj även följande alternativ:

   * **Inga ytterligare inställningar**  - Markerar inte för publicering av XML-filen som genereras.

   * **Markera för publicering**  - Markera för publicering den XML-fil som genereras.

   * **Tillåt delvis generering**  - Sökmotorer kan avvisa en XML-fil om den inte innehåller fullständig metadatainformation för alla videoklipp. Med det här alternativet genereras XML-filen även om metadata inte är tillgängliga för vissa videoklipp. En varning registreras på rapportskärmen. Välj det här alternativet om du tänker exportera XML-filen och bearbeta den saknade informationen manuellt.

### Väljer genereringsinställningar {#choosing-generation-settings}

I området Genereringsinställningar visas indatafält för Video SiteMap, eller mRSS-feed, eller båda, samt namn på metadatafält på panelen Metadata. Använd området Allmänna inställningar för att mappa inmatningsfält till metadatafält. På så sätt anger du var Dynamic Media Classic ska hämta metadata för Video Sitemap och/eller mRSS-feed.

1. Välj en metadatavy på menyn Metadatavy. När du har valt en vy visas namnen på metadatafälten på panelen Metadata.
Se [Metadatavyer](application-setup.md#metadata_views).
1. Dra metadatafältnamn från panelen Metadata till indatafälten Landningssida, Titel, Beskrivning, Taggar och Kategori. Fälten Landningssida, Titel och Beskrivning är obligatoriska.

   >[!NOTE]
   >
   >Du kan också manuellt ange data i indatafält.

1. Gör något av följande:

   * Om du vill spara inställningarna utan att generera XML-filen klickar du på **[!UICONTROL Save]**.
   * Klicka på **[!UICONTROL Save & Generate]** om du vill spara och generera filen.

      XML-filen genereras och registreras i jobbloggen. Webbplatskarta för video (video-sitemap) och RSS-flöden (Media RSS) (mrss-feed) lagras i företagets rotmapp.

>[!NOTE]
>
>Publicera webbplatskartan för video eller mRSS-flöden innan du kan skicka den till sökmotorer. Video Sitemap- och Media RSS-matningsfiler (mRSS) lagras i företagets rotmapp. Markera dessa XML-filer för publicering, om det behövs, och klicka på **[!UICONTROL Publish]**.

## Skicka videowebbplatskartor och RSS-feed-filer till sökmotorer {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Video Sitemap- och Media RSS-matningsfiler (mRSS) lagras i företagets rotmapp:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Kopiera en av dessa URL:er till sökmotorns webbmaster-verktyg för att skicka din Video Sitemap- eller Media RSS-matningsfil (mRSS) till sökmotorer.

## Visa SEO-rapporter för video {#viewing-video-seo-reports}

Visa SEO-rapporter för video på sidan för optimeringsrapport för videosökmotor. Om du vill öppna den här sidan klickar du på **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Reports]** i fältet Global Navigation.

Om fel uppstår när en rapport genereras visas de på rapportsidan.
