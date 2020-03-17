---
title: Publiceringsinställningar
seo-title: Publiceringsinställningar
description: 'null'
seo-description: Inställningarna på skärmen Publiceringsinställningar avgör hur resurser levereras som standard från dynamiska Media Classic-servrar till webbplatser eller program.
uuid: 196f25c8-abf5-4c5d-8f6f-bc70007a0301
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
discoiquuid: cba59093-28b6-4490-b838-d942b72ad1ec
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Publiceringsinställningar {#publish-setup}

Inställningarna på skärmen Publiceringsinställningar avgör hur resurser levereras som standard från dynamiska Media Classic-servrar till webbplatser eller program. Om ingen inställning har angetts levererar Dynamic Media Classic-servern en resurs enligt en standardinställning på en publiceringsinställningsskärm. En begäran om att leverera en bild som inte innehåller ett upplösningsattribut ger till exempel en bild med inställningen för standardobjektupplösning på skärmen Bildserver.

Administratörer kan ändra standardinställningarna på bildservern, bildåtergivningen och vinjettskärmarna för att ange standardinställningar för att leverera resurser från servrar.

Om du vill öppna publiceringsinställningarna klickar du på Inställningar > Programinställningar > Publiceringsinställningar.

>[!NOTE]
>
>Publiceringsinstallationsskärmarna är avsedda att användas av erfarna webbplatsutvecklare och programmerare. Dynamic Media Classic förutsätter att användare som ändrar inställningar på dessa skärmar känner till Scene7 Publishing System, HTTP-protokollets standarder och konventioner samt grundläggande bildbehandlingsteknik.

## Bildserver {#image-server}

Bildserverskärmen används för att ange standardinställningar för att leverera bilder från bildservrar. Inställningarna är tillgängliga i dessa fem kategorier (mer information om inställningarna finns på skärmen Image Server).

Ändra dessa inställningar endast med hjälp av en supporttekniker för Dynamic Media Classic.

**Kataloghantering** Dessa inställningar avgör hur Scene7 Publishing System och katalogen interagerar. Till skillnad från de flesta webbservrar går URL-anrop till Dynamic Media Image Server till en manifest- eller katalogfil i stället för till en bildfil. Katalogfilen (som inte ska blandas ihop med en e-katalog) innehåller en lista över allt innehåll som publiceras till bildservern tillsammans med sökvägen till varje bild. Om du har ett Digimarc-ID anger du din användarinformation i avsnittet Användarinformation för Digimarc.

**Attribut** för begäran Dessa inställningar begränsar antalet bilder som kan levereras från servern.

**Standardattribut** för begäran De här inställningarna gäller standardutseendet för bilder.

**Vanliga miniatyrattribut** De här inställningarna gäller för miniatyrbildernas standardutseende och justering.

**Standardvärden för katalogfält** Dessa inställningar gäller för upplösningen och standardminiatyrbildstypen för bilder.

**Färghanteringsattribut** Dessa inställningar avgör vilka ICC-färgprofiler som används.

**Kompatibilitetsattribut** Den här inställningen gör att inledande och efterföljande stycken i textlager kan behandlas som de var i version 3.6 för bakåtkompatibilitet.

**Lokaliseringsstöd** Med dessa inställningar kan du hantera flera språkattribut. Här kan du också ange en sträng för språkområdeskarta så att du kan definiera vilka språk du vill ha stöd för de olika verktygstipsen i visningsprogram.

Om du till exempel är ett flernationellt varumärke som säljer i olika länder kan du se till att varje land har ett eget språkspecifikt visningsprogram. Om du vill använda den här funktionen anger du en sträng för språkområdeskarta. Därefter redigerar du verktygstipstexten i en visningsprogramförinställning genom att lägga till de översatta textsträngarna för det språk du vill använda.

>[!NOTE]
> Om du vill ställa in alternativ för lokaliseringsstöd kontaktar du Adobe Dynamic Media Classic Technical Support eller skickar ett e-postmeddelande till s7support@adobe.com där du behöver hjälp med installationen.

Mer information om hur du konfigurerar **lokaliseringsstöd** finns i [Saker att tänka på när du konfigurerar lokalisering av resurser](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Att tänka på när lokalisering av resurser konfigureras {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Om du vill ställa in alternativ för lokaliseringsstöd i Scene7 Publishing System, t.ex. fältet för språkinställningar, kontaktar du Adobe Dynamic Media Classic Technical Support. Du kan också skicka ett e-postmeddelande till s7support@adobe.com som begär installationshjälp.

Ett vanligt sätt att använda Scene7 Publishing System (SPS) är att hantera produktbilder på e-handelswebbplatser. Internationella företag står inför utmaningen att resurser för liknande produkter ser annorlunda ut från land till land. Oftast är skillnaderna för en mycket liten del av det totala mediet. Att hantera sådana skillnader genom att kopiera alla resurser för vart och ett av länderna och skriva över bara skillnaderna är en stor insats och motsäger den enda huvudtillgångsmetaforen. Skillnaderna i resurser kan uppstå, från landspecifika videor med olika ljudspår, till subtila men viktiga skillnader i en strömsladd som används med produkten. Dynamic Media Classic använder en grundläggande sökfunktion. Du definierar i vilken ordning som resurssuffixen som Image Server söker efter, med utgångspunkt i önskad språkinställning.

**Hur resurser lokaliseras**

Språkinställningen för en IS-begäran (Image Serving) identifieras med följande IS/IR-kommando (Image Rendering):

`locale=`

Det här kommandot accepterar en sträng för språk-ID (locId) som inte är skiftlägeskänslig. Språk-ID:t är vanligtvis en 2-6-teckensträng som består av bokstäver och&quot;_&quot;.

IS stöder godtyckliga utskrivbara ASCII-strängar. `locale=` Kommandot har ett globalt omfång, vilket innebär att det tillämpas på hela begäran, inklusive alla kapslade IS- och IR-begäranden, refererade mallar och bildlager. Det finns inte stöd för flera språkområden per begäran, t.ex. olika språkområden för varje lager. Det går dock att tillåta explicita åsidosättningar i kapslade begäranden.

Om `locale=` inte anges skickas `attribute::DefaultLocale` till översättningsmotorerna. Begränsad indatavalidering används för `locale=` värdet. Tomma `locale=` värden tillåts. Eftersom `locale=` har ett globalt omfång `attribute::DefaultLocale` anges huvudkatalogen för hela begäran.

Några av fördelarna med att använda `locale=` och `attribute::DefaultLocale` inkludera:

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

Scene7 Publishing och Image Serving har ett gränssnitt som gör det möjligt att lokalisera bilder och statiskt innehåll.

Utan lokalisering ser en Image Server-URL ut så här:

`https://server/is/image/company/image`

Vid lokalisering lägger en Image Server-URL till parametern i sökvägen, som i följande exempel: `locale=`

`https://server/is/image/company/image?locale=de_DE`

När http-anropet tas emot av Image Server tolkas `locale=` parametern via fältet localeMap som finns i **Inställningar** > **Programinställningar** > **Publiceringsinställningar** > **Bildserver** > gruppen **** Lokaliseringsstöd¥.

Fältet Lokalkarta innehåller en lista med poster som separeras med lodsymbolen (|).

Varje post består av en kommaavgränsad lista med värden. Det första värdet är det sökvärde som skickas av `locale=` parametern. De återstående värdena är suffix-/ersättningsvärden som sedan testas tills ett resultat har skapats i en befintlig bild.

Om ett suffixvärde eller ett ersättningsvärde används beror på inställningen för Global Locale (Global Locale) i **Inställningar** > **Application Setup** > **Publish Setup** > **Image Server** > gruppen **Localization Support** (Lokaliseringsstöd).

>[!NOTE]
>
>Inställningen Global Locale är för närvarande bara möjlig när du anger den via API:t, inte i gränssnittet för Scene7 Publishing System.

**Exempel på suffix**

| URL | localeMap-ID:n | Resultat |
|--- |--- |--- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | Observera att GlobalLocale inte har definierats. Språkinställningsparametern de_DE matchas mot den första posten i localeMap. Det första motsvarande värdet _DE läggs till som ett suffix till resursen image_DE och ett försök görs att hitta det på bildservern. Om den hittas på servern returneras den. I annat fall används det andra värdet &quot;&quot; som suffix, vilket resulterar i att själva bilden returneras. |

**Exempel på ersättning**

| URL | ID:n för GlobalLocale och localeMap | Resultat |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | I ersättningsexemplet ovan anges GlobalLocale till main. Språkinställningsparametern de_DE matchas mot den första posten i localeMap. Delsträngen GlobalLocale hittas och ersätts med det första motsvarande värdet i localeMap: image-de-01. Om den hittas på Image Server returneras den. Om inte ersätts det andra värdet, vilket resulterar i image-main-01. |

Om ingen språkinställning har definierats i URL:en tar Image Server DefaultLocale, om den är definierad, och tillämpar den på URL:en.

Om en okänd eller tom språkområdesparameter anges `locale=`skannas localeMap för det tomma värdet &quot;som börjar med,&quot;. Det är viktigt att konfigurera detta så att ett standardspråk används för okända språk.

**Om defaultImage**

Bildservern försöker att välja det begärda språket, det ena efter det andra. Om ingen matchning hittas används språkalternativen för defaultImage och den matchande versionen returneras. Därför bör varje språkinställning innehålla ett alternativ för bilden utan lokalisering, eller lokaliserade defaultImage-versioner bör vara tillgängliga i Scene7 Publishing System.

**Scenarier för att hitta localeMap**

Anta att du vill ha stöd för följande språk:

`en, en_us, en_uk, de, de_at, de_de, fr`

Du mappar dessa språkområden till suffixen `_E`, `_G`och `_F`för engelska, tyska respektive franska. För alla exempel är det generiska ID:t för indatabilden `myImg`.

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

Du kan också ha ett dedikerat locSuffix, till exempel U, för okända språk, och tvinga till standardbilden om det inte `_U` finns någon, som i följande exempel:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

Du kan också mappa direkt till det generiska ID:t, som i följande exempel:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

*Söka efter localeMap med hjälp av en sökning på flera nivåer*

Det är ofta önskvärt att gruppera språkområden, t.ex. europeiska, Mellanöstern och Nordamerika, för att ta hänsyn till regionala standarder, t.ex. hudexponering. Du kan uppnå den här effekten med en sökning på flera nivåer.

Anta i det här exemplet att du vill ha stöd för samlingar för väst- och Mellanöstern-användning. Båda samlingarna är baserade på den generiska bildsamlingen, och båda lägger till eller ändrar vissa bilder. Båda samlingarna förfinas sedan ytterligare för specifika språkområden, t.ex. `m1, m2` för två varianter från Mellanöstern, och `w1, w2,` för tre västerländska språkområden, förutom att bilderna delas för `w3` och `w1` `w3`. Okända språk mappas endast till den generiska samlingen och har inte tillgång till språkspecifika bilder. Så här skulle kartan se ut:

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

Om du använder det första exemplet som bas kan bilder för alla språk ha suffixen `_1`, `_2`eller `_3`. Bilder som är specifika för franska språk kan ha suffixen `_22` eller suffixet `_23` . Och bilder som är specifika för tyska språk kan ha suffixen `_470` eller `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | Utdata-ID att söka efter |
|--- |--- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| Alla andra | myImg_1, myImg_2, myImg_3 |

**Viktiga överväganden vid implementering av lokaliseringsstöd**

* Lokaliseringen är begränsad till ID-baserade tillgångsanrop och kan inte användas för sökvägsbaserade resursanrop. När videoklipp med språkområde anropas måste de därför anropas som företag/tillgångs-ID. ingen fullständig sökväg till videon. Det innebär att du inte kan använda rtmp vid lokalisering eftersom den metoden endast är avsedd för sökvägsbaserade videoanrop.
* Du kan inte använda en uppsättning med blandade media som innehåller en enda video när localeMap är aktivt, annars misslyckas anropet till innehållet i uppsättningen. Du kan undvika det här problemet genom att lägga till en enda video i en adaptiv videouppsättning. Lägg sedan till den adaptiva videouppsättningen i en blandad medieuppsättning.
* Vissa förfrågningar är inte lokaliserade, till exempel förfrågningar om innehållet i en adaptiv videouppsättning. Om du tänker använda adaptiva videouppsättningar tillsammans med lokalisering bör du därför placera den adaptiva videouppsättningen i en blandad medieuppsättning. Anropa sedan uppsättningen till ett visningsprogram för blandade media med `locale=` parametern .

## Bildåtergivning {#image-renderer}

Skärmen Bildåtergivning används för att ange standardinställningar för att leverera bilduppsättningar från bildåtergivningsservrar. Inställningarna är tillgängliga i följande fem kategorier (mer information om inställningarna finns på skärmen Image Server):

**Kataloghantering** Dessa inställningar avgör hur Scene7 Publishing System och katalogfilen interagerar. URL-anrop till den dynamiska Media Classic Render Server görs till katalogen, som i sin tur anropar för att leverera bilder från servern. Ändra dessa inställningar endast med hjälp av en supporttekniker för Dynamic Media Classic.

**Sessionsattribut** Dessa inställningar anger felparametrar, URL:er för relativa bild-URL:er och huruvida objektöverlappning är tillåten.

**Standardmaterialattribut** De här inställningarna anger standardinställningar för upplösning och skärpa för bilder.

**Svarsbildattribut** Dessa inställningar gäller standardutseendet för bilder.

**Färghanteringsattribut** Dessa inställningar gäller bildens standardfärginställningar.

## Vinjett {#vignette}

Vinjettskärmen innehåller inställningar för att ange standardutseende för vinjettering (se själva skärmen för detaljerade beskrivningar av alternativen).