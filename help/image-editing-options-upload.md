---
title: Bildredigeringsalternativ vid överföring
description: Lär dig mer om de bildredigeringsalternativ som är tillgängliga vid tidpunkten för överföringen.
uuid: 0912ae6f-41c9-41b5-94d1-e266face782e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: d3f21cdf-2cb3-46e8-955a-b8daf0b233bc
feature: Dynamic Media Classic,Resurshantering
role: Yrkesverksamma inom affärsverksamhet
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '1145'
ht-degree: 0%

---


# Bildredigeringsalternativ vid överföring{#image-editing-options-at-upload}

När du överför bildfiler, inklusive AI-, EPS- och PSD-filer, kan du utföra följande redigeringsåtgärder i dialogrutan Alternativ för överföringsjobb:

* Beskär tomt utrymme från bildens kant.
* Beskär manuellt från bildsidorna.
* Välj en färgprofil.
* Skapa en mask från en urklippsbana.
* Öka skärpan i bilder med oskarpa maskningsalternativ
* Blockera bakgrund

Dessa alternativ finns på överföringsskärmen under Bildredigeringsalternativ.

**Beskära tomt utrymme från bilder**

Om du vill beskära pixlar med tomt utrymme automatiskt från en bild väljer du Beskär-menyn och sedan Beskär. Välj sedan följande alternativ:

* **Trimma bort baserat**
påVälj om du vill beskära baserat på färg eller genomskinlighet:

* ****
FärgVälj alternativet Färg. I listrutan Hörn väljer du sedan det hörn i bilden som har den färg som bäst motsvarar den vitfärgen som du vill beskära.

* ****
GenomskinlighetVälj alternativet Genomskinlighet.

* ****
ToleransDra i skjutreglaget för att ange en tolerans mellan 0 och 1:

* **Trimma baserat på**
färgAnge 0 om du bara vill beskära pixlar om de exakt matchar färgen som du valde i hörnet av bilden. Nummer som ligger närmare 1 ger större färgskillnader.

* **Trimma baserat på**
genomskinlighetAnge 0 om pixlarna bara ska beskäras om de är helt genomskinliga. siffror närmare 1 ger större genomskinlighet.

**Beskära manuellt från bildsidorna**

Om du vill beskära manuellt från sidorna av en bild väljer du Beskär-menyn och sedan Manuell. Ange sedan antalet pixlar att beskära från en sida eller från varje sida av bilden. Hur mycket av bilden som beskärs beror på bildfilens ppi-inställning (pixlar per tum). Om bilden till exempel visar 150 ppi och du anger 75 i textrutorna Överkant, Höger, Underkant och Vänster beskärs en halv tum från varje sida.

**Välja en färgprofil**

Välj ett färgprofilsalternativ för att välja en färgrymd för bilden:

* **Konvertera till**
sRGBConverts till sRGB (röd standardgrön blå). sRGB är den rekommenderade färgrymden för visning av bilder på webbsidor.

* **Behåll ursprunglig**
färgrymdBehåller den ursprungliga färgrymden.

* **Anpassad från >**
TillÖppnar menyer så att du kan välja färgmodellen Konvertera från och Konvertera till. Du kan välja en standardfärgmodell för Photoshop eller en färgmodell som du har överfört till Dynamic Media Classic.

