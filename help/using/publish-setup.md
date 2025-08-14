---
title: Publiceringsinställningar
description: Med inställningarna för publiceringsinställningar kan du bestämma hur resurser levereras som standard från Adobe Dynamic Media Classic-servrar till webbplatser eller program.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 699d4c12-e47b-4c6b-86f3-dc7aaaa56c1e
topic: Administration, Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '2318'
ht-degree: 0%

---

# Publiceringsinställningar {#publish-setup}

Inställningarna på sidan Publiceringsinställningar avgör hur resurser levereras som standard från Adobe Dynamic Media Classic-servrar till webbplatser eller program. Om ingen inställning har angetts levererar Adobe Dynamic Media Classic-servern en resurs enligt en standardinställning på en publiceringsinställningssida. En begäran om att leverera en bild som inte innehåller ett upplösningsattribut ger till exempel en bild med inställningen för standardobjektupplösning på sidan Bildserver.

Administratörer kan ändra standardinställningarna på sidorna Image Server, Image Renderer och Vinjettering för att skapa standardinställningar för att leverera resurser från servrar.

Öppna sidorna i Publiceringsinställningar genom att gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]**.

>[!NOTE]
>
>Publiceringsinstallationssidorna är till för erfarna webbplatsutvecklare och programmerare. Adobe Dynamic Media Classic förutsätter att användare som ändrar inställningar på dessa sidor känner till Adobe Dynamic Media Classic, HTTP-protokollets standarder och konventioner samt grundläggande bildbehandlingsteknik.

## Bildserver {#image-server}

Sidan Image Server används för att ange standardinställningar för att leverera bilder från bildservrar. Inställningarna är tillgängliga i dessa fem kategorier (se sidan Image Server för mer ingående beskrivningar av inställningarna).

Ändra dessa inställningar endast med hjälp av en supportperson från Adobe Dynamic Media Classic.

* **[!UICONTROL Catalog Management]**: De här inställningarna avgör hur Adobe Dynamic Media Classic och katalogen interagerar. Till skillnad från de flesta webbservrar går URL-anrop till Dynamic Media Image Server till en manifest- eller katalogfil i stället för till en bildfil. Katalogfilen (som inte ska blandas ihop med en e-katalog) innehåller en lista med allt innehåll som publiceras till Image Server. Den innehåller också sökvägen till varje bild. Om du har ett Digimarc-ID anger du din användarinformation i avsnittet Användarinformation för Digimarc.

* **[!UICONTROL Request Attributes]**: De här inställningarna begränsar antalet bilder som kan levereras från servern. *maximum* **[!UICONTROL Reply Image Size Limit]** är till exempel **[!UICONTROL Width]** 5000 och **[!UICONTROL Height]** 5000.

* **[!UICONTROL Default Request Attributes]**: De här inställningarna gäller standardutseendet för bilder.

* **[!UICONTROL Common Thumbnail Attributes]**: De här inställningarna gäller för miniatyrbildernas standardutseende och justering.

* **[!UICONTROL Defaults for Catalog Fields]**: De här inställningarna gäller för upplösningen och standardminiatyrbildstypen för bilder.

* **[!UICONTROL Color Management Attributes]**: De här inställningarna avgör vilka ICC-färgprofiler som används.

* **[!UICONTROL Compatibility Attributes]**: Den här inställningen gör att inledande och efterföljande stycken i textlager kan hanteras som de var i version 3.6 för bakåtkompatibilitet.

