---
title: Publiceringsinställningar
description: Med inställningarna för publiceringsinställningar kan du bestämma hur resurser levereras som standard från Dynamic Media Classic-servrar till webbplatser eller program.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Administrator
translation-type: tm+mt
source-git-commit: 5efad4fff11c9818d43d46ebbbce5335ee1e72b8
workflow-type: tm+mt
source-wordcount: '2416'
ht-degree: 0%

---


# Publiceringsinställningar {#publish-setup}

Inställningarna på skärmen Publiceringsinställningar avgör hur resurser levereras som standard från Dynamic Media Classic-servrar till webbplatser eller program. Om ingen inställning har angetts levererar Dynamic Media Classic-servern en resurs enligt en standardinställning på en publiceringsinställningsskärm. En begäran om att leverera en bild som inte innehåller ett upplösningsattribut ger till exempel en bild med inställningen för standardobjektupplösning på skärmen Bildserver.

Administratörer kan ändra standardinställningarna på bildservern, bildåtergivningen och vinjettskärmarna för att ange standardinställningar för att leverera resurser från servrar.

Om du vill öppna installationsfönstren klickar du på **Inställningar** > **Programinställningar** > **Publiceringsinställningar**.

>[!NOTE]
>
>Publiceringsinstallationsskärmarna är avsedda att användas av erfarna webbplatsutvecklare och programmerare. Dynamic Media Classic förutsätter att användare som ändrar inställningar på dessa skärmar känner till Dynamic Media Classic, HTTP-protokollets standarder och konventioner samt grundläggande bildbehandlingsteknik.

## Bildserver {#image-server}

Bildserverskärmen anger standardinställningar för att leverera bilder från bildservrar. Inställningarna är tillgängliga i dessa fem kategorier (mer information om inställningarna finns på skärmen Image Server).

Ändra dessa inställningar endast med hjälp av en Dynamic Media Classic-supportperson.

**KataloghanteringDe här** inställningarna avgör hur Dynamic Media Classic och katalogen interagerar. Till skillnad från de flesta webbservrar går URL-anrop till Dynamic Media Image Server till en manifest- eller katalogfil i stället för till en bildfil. Katalogfilen (som inte ska blandas ihop med en e-katalog) innehåller en lista över allt innehåll som publiceras till bildservern tillsammans med sökvägen till varje bild. Om du har ett Digimarc-ID anger du din användarinformation i avsnittet Användarinformation för Digimarc.

**Begär** attributDe här inställningarna begränsar antalet bilder som kan levereras från servern. Till exempel är *maximum* **[!UICONTROL Reply Image Size Limit]** **[!UICONTROL Width]** 5000 och **[!UICONTROL Height]** 5000.

**Standardattribut för** begäranDe här inställningarna gäller standardutseendet för bilder.

**Vanliga** miniatyrattributDe här inställningarna gäller för miniatyrbildernas standardutseende och justering.

**Standardvärden för** katalogfältDe här inställningarna gäller för upplösningen och standardminiatyrbildstypen för bilder.

**Färghanteringsattribut** De här inställningarna bestämmer vilka ICC-färgprofiler som används.

**Kompatibilitetsattribut** Den här inställningen gör att inledande och efterföljande stycken i textlager kan behandlas som de var i version 3.6 för bakåtkompatibilitet.

**LokaliseringsstödMed** de här inställningarna kan du hantera flera språkattribut. Här kan du också ange en sträng för språkområdeskarta så att du kan definiera vilka språk du vill ha stöd för de olika verktygstipsen i visningsprogram.

Om du till exempel är ett flernationellt varumärke som säljer i olika länder kan du se till att varje land har ett eget språkspecifikt visningsprogram. Om du vill använda den här funktionen anger du en sträng för språkområdeskarta. Därefter redigerar du verktygstipstexten i en visningsprogramförinställning genom att lägga till de översatta textsträngarna för det språk du vill använda.

>[!NOTE]
> [Använd Admin Console för att skapa ett supportärende om du vill ställa in alternativ för lokaliseringsstöd.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) I ditt supportärende, begär du hjälp med konfiguration.