Se [ICC-profiler](icc-profiles.md#icc_profiles).

**Skapa en mask från en urklippsbana**

Välj **Skapa mask från urklippsbana** om du vill skapa en mask för bilden baserat på dess urklippsbaneinformation. Det här alternativet gäller bilder som skapats med bildredigeringsprogram där en urklippsbana har skapats.

**Öka skärpan i en bild med Oskarp mask**

Med det här filtret kan du finjustera en skärpefiltereffekt på den slutliga nedsamplade bilden, styra intensiteten i effekten, radien för effekten (mätt i pixlar) och ett kontrasttröskelvärde som ignoreras.

Den här effekten använder samma alternativ som Photoshop Oskarp mask-filter. Till skillnad från vad namnet antyder är Oskarp mask ett skärpefilter.

Under Oskarp mask anger du önskade alternativ. Inställningsalternativen beskrivs i följande tabell:

| Oskarp mask, alternativ | Beskrivning |
|--- |--- |
| Belopp | Styr mängden kontrast som används på kantpixlar.<br><br>Tänk på det som intensiteten i effekten. Den största skillnaden mellan mängdvärdena för Oskarp mask i Dynamic Media Classic och mängdvärdena i Adobe Photoshop är att Photoshop har ett intervall på 1 till 500 %. I Dynamic Media Classic är värdeintervallet 0,0 till 5,0. Värdet 5.0 i Dynamic Media Classic motsvarar 500 % i Photoshop. värdet 0,9 motsvarar 90 % och så vidare. |
| Radie | Styr radien för effekten. <br><br>Värdeintervallet är 0-250. Effekten körs på alla pixlar i en bild och strålar ut från alla pixlar i alla riktningar. Radien mäts i pixlar. Om du till exempel vill få en liknande skärpeeffekt för en bild på 2 000 x 2 000 pixlar och en bild på 500 x 500 pixlar anger du en radie på två pixlar för bilden på 2 000 x 2 000 pixlar och ett radievärde på en pixel för bilden på 500 x 500 pixlar . Ett större värde används för en bild som har fler pixlar. |
| Tröskelvärde | Tröskelvärde är ett kontrastintervall som ignoreras när filtret Oskarp mask används. Detta är viktigt så att inget &quot;brus&quot; uppstår i en bild när filtret används. Värdeintervallet är 0-255, vilket är antalet intensitetssteg i en gråskalebild. 0=svart, 128=50% grått och 255=vitt.<br><br>Ett tröskelvärde på 12 ignorerar t.ex. små variationer i hudtonens ljusstyrka för att undvika att lägga till brus, men ändå ger kantkontrast till kontrastområden som där ögonfransarna möts av hud.<br><br>Om du t.ex. har ett foto av någons ansikte påverkar Oskarp mask de kontrastrika delarna av bilden, t.ex. där ögonfransar och hud möts för att skapa ett tydligt kontrastområde och den utjämnade huden. Även den jämnaste huden uppvisar subtila förändringar i intensitetsvärden. Om du inte använder ett tröskelvärde framhäver filtret dessa subtila ändringar i hudpixlar. I sin tur skapas en högljudd och oönskad effekt medan kontrasten på ögonfransarna ökar, vilket ökar skärpan.<br><br>För att undvika det här problemet introduceras ett tröskelvärde som instruerar filtret att ignorera pixlar som inte förändrar kontrasten dramatiskt, som mjuk hud. <br><br>Lägg märke till texturen bredvid dragkedjan i zippargrafiken som visades tidigare. Bildbrus visas eftersom tröskelvärdena var för låga för att undertrycka bruset. |
| Monokrom | Markera för att få bildintensiteten oskarp mask (intensitet).<br><br>Avmarkera alternativet om du vill skapa en oskarp mask för varje färgkomponent separat. |

Se även [Öka skärpan i en bild](sharpening-image.md#sharpening_an_image).

Se även [Skärpa bilder i Scene7 Publishing System och på Image Server](/help/assets/s7_sharpening_images.pdf).

**Blockera bakgrund**

Du kan använda Blockera bakgrund för att automatiskt ta bort bakgrunden i en bild när du överför den. Den här tekniken är användbar för att dra uppmärksamheten till ett visst objekt och få det att sticka ut från en rörig bakgrund.

| Alternativ för Spara ur bakgrund | Beskrivning |
|:--- |:--- |
| Blockera bakgrund | Välj om du vill aktivera eller aktivera funktionen och alternativen för Spara ur bakgrund. |
| Hörn | Obligatoriskt.<br><br>Hörnet på bilden som används för att definiera bakgrundsfärgen som ska blockeras.<br><br>Du kan välja mellan  <b>Övre vänster, Nedre vänster, Övre höger och Nedre höger</b>. |
| Fyllningsmetod | Obligatoriskt. <br><br>Styr pixelgenomskinlighet från den hörnplats som du anger.<br><br>Du kan välja bland följande fyllningsmetoder: <ul><li><b>Flood Fill</b>  - gör alla pixlar genomskinliga som matchar det hörn du har angett och som är anslutet till det.</li><li><b>Matcha pixlar</b> - gör alla matchande pixlar genomskinliga, oavsett var de finns i bilden.</li></ul> |
| Tolerans | Valfritt.<br><br>Styr den tillåtna variationen i pixelfärgmatchning baserat på den hörnplats som du anger.<br><br>Använd värdet 0,0 om du vill matcha pixelfärgerna exakt, eller använd värdet 1,0 om du vill tillåta den största variationen. |

>[!MORELIKETHIS]
>
>* [Beskära en bild](cropping-image.md#cropping_an_image)

