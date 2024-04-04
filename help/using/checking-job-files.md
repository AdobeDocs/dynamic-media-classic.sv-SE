---
title: Kontrollera jobbfiler
description: Lär dig kontrollera jobbfiler i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: b6b11e1c-5eda-4bdb-8ffb-ecd3678f2352
topic: Administration, Content Management
level: Intermediate
source-git-commit: f054057d383b26e9088582f418f62504c3f327d8
workflow-type: tm+mt
source-wordcount: '1559'
ht-degree: 0%

---

# Kontrollera jobbfiler{#checking-job-files}

Adobe Dynamic Media Classic erbjuder jobbsidan för att övervaka filöverföringar till Adobe Dynamic Media Classic och filer som du publicerar på Adobe Dynamic Media Classic-servrar. Du kan granska överförings- och publiceringsjobb på jobbsidan, kontrollera status för jobb och avbryta publiceringsjobb från den här sidan. Du kan också schemalägga överförings- och publiceringsjobb.

När du överför resurser visas en snurrande ikon bredvid menyn Jobb, som anger att ett jobb pågår och hur många filer som bearbetas. Du kan markera ikonen om du vill visa mer information om det aktiva jobbet.

>[!NOTE]
>
>En lista över dina nyligen publicerade jobb finns också på sidan Senaste aktivitet. Välj **[!UICONTROL Recent]** i fältet Global navigering.

## Om sidan Jobb {#about-the-jobs-page}

Välj **[!UICONTROL Jobs]** i fältet Global navigering så att sidan Jobb öppnas. Som standard listas jobb med början från den senaste.

Jobb visas i följande kategorier på fliken Historik på sidan Jobb:

* **[!UICONTROL Job Type]** - En ikon anger jobbtypen: Överför och Publicera är de vanligaste jobbtyperna.

* **[!UICONTROL Job Name]** - Jobbets namn. Namnet innehåller den användardefinierade delen av namnet samt datum och tid.

* **[!UICONTROL Started]** - När jobbet påbörjades.

* **[!UICONTROL Total]** - Antal överförda filer.

* **[!UICONTROL W (warnings)]** - Antal varningar i jobbet (om sådana finns). Varningar indikerar problem med jobbet som inte påverkade det övergripande jobbslutförandet. Dessa varningar kan vanligtvis ignoreras eftersom de rapporterar om dolda filer. Till exempel: `.DS_store` filer (Mac) och Thumbs.db-filer (Windows®) innehåller information om hur du visar bildfiler för användare. Varningsposter för dessa filer kan dock ignoreras eftersom de inte gäller hur dessa filer används i Adobe Dynamic Media Classic. Du kan dubbelklicka på ett jobbnamn för att få detaljerad information om varningar.

* **[!UICONTROL E (errors)]** - Visar antalet fel i jobbet (om sådana finns). Du kan dubbelklicka på ett jobbnamn för att få detaljerad information om fel.

* **[!UICONTROL Duration]** - Hur lång tid det tog att slutföra jobbet.

* **[!UICONTROL Status]** - Visar status för jobbet.

* **[!UICONTROL Destination]** - För överföringsjobb, företagsnamnet och mappen som filerna överfördes till. Den här kategorin gäller inte för jobb för publicering.

* **[!UICONTROL Submitted By]** - Visar vem som överförde resurserna.

>[!NOTE]
>
>Du kan avbryta pågående publicerings- och överföringsjobb genom att välja **[!UICONTROL Cancel]** intill förloppsindikatorn.

## Ändra vyer på sidan Jobb {#changing-views-on-the-jobs-page}

Använd följande tekniker för att sortera jobb eller ändra vyn på fliken Historik på sidan Jobb:

* **[!UICONTROL Sorting]** - Välj ett kolumnnamn om du vill sortera listan efter en viss kolumn. Du kan välja växeln bredvid kolumnnamnet för att sortera i fallande eller stigande ordning.

* **[!UICONTROL Date Range]** - Välj **[!UICONTROL Date Range]** och välj ett alternativ för att begränsa listan med jobb till aktuellt datum, föregående vecka eller föregående månad. Välj **[!UICONTROL Custom Date Range]** anger du sedan ett specifikt datumintervall.

* **[!UICONTROL Job Type]** - Välj **[!UICONTROL Job Type]** meny och välj **[!UICONTROL Publish]** eller **[!UICONTROL Upload]** för att begränsa listan till publiceringsjobb eller överföringsjobb. Välj **[!UICONTROL All]** för att se båda typerna av jobb.

