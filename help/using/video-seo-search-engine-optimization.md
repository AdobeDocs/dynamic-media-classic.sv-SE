---
title: Video SEO (sökmotoroptimering)
description: Lär dig hur du konfigurerar SEO-inställningar för video i Adobe Dynamic Media Classic.
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
feature: Dynamic Media Classic
role: Admin
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
topic: Content Management
level: Intermediate
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '998'
ht-degree: 0%

---

# Video SEO (sökmotoroptimering){#video-seo-search-engine-optimization}

SEO är processen att förbättra trafiken till en webbplats från sökmotorer. Sökmotorer är utmärkta på att samla in information om textbaserat innehåll, men de kan inte hämta in information om video på ett adekvat sätt om de inte får den här informationen.

Med Adobe Dynamic Media Classic Video SEO kan du använda videometadata för att ge sökmotorer beskrivningar av videoklipp. Med Adobe Dynamic Media Classic kan du skapa webbplatskartor för video och mRSS-flöden. De här XML-standardfilerna används för att skicka videoinformation till sökmotorer:

* **Webbplatskarta för video** - Informerar Google om exakt var och vad videoinnehållet finns på en webbplats. Så videor är helt sökbara på Google. En webbplatskarta för video kan till exempel ange körningstid och videokategorier. Mer information om webbplatskartor finns i [Alternativ för videowebbplatskartor och videowebbplatskartor](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

* **mRSS-feed (Media Really Simple Syndication)** - Används av innehållsutgivare för att skicka mediefiler till Yahoo! Videosökning. Mer information om mRSS-flöden finns i [Alternativ för videowebbplatskartor och videowebbplatskartor](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

>[!NOTE]
>
>Google har stöd för både Video Sitemap och mRSS feed-protokollet för att skicka information till sökmotorer.

Adobe Dynamic Media Classic kan generera videosemappningar och mRSS-flöden från metadata som lagras med varje video. När du skapar videosemappningar och mRSS-flöden bestämmer du vilka metadatafält från videofiler som ska inkluderas. På det här sättet beskriver du videoklipp för sökmotorer så att sökmotorer kan dirigera trafik till videofilmer på din webbplats på ett mer exakt sätt.

>[!NOTE]
>
>Innan du skapar en webbplatskarta för video eller RSS-feed bör du ta reda på vilka fält sökmotorn behöver i XML-filen och hur du strukturerar dessa fält. Om du vill skapa en lyckad webbplatskarta för video eller mRSS-feed måste den uppfylla kraven i sökmotorn.

Adobe Dynamic Media Classic skapar rapporter om webbplatskartor för video och mRSS-flöden när du har genererat dem. Rapporterna finns på sidan Video SEO Report.

>[!NOTE]
>
>För Video Sitemaps och mRSS-flöden hämtar Adobe Dynamic Media Classic endast metadata från videoklipp som har markerats för publicering. Markera videoklipp för publicering för att inkludera deras metadata i webbplatskartor för video och mRSS-flöden.

## Välj SEO-inställningar för video {#choosing-video-seo-settings}

Välj SEO-inställningar för video för webbplatskartor och mRSS-flöden på **[!UICONTROL Video Search Engine Optimization Settings]** sida. Om du vill öppna den här sidan går du till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Settings]**.

I **[!UICONTROL General Setting]** väljer du om du vill generera videosemappningar, mRSS-flöden eller både och. I **[!UICONTROL Generation Settings]** mappa metadatafält till indatafält.

När du har valt inställningar väljer du **[!UICONTROL Save]** (eller **[!UICONTROL Save & Generate]**) för att skapa Video Sitemap, mRSS-flöden eller båda.

### Ställ in allmänna inställningar {#choosing-general-settings}

På **[!UICONTROL Generation Mode]** väljer du ett rapportläge:

* **Webbplatskarta för video** - Skapa en webbplatskarta för video.

* **mRSS-feed** - Skapa en mRSS-matning (Media RSS).

* **Båda** - Skapa båda typerna av XML-filer.

* **Av** - Välj det här alternativet om du vill sluta generera video-platskartor och media-RSS-flöden (mRSS).

På **[!UICONTROL Automatic/Manual Mode]** väljer du om du vill generera automatiskt eller manuellt:

* **Automatiskt läge** - Adobe Dynamic Media Classic genererar automatiskt en video-platskarta, media-RSS (mRSS) eller båda, varje dag. Välj **[!UICONTROL Mark for Publish]** om du vill att XML-filen som genereras av Adobe Dynamic Media Classic ska markeras automatiskt.

   * **Markera för publicering** Markerar för publicering av XML-filen som genereras.

* **Manuellt läge** - Adobe Dynamic Media Classic genererar videowebbplatskartan, Media RSS-matning (mRSS) eller båda, när du väljer **[!UICONTROL Generate]** eller **[!UICONTROL Save & Generate]** på skärmen Optimeringsinställningar för videosökning. Välj även följande alternativ:

   * **Inga ytterligare inställningar** - Markerar inte för publicering av XML-filen som genereras.

   * **Markera för publicering** - Markerar för publicering av XML-filen som genereras.

   * **Tillåt partiell generering** - Sökmotorer kan avvisa en XML-fil om den inte innehåller fullständig metadatainformation för alla videor. Med det här alternativet genereras XML-filen även om metadata inte är tillgängliga för vissa videoklipp. En varning registreras på rapportskärmen. Välj det här alternativet om du tänker exportera XML-filen och bearbeta den saknade informationen manuellt.

### Välja genereringsinställningar {#choosing-generation-settings}

I området Genereringsinställningar visas indatafält för Video SiteMap, eller mRSS-feed, eller båda, samt namn på metadatafält på panelen Metadata. Använd området Allmänna inställningar för att mappa inmatningsfält till metadatafält. På så sätt anger du för Adobe Dynamic Media Classic var metadata för Video Sitemap och/eller mRSS-feed ska hämtas.

1. Välj en metadatavy på menyn Metadatavy. När du har valt en vy visas namnen på metadatafälten på panelen Metadata.
Se [Metadatavyer](application-setup.md#metadata_views).
1. Dra metadatafältnamn från panelen Metadata till indatafälten Landningssida, Titel, Beskrivning, Taggar och Kategori. Fälten Landningssida, Titel och Beskrivning är obligatoriska.

   >[!NOTE]
   >
   >Du kan också manuellt ange data i indatafält.

1. Gör något av följande:

   * Om du vill spara inställningarna utan att generera XML-filen väljer du **[!UICONTROL Save]**.
   * Om du vill spara och generera filen väljer du **[!UICONTROL Save & Generate]**.

     XML-filen genereras och registreras i jobbloggen. Webbplatskarta för video (video-sitemap) och RSS-flöden (Media RSS) (mrss-feed) lagras i företagets rotmapp.

>[!NOTE]
>
>Publicera webbplatskartan för video eller mRSS-flöden innan du kan skicka den till sökmotorer. Video Sitemap- och Media RSS-matningsfiler (mRSS) lagras i företagets rotmapp. Markera XML-filerna för publicering, om det behövs, och välj **[!UICONTROL Publish]**.

## Skicka videowebbplatskartor och RSS-feed-filer till en sökmotor {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Video Sitemap- och Media RSS-matningsfiler (mRSS) lagras i företagets rotmapp:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Kopiera en av dessa URL:er till sökmotorns webbmaster-verktyg för att skicka din Video Sitemap- eller Media RSS-matningsfil (mRSS) till sökmotorer.

## Visa SEO-rapporter för video {#viewing-video-seo-reports}

Visa SEO-rapporter för video på sidan för optimeringsrapport för videosökmotor. Om du vill öppna den här sidan går du till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Reports]**.

Om fel uppstår när en rapport genereras visas de på rapportsidan.
