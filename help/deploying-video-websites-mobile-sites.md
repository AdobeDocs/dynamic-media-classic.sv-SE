---
title: Distribuera video till webbplatser och mobilsajter
description: Lär dig hur du distribuerar video till webbplatser och mobilsajter från Adobe Dynamic Media Classic.
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 3df22d48-edb5-4927-aefb-104b53f81f1a
source-git-commit: 44045daa35052f01a26c67e0b2a0fb1405c53292
workflow-type: tm+mt
source-wordcount: '1587'
ht-degree: 1%

---

# Distribuera video till webbplatser och mobilsajter{#deploying-video-to-your-websites-and-mobile-sites}

Webbplatser, mobilsajter och datorprogram har åtkomst till serverinnehåll i Adobe Dynamic Media Classic, inklusive video, via URL-strängar eller inbäddad kod. Adobe Dynamic Media Classic aktiverar dessa URL-strängar under publiceringsprocessen. Om du vill placera URL-strängen eller inbäddningskoden för videon på webbsidor, mobilsidor och datorprogram kopierar du den från Adobe Dynamic Media Classic.

>[!NOTE]
>
>URL:en eller inbäddningskoden är inte aktiv förrän du publicerar resursen.

## Publicera video {#publishing-video}

Genom att publicera en video kan Adobe Dynamic Media Classic-servrar leverera video till webbplatser, mobilsajter och applikationer.

Det finns två olika metoder som du kan använda för att publicera video:

* **Publicera videoklipp automatiskt och direkt vid överföring**  - Som en del av videoöverföringen kan Adobe Dynamic Media Classic automatiskt publicera videoklipp när de överförs och kodas. Denna möjlighet att publicera direkt innebär att man inte behöver publicera videor separat efter det att man gjort det.

* **Publicera videon manuellt efter överföring**  - Om du inte vill publicera videoklipp direkt kan du publicera videoklipp manuellt när du vill.

När du har publicerat videofilmer aktiveras URL-strängarna för HTML-sidan eller programkoden i Adobe Dynamic Media Classic.

**Så här publicerar du video:**

1. Gör något av följande:

   * Om du vill publicera videoklipp automatiskt och omedelbart vid överföring väljer du **[!UICONTROL Publish after uploading]** på sidan Överför. Du är färdig; det inte finns några fler steg att slutföra.
   * Om du vill publicera videoklipp manuellt efter överföringen markerar du videoklippen på panelen Bläddra och väljer sedan **Publicera** på fältet Global navigering.

## Länka en video-URL till en mobilwebbplats eller en webbplats {#linking-a-video-url-to-a-mobile-site-or-a-website}

När du har publicerat en video kan du hämta dess URL för användning på din webbplats, på din mobila webbplats eller i datorprogrammet. Använd video-URL:en när du vill visa video i ett popup-fönster eller modalt fönster ovanpå webbsidan.

När en kund väljer länken identifieras deras enhet, bandbredd och skärmstorlek automatiskt. Lämplig video visas för uppspelning i ett fördefinierat visningsprogram för datorer eller i mobilenhetens inbyggda videospelare för smarttelefoner och surfplattor.

