---
title: Publish-filer
description: Lär dig hur du publicerar dina resurser på Dynamic Media Image Servers.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 91b73a09-c5b5-4001-b36f-6bebe65717ff
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '1626'
ht-degree: 0%

---

# Publish-filer{#publishing-files}

Du publicerar dina resurser på Dynamic Media Image Servers. Du kan publicera resurser på en enstaka gång eller ordna så att Adobe Dynamic Media Classic publicerar resurser enligt ett återkommande schema. När resurserna har publicerats är de tillgängliga för leverans. Du kan kopiera URL-anropen från Adobe Dynamic Media Classic och lägga till dem på din webbplats eller i ditt program.

Adobe Dynamic Media Classic stöder nu leverans av alla bilder och videor via HTTP/2. Det betyder att en publicerad URL eller inbäddad kod för bilden eller videon är tillgänglig för integrering med alla program som accepterar en värdbaserad resurs. Den publicerade resursen använder HTTP/2-protokollet för att leverera den. Den här leveransmetoden förbättrar sättet som webbläsare och servrar kommunicerar på, vilket ger bättre respons och laddningstider för alla era Adobe Dynamic Media Classic-resurser. Se [HTTP2 Delivery of Content FAQ](https://experienceleague.adobe.com/sv/docs/experience-manager-65/content/assets/dynamic/http2).

## Publish efter överföring {#publish-after-uploading}

Assets är antingen publicerat eller opublicerat. Som standard markeras alla resurser som du överför till Adobe Dynamic Media Classic automatiskt för publicering.

Mer information finns i [Instant Publish Notice PDF](/help/using/assets/rendering-instant-publish-notification.pdf).

Använd dessa tekniker för att markera resurser för publicering:

* **[!UICONTROL Publish After Uploading]**: På sidan Överför väljer du **[!UICONTROL Publish After Uploading]** längst ned. Standardläget är ett markerat läge.

* **[!UICONTROL Publish After Uploading]**: Välj **[!UICONTROL Publish After Uploading]** i dialogrutan Jobbalternativ. Standardläget är ett markerat läge.

Vissa underordnade resurser markeras automatiskt för publicering när deras överordnade objekt markeras för publicering. I den här tabellen visas underordnade resurser som markerats för publicering automatiskt.

| Överordnat objekt (grupp) | Underordnade (medlem) objekt |
| --- | --- |
| Bilduppsättningar | Bilder i uppsättningen. |
| Uppsättningar med färgrutor | Färgrutor i uppsättningen. |
| Snurra uppsättningar | Bilder i uppsättningen. |
| Mallar | Mallfiler, sidor och bilder. |

Härledda bilder markeras också automatiskt för publicering när deras överordnade bilder publiceras. Härledda bilder innehåller bilder som du har justerat med bildredigeringsalternativ. Du kan se de här härledda bilderna i detaljvyn under Byggnader och derivat.

## Skapa ett publiceringsjobb {#creating-a-publish-job}

Skapa ett publiceringsjobb för att publicera resurser som du har överfört till Adobe Dynamic Media Classic-servrar, men vill inte publicera dem automatiskt än. Du kan göra en engångspublicering eller schemalägga jobb som ska upprepas regelbundet. Adobe Dynamic Media Classic erbjuder avancerade publiceringsalternativ för publicering på specifika servrar och alternativ för publicering av material som redan har publicerats.

**Så här skapar du ett publiceringsjobb:**

1. Välj **[!UICONTROL Publish]** i fältet Global navigering.
1. I dialogrutan Publicera väljer du om du vill ha ett engångs- eller återkommande publiceringsjobb.

   Se [Skapa ett engångspubliceringsjobb](publishing-files.md#creating_a_one_time_publish_job) och [Skapa ett återkommande publiceringsjobb](publishing-files.md#creating_a_recurring_publish_job).

1. Ange ett jobbnamn.
1. Du kan även visa Avancerade alternativ och välja dessa alternativ.

   Se [Avancerade publiceringsalternativ](publishing-files.md#advanced_publish_options).

1. Välj **[!UICONTROL Submit Publish]**.

Adobe Dynamic Media Classic spårar publiceringsjobb på jobbsidan. Du kan granska publiceringsjobb på den sidan.

>[!NOTE]
>
>Assets som du har publicerat på nytt (du har publicerat dem tidigare) visas inte omedelbart på webbplatsen på grund av funktionen för webbaserad cachelagring i leveransnätverket (CDN). Se [Återpublicerade resurser och CDN-fördröjningar](publishing-files.md#republished_assets_and_cdn_delays).

### Skapa ett engångspubliceringsjobb {#creating-a-one-time-publish-job}

Skapa ett engångspubliceringsjobb genom att välja alternativet **[!UICONTROL One-Time]** på publiceringssidan.

Om du vill att publiceringsjobbet ska utföras senare väljer du **[!UICONTROL One-Time]** på publiceringssidan. Välj **[!UICONTROL Schedule For Later]** i listrutan. Använd kalendern och tidsreglaget för att välja dag och tid för publiceringsjobbet.

### Skapa ett återkommande publiceringsjobb {#creating-a-recurring-publish-job}

Skapa ett återkommande publiceringsjobb genom att välja **[!UICONTROL Recurring]** på publiceringssidan.

Välj sedan alternativet Upprepa **[!UICONTROL Daily]**, **[!UICONTROL Weekly]**, **[!UICONTROL Monthly]** eller **[!UICONTROL Custom]** och ange sedan när du vill att publiceringsjobbet ska upprepas. Adobe Dynamic Media Classic presenterar kalenderverktyg för schemaläggning av det återkommande publiceringsjobbet. Du kan markera alternativet **[!UICONTROL Custom]** och ange en regel i textfältet Regel för att beskriva ett anpassat jobbintervall.

Se [Skapa ett anpassat tidsintervall för överföring eller publiceringsjobb](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>Återkommande publicerings- (och överföringsjobb) jobb visas på sidan Jobs. Du kan redigera eller ta bort ett schemalagt jobb genom att gå till fliken Schemalagda på sidan Jobb.

### Avancerade publiceringsalternativ {#advanced-publish-options}

Du kan visa de avancerade alternativen på publiceringssidan och välja följande alternativ för att hantera ett publiceringsjobb:

* **[!UICONTROL Publish To]**: Välj en servertyp om du bara vill publicera resurser på en viss server.

* **[!UICONTROL Publish]**: Som standard publicerar Adobe Dynamic Media Classic bara resurser som är nya och som inte har publicerats tidigare (alternativet Nytt sedan senaste Publish). Du kan dock välja **[!UICONTROL Full Publish]** så att du även kan publicera resurser som har uppdaterats eller ändrats sedan de publicerades senast. Välj **[!UICONTROL Full w/ Search Data]** om du publicerar en e-katalog och du vill att läsarna ska kunna söka efter den med nyckelord.

* **[!UICONTROL Run Job As]**: Välj ett användarnamn i listan. Du kan sortera jobb efter användarnamn på sidan Jobb. Genom att välja ett namn associerar du ett publiceringsjobb med en användare.

**[!UICONTROL HTTP Notification]**: Ange en URL för att aktivera efterföljande publiceringsjobb.

Se [Använd ett överförings- eller publiceringsjobb som utlösare](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).)

## Avbryta ett publiceringsjobb {#canceling-a-publish-job}

Du kan avbryta ett pågående publiceringsjobb. Om du är administratör kan du dessutom avbryta ett pågående publiceringsjobb från företagets jobbsida.

Om du vill avbryta ett publiceringsjobb går du till sidan Jobb och väljer **[!UICONTROL Cancel]**. På fliken Schemalagda på sidan Jobb kan du pausa eller återuppta ett jobb genom att avmarkera eller markera kryssrutan i jobbkolumnen.

>[!NOTE]
>
>När du har avslutat ett publiceringsjobb ändras dess status till&quot;stoppa&quot; tills jobbet når en punkt där det kan stanna säkert. Det kan ta en stund att avbryta ett publiceringsjobb om jobbet håller på att hämta data från databasen.

## Publish-resurser manuellt {#manually-publishing-assets}

Du kan publicera enskilda resurser manuellt i stället för att skapa ett publiceringsjobb. När du publicerar uppsättningar, till exempel en bilduppsättning eller en adaptiv videouppsättning, publiceras uppsättningen (eller &quot;överordnad&quot;) och alla medlemmar (eller &quot;underordnade&quot;) i uppsättningen.

Opublicerade resurser visas i användargränssnittet med en grå, rund ikon med ett snedstreck (opublicerat läge) till vänster om resursens namn. När en resurs har publicerats blir ikonen grön och har en vit bock i mitten (publicerat läge).

**Så här publicerar du resurser manuellt:**

1. Gör något av följande:

   * I Stödrastervisning, listvy eller detaljvy använder du standardmetoder för att välja en eller flera opublicerade resurser.

     Gå till **[!UICONTROL File]** > **[!UICONTROL Publish]** i fältet Global navigering.

   * I Stödrastervisning, listvy eller detaljvy väljer du den grå, runda ikonen med ett snedstreck till vänster om resursens namn.

## Avpublicera resurser manuellt {#manually-unpublishing-assets}

Du kan avpublicera enskilda resurser manuellt. När du avpublicerar uppsättningar, till exempel en uppsättning med färgrutor eller en eCatalog, försätts själva uppsättningen (eller&quot;överordnad&quot;) i ett opublicerat läge. Medlemmarna (eller&quot;underordnade&quot;) i uppsättningen påverkas dock inte. De behåller i stället sitt befintliga publicerade eller opublicerade läge.

Publicerade resurser visas i användargränssnittet med en rund, grön ikon med en vit bock i mitten (publicerat läge) till vänster om resursens namn. När en resurs inte har publicerats blir ikonen grå med ett snedstreck (opublicerat läge),

**Så här avpublicerar du resurser manuellt:**

1. Gör något av följande:

   * I Stödrastervisning, listvy eller detaljvy väljer du en eller flera publicerade resurser.

     Gå till **[!UICONTROL File]** > **[!UICONTROL Unpublish]** i fältet Global navigering.

   * I Stödrastervisning, listvy eller detaljvy väljer du den runda, gröna bockmarkeringsikonen till vänster om resursens namn.

## Hämta publiceringshistorik för en resurs {#getting-an-asset-s-publish-history}

Det senaste datumet då en resurs publicerades visas i detaljvyn högst upp på panelen. Du kan få mer information om publiceringshistoriken genom att öppna panelen Historik och publicerade servrar i detaljvyn. Därifrån kan du se när resursen publicerades och till vilka servrar den publicerades.

## Återpublicerade resurser och CDN-förseningar {#republished-assets-and-cdn-delays}

Adobe Dynamic Media Classic-resurser distribueras i leveransnätverket (CDN). CDN är ett system med datorservrar som är sammankopplade och som på ett transparent sätt samarbetar för att leverera innehåll, särskilt stort medieinnehåll, till slutanvändarna. I CDN-systemet lagras webbinnehåll i cacheminnen på Internet (kallas edge cache-nätverk). Webbinnehåll levereras från webbcachen till slutanvändarna för snabbare leveranser.

Första gången någon hämtar en webbsida levereras resurserna till en CDN-webbcache-server. Den här servern lagrar dem så att nästa gång någon i samma område öppnar webbsidan, levereras samma cachelagrade innehåll snabbare. Innehållet levereras snabbare eftersom det ligger närmare slutanvändaren. CDN gör att webbsidor visas snabbare. Den minskar behovet av bandbredd på den centrala servern eftersom innehållet levereras från edge cache-nätverket, inte från en central server i varje instans.

Nypublicerat Adobe Dynamic Media Classic-material är tillgängligt direkt för slutanvändaren och fyller snabbt i edge cache-nätverket. Nypublicerat innehåll, d.v.s. bilder som har samma namn som bilder som tidigare publicerats till en Image Server, uppdateras inte i CDN på upp till tio timmar. I stället ser slutanvändarna vad som finns i en webbcache i CDN-nätverket. Därför verkar dina återpublicerade Adobe Dynamic Media Classic-resurser inte visas för slutanvändarna på tio timmar.

Om du vill att dina nypublicerade bildresurser ska vara tillgängliga tidigare än tio timmars fördröjning kan du tömma webbinarier på CDN. När du tömmer dessa webb-cacher tas gammalt innehåll bort från CDN-webbcachen och ersätts med dina senast publicerade resurser.

Om du vill tömma cachen går du till **[!UICONTROL File]** > **[!UICONTROL Invalidate CDN]** i fältet Global navigering. Alla markerade filer tas bort från cachen. Om det inte finns några publicerbara resurser, eller om du inte är företagsadministratör, är alternativet Ta bort från CDN inte tillgängligt.

>[!MORELIKETHIS]
>
>* [Kontrollera jobbfiler](checking-job-files.md)
>* [Redigera, ta bort, pausa och återuppta återkommande jobb](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)
