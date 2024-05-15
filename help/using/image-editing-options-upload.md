---
title: Alternativ för finjustering av bilder vid överföring
description: Lär dig mer om de alternativ för finjustering som är tillgängliga vid överföringen i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 2d9fc6d8-973f-4aaa-bc2c-b49cda2cde58
topic: Administration, Content Management
level: Intermediate
source-git-commit: 163eb32112ec6fbefd1dacf48212353ff3053d54
workflow-type: tm+mt
source-wordcount: '1169'
ht-degree: 0%

---

# Alternativ för finjustering av bilder vid överföring{#image-editing-options-at-upload}

När du överför bildfiler, inklusive AI-, EPS- och PSD-filer, kan du utföra följande redigeringsåtgärder i dialogrutan Alternativ för överföringsjobb:

* Beskär tomt utrymme från bildens kant.
* Beskär manuellt från bildsidorna.
* Välj en färgprofil.
* Skapa en mask från en urklippsbana.
* Öka skärpan i bilder med oskarpa maskningsalternativ
* Blockera bakgrund

Dessa alternativ finns på sidan Överför under **[!UICONTROL Imaging Edit Options]** rubrik.

## Beskära tomt utrymme från bilder

Du kan beskära pixlar med tomt utrymme automatiskt från en bild. I dialogrutan Alternativ för överföring av jobb väljer du **[!UICONTROL Crop Options]**. I **[!UICONTROL Crop]** nedrullningsbar lista, välja **[!UICONTROL Trim]**. Välj sedan följande alternativ:

* **[!UICONTROL Trim Away Based On]** - Välj i den här listrutan om du vill beskära baserat på färg eller genomskinlighet:

   * **[!UICONTROL Color]** - Välj **[!UICONTROL Color]** alternativ. Sedan, från **[!UICONTROL Corner]** i den nedrullningsbara listan markerar du hörnet på bilden med den färg som bäst motsvarar den vita färgen som du vill beskära.

   * **[!UICONTROL Transparency]** - Välj alternativet Genomskinlighet.

* **[!UICONTROL Tolerance]** - Dra skjutreglaget för att ange en tolerans mellan 0 och 1:

   * **Trimma baserat på färg** - Ange 0 om du bara vill beskära pixlar om de exakt matchar färgen som du valde i hörnet av bilden. Nummer som ligger närmare 1 ger större färgskillnader.

   * **Trimma baserat på genomskinlighet** - Ange 0 om du bara vill beskära pixlar om de är genomskinliga. Med siffror närmare 1 får du mer genomskinlighet.

## Beskär manuellt från bildsidorna

Om du vill beskära manuellt från sidorna av en bild väljer du Beskär-menyn och sedan Manuell. Ange sedan antalet pixlar att beskära från en sida eller från varje sida av bilden. Hur mycket av bilden som beskärs beror på bildfilens ppi-inställning (pixlar per tum). Anta att bilden visar 150 ppi. Sedan anger du 75 i textrutorna Överkant, Höger, Underkant och Vänster. Nu beskärs varje sida med 0,5 tum.

## Välja en färgprofil

Välj en färgmodell för bilden genom att välja ett färgprofilalternativ:

* **[!UICONTROL Convert To sRGB]** - Konverterar till sRGB (Standard Red Green Blue). sRGB är den rekommenderade färgrymden för visning av bilder på webbsidor.

* **[!UICONTROL Keep Original Color Space]** - Behåller den ursprungliga färgrymden.

* **[!UICONTROL Custom From]** > **[!UICONTROL To]** - Öppnar menyer så att du kan välja färgmodellen Konvertera från och Konvertera till. Du kan välja en standardfärgmodell för Photoshop eller en färgmodell som du har överfört till Adobe Dynamic Media Classic.