Mer information om hur du konfigurerar **lokaliseringsstöd** finns i [Att tänka på när du konfigurerar lokalisering av resurser](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Att tänka på när du konfigurerar lokalisering av resurser {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Om du vill ställa in alternativ för lokaliseringsstöd i Dynamic Media Classic, till exempel fältet för språkinställningar, [använder du Admin Console för att skapa ett supportärende.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) I ditt supportärende, begär du hjälp med konfiguration.

Ett vanligt sätt att använda Dynamic Media Classic är att hantera produktbilder på e-handelswebbplatser. Internationella företag står inför utmaningen att resurser för liknande produkter ser annorlunda ut från land till land. Oftast är skillnaderna för en mycket liten del av det totala mediet. Att hantera sådana skillnader genom att kopiera alla tillgångar för vart och ett av länderna och skriva över bara skillnaderna är en stor insats och motsäger den enda överordnad tillgångsmetaforen. Skillnaderna i resurser kan uppstå, från landspecifika videor med olika ljudspår, till subtila men viktiga skillnader i en strömsladd som används med produkten. Dynamic Media Classic använder en grundläggande sökfunktion. Du definierar i vilken ordning som resurssuffixen som Image Server söker efter, med utgångspunkt i önskad språkinställning.

**Hur resurser lokaliseras**

Språkinställningen för en IS-begäran (Image Serving) identifieras med följande IS/IR-kommando (Image Rendering):

`locale=`

Det här kommandot accepterar en sträng för språk-ID (locId) som inte är skiftlägeskänslig. Språk-ID:t är vanligtvis en 2-6-teckensträng som består av bokstäver och&quot;_&quot;.

IS stöder godtyckliga utskrivbara ASCII-strängar. Kommandot `locale=` har ett globalt omfång, vilket innebär att det tillämpas på hela begäran, inklusive alla kapslade IS- och IR-begäranden, refererade mallar och bildlager. Det finns inte stöd för flera språkområden per begäran, t.ex. olika språkområden för varje lager. Det går dock att tillåta explicita åsidosättningar i kapslade begäranden.

Om `locale=` inte anges skickas `attribute::DefaultLocale` till översättningsmotorerna. Begränsad indatavalidering används för `locale=`-värdet. Tomma `locale=`-värden tillåts. Eftersom `locale=` har ett globalt omfång anges `attribute::DefaultLocale` av huvudkatalogen för hela begäran.

Några av fördelarna med att använda `locale=` och `attribute::DefaultLocale` är följande:

* Dela innehåll för flera språkområden.
* Använd språkspecifikt innehåll med generiska ID:n.
* Flexibla regler för namngivning och hantering av språkspecifikt innehåll, som prefix kontra suffix eller språkspecifikt innehåll i en separat katalog.
* Stöd för direktåtkomst till språkspecifika versioner.
* Sammansatta objekt, t.ex. bilduppsättningar, kan innehålla generiska referenser till potentiellt språkspecifikt innehåll.
* Stöder allt innehåll som hanteras av kataloger som kan behöva lokaliseras, inklusive bilder, bilduppsättningar, vinjetter, material och poster för visningsprogramkonfiguration.
* Minimera förändringar i IPS-databasen och IS-manifestmekanismer.
* Stöd för statiskt innehåll som videor och skal läggs till när RFC IS-63 implementeras.
* Standardspråket kan konfigureras.

**Programscenarier**

| Program | Scenario |
|--- |--- |
| Visningsprogramlokalisering | När statiska innehållskataloger har implementerats styrs lokaliseringen helt och hållet med parametern locale=, som bifogas alla begäranden som görs till IS. Konfigurationsposter, skal, välkomstskärmar och så vidare, kan ha språkspecifika varianter eller inte. Rätt innehåll tillhandahålls av IS utan att användaren behöver veta vilket innehåll som är lokaliserat och vilka ID:n det är. |
| Bilder och video | Flernationella företag har ofta en blandning av generiskt och språkspecifikt innehåll. Med den här funktionen kan en referens till en bild eller video vara allmän och IS visar det språkspecifika innehållet om det är tillgängligt. |
| Bilduppsättningar och medieuppsättningar | Hela bilduppsättningen kan vara annorlunda för vissa språk, t.ex. när en eCatalog är helt annorlunda, med översättningen från en allmän till en språkområdesspecifik bilduppsättning som hanteras av visningsprogrammet. Oftast kan enskilda ID:n i en allmän uppsättning referera till lokaliserat innehåll. De flesta foton i en enhet kan till exempel vara desamma på alla språk, förutom fotot på kontrollpanelen. IS översätter automatiskt ID:n, så du behöver inte generera språkspecifika bilduppsättningar. |

**Implementera resurslokalisering**

Dynamic Media Classic och Image Serving har ett gränssnitt som möjliggör lokalisering av bilder och statiskt innehåll.

Utan lokalisering ser en Image Server-URL ut så här:

`https://server/is/image/company/image`

Vid lokalisering lägger en Image Server-URL till parametern `locale=` i sökvägen, som i följande exempel:

`https://server/is/image/company/image?locale=de_DE`

När http-anropet tas emot av Image Server tolkas parametern `locale=` via fältet localeMap i **Inställningar** > **Programinställningar** > **Publiceringsinställningar** > **Bildserver** > **Lokaliseringsstöd&lt;a10/ > grupp.**

Fältet Lokalkarta innehåller en lista med poster som separeras med lodsymbolen (|).

Varje post består av en kommaavgränsad lista med värden. Det första värdet är det sökvärde som skickas av parametern `locale=`. De återstående värdena är suffix-/ersättningsvärden som sedan testas tills ett resultat har skapats i en befintlig bild.

Om ett suffixvärde eller ett ersättningsvärde används beror på inställningen för Global Locale i **Inställningar** > **Programinställningar** > **Publiceringsinställningar** > **Image Server** > **Lokaliseringsstöd**.

>[!NOTE]
>
>Inställningen Global Locale är för närvarande bara möjlig om du anger den via API:t, inte i Dynamic Media Classic-gränssnittet.

**Exempel på suffix**

| URL | localeMap-ID:n | Resultat |
|--- |--- |--- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | Observera att GlobalLocale inte har definierats. Språkinställningsparametern de_DE matchas mot den första posten i localeMap. Det första motsvarande värdet _DE läggs till som ett suffix till resursen image_DE och ett försök görs att hitta det på bildservern. Om den hittas på servern returneras den. I annat fall används det andra värdet &quot;&quot; som suffix, vilket resulterar i att själva bilden returneras. |

**Exempel på ersättning**

| URL | ID:n för GlobalLocale och localeMap | Resultat |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | I ersättningsexemplet ovan anges GlobalLocale till main. Språkinställningsparametern de_DE matchas mot den första posten i localeMap. Delsträngen GlobalLocale hittas och ersätts med det första motsvarande värdet i localeMap: image-de-01. Om den hittas på Image Server returneras den. Om inte ersätts det andra värdet, vilket resulterar i image-main-01. |

Om ingen språkinställning har definierats i URL:en tar Image Server DefaultLocale, om den är definierad, och tillämpar den på URL:en.

Om en okänd eller tom språkområdesparameter anges med `locale=` genomsöks localeMap efter det tomma värdet &quot;som börjar med,&quot;. Det är viktigt att konfigurera detta så att ett standardspråk används för okända språk.

**Om defaultImage**

Bildservern försöker att välja det begärda språket, det ena efter det andra. Om ingen matchning hittas används språkalternativen för defaultImage och den matchande versionen returneras. Därför bör varje språkinställning innehålla ett alternativ för bilden utan lokalisering, eller lokaliserade defaultImage-versioner bör vara tillgängliga i Dynamic Media Classic.

**Scenarier för att hitta localeMap**

Anta att du vill ha stöd för följande språk:

`en, en_us, en_uk, de, de_at, de_de, fr`

Du mappar dessa språkinställningar till suffixen `_E`, `_G` och `_F` för engelska, tyska respektive franska. För alla exempel är det allmänna ID:t för indatabilden `myImg`.

*Standardbeteende för att hitta localeMap*

Språk-ID:n mappas till motsvarande suffix. Om det inte finns något språkspecifikt ID i katalogen görs ett försök att använda det generiska ID:t. Observera de tomma locSuffix-värdena som mappar till det generiska ID:t.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | Utdata-ID att söka efter |
|--- |--- |
| en,en_us, en_uk | myImg_E, myImg |
| de,de_de,de_at | myImg_D, myImg |
| fr | myImg_F, myImg |
| Alla andra | - |

*Söka efter localeMap när språkinställningen är okänd*

Du kan mappa okända språk till specifika ID:n eller till generiska ID:n. Du kan till exempel mappa okända språkinställningar till engelska ID:n, eller om de inte finns, till generiska ID:n.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | Utdata-ID att söka efter |
|--- |--- |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| Alla andra | myImg_E,myImg |

Du kan också ha ett dedikerat locSuffix, till exempel U, bara för okända språkinställningar, och tvinga till standardbilden om det inte finns någon `_U`, som i följande exempel:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

Du kan också mappa direkt till det generiska ID:t, som i följande exempel:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

*Söka efter localeMap med hjälp av en sökning på flera nivåer*

Det är ofta önskvärt att gruppera språkområden, t.ex. europeiska, Mellanöstern och Nordamerika, för att ta hänsyn till regionala standarder, t.ex. hudexponering. Du kan uppnå den här effekten med en sökning på flera nivåer.

Anta i det här exemplet att du vill ha stöd för samlingar för väst- och Mellanöstern-användning. Båda samlingarna är baserade på den generiska bildsamlingen, och båda lägger till eller ändrar vissa bilder. Båda samlingarna har sedan förfinats ytterligare för specifika språkområden, till exempel `m1, m2` för två mellanöstra varianter och `w1, w2,` och `w3` för tre västerländska språkområden, förutom att bilder delas för `w1` och `w3`. Okända språk mappas endast till den generiska samlingen och har inte tillgång till språkspecifika bilder. Så här skulle kartan se ut:

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale= | Utdata-ID att söka efter |
|--- |--- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| Alla andra | mylmg |

*Söka efter localeMap genom att söka efter specifika ID:n*

Vissa namngivningskonventioner kanske inte stöder generiska bild-ID:n. De generiska ID:n från begäran måste mappas till ett specifikt ID i katalogen. Det kan dock finnas tillfällen då det exakta specifika ID:t inte är känt.

Om du använder det första exemplet som bas kan bilder för alla språk ha suffixen `_1`, `_2` eller `_3`. Bilder som är specifika för franska språk kan ha suffixen `_22` eller `_23`. Och bilder som är specifika för tyska språk kan ha suffixen `_470` eller `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | Utdata-ID att söka efter |
|--- |--- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| Alla andra | myImg_1, myImg_2, myImg_3 |

**Viktiga överväganden vid implementering av lokaliseringsstöd**

* Lokaliseringen är begränsad till ID-baserade tillgångsanrop och kan inte användas för sökvägsbaserade resursanrop. När videoklipp med språkområde anropas måste de därför anropas som företag/tillgångs-ID. ingen fullständig sökväg till videon. Det innebär att du inte kan använda rtmp vid lokalisering eftersom den metoden endast är avsedd för sökvägsbaserade videoanrop.
* Du kan inte använda en uppsättning med blandade media som innehåller en enda video när localeMap är aktivt, annars misslyckas anropet till innehållet i uppsättningen. Du kan undvika det här problemet genom att lägga till en enda video i en adaptiv videouppsättning. Lägg sedan till den adaptiva videouppsättningen i en blandad medieuppsättning.
* Vissa förfrågningar är inte lokaliserade, till exempel förfrågningar om innehållet i en adaptiv videouppsättning. Om du tänker använda adaptiva videouppsättningar tillsammans med lokalisering bör du därför placera den adaptiva videouppsättningen i en blandad medieuppsättning. Anropa sedan uppsättningen till ett visningsprogram för blandade media med parametern `locale=`.

## Bildåtergivning {#image-renderer}

Skärmen Bildåtergivning används för att ange standardinställningar för att leverera bilduppsättningar från bildåtergivningsservrar. Inställningarna är tillgängliga i följande fem kategorier (mer information om inställningarna finns på skärmen Image Server):

**Kataloghantering** De här inställningarna avgör hur Dynamic Media Classic och katalogfilen interagerar. Dynamic Media Classic Render Server URL-anrop görs till katalogen, som i sin tur anropar för att leverera bilder från servern. Ändra dessa inställningar endast med hjälp av en Dynamic Media Classic-supportperson.

**Sessionsattribut** De här inställningarna anger felparametrar, URL:er för relativa bild-URL:er och om objektöverlappning tillåts.

**StandardmaterialattributDe här** inställningarna anger standardinställningar för upplösning och skärpa för bilder.

**Attribut** för svarsbildDe här inställningarna gäller standardutseendet för bilder.

**FärghanteringsattributDe här** inställningarna gäller bildens standardfärginställningar.

## Vinjett {#vignette}

Vinjettskärmen innehåller inställningar för att ange standardutseende för vinjettering (se själva skärmen för detaljerade beskrivningar av alternativen).
