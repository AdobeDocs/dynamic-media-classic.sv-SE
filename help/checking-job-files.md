---
title: Kontrollerar jobbfiler
description: Lär dig hur du kontrollerar jobbfiler.
uuid: 8241a894-3014-4a5c-96ef-71f3aaa3716a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: d53ae5dd-8daf-4d87-b9a6-3039bad30538
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
exl-id: b6b11e1c-5eda-4bdb-8ffb-ecd3678f2352
translation-type: tm+mt
source-git-commit: 98463dbc24e141547d01bd3f71b1b9fe3a692c14
workflow-type: tm+mt
source-wordcount: '1582'
ht-degree: 1%

---

# Kontrollerar jobbfiler{#checking-job-files}

Dynamic Media Classic erbjuder jobbsidan för att övervaka filöverföringar till Dynamic Media Classic och filer som du publicerar på Dynamic Media Classic-servrar. Du kan granska överförings- och publiceringsjobb på jobbsidan, kontrollera status för jobb och avbryta publiceringsjobb från den här sidan. Du kan också schemalägga överförings- och publiceringsjobb.

När du överför resurser visas en snurrande ikon bredvid menyn Jobb, som anger att ett jobb pågår och hur många filer som bearbetas. Du kan klicka på ikonen om du vill visa mer information om det aktiva jobbet.

>[!NOTE]
>
>En lista över dina nyligen publicerade jobb finns också på sidan Senaste aktivitet. Klicka på **[!UICONTROL Recent]** i fältet Global navigering för att öppna den här sidan.

## Om sidan Jobb {#about-the-jobs-page}

Välj **[!UICONTROL Jobs]** i fältet Global navigering för att öppna sidan Jobs. Som standard listas jobb med början från den senaste.

Jobb visas i följande kategorier på fliken Historik på sidan Jobb:

**JobbtypEn** ikon anger jobbtypen: Överföring och publicering är de vanligaste jobbtyperna.

**Jobbnamn** Jobbets namn. Namnet innehåller den användardefinierade delen av namnet samt datum och tid.

**** StartadesNär jobbet startades.

**Totalt** antal överförda filer.

**W (varningar)** Antalet varningar i jobbet (om sådana finns). Varningar indikerar problem med jobbet som inte påverkade det övergripande jobbslutförandet. Dessa varningar kan vanligtvis ignoreras eftersom de rapporterar om dolda filer. Till exempel innehåller `.DS_store`-filer (Macintosh) och Thumbs.db-filer (Windows®) information om hur du visar bildfiler för användare. Du kan dock ignorera varningsmeddelanden om de här filerna eftersom de inte gäller hur filerna används i Dynamic Media Classic. Du kan dubbelklicka på ett jobbnamn för att få detaljerad information om varningar.

**E (fel)** Visar antalet fel i jobbet (om det finns några). Du kan dubbelklicka på ett jobbnamn för att få detaljerad information om fel.

**** VaraktighetHur lång tid det tog att slutföra jobbet.

**Status** Visar jobbets status.

**Mål** För överföringsjobb, företagsnamnet och mappen som filerna överfördes till. Den här kategorin gäller inte för publiceringsjobb.

**Skickat** avListor som överförde tillgångarna.

***Obs **: Du kan avbryta pågående publicerings- och överföringsjobb genom att klicka på knappen Avbryt bredvid förloppsindikatorn.*

## Ändra vyer på jobbsidan {#changing-views-on-the-jobs-page}

Använd följande tekniker för att sortera jobb eller ändra vyn på fliken Historik på sidan Jobb:

**** SorteringVälj ett kolumnnamn om du vill sortera listan efter en viss kolumn. Du kan välja växeln bredvid kolumnnamnet för att sortera i fallande eller stigande ordning.

**DatumintervallVälj** menyn Datumintervall och välj ett alternativ för att begränsa listan med jobb till aktuellt datum, föregående vecka eller föregående månad. Välj Anpassat datumintervall och ange sedan ett specifikt datumintervall.

**Jobbtyp** Välj menyn Jobbtyp och välj Publicera eller Överför för att begränsa listan till publiceringsjobb eller överföringsjobb. Välj Alla om du vill visa båda typerna av jobb.

**** VisaVälj Visa > Mina jobb eller Visa > Alla jobb för att begränsa listan till jobb som du har beställt eller jobb som personer i ditt företag har beställt.