* **[!UICONTROL Localization Support]**: Med de här inställningarna kan du hantera flera språkattribut. Här kan du också ange en sträng för språkområdeskarta så att du kan definiera vilka språk du vill ha stöd för de olika verktygstipsen i visningsprogram.

  Om du till exempel är ett flernationellt varumärke som säljer i olika länder kan du se till att varje land har ett eget språkspecifikt visningsprogram. Om du vill använda den här funktionen anger du en sträng för språkområdeskarta. Därefter redigerar du verktygstipstexten i en visningsprogramförinställning. Lägg bara till de översatta textsträngarna för det språk du vill ha.

  >[!NOTE]
  > [Använd Admin Console för att skapa ett supportärende om du vill konfigurera supportalternativ för lokalisering.](https://helpx.adobe.com/se/enterprise/using/support-for-experience-cloud.html) I ditt supportärende, begär du hjälp med installationen.

  Mer information om hur du konfigurerar **[!UICONTROL Localization Support]** finns i [Att tänka på när du konfigurerar lokalisering av resurser](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Att tänka på när lokalisering av resurser konfigureras {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Om du vill ställa in alternativ för lokaliseringsstöd i Adobe Dynamic Media Classic, t.ex. fältet Lokalkarta, [använder du Admin Console för att skapa ett supportärende.](https://helpx.adobe.com/se/enterprise/using/support-for-experience-cloud.html) I ditt supportärende, begär du hjälp med installationen.

Ett vanligt sätt att använda Adobe Dynamic Media Classic är att hantera produktbilder på webbplatser med e-Commerce. Internationella företag står inför utmaningen att resurser för liknande produkter ser annorlunda ut från land till land. Oftast gäller skillnaderna några delar av det totala mediet. Att hantera sådana skillnader genom att kopiera alla tillgångar för vart och ett av länderna och skriva över endast skillnaderna är en stor insats och motsäger den enda primära tillgångsmetaforen. Skillnaderna i resurser kan uppstå, från landspecifika videor med olika ljudspår, till subtila men viktiga skillnader i en strömsladd som används med produkten. Adobe Dynamic Media Classic använder en grundläggande sökfunktion. Du definierar i vilken ordning som resurssuffixen som Image Server söker efter, med utgångspunkt i önskad språkinställning.

#### Hur resurser lokaliseras

Språkinställningen för en IS-begäran (Image Serving) identifieras med följande IS/IR-kommando (Image Rendering):

`locale=`

Det här kommandot accepterar en sträng för språk-ID (locId) som inte är skiftlägeskänslig. Språk-ID:t är vanligtvis en 2-6-teckensträng som består av bokstäver och `_`.

IS stöder godtyckliga utskrivbara ASCII-strängar. Kommandot `locale=` har ett globalt omfång, vilket innebär att det tillämpas på hela begäran, inklusive alla kapslade IS- och IR-begäranden, refererade mallar och bildlager. Det finns inte stöd för flera språkområden per begäran, t.ex. olika språkområden för varje lager. Det går dock att tillåta explicita åsidosättningar i kapslade begäranden.

Om `locale=` inte anges skickas `attribute::DefaultLocale` till översättningsmotorerna. Begränsad indatavalidering används för värdet `locale=`. Tomma `locale=` värden tillåts. Eftersom `locale=` har ett globalt omfång, tillhandahålls `attribute::DefaultLocale` av huvudkatalogen för hela begäran.

Några av fördelarna med att använda `locale=` och `attribute::DefaultLocale` är följande:

* Dela innehåll för flera språkområden.
* Använd språkspecifikt innehåll med generiska ID:n.
* Flexibla regler för namngivning och hantering av språkspecifikt innehåll, som prefix kontra suffix eller språkspecifikt innehåll i en separat katalog.
* Stöd för språkspecifika versioner.
* Sammansatta objekt, t.ex. bilduppsättningar, kan ibland innehålla generiska referenser till potentiellt språkspecifikt innehåll.
* Stöder allt innehåll som hanteras av kataloger som behöver lokaliseras, inklusive bilder, bilduppsättningar, vinjetter, material och poster för visningsprogramkonfiguration.
* Minimera förändringar i IPS-databasen och IS-manifestmekanismer.
* Stöd för statiskt innehåll som videor och skal läggs till när RFC IS-63 implementeras.
* Standardspråket är konfigurerbart.

#### Programscenarier

| Program | Scenario |
| --- | --- |
| Lokalisering av visningsprogram | När statiska innehållskataloger har implementerats styrs lokaliseringen helt och hållet med parametern locale=, som bifogas alla begäranden som görs till IS. Konfigurationsposter, skal, välkomstskärmar och så vidare, kan ha språkspecifika varianter eller inte. Rätt innehåll tillhandahålls av IS utan att användaren behöver veta vilket innehåll som är lokaliserat och vilka ID:n det är. |
| Bilder och video | Flernationella företag har ofta en blandning av generiskt och språkspecifikt innehåll. Med den här funktionen kan en referens till en bild eller video vara allmän och IS visar det språkspecifika innehållet om det är tillgängligt. |
| Bilduppsättningar och medieuppsättningar | Hela bilduppsättningen kan vara annorlunda för vissa språk, till exempel när en eCatalog är annorlunda, med översättningen från en allmän till en språkområdesspecifik bilduppsättning som hanteras av visningsprogrammet. Oftast kan enskilda ID:n i en generisk uppsättning referera till innehåll som är lokaliserat. De flesta foton i en enhet kan till exempel vara desamma på alla språk, förutom fotot på kontrollpanelen. IS översätter ID:n automatiskt, så du behöver inte generera språkspecifika bilduppsättningar. |

#### Implementera resurslokalisering

Adobe Dynamic Media Classic och Image Serving har ett gränssnitt som gör det möjligt att lokalisera bilder och statiskt innehåll.

Utan lokalisering ser en Image Server-URL ut så här:

`https://server/is/image/company/image`

Vid lokalisering lägger en Image Server-URL till parametern `locale=` i sökvägen, som i följande exempel:

`https://server/is/image/company/image?locale=de_DE`

När http-anropet tas emot av Image Server tolkas parametern `locale=` via fältet `localeMap` i **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Localization Support]**.

Fältet Lokalkarta innehåller en lista med poster som separeras med lodsymbolen (|).

Varje post består av en kommaavgränsad lista med värden. Det första värdet är det sökvärde som skickas via parametern `locale=`. De återstående värdena är suffix-/ersättningsvärden som sedan testas tills ett resultat har skapats i en befintlig bild.

Om ett suffixvärde eller ett ersättningsvärde används beror på inställningen för Global Locale i gruppen **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Localization Support]**.

>[!NOTE]
>
>Inställningen Global Locale är bara möjlig när du anger den via API:t, inte i Adobe Dynamic Media Classic-gränssnittet.

**Exempel på suffix:**

| URL | localeMap-ID | Resultat | Anteckningar |
| --- | --- | --- | --- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,` | `fr_FR,_FR,` | Observera att GlobalLocale inte har definierats. Språkparametern de_DE matchas mot den första posten i `localeMap`. Det första motsvarande värdet _DE läggs till som ett suffix till resursen image_DE och ett försök görs att hitta det på bildservern. Om den hittas på servern returneras den. I annat fall används det andra värdet &quot;&quot; som suffix, vilket resulterar i att själva bilden returneras. |

**Exempel på ersättning:**

| URL | `GlobalLocale` och `localeMap` ID | Resultat | Anteckningar |
| --- | --- | --- | --- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main` | `fr_FR,fr,main` | I ersättningsexemplet ovan anges GlobalLocale till main. Språkparametern de_DE matchas mot den första posten i `localeMap`. Delsträngen GlobalLocale hittades och ersätts med det första motsvarande värdet `de` i `localeMap`: `image-de-01`. Om den hittas på Image Server returneras den. Om inte ersätts det andra värdet, vilket resulterar i `image-main-01`. |

Om ingen språkinställning har definierats i URL:en tar Image Server DefaultLocale, om den är definierad, och tillämpar den på URL:en.

Om en okänd eller tom språkparameter anges med `locale=`, genomsöks `localeMap` efter det tomma värdet &quot;som börjar med&quot;. Det är viktigt att ha ett standardspråk för okända språk.

#### Om defaultImage

Bildservern försöker att välja det begärda språket, det ena efter det andra. Om ingen matchning hittas används språkalternativen för defaultImage och den matchande versionen returneras. Därför måste varje språkinställning innehålla ett alternativ för bilden utan lokalisering, eller lokaliserade defaultImage-versioner är tillgängliga i Adobe Dynamic Media Classic.

#### Scenarier för att hitta localeMap

Anta att du vill ha stöd för följande språk:

`en, en_us, en_uk, de, de_at, de_de, fr`

Du mappar de här språkinställningarna till suffixen `_E` (engelska), `_G` (tyska) och `_F` (franska). För alla exempel är det generiska indatabilds-ID `myImg`.

##### Standardbeteende för att hitta localeMap

Språk-ID:n mappas till motsvarande suffix. Om det inte finns något språkspecifikt ID i katalogen görs ett försök att använda det generiska ID:t. Observera de tomma locSuffix-värdena som mappas till det generiska ID:t.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | Utdata-ID att söka efter |
| --- | --- |
| en, en_us, en_uk | myImg_E, myImg |
| de, de_de | myImg_D, myImg |
| fr | myImg_F, myImg |
| Alla andra | : |

##### Söka efter localeMap när språkinställningen är okänd

Du kan mappa okända språk till specifika ID:n eller till generiska ID:n. Du kan till exempel mappa okända språkinställningar till engelska ID:n, eller om de inte finns, till allmänna ID:n.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | Utdata-ID att söka efter |
| --- | --- |
| de, de_de | myImg_D, myImg |
| fr | myImg_F, myImg |
| Alla andra | myImg_E, myImg |

Du kan också ha ett dedikerat locSuffix, till exempel U, för okända språkinställningar, och tvinga till standardbilden om det inte finns någon `_U`, som i följande exempel:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

Du kan också mappa direkt till det generiska ID:t, som i följande exempel:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

##### Söka efter localeMap med hjälp av en sökning på flera nivåer

Det är ofta önskvärt att gruppera språkområden, t.ex. europeiska, Mellanöstern och Nordamerika, för att ta hänsyn till regionala standarder, t.ex. hudexponering. Du kan uppnå den här effekten med en sökning på flera nivåer.

Anta till exempel att du vill ha stöd för samlingar för västerländsk och mellanöstern. Båda samlingarna är baserade på den generiska bildsamlingen, och båda lägger till eller ändrar vissa bilder. Båda samlingarna förfinas sedan ytterligare för specifika språkområden. Till exempel `m1, m2` för två varianter i Mellanöstern och `w1, w2,` och `w3` för tre västerländska språkinställningar, förutom att bilder delas för `w1` och `w3`. Okända språk mappas endast till den generiska samlingen och har inte tillgång till språkspecifika bilder. Så här skulle kartan se ut:

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale= | Utdata-ID att söka efter |
| --- | --- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| Alla andra | mylmg |

##### Hitta språkinställningskartan genom att söka efter specifika ID:n

Vissa namngivningskonventioner stöder inte generiska bild-ID:n. De generiska ID:n från begäran måste mappas till ett specifikt ID i katalogen. Det finns dock instanser där det exakta specifika ID:t inte är känt.

Om du använder det första exemplet som bas kan bilder för alla språk ha suffixen `_1`, `_2` eller `_3`. Bilder som är specifika för franska språk kan ha suffixen `_22` eller `_23`. Och bilder som är specifika för tyska språkområden kan ha suffixen `_470` eller `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | Utdata-ID att söka efter |
| --- | --- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| Alla andra | myImg_1, myImg_2, myImg_3 |

##### Viktiga överväganden vid implementering av lokaliseringsstöd

* Lokaliseringen är begränsad till ID-baserade resursanrop och kan inte användas för sökvägsbaserade resursanrop. När du anropar videoklipp med språkområde måste det därför anropas som företags-ID eller resurs-ID. Ingen fullständig sökväg till videon. Du kan inte använda `RTMP` för lokalisering eftersom den metoden endast är avsedd för sökvägsbaserade videoanrop.
* Du kan inte använda en uppsättning med blandade media som innehåller en enda video när localeMap är aktivt, annars misslyckas anropet till innehållet i uppsättningen. Du kan lösa det här problemet genom att lägga till en enda video i en adaptiv videouppsättning. Lägg sedan till den adaptiva videouppsättningen i en blandad medieuppsättning.
* Vissa förfrågningar är inte lokaliserade, till exempel förfrågningar om innehållet i en adaptiv videouppsättning. Om du tänker använda adaptiva videouppsättningar med lokalisering, ska du därför placera den adaptiva videouppsättningen i en blandad mediamängd. Anropa sedan uppsättningen till ett visningsprogram för blandade media med parametern `locale=`.

## Bildåtergivning {#image-renderer}

Sidan Bildåtergivning används för att ange standardinställningar för att leverera bilduppsättningar från bildåtergivningsservrar. Inställningarna är tillgängliga i följande fem kategorier (mer information om inställningarna finns på sidan Image Server):

* **[!UICONTROL Catalog Management]**: De här inställningarna avgör hur Adobe Dynamic Media Classic och katalogfilen interagerar. Adobe Dynamic Media Classic Render Server URL-anrop görs till katalogen, som i sin tur anropar för att leverera bilder från servern. Ändra dessa inställningar endast med hjälp av en supportperson från Adobe Dynamic Media Classic.

* **[!UICONTROL Session Attributes]**: De här inställningarna anger felparametrar, URL:en för relativa bild-URL:er och om objektöverlappning tillåts.

* **[!UICONTROL Default Material Attributes]**: De här inställningarna anger standardinställningar för upplösning och skärpa för bilder.

* **[!UICONTROL Response Image Attributes]**: De här inställningarna gäller standardutseendet för bilder.

* **[!UICONTROL Color Management Attributes]**: De här inställningarna gäller bildens standardfärginställningar.

## Vinjett {#vignette}

På sidan Vinjett finns inställningar för att ange standardutseende för vinjetter (mer information om alternativen finns på själva sidan).