Se [ICC-profiler](icc-profiles.md#icc_profiles).

## Skapa en mask från en urklippsbana

Om du vill skapa en mask för bilden baserat på dess urklippsbaneinformation markerar du **[!UICONTROL Create Mask From Clipping Path]**. Det här alternativet gäller bilder som skapats med bildredigeringsprogram där en urklippsbana har skapats.

## Öka skärpan i en bild med Oskarp mask

Med det här filtret kan du finjustera en skärpefiltereffekt på den slutliga nedsamplade bilden. Det hjälper dig att styra intensiteten i effekten, radien för effekten (mätt i pixlar) och ett tröskelvärde för kontrast som ignoreras.

Den här effekten använder samma alternativ som Photoshop Oskarp mask-filter. Till skillnad från vad namnet antyder är Oskarp mask ett skärpefilter.

Under Oskarp mask anger du önskade alternativ. Inställningsalternativen beskrivs i följande tabell:

| Oskarp mask, alternativ | Beskrivning |
| --- | --- |
| Belopp | Mängd styr mängden kontrast som används på kantpixlar.<br><br>Tänk på det som intensiteten i effekten. Det finns en skillnad mellan värdena för Oskarp mask i Dynamic Media Classic och i Adobe Photoshop. Den största skillnaden är att Photoshop har ett beloppsintervall på 1 till 500 %. I Adobe Dynamic Media Classic är värdeintervallet 0,0 till 5,0. Värdet 5.0 i Adobe Dynamic Media Classic motsvarar 500 % i Photoshop, värdet 0,9 motsvarar 90 % och så vidare. |
| Radie | Styr radien för effekten. <br><br>Värdet är 0-250. Effekten körs på alla pixlar i en bild och strålar ut från alla pixlar i alla riktningar. Radien mäts i pixlar. Om du till exempel vill få en liknande skärpeeffekt för en bild på 2 000 × 2 000 pixlar och en bild på 500 × 500 pixlar, skulle du ange en radie på två pixlar för bilden på 2 000 × 2 000 pixlar. Ange sedan radien 1 pixel på bilden med 500 × 500 pixlar. Ett större värde används för en bild som har fler pixlar. |
| Tröskelvärde | Tröskelvärde är ett kontrastintervall som ignoreras när filtret Oskarp mask används. Den här effekten är viktig så att inget &quot;brus&quot; uppstår i en bild när filtret används. Värdeintervallet är 0-255, vilket är antalet intensitetssteg i en gråskalebild. 0=svart, 128=50% grått och 255=vitt.<br><br>Ett tröskelvärde på 12 ignorerar t.ex. små variationer i hudtonens ljusstyrka för att undvika att lägga till brus, men ändå ger kantkontrast till kontrastområden som där ögonfransarna möts av hud.<br><br>Om du t.ex. har ett foto av någons ansikte kommer Oskarp mask att påverka de kontrastrika delarna av bilden. Till exempel där ögonfransar och hud möts för att skapa ett tydligt kontrastområde och den utjämnade huden. Även den jämnaste huden uppvisar subtila förändringar i intensitetsvärden. Om du inte använder ett tröskelvärde framhäver filtret dessa subtila ändringar i hudpixlar. I sin tur skapas en högljudd och oönskad effekt medan kontrasten på ögonfransarna ökar, vilket ökar skärpan.<br><br>För att undvika det här problemet introduceras ett tröskelvärde som instruerar filtret att ignorera pixlar som inte förändrar kontrasten dramatiskt, som mjuk hud. <br><br>Lägg märke till texturen bredvid dragkedjan i zippargrafiken som visades tidigare. Bildbrus visas eftersom tröskelvärdena är för låga för att undertrycka bruset. |
| Monokrom | Markera för att få bildintensiteten oskarp mask (intensitet).<br><br>Avmarkera alternativet om du vill skapa en oskarp mask för varje färgkomponent separat. |

Se även [Öka skärpan i en bild](sharpening-image.md#sharpening_an_image).

Se även [Öka skärpan i bilder i Adobe Dynamic Media och på Image Server](/help/using/assets/s7_sharpening_images.pdf).

## Blockera bakgrund

Använd Blockera bakgrund så att du automatiskt kan ta bort bakgrunden i en bild när du överför den. Den här tekniken är användbar för att dra uppmärksamheten till ett visst objekt och få det att sticka ut från en rörig bakgrund.

| Alternativ för Spara ur bakgrund | Beskrivning |
| --- | --- |
| Blockera bakgrund | Välj om du vill aktivera eller aktivera funktionen Blockera bakgrund och alternativen. |
| Hörn | Obligatoriskt.<br>Hörnet på bilden som används för att definiera bakgrundsfärgen som ska blockeras.<br>Du kan välja mellan <b>Övre vänster, Nedre vänster, Övre höger eller Nedre höger</b>. |
| Fyllningsmetod | Obligatoriskt. <br>Styr pixelgenomskinlighet från den hörnplats som du anger.<br>Du kan välja bland följande fyllningsmetoder:<br>・ <b>Flood Fill</b> - gör alla pixlar genomskinliga som matchar det hörn du har angett och som är kopplat till det.<br>・ <b>Matcha pixlar</b> - gör alla matchande pixlar genomskinliga, oavsett var de finns i bilden. |
| Ttolerans | Valfritt.<br>Styr den tillåtna variationen i pixelfärgmatchning baserat på den hörnplats som du anger.<br>Använd värdet 0,0 om du vill matcha pixelfärgerna exakt. Du kan också använda värdet 1,0 för att få största möjliga variation. |

>[!MORELIKETHIS]
>
>* [Beskära en bild](cropping-image.md#cropping_an_image)