## Visa, kopiera eller skriva ut en jobbdetaljrapport {#viewing-copying-or-printing-a-job-details-report}

Dubbelklicka på namnet på en rapport på jobbsidan för att öppna sidan Jobbdetaljer. Den här sidan innehåller en sammanfattningsrapport om filerna i jobbet. Klicka på Visa detalj om du vill visa en posts Dynamic Media Classic ID, målsökväg och statusinformation. Om du överförde en PDF- eller PostScript-fil som kräver teckensnitt som inte finns i Dynamic Media Classic visas en lista med de saknade teckensnitten i rapporten.

Du kan kopiera den här informationen till Urklipp.

1. Dubbelklicka på namnet på en rapport på jobbsidan för att öppna sidan Jobbdetaljer.
1. Klicka på Visa detalj för att få en detaljerad rapport om ett inlägg.
1. Klicka på Kopiera till Urklipp.

## Hantera återkommande överförings- och publiceringsjobb {#handling-recurring-upload-and-publish-jobs}

Återkommande överförings- och publiceringsjobb som du skapar på sidorna Överför och Publicera visas på fliken Schemalagda på sidan Jobb. Du kan redigera och ta bort återkommande jobb på fliken Schemalagda.

Välj knappen Jobb i fältet Global navigering och på sidan Jobb väljer du fliken Schemalagda för att redigera och ta bort återkommande jobb.

>[!NOTE]
>
>Du kan filtrera jobblistan på fliken Schemalagda med menyerna Jobbtyp och Visa. Välj en jobbtyp om du vill begränsa listan till att publicera jobb av en viss typ. Välj alternativet Visa om du vill visa jobb som du har skapat eller jobb som har skapats av alla i företaget.

### Redigera, ta bort, pausa och återuppta återkommande jobb {#editing-deleting-pausing-and-resuming-recurring-jobs}

Markera ett återkommande jobb på sidan Jobb och följ dessa instruktioner för att redigera eller ta bort det:

**Redigera ett återkommande** jobbVälj knappen Redigera och ange schemainformation i dialogrutan Redigera schemalagt jobb. Om du vill att jobbet ska upprepas med valfritt intervall väljer du Upprepa > Anpassa.

