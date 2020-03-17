---
title: Video SEO (sökmotoroptimering)
seo-title: Video SEO (sökmotoroptimering)
description: 'null'
seo-description: Lär dig hur du konfigurerar SEO-inställningar för video.
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
translation-type: tm+mt
source-git-commit: de7d2608f94935f238a11d8310b97dddc5476f57

---


# Video SEO (sökmotoroptimering){#video-seo-search-engine-optimization}

SEO är processen att förbättra trafiken till en webbplats från sökmotorer. Sökmotorer är utmärkta på att samla in information om textbaserat innehåll, men de kan inte hämta in information om video på ett adekvat sätt om de inte får den här informationen.

Med hjälp av Dynamic Media Classic Video SEO kan du använda videometadata för att ge sökmotorer beskrivningar av videoklipp. Med Dynamic Media Classic kan du skapa webbplatskartor för video och mRSS-flöden. Det här är XML-filer av standardtyp för att skicka videoinformation till sökmotorer:

**Video Sitemap** Informerar Google om exakt var och vad videomaterialet finns på en webbplats. Därför är videor helt sökbara på Google. En webbplatskarta för video kan till exempel ange körningstid och videokategorier. Mer information om webbplatskartor finns på https://www.google.com/support/webmasters/bin/answer.py?answer=80471.

**mRSS-matning (Media Really Simple Syndication)** som används av utgivare för att skicka mediefiler till Yahoo! Videosökning. Mer information om mRSS-flöden finns på https://www.rssboard.org/media-rss.

>[!NOTE]
>
>Google stöder både Video Sitemap- och mRSS-feed-protokollet för att skicka information till sökmotorer.

Med Dynamic Media Classic kan du generera webbplatskartor för video och mRSS-flöden från metadata som lagras med varje video. När du skapar videosemappningar och mRSS-flöden bestämmer du vilka metadatafält från videofiler som ska inkluderas. På det här sättet beskriver du dina videoklipp för sökmotorer så att sökmotorer kan dirigera trafik till videoklipp på din webbplats mer exakt

>[!NOTE]
>
>Innan du skapar en webbplatskarta för video eller RSS-feed bör du ta reda på vilka fält sökmotorn behöver i XML-filen och hur du strukturerar dessa fält. Om du vill skapa en lyckad webbplatskarta för video eller mRSS-feed måste den uppfylla kraven i sökmotorn.

Med Dynamic Media Classic skapas rapporter om webbplatskartor för video och mRSS-flöden när du har genererat dem. Dessa rapporter finns på videons SEO-rapportskärm.

>[!NOTE]
>
>För Video Sitemaps och mRSS-flöden hämtar Dynamic Media Classic endast metadata från videoklipp som har markerats för publicering. Markera videoklipp för publicering för att inkludera deras metadata i webbplatskartor för video och mRSS-flöden.

## Välja SEO-inställningar för video {#choosing-video-seo-settings}

Välj SEO-inställningar för video för webbplatskartor och mRSS-flöden på skärmen Optimeringsinställningar för videosökmotor. Om du vill öppna den här skärmen väljer du Konfigurera > Programinställningar > Video SEO > Inställningar.

Under Allmänna inställningar väljer du om du vill generera webbplatskartor för video, mRSS-flöden eller både och. Mappa metadatafält till indatafält i området Genereringsinställningar.

När du har valt inställningar klickar du på Generera (eller Spara och generera) för att skapa videosemap, mRSS-flöden eller båda.

### Välj allmänna inställningar {#choosing-general-settings}

Välj ett rapportläge i listrutan Genereringsläge:

**Webbplatskarta** för video Skapa en webbplatskarta för video.

**mRSS-feed** Skapa en mRSS-matning (Media RSS).

**Båda** Skapa båda typerna av XML-filer.

**Av** Välj det här alternativet om du vill sluta generera videosemappningar och en Media RSS-matning (mRSS).

I listrutan Automatiskt/Manuellt läge väljer du om du vill generera automatiskt eller manuellt:

**Med det automatiska läget** Dynamic Media Classic genereras automatiskt en video-platskarta, en media-RSS-matning (mRSS) eller båda, varje dag. Välj alternativet Markera för publicering om du automatiskt vill markera XML-filen som genereras i Dynamic Media Classic för publicering.

**Manuellt läge** Dynamic Media Classic genererar videosemappningen, Media RSS-matningen (mRSS) eller både och när du klickar på Generera eller Spara och generera på skärmen Optimeringsinställningar för videosökning. Välj även följande alternativ:

**Inga ytterligare inställningar** Markerar inte för publicering av XML-filen som genereras.

**Markera för publiceringsmärken** för att publicera XML-filen som genereras.

**Tillåt sökmotorer med delvis generering** kan avvisa en XML-fil om den inte innehåller fullständig metadatainformation för alla videoklipp. Med det här alternativet genereras XML-filen även om metadata inte är tillgängliga för vissa videoklipp. En varning registreras på rapportskärmen. Välj det här alternativet om du tänker exportera XML-filen och bearbeta den saknade informationen manuellt.

### Välja genereringsinställningar {#choosing-generation-settings}

I området Genereringsinställningar visas indatafält för Video Sitemap och/eller mRSS-feed och namn på metadatafält på panelen Metadata. Använd området Allmänna inställningar för att mappa inmatningsfält till metadatafält. Genom att göra det anger du för Dynamic Media Classic var metadata för Video Sitemap och/eller mRSS-feed ska hämtas.

1. Välj en metadatavy på menyn Metadatavy. När du har valt en vy visas namnen på metadatafälten på panelen Metadata. (Mer information om metadatavyer finns i [Metadatavyer](application-setup.md#metadata_views).)
1. Dra metadatafältnamn från panelen Metadata till indatafälten Landningssida, Titel, Beskrivning, Taggar och Kategori. Fälten Landningssida, Titel och Beskrivning är obligatoriska.

   >[!NOTE]
   >
   >Du kan också manuellt ange data i indatafält.

1. Klicka på Spara (för att spara inställningarna utan att generera XML-filen), Generera (för att generera XML-filen) eller Spara och generera (för att spara och generera filen).

   XML-filen genereras och registreras i jobbloggen. Webbplatskarta för video (video-sitemap) och RSS-flöden (Media RSS) (mrss-feed) lagras i företagets rotmapp.

>[!NOTE]
>
>Du måste publicera webbplatskartan för video eller mRSS-flöden innan du kan skicka den till sökmotorer. Video Sitemap- och Media RSS-matningsfiler (mRSS) lagras i företagets rotmapp. Markera dessa XML-filer för publicering, om det behövs, och klicka på Publicera.

## Skicka videowebbplatskartor och RSS-feed-filer till sökmotorer {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Video Sitemap- och Media RSS-matningsfiler (mRSS) lagras i företagets rotmapp:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Kopiera en av dessa URL:er till sökmotorns webbmaster-verktyg för att skicka din Video Sitemap- eller Media RSS-matningsfil (mRSS) till sökmotorer.

## Visa SEO-rapporter för video {#viewing-video-seo-reports}

Visa SEO-rapporter för video på skärmen för optimeringsrapport för videosökmotor. Om du vill öppna den här skärmen klickar du på Inställningar > Programinställningar > Video SEO > Rapporter.

Om fel uppstår när en rapport genereras visas de på rapportskärmen.