---
title: Distribuera video till webbplatser och mobilsajter
seo-title: Distribuera video till webbplatser och mobilsajter
description: 'null'
seo-description: Lär dig hur du distribuerar video till webbplatser och mobilsajter.
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Distribuera video till webbplatser och mobilsajter{#deploying-video-to-your-websites-and-mobile-sites}

Webbplatser, mobilsajter och datorprogram får tillgång till dynamiskt Media Classic-serverinnehåll, inklusive video, via URL-strängar eller inbäddad kod. Dynamic Media Classic aktiverar dessa URL-strängar under publiceringsprocessen. Om du vill placera URL-strängen eller bädda in koden för videon på dina webbsidor, mobilsidor och datorprogram kopierar du den från Scene7 Publishing System.

>[!NOTE]
>
>URL:en eller inbäddningskoden är inte aktiv förrän du publicerar resursen.

## Publicera video {#publishing-video}

Genom att publicera en video kan Dynamic Media Classic-servrar leverera video till webbplatser, mobilsajter och applikationer.

Det finns två olika metoder som du kan använda för att publicera video:

* **Publicera videoklipp automatiskt och direkt vid överföring**

   Som en del av videoöverföringen kan Dynamic Media Classic automatiskt publicera videor när de överförs och kodas. Denna möjlighet att publicera direkt innebär att man inte behöver publicera videor separat efter det att man gjort det.

* **Publicera video manuellt efter överföring**

   Om du inte vill publicera videoklipp direkt kan du när som helst publicera videoklipp manuellt.

När du har publicerat videofilmer aktiverar Scene7 Publishing System URL-strängarna för HTML-sidan eller programkoden.

**Publicera video**

1. Gör något av följande:

   * Om du vill publicera videoklipp automatiskt och omedelbart vid överföring klickar du på **Publicera efter överföring** på överföringsskärmen. Du är färdig; det inte finns några fler steg att slutföra.
   * Om du vill publicera videoklipp manuellt efter överföringen markerar du videoklippen på panelen Bläddra och klickar sedan på **Publicera** i fältet Global navigering.

## Länka en video-URL till en mobilwebbplats eller en webbplats {#linking-a-video-url-to-a-mobile-site-or-a-website}

När du har publicerat en video kan du hämta dess URL för användning på din webbplats, på din mobila webbplats eller i datorprogrammet. Använd video-URL:en när du vill visa video i ett popup-fönster eller modalt fönster ovanpå webbsidan.

När en kund klickar på länken identifieras deras enhet, bandbredd och skärmstorlek automatiskt. Lämplig video visas för uppspelning i ett fördefinierat visningsprogram för datorer eller i mobilenhetens inbyggda videospelare för smarttelefoner och surfplattor.

Se även [Bädda in videovisningsprogrammet på en webbsida](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**Så här länkar du en video-URL till en mobilwebbplats eller en webbplats**

1. Klicka på **Video** eller **Adaptiv videouppsättning** i listrutan Visa på panelen Resursbläddring.
1. navigera till resursmappen som innehåller den video- eller adaptiva videouppsättning som du vill länka i resurspanelen till vänster.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Klicka på **Stödrastervisning** eller **Listvy**. Dubbelklicka på videominiatyrbilden för en enskild resurs på panelen Resursbläddring för att öppna den i detaljvyn. I panelen URL:er och panelen Bädda in kod till höger, under HTTP-direktuppspelning, klickar du på **Kopiera URL** till höger om det visningsprogram du vill använda. Det är en god idé att kopiera den URL som är kopplad till `Universal_HTML5_Video` visningsprogrammet.
   * Klicka på **Stödrastervisning**. Markera en enskild resurs på panelen Resursbläddring och klicka sedan under miniatyrbilden på **Förhandsvisa** > **Visningsprogramlista**.

      Klicka på **Kopiera URL** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista. Det är en god idé att kopiera den URL som är kopplad till `Universal_HTML5_Video` visningsprogrammet.

   * Klicka på **Listvy**. Markera en enskild resurs på panelen Resursbläddring och klicka sedan på **Förhandsvisa** > **Visningslista** till höger om miniatyrbilden.

      Klicka på **Kopiera URL** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista. Det är en god idé att kopiera den URL som är kopplad till `Universal_HTML5_Video` visningsprogrammet.

   * Klicka på **Stödrastervisning**, **Listvy** eller **Detaljvy**. Klicka på **Förhandsgranska** > **Visningsprogramlista** i samma verktygsfält.

      Klicka på **Kopiera URL** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista. Det är en god idé att kopiera den URL som är kopplad till `Universal_HTML5_Video` visningsprogrammet.

1. Klistra in HTML5-videons URL-länk på webbplatsen och den mobila webbplatsen.

## Bädda in videovisningsprogrammet på en webbsida {#embedding-the-video-viewer-on-a-web-page}

Använd funktionen Bädda in kod när du vill spela upp videon som är inbäddad på webbsidan. Du kopierar inbäddningskoden till Urklipp så att du kan klistra in den på webbsidorna. Det är inte tillåtet att redigera koden i dialogrutan Bädda in kod.

Se även [Länka en video-URL till en mobilwebbplats eller en webbplats](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**Bädda in videovisningsprogrammet på en webbsida**

1. Klicka på **Video** eller **Adaptiv videouppsättning** i listrutan Visa på panelen Resursbläddring.
1. navigera till resursmappen som innehåller den video- eller adaptiva videouppsättning vars inbäddningskod du vill kopiera i resurspanelen till vänster.
1. Gör något av följande ovanför panelen Resurssökning, till höger i verktygsfältet:

   * Klicka på **Stödrastervisning** eller **Listvy**. Dubbelklicka på videominiatyrbilden för en enskild resurs i panelen Resursbläddring för att öppna den i detaljvyn. I panelen URL:er och panelen Bädda in kod till höger, under HTTP-direktuppspelning, klickar du på **Bädda in kod** till höger om det visningsprogram du vill använda. Det bästa är att klicka på **Bädda in kod** som är kopplad till `Universal_HTML5_Video` visningsprogrammet.
   * Klicka på **Stödrastervisning**. Markera en enskild resurs på panelen Resursbläddring och klicka sedan under miniatyrbilden för videon på **Förhandsgranska** > **Visningsprogramlista**.

      Klicka på **Bädda in kod** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista. Det bästa är att klicka på **Bädda in kod** som är kopplad till `Universal_HTML5_Video` visningsprogrammet.

   * Klicka på **Listvy**. Markera en enskild resurs på panelen Resursbläddring och klicka sedan på **Förhandsvisa** > **Visningslista** till höger om miniatyrbilden.

      Klicka på **Bädda in kod** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista. Det bästa är att klicka på **Bädda in kod** som är kopplad till `Universal_HTML5_Video` visningsprogrammet.

   * Klicka på **Stödrastervisning**, **Listvy** eller **Detaljvy**. Klicka på **Förhandsgranska** > **Visningsprogramlista** i samma verktygsfält.

      Klicka på **Bädda in kod** under åtgärdskolumnen i tabellen på sidan Visningsprogramlista. Det bästa är att klicka på **Bädda in kod** som är kopplad till `Universal_HTML5_Video` visningsprogrammet.

1. I dialogrutan Bädda in kod klickar du på **Kopiera till Urklipp**.

   Det är inte tillåtet att redigera koden i dialogrutan Bädda in kod.

1. Klicka på **Stäng**.
1. Klistra in inbäddningskoden på dina webbsidor.

### Implementera inbäddningskod för att använda HTML5-video med MP4-videoresurser {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Om du inte använder videospelaren Dynamic Media Classic HTML5, utan i stället vill använda den inbyggda HTML5- `<video>` -taggen med MP4-videoresurser, kan du använda följande exempel på inbäddningskod:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Ersätt `"S7 video thumbnail URL"` med videons miniatyrbilds-URL. Det här är videons miniatyrbild som en användare ser innan de spelar upp videon.

   Se [Hämta URL-adresser för](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls)videominiatyrbilder.

* Ersätt `"S7 OGG video asset URL (no player)"` med videons progressiva URL för OGG-video.

   Se [Länka en video-URL till en mobilwebbplats eller en webbplats](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Ersätt `"S7 MP4 mobile progressive video asset URL (no player)"` med videons mobila progressiva URL.

   Se [Länka en video-URL till en mobilwebbplats eller en webbplats](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Distribuera video med en videospelare från tredje part {#deploying-video-using-a-third-party-video-player}

Om du använder en videospelare från tredje part eller en anpassad inbyggd videospelare i stället för ett dynamiskt Media Classic-videovisningsprogram, kan du få en direkt video-URL som fungerar för HLS-videoströmning med flera bithastigheter eller progressiv nedladdning.

**Distribuera video med en videospelare från tredje part**

1. I Scene7 Publishing System klickar du på **Inställningar** > **Programinställningar** > **Allmänna inställningar** i det globala navigeringsfältet.
1. Beroende på vilken typ av URL som du vill använda gör du något av följande:
* Generera en URL för direktuppspelad HLS-video (flerbithastighet)

   Skapa den direkta URL:en med följande syntax på sidan **Allmänna inställningar** i gruppen **Servrar** i textfältet **Publicerat servernamn** : Anta `server/is/content/company/folder/filename.m3u8`till exempel att namnet på den publicerade servern är `https://s7d9.scene7.com/.` Använda syntaxen i steg 2, så kan den direkta URL:en se ut så här:
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* Generera en URL för direktuppspelad HLS-video (enkelbithastighet)

   Skapa den direkta URL:en med följande syntax på sidan **Allmänna inställningar** i gruppen **Servrar** i textfältet **HLS Streaming Server Name** :
   `server/company/folder/filename.ext.m3u8`
Anta till exempel att namnet på servern för HLS-direktuppspelning är `https://s7mbrstream.scene7.com/hls-vod/`. Med syntaxen i steg 2 kan den direkta URL:en se ut så här:
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* Generera en URL för direkt progressiv video

   På sidan **Allmänna inställningar** för programmet, i gruppen **Servrar** , i textfältet **Progressivt** videoservernamn, konstruerar du den direkta eVideo-URL:en med följande syntax: Anta till `server/company/folder/filename`exempel att namnet på den progressiva videoservern är `https://s7d9.scene7.com/is/content/`. Med syntaxen i steg 2 kan den direkta URL:en se ut så här:
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## Arbeta med videominiatyrer {#working-with-video-thumbnails}

Dynamic Media Classic genererar miniatyrer för kodade videoklipp och förkodade videoklipp. Du kan använda videominiatyrer som vilken bildresurs som helst. Dessutom kan du hämta URL:er för de videominiatyrer som genereras av Dynamic Media Classic och distribuera dessa URL:er utanför SPS. Du kan till exempel distribuera miniatyrbilderna i sökresultat, relaterade videolistor och videouppspelningslistor på en webbplats.

Miniatyrbilder genereras baserat på den första heterogena bildrutan (inte en helt svart bildruta, eller en helt vit bildruta o.s.v.) i videon.

### Hämta URL-adresser för videominiatyrbilder {#obtaining-video-thumbnail-urls}

Dynamic Media Classic genererar videominiatyrer automatiskt under överföringsprocessen. Miniatyrbilderna visas i panelen Bläddra i listvyn och stödrastervyn.

Utför en publiceringsåtgärd för att generera URL:er för videominiatyrer.

Se [Publicera video](deploying-video-websites-mobile-sites.md#publishing_video).

Efter publiceringen kan du hämta URL:er för videominiatyrbilder i detaljvyn på panelen URL:er och Bädda in kod. Klicka på **Kopiera URL** till höger om videominiatyrbilden för att kopiera URL:en

### Ändra affischbildrutor i videovisningsprogram {#modifying-poster-frames-in-video-viewers}

Affischbildrutan ** är den första bildrutan som visas i videovisningsprogrammen innan videon börjar spelas upp. I Dynamic Media Classic används videominiatyrer som affischbildrutor.

Du kan använda bildmodifieringar i affischbildrutan. Du kan till exempel beskära affischramen eller göra den genomskinlig. Om du vill ändra affischbildrutan öppnar du konfigurationsskärmen för videovisningsprogrammet och anger modifierare i avsnittet Förhandsvisningsbildsmodifierare.

Se [Lägga till eller redigera en förinställning](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)för visningsprogram för video.

Se [www.adobe.com/go/learn_s7_image_server_guide_en](https://www.adobe.com/go/learn_s7_image_server_guide_en).

Du kan också ändra videominiatyrbilder genom att lägga till modifierare till URL:er för videominiatyrbilder.

>[!MORELIKETHIS]
>
>* [Publicera filer ](publishing-files.md#publishing_files)