Se [Skapa ett anpassat tidsintervall för överföring eller publicering](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

**Ta bort ett återkommande** jobbVälj knappen Ta bort.

**Pausa (och återuppta) ett återkommande** jobbAvmarkera kryssrutan i kolumnen Aktiv om du vill pausa ett jobb. markera en kryssruta för att återuppta ett pausat jobb.

### Skapar ett anpassat tidsintervall för överföring eller publiceringsjobb {#creating-a-custom-upload-or-publish-job-time-interval}

Om du vill skapa ett anpassat tidsintervall för en överföring (via FTP) eller ett publiceringsjobb väljer du Upprepa > Anpassad på sidan Överför eller Publicera. Ange sedan siffror och jokertecken i rutan Regel för att ange ett tidsintervall för överförings- eller publiceringsjobben som ska återkomma.

Syntaxen för att beskriva anpassade tidsintervall för överföring och publicering i rutan Regel är:

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

Till exempel schemalägger `0 15 10 * * ?` ett jobb vid 10:15.00 varje dag.

I följande tabeller och listor beskrivs hur du beskriver ett tidsintervall i rutan Regel.

I den här tabellen visas tidsökningar, deras tillåtna värden och de jokertecken som de stöder:

| Tidssteg | Tillåtna värden | Kommentarer | Jokertecken stöds |
|--- |--- |--- |--- |
| Sekunder | 0-59 |  | `, - * /` |
| Minuter | 0-59 |  | `, - * /` |
| Timmar | 0-23 | Observera användningen av en 24-timmarsklocka. | `, - * /` |
| Dag i månaden | 1-31 | Du kan inte ange ett numeriskt värde för både&quot;dag i månaden&quot; och&quot;dag i veckan&quot;. Ett av dessa fält måste innehålla jokertecknet `?`. | `, - * / ? L C` |
| Månad | 1-12 eller jan, feb, mar, apr, maj, jun, juli, aug, sep, sep, okt, nov, dec | Värdena är skiftlägeskänsliga. | `, - * /` |
| Veckodag | Mån, Tue, Wed, Thu, Fri, Sat, Sun | Värdena är skiftlägeskänsliga. Du kan inte ange ett numeriskt värde för både&quot;dag i månaden&quot; och&quot;dag i veckan&quot;. Ett av dessa fält måste innehålla jokertecknet `?`. | `, - * / ? L C #` |
| År (valfritt) | Tom eller 1970-2099 |  | `, - * /` |


I den här tabellen beskrivs de jokertecken som är tillåtna i rutan Regel och hur du använder dem:

| Jokertecken | Namn | Vad det beskriver |
|--- |--- |--- |
| `*` | Asterisk | Alla värden (till exempel &quot;varje minut&quot;). |
| `?` | Frågetecken | Inget specifikt värde (t.ex. &quot;någon minut inom den angivna timmen&quot;). |
| `,` | Komma | Andra värden (t.ex. &quot;Måndag och onsdag&quot;). |
| `-` | Bindestreck | Värdeintervall (t.ex. &quot;Måndag till fredag&quot;). |
| `/` | Snedstreck | Ökningar (t.ex. &quot;var 15:e minut&quot;). |
| `L` | Versalt L | Sista&quot;dag i månaden&quot; eller&quot;veckodag&quot; (endast tillgängligt för dessa fält). Om månaden till exempel är januari, schemaläggs jobbet till den 31 januari med ett L-värde för fältet &quot;dag i månaden&quot;. I fältet Veckodag kan du ange det här tecknet enbart för att schemalägga jobbet på lördag. Du kan använda den med ett tal (till exempel `6L`) för att ange sista fredagen i månaden. Ange inte `L` med jokertecken för kommatecken eller bindestreck. |
| `#` | Nummertecken | &quot;Nth&quot; veckodag i månaden (endast tillgängligt för fältet &quot;day of the week&quot;). Till exempel anger `6#3` i fältet &quot;veckodag&quot; den tredje fredagen i månaden. `6` betecknar &quot;fredag&quot; (den sjätte dagen i veckan) och `3` den tredje förekomsten i månaden. |
| `C` | # Versalt C | Första kalendern &quot;dag i månaden&quot; eller &quot;veckodag&quot; (endast tillgängligt för dessa fält). Om du till exempel anger värdet `1C` för &quot;dag i månaden&quot; schemaläggs den första dagen i kalendern som inträffar den femte eller senare. Om du anger `1C` för veckodagen schemaläggs den första dagen i kalendern som inträffar på eller efter söndag |

Den här listan innehåller exempel på hur du beskriver tidsintervall i rutan Regel:

* 0 0 12 * * ?: Ingen varje dag
* 0 15 10 - *: 10.15 varje dag
* 0 0/5 14 * * ?: Var 5:e minut mellan kl. 2:55 varje dag
* 0 0/5 14,18 * * ?: Var 5:e minut mellan kl. 2:55 varje dag och var 5:e minut mellan kl. 6:00 och kl. 6:55 varje dag
* 0 10,44 14 - 3: Ved kl. 2.10 och kl. 2.44 varje onsdag i mars
* 0 15 10 - *: mån-fre kl. 10.15 varje veckodag
* 0 15 10 20 * ?: Klockan 10.15 den 20 varje månad
* 0 15 10 L * ?: Klockan 10.15 den sista dagen i varje månad
* 0 15 10 - * 6L: Klockan 10.15 den sista fredagen varje månad
* 0 15 10 * * 6#3: Klockan 10.15 den tredje fredagen varje månad

## Använda ett överförings- eller publiceringsjobb som utlösare {#using-an-upload-or-publish-job-as-a-trigger}

När du överför resurser via FTP eller kör ett publiceringsjobb kan du schemalägga ett efterföljande jobb så att det börjar när överföringen är klar. (Om andra jobb är schemalagda att starta, köas jobbet som du schemalägger här bakom dem.) Det nya jobbet skickar ett meddelande till den adress du anger så att koden på den platsen kan utlösas. Detta uppföljningsjobb får samma namn som det aktuella överföringsjobbet, men med prefixet _Pub.

Om du vill att ett överförings- eller publiceringsjobb ska utlösa ett annat jobb väljer du Avancerat på sidan Överför eller Publicera. Ange sedan URL:en i textfältet HTTP-meddelande.