Se även [Bädda in visningsprogrammet på en webbsida](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**Så här länkar du en video-URL till en mobilwebbplats eller en webbplats:**

1. Välj **[!UICONTROL Video]** eller **[!UICONTROL Adaptive Video Set]** i listrutan i panelen Resurssökning.**[!UICONTROL Show]**
1. navigera till resursmappen som innehåller den video- eller adaptiva videouppsättning som du vill länka i resurspanelen till vänster.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Välj **[!UICONTROL Grid View]** eller **[!UICONTROL List View]**. Dubbelklicka på videominiatyrbilden för en enskild resurs i panelen Resursbläddring för att öppna den i detaljvyn. Välj **[!UICONTROL Copy URL]** till höger om det visningsprogram du vill använda under HTTP-direktuppspelning på panelen URL:er och Bädda in kod till höger. Du bör kopiera den URL som är kopplad till `Universal_HTML5_Video`-visningsprogrammet.
   * Välj **[!UICONTROL Grid View]**. Markera en enskild resurs på panelen Resursbläddring och gå sedan till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** under miniatyrbilden.

      Välj **[!UICONTROL Copy URL]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista. Du bör kopiera den URL som är kopplad till `Universal_HTML5_Video`-visningsprogrammet.

   * Välj **[!UICONTROL List View]**. Markera en enskild resurs på panelen Resursbläddring och gå sedan till höger om miniatyrbilden till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Välj **[!UICONTROL Copy URL]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista. Du bör kopiera den URL som är kopplad till `Universal_HTML5_Video`-visningsprogrammet.

   * Välj **[!UICONTROL Grid View]**, **[!UICONTROL List View]** eller **[!UICONTROL Detail View]**. Gå till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** på samma verktygsfält.

      Välj **[!UICONTROL Copy URL]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista. Du bör kopiera den URL som är kopplad till `Universal_HTML5_Video`-visningsprogrammet.

1. Klistra in HTML5-videons URL-länk på webbplatsen och den mobila webbplatsen.

## Bädda in videovisningsprogrammet på en webbsida {#embedding-the-video-viewer-on-a-web-page}

Använd funktionen Bädda in kod när du vill spela upp videon som är inbäddad på webbsidan. Du kopierar inbäddningskoden till Urklipp så att du kan klistra in den på webbsidorna. Det är inte tillåtet att redigera koden i dialogrutan Bädda in kod.

Se även [Länka en video-URL till en mobilwebbplats eller en webbplats](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**Så här bäddar du in videovisningsprogrammet på en webbsida:**

1. Välj **[!UICONTROL Video]** eller **[!UICONTROL Adaptive Video Set]** i listrutan Visa på panelen Resurser.
1. navigera till resursmappen som innehåller den video- eller adaptiva videouppsättning vars inbäddningskod du vill kopiera i resurspanelen till vänster.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Välj **[!UICONTROL Grid View]** eller **[!UICONTROL List View]**. Dubbelklicka på videominiatyrbilden för en enskild resurs i panelen Resursbläddring för att öppna den i detaljvyn. Välj **[!UICONTROL Embed Code]** till höger om det visningsprogram du vill använda under HTTP-direktuppspelning på panelen URL:er och Bädda in kod till höger. Välj **[!UICONTROL Embed Code]** som är associerat med `Universal_HTML5_Video`-visningsprogrammet som en god rutin.
   * Välj **[!UICONTROL Grid View]**. Markera en enskild resurs på panelen Resursbläddring och välj **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** under miniatyrbilden för videon.

      Välj **[!UICONTROL Embed Code]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista. Välj **[!UICONTROL Embed Code]** som är associerat med `Universal_HTML5_Video`-visningsprogrammet som en god rutin.

   * Välj **[!UICONTROL List View]**. Markera en enskild resurs på panelen Resursbläddring och gå sedan till höger om miniatyrbilden till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      Välj **[!UICONTROL Embed Code]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista. Välj **[!UICONTROL Embed Code]** som är associerat med `Universal_HTML5_Video`-visningsprogrammet som en god rutin.

   * Välj **[!UICONTROL Grid View]**, **[!UICONTROL List View]** eller **[!UICONTROL Detail View]**. Gå till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]** på samma verktygsfält.

      Välj **[!UICONTROL Embed Code]** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista. Välj **[!UICONTROL Embed Code]** som är associerat med `Universal_HTML5_Video`-visningsprogrammet som en god rutin.

1. Välj **[!UICONTROL Copy to Clipboard]** i dialogrutan Bädda in kod.

   Det är inte tillåtet att redigera koden i dialogrutan Bädda in kod.

1. välj **[!UICONTROL Close]**.
1. Klistra in inbäddningskoden på dina webbsidor.

### Implementera inbäddningskod för HTML5-video med MP4-videor {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Om du inte använder videospelaren Adobe Dynamic Media Classic HTML5, utan i stället vill använda den inbyggda HTML5 `<video>`-taggen med MP4-videoresurser, kan du använda följande exempel på inbäddningskod:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Ersätt `"S7 video thumbnail URL"` med videons miniatyrbilds-URL, som är videons miniatyrbild som en användare ser innan de spelar upp videon.

   Se [Hämta URL-adresser för videominiatyrbilder](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Ersätt `"S7 OGG video asset URL (no player)"` med videons progressiva URL för OGG-video.

   Se [Länka en video-URL till en mobilwebbplats eller en webbplats](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Ersätt `"S7 MP4 mobile progressive video asset URL (no player)"` med videons mobila progressiva URL.

   Se [Länka en video-URL till en mobilwebbplats eller en webbplats](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Distribuera video med en videospelare från tredje part {#deploying-video-using-a-third-party-video-player}

Om du använder en videospelare från en annan leverantör eller en anpassad videospelare i stället för ett Dynamic Media Classic-visningsprogram, får du den direkta video-URL som fungerar för HLS-videoströmning med flera bithastigheter eller progressiv nedladdning.

**Så här distribuerar du video med en videospelare från tredje part:**

1. I Adobe Dynamic Media Classic går du till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** i fältet Global Navigation.
1. Beroende på vilken typ av URL som du vill använda gör du något av följande:

* Generera en URL för direktuppspelad HLS-video (flerbithastighet)

   På sidan **[!UICONTROL Application General Settings]** skapar du den direkta URL:en i gruppen **[!UICONTROL Servers]** i textfältet **[!UICONTROL Published Server Name]**. Använd följande syntax: `server/is/content/company/folder/filename.m3u8`

   Anta till exempel att namnet på den publicerade servern är `https://s7d9.scene7.com/.` Om du använder syntaxen i steg 2 kan den direkta URL:en se ut så här:
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* Generera en URL för direktuppspelad HLS-video (enkelbithastighet)

   På sidan **[!UICONTROL Application General Settings]** i gruppen **[!UICONTROL Servers]** i textfältet **[!UICONTROL HLS Streaming Server Name]** konstruerar du den direkta URL:en med följande syntax:

   `server/company/folder/filename.ext.m3u8`

   Anta till exempel att namnet på servern för HLS-direktuppspelning är `https://s7mbrstream.scene7.com/hls-vod/`. Med syntaxen i steg 2 kan den direkta URL:en se ut så här:
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* Generera en URL för direkt progressiv video

   På sidan **[!UICONTROL Application General Settings]** i gruppen **[!UICONTROL Servers]** i textfältet **[!UICONTROL Progressive Video Server Name]** konstruerar du den direkta eVideo-URL:en med följande syntax:

   `server/company/folder/filename`

   Anta till exempel att namnet på den progressiva videoservern är `https://s7d9.scene7.com/is/content/`. Med syntaxen i steg 2 kan den direkta URL:en se ut så här:
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## Arbeta med videominiatyrer {#working-with-video-thumbnails}

Adobe Dynamic Media Classic genererar miniatyrbilder för kodade videofilmer och förkodade videofilmer. Du kan använda videominiatyrer som vilken bildresurs som helst. Dessutom kan du hämta URL:er för de videominiatyrbilder som skapas i Adobe Dynamic Media Classic och distribuera dessa URL:er utanför Adobe Dynamic Media Classic. Du kan till exempel distribuera miniatyrbilderna i sökresultat, relaterade videolistor och videouppspelningslistor på en webbplats.

Miniatyrbilder genereras baserat på den första heterogena bildrutan (inte en helt svart bildruta, eller en helt vit bildruta o.s.v.) i videon.

### Hämta URL-adresser för videominiatyrbilder {#obtaining-video-thumbnail-urls}

Adobe Dynamic Media Classic genererar videominiatyrer automatiskt under överföringen. Miniatyrbilderna visas i panelen Bläddra i listvyn och stödrastervyn.

Utför en publiceringsåtgärd för att generera URL:er för videominiatyrer.

Se [Publicera video](deploying-video-websites-mobile-sites.md#publishing_video).

Efter publiceringen kan du hämta URL:er för videominiatyrbilder i detaljvyn på panelen URL:er och Bädda in kod. Välj **[!UICONTROL Copy URL]** till höger om videominiatyrbilden så att du kan kopiera dess URL.

### Ändra affischbildrutor i videovisningsprogram {#modifying-poster-frames-in-video-viewers}

*affischbildrutan* är den första bildrutan som visas i videomottagare innan videon börjar spelas upp. I Adobe Dynamic Media Classic används videominiatyrer som affischbildrutor.

Du kan använda bildmodifieringar i affischbildrutan. Du kan till exempel beskära affischramen eller göra den genomskinlig. Om du vill ändra affischbildrutan öppnar du konfigurationsskärmen för videovisningsprogrammet och anger modifierare i avsnittet Förhandsvisningsbildsmodifierare.

Se [Lägga till eller redigera en förinställning för visningsprogram för video](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Se [Image Serving Guide](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-is-home.html?lang=en#image-serving-api).

Du kan också ändra videominiatyrbilder genom att lägga till modifierare till URL:er för videominiatyrbilder.

>[!MORELIKETHIS]
>
>* [Publicera filer](publishing-files.md#publishing_files)