* **[!UICONTROL Show]** - Gå till **[!UICONTROL Show]** > **[!UICONTROL My Jobs]** eller **[!UICONTROL Show]** > **[!UICONTROL All Jobs]** för att begränsa listan till jobb som du beställt eller jobb som personer i ditt företag beställt.

## Visa eller kopiera eller skriv ut en jobbdetaljrapport {#viewing-copying-or-printing-a-job-details-report}

Dubbelklicka på namnet på en rapport på jobbsidan så att sidan Jobbinformation öppnas. Den här sidan innehåller en sammanfattningsrapport om filerna i jobbet. Välj **[!UICONTROL View Detail]** så att du kan se en anmälnings Adobe Dynamic Media Classic-ID, målsökväg och statusinformation. Om du överförde en PDF- eller PostScript-fil som kräver teckensnitt som inte finns i Adobe Dynamic Media Classic visas en lista med de saknade teckensnitten i rapporten.

Du kan kopiera informationen till Urklipp.

1. Dubbelklicka på namnet på en rapport på sidan Jobs.
1. På sidan Jobbinformation väljer du **[!UICONTROL View Detail]** för att få en detaljerad rapport om ett tävlingsbidrag.
1. Välj **[!UICONTROL Copy to Clipboard]**.

## Hantera återkommande överförings- och publiceringsjobb {#handling-recurring-upload-and-publish-jobs}

Återkommande överförings- och publiceringsjobb som du skapar på sidorna Överför och Publicera visas på fliken Schemalagda på sidan Jobb. Du kan redigera och ta bort återkommande jobb på fliken Schemalagda.

Välj knappen Jobb i fältet Global navigering och välj på sidan Jobb **[!UICONTROL Scheduled]** så att du kan redigera och ta bort återkommande jobb.

>[!NOTE]
>
>Du kan filtrera jobblistan på **[!UICONTROL Scheduled]** med **[!UICONTROL Job Type]** och **[!UICONTROL Show]** menyer. Välj en jobbtyp så att du kan begränsa listan till att publicera jobb av en viss typ. Välj en **[!UICONTROL Show]** så att du kan visa jobb som du har skapat eller jobb som har skapats av alla i företaget.

### Redigera, ta bort, pausa och återuppta återkommande jobb {#editing-deleting-pausing-and-resuming-recurring-jobs}

Välj ett återkommande jobb på sidan Jobb och följ dessa instruktioner om du vill redigera eller ta bort det:

* **Redigera ett återkommande jobb** - Välj **[!UICONTROL Edit]** och ange schemainformation i dialogrutan Redigera schemalagt jobb. Om du vill att jobbet ska återkomma med valfritt intervall går du till **[!UICONTROL Repeat]** > **[!UICONTROL Custom]**.

