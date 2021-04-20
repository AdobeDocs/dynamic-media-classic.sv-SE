---
title: 'Publicera filer '
description: '"Lär dig hur du publicerar dina resurser på Dynamic Media Image Servers. Du kan publicera resurser en gång eller ordna så att Dynamic Media Classic publicerar resurser enligt ett återkommande schema. När resurserna har publicerats är de tillgängliga för leverans. Du kan kopiera URL-anropen från Dynamic Media Classic och lägga till dem på din webbplats eller i ditt program."'
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '1715'
ht-degree: 0%

---


# Publicera filer {#publishing-files}

Du publicerar dina resurser på Dynamic Media Image Servers. Du kan publicera resurser en gång eller ordna så att Dynamic Media Classic publicerar resurser enligt ett återkommande schema. När resurserna har publicerats är de tillgängliga för leverans. Du kan kopiera URL-anropen från Dynamic Media Classic och lägga till dem på webbplatsen eller i programmet.

Dynamic Media Classic har nu stöd för leverans av alla bilder och videor via HTTP/2. Det betyder att en publicerad URL eller inbäddningskod för bilden eller videon är tillgänglig för integrering med alla program som accepterar en värdbaserad resurs. Den publicerade resursen levereras sedan via HTTP/2-protokollet. Den här leveransmetoden förbättrar kommunikationen mellan webbläsare och servrar, vilket ger bättre respons och laddningstider för alla dina Dynamic Media Classic-resurser. Se [HTTP2 Delivery of Content FAQ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/http2.html#dynamic).

## Publicera efter överföring av {#publish-after-uploading}

Resurser i publicerat eller opublicerat läge. Som standard markeras alla resurser som du överför till Dynamic Media Classic automatiskt för publicering.

Mer information finns i [PDF-filen med snabbpubliceringsmeddelande](/help/assets/rendering-instant-publish-notification.pdf).

Använd dessa tekniker för att markera resurser för publicering:

* **Publicera efter**
överföring På sidan Överför väljer du Publicera efter överföring längst ned. Standardläget är ett markerat läge.

* **Publicera efter**
överföringVälj Publicera efter överföring i dialogrutan Jobbalternativ. Standardläget är ett markerat läge.

Vissa underordnade resurser markeras automatiskt för publicering när deras överordnade objekt markeras för publicering. I den här tabellen visas underordnade resurser som markerats för publicering automatiskt.

| Överordnat objekt (grupp) | Underordnade (medlem) objekt |
|--- |--- |
| Bilduppsättningar | Bilder i uppsättningen. |
| Färgruteuppsättningar | Färgrutor i uppsättningen. |
| Rotationsset | Bilder i uppsättningen. |
| Mallar | Mallfiler, sidor och bilder. |

Härledda bilder markeras också automatiskt för publicering när deras överordnade bilder publiceras. Härledda bilder innehåller bilder som du har justerat med bildredigeringsalternativ. Du kan se de här härledda bilderna i detaljvyn under Byggnader och derivat.

## Skapar ett publiceringsjobb {#creating-a-publish-job}

Skapa ett publiceringsjobb för att publicera resurser som du har överfört till Dynamic Media Classic-servrar, men välj att inte publicera dem automatiskt än. Du kan göra en engångspublicering eller schemalägga återkommande jobb. Dynamic Media Classic erbjuder avancerade publiceringsalternativ för publicering på specifika servrar och alternativ för publicering av material som redan har publicerats.

**Skapa ett publiceringsjobb**

1. Klicka på **Publicera** i fältet Global Navigation.
1. I dialogrutan Publicera väljer du om du vill ha ett enstaka eller återkommande publiceringsjobb.

   Se [Skapa ett engångspubliceringsjobb](publishing-files.md#creating_a_one_time_publish_job) och [Skapa ett återkommande publiceringsjobb](publishing-files.md#creating_a_recurring_publish_job).

1. Ange ett jobbnamn.
1. Du kan även visa Avancerade alternativ och välja dessa alternativ.

   Se [Avancerade publiceringsalternativ](publishing-files.md#advanced_publish_options).

1. Klicka på **Skicka publicering**.

Dynamic Media Classic spårar publiceringsjobb på jobbsidan. Du kan granska publiceringsjobb på den sidan.

>[!NOTE]
>
>Resurser som du publicerar på nytt (du har publicerat dem tidigare) visas inte direkt på webbplatsen på grund av webb-cachningsmekanismen i leveransnätverket (CDN). Se [Återpublicerade resurser och CDN-fördröjningar](publishing-files.md#republished_assets_and_cdn_delays).

### Skapar ett engångspubliceringsjobb {#creating-a-one-time-publish-job}

Skapa ett engångspubliceringsjobb genom att välja alternativet Enstaka gång på sidan Publicera.

Om du vill att publiceringsjobbet ska utföras vid ett senare datum väljer du menyn När och väljer Schemalägg för senare. Använd sedan skjutreglagen Kalender och Tid för att välja dag och tid för publiceringsjobbet.

### Skapar ett återkommande publiceringsjobb {#creating-a-recurring-publish-job}

Skapa ett återkommande publiceringsjobb genom att välja alternativet Återkommande på sidan Publicera.

Välj sedan alternativet Upprepa - varje dag, Varje vecka, Varje månad eller Anpassad - för att deklarera när du vill att publiceringsjobbet ska återkomma. I Dynamic Media Classic visas kalenderverktyg för schemaläggning av det återkommande publiceringsjobbet. Du kan välja alternativet Egen och ange en regel i rutan Regel för att beskriva ett anpassat jobbintervall.

Se [Skapa ett anpassat tidsintervall för överföring eller publicering](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>Återkommande publicerings- (och överföringsjobb) jobb visas på sidan Jobs. Du kan redigera eller ta bort ett schemalagt jobb genom att gå till fliken Schemalagda på sidan Jobb.

### Avancerade publiceringsalternativ {#advanced-publish-options}

Du kan visa de avancerade alternativen på sidan Publicera och välja följande alternativ för att hantera ett publiceringsjobb:

* **Publicera**
tillVälj en servertyp om du bara vill publicera resurser på en viss server, inte på alla servrar.

* ****
PublishSom standard publicerar Dynamic Media Classic endast resurser som är nya och som inte har publicerats tidigare (alternativet Ny sedan senaste publicering). Du kan dock välja Fullständig publicering om du även vill publicera resurser som har uppdaterats eller ändrats sedan de publicerades senast. Välj Fullständig w/ Sök data om du publicerar en e-katalog och vill att läsarna ska kunna söka efter den med nyckelord.

* **Kör jobb**
somVälj ett användarnamn i listan. Du kan sortera jobb efter användarnamn på sidan Jobb. Genom att välja ett namn associerar du ett publiceringsjobb med en användare.

**HTTP-**
meddelande Ange en URL för att aktivera efterföljande publiceringsjobb.

Se [Använda ett överförings- eller publiceringsjobb som utlösare](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).)

## Avbryter ett publiceringsjobb {#canceling-a-publish-job}

Du kan avbryta ett pågående publiceringsjobb. Om du är administratör kan du dessutom avbryta ett pågående publiceringsjobb från företagets jobbsida.

Om du vill avbryta ett publiceringsjobb går du till sidan Jobb och klickar på Avbryt. På fliken Schemalagda på sidan Jobb kan du pausa eller återuppta ett jobb genom att avmarkera eller markera kryssrutan i kolumnen Aktiv för jobbet.

>[!NOTE]
>
>När du har avslutat ett publiceringsjobb ändras dess status till&quot;stoppa&quot; tills jobbet når en punkt där det kan stanna säkert. Det kan ta en stund att avbryta ett publiceringsjobb om jobbet håller på att hämta data från databasen.

## Publicera resurser {#manually-publishing-assets} manuellt

Du kan publicera enskilda resurser manuellt i stället för att skapa ett publiceringsjobb. När du publicerar uppsättningar, till exempel en bilduppsättning eller en adaptiv videouppsättning, publiceras uppsättningen (eller &quot;överordnad&quot;) och alla medlemmar (eller &quot;underordnade&quot;) i uppsättningen.

Opublicerade resurser visas i användargränssnittet med en grå, rund ikon med ett snedstreck (opublicerat läge) till vänster om resursens namn. När en resurs har publicerats blir ikonen grön och har en vit bockmarkering i mitten (publicerat läge).

**Publicera resurser manuellt**

1. Gör något av följande:

   * I Stödrastervisning, listvy eller detaljvy använder du standardmetoder för att välja en eller flera opublicerade resurser.

      Klicka på **Arkiv > Publicera** i det globala navigeringsfältet.

   * I Stödrastervisning, listvy eller detaljvy klickar du på den grå, runda ikonen med ett snedstreck till vänster om resursens namn.

## Manuellt avpublicera resurser {#manually-unpublishing-assets}

Du kan avpublicera enskilda resurser manuellt. När du avpublicerar uppsättningar, till exempel en uppsättning med färgrutor eller en eCatalog, försätts själva uppsättningen (eller&quot;överordnad&quot;) i ett opublicerat läge. Medlemmarna (eller &quot;barn&quot;) i uppsättningen påverkas dock inte. i stället behåller de sitt befintliga publicerade eller opublicerade läge.

Publicerade resurser visas i användargränssnittet med en rund, grön ikon med en vit bock i mitten (publicerat läge) till vänster om resursens namn. När en resurs inte har publicerats blir ikonen grå med ett snedstreck (opublicerat läge),

**Avpublicera resurser manuellt**

1. Gör något av följande:

   * I Stödrastervisning, listvy eller detaljvy väljer du en eller flera publicerade resurser.

      Klicka på **Arkiv > **Avpublicera** i det globala navigeringsfältet.

   * I Stödrastervisning, listvy eller detaljvy klickar du på den runda, gröna bockmarkeringsikonen till vänster om resursens namn.

## Hämta publiceringshistorik för en resurs {#getting-an-asset-s-publish-history}

Det senaste datumet när en resurs publicerades visas i detaljvyn högst upp på panelen. Du kan få mer information om publiceringshistoriken genom att öppna panelen Historik och publicerade servrar i detaljvyn. Därifrån kan du se när resursen publicerades och till vilka servrar den publicerades.

## Återpublicerade resurser och CDN-fördröjningar {#republished-assets-and-cdn-delays}

Dynamic Media Classic-resurser distribueras i leveransnätverket (CDN). CDN är ett system med datorservrar som är sammankopplade och som på ett transparent sätt samarbetar för att leverera innehåll, särskilt stort medieinnehåll, till slutanvändarna. I CDN-systemet lagras webbinnehåll i webbcacheminnen över Internet (kallas edge cache-nätverk). Webbinnehåll levereras från dessa webb-cacheminnen till slutanvändarna för snabbare leveranser.

Första gången någon hämtar en webbsida levereras resurserna till en CDN-webbcache-server. De lagras på den här servern så att nästa gång någon i samma område öppnar webbsidan kan samma cachelagrade innehåll levereras snabbare. Innehållet levereras snabbare eftersom det ligger närmare slutanvändaren. CDN gör att webbsidor visas snabbare. Den minskar behovet av bandbredd på den centrala servern eftersom innehållet levereras från edge cache-nätverket, inte från en central server i varje instans.

Nypublicerat Dynamic Media Classic-material är tillgängligt direkt för slutanvändaren och fyller snabbt i edge cache-nätverket. Nypublicerat innehåll (bilder som har exakt samma namn som bilder som tidigare publicerats på en bildserver) uppdateras inte på CDN på upp till tio timmar. I stället ser slutanvändarna vad som finns i ett webbcacheminne i CDN-nätverket. Därför kanske dina ompublicerade Dynamic Media Classic-resurser inte visas för slutanvändarna på tio timmar.

Om du vill att dina nypublicerade bildresurser ska vara tillgängliga tidigare än tio timmars fördröjning kan du tömma webcacher på CDN. När du tömmer dessa webbcacher tas gammalt innehåll bort från CDN-webbcachen och ersätts med dina senast publicerade resurser.

Om du vill tömma cachen klickar du på Arkiv > Invalidera CDN. Alla markerade filer tas bort från cacheminnet. Om det inte finns några publicerbara resurser, eller om du inte är företagsadministratör, är alternativet Ta bort från CDN inte tillgängligt.

>[!MORELIKETHIS]
>
>* [Kontrollerar jobbfiler](checking-job-files.md)
>* [Redigera, ta bort, pausa och återuppta återkommande jobb](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)