Se [Skapa ett anpassat tidsintervall för överföring eller publiceringsjobb](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

* **Ta bort ett återkommande jobb** - Välj **[!UICONTROL Delete]** -knappen.

* **Pausa (och återuppta) ett återkommande jobb** - Avmarkera kryssrutan i kolumnen Aktiv om du vill pausa ett jobb. Markera kryssrutan om du vill återuppta ett pausat jobb.

### Skapa ett anpassat tidsintervall för överföring eller publiceringsjobb {#creating-a-custom-upload-or-publish-job-time-interval}

Om du vill skapa ett anpassat tidsintervall för en överföring (via FTP) eller ett publiceringsjobb går du till sidan Överför eller Publicera. **[!UICONTROL Repeat]** > **[!UICONTROL Custom]**. Ange sedan siffror och jokertecken i rutan Regel som beskriver ett tidsintervall för överförings- eller publiceringsjobben som ska återkomma.

Syntaxen för att beskriva anpassade tidsintervall för överföring och publicering i rutan Regel är:

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

Till exempel: `0 15 10 * * ?` schemalägger ett jobb kl. 10.15.00 varje dag.

I följande tabeller och listor beskrivs hur du beskriver ett tidsintervall i rutan Regel.

I den här tabellen visas tidsökningar, tillåtna värden och jokertecken som stöds:

| Tidsökningar | Tillåtna värden | Kommentar | Jokertecken stöds |
|--- |--- |--- |--- |
| Sekunder | 0-59 |  | `, - * /` |
| Minuter | 0-59 |  | `, - * /` |
| Timmar | 0-23 | Observera användningen av en 24-timmarsklocka. | `, - * /` |
| Dag i månaden | 1-31 | Du kan inte ange ett numeriskt värde för både&quot;dag i månaden&quot; och&quot;dag i veckan&quot;. Ett av dessa fält måste ha en `?` jokertecken. | `, - * / ? L C` |
| Månad | 1-12 eller jan, feb, mar, apr, maj, jun, jul, aug, sep, sep, okt, nov, dec | Värdena är skiftlägeskänsliga. | `, - * /` |
| Veckodag | Mån, Tue, Wed, Thu, Fri, Sat, Sun | Värdena är skiftlägeskänsliga. Du kan inte ange ett numeriskt värde för både&quot;dag i månaden&quot; och&quot;dag i veckan&quot;. Ett av dessa fält måste ha en `?` jokertecken. | `, - * / ? L C #` |
| År (valfritt) | Tom eller 1970-2099 |  | `, - * /` |


I den här tabellen beskrivs de jokertecken som är tillåtna i rutan Regel och hur du använder dem:

| Jokertecken | Namn | Vad det beskriver |
| --- | --- | --- |
| `*` | Asterisk | Alla värden (till exempel &quot;varje minut&quot;). |
| `?` | Frågetecken | Inget specifikt värde (till exempel &quot;någon minut inom den angivna timmen&quot;). |
| `,` | Komma | Andra värden (till exempel &quot;Måndag och onsdag&quot;). |
| `-` | Bindestreck | Värdeintervall (t.ex. &quot;Måndag till fredag&quot;). |
| `/` | Snedstreck | Ökningar (t.ex. &quot;var 15:e minut&quot;). |
| `L` | Versalt L | Sista&quot;dag i månaden&quot; eller&quot;veckodag&quot; (endast tillgängligt för dessa fält). Om månaden till exempel är januari, schemaläggs jobbet till den 31 januari med ett L-värde för fältet &quot;dag i månaden&quot;. I fältet Veckodag kan du ange det här tecknet enbart för att schemalägga jobbet på lördag. Du kan använda den med ett tal (till exempel `6L`) för att ange sista fredagen i månaden. Ange inte `L` med kommatecken eller bindestreck. |
| `#` | Nummertecken | &quot;Nth&quot; veckodag i månaden (endast tillgängligt för fältet &quot;day of the week&quot;). Till exempel: `6#3` i fältet &quot;veckodag&quot; anger den tredje fredagen i månaden. The `6` betecknar &quot;fredag&quot; (den sjätte dagen i veckan) och `3` Anger den tredje förekomsten i månaden. |
| `C` | # Versalt C | Första kalendern &quot;dag i månaden&quot; eller &quot;veckodag&quot; (endast tillgängligt för dessa fält). Ange till exempel värdet `1C` för &quot;dag i månaden&quot; schemaläggs den första dagen i kalendern som infaller den femte eller senare. För veckodagen anger du `1C` schemalägger den första dagen i kalendern som inträffar på eller efter söndag. |

Den här listan innehåller exempel på hur du beskriver tidsintervall i rutan Regel:

* `0 0 12 * * ?` : Ingen varje dag
* `0 15 10 ? * *` : 10.15 varje dag
* `0 0/5 14 * * ?`: Var femte minut mellan kl. 2:55 varje dag
* `0 0/5 14,18 * * ?` : Var femte minut mellan kl. 2:55 varje dag och var femte minut mellan kl. 6:00 och kl. 6:55 varje dag
* `0 10,44 14 ? 3` : ons kl. 2:10 och kl. 2:44 varje onsdag i mars
* `0 15 10 ? *` : mån-fre kl. 10.15 varje veckodag
* `0 15 10 20 * ?` : Klockan 10.15 den 20 varje månad
* `0 15 10 L * ?` : Klockan 10.15 den sista dagen i varje månad
* `0 15 10 ? * 6L` : Kl. 10.15 sista fredagen varje månad
* `0 15 10 * * 6#3` : Klockan 10.15 den tredje fredagen varje månad

## Använd ett överförings- eller publiceringsjobb som utlösare {#using-an-upload-or-publish-job-as-a-trigger}

När du överför resurser via FTP eller kör ett publiceringsjobb, kan du schemalägga ett efterföljande jobb att börja när överföringen är klar. (Om andra jobb är schemalagda att starta, köas jobbet som du schemalägger här bakom dem.) Det nya jobbet skickar ett meddelande till den adress som du anger så att koden på den platsen kan utlösas. Detta uppföljningsjobb får samma namn som det aktuella överföringsjobbet, men med prefixet _Pub.

Om du vill att ett överförings- eller publiceringsjobb ska utlösa ett annat jobb väljer du **[!UICONTROL Advanced]** på sidan Överför eller Publicera. Ange sedan URL:en i textfältet HTTP-meddelande.
