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
source-git-commit: bb229047c0c9b3855453ea15dcd1f9754bc65cef
workflow-type: tm+mt
source-wordcount: '1562'
ht-degree: 0%

---

# Kontrollera jobbfiler{#checking-job-files}

Adobe Dynamic Media Classic erbjuder jobbsidan för att övervaka filöverföringar till Adobe Dynamic Media Classic och filer som du publicerar på Adobe Dynamic Media Classic-servrar. Du kan granska, överföra och publicera jobb på sidan Jobs, kontrollera status för jobb och avbryta publiceringsjobb från den här sidan. Du kan också schemalägga överförings- och publiceringsjobb.

När du överför resurser visas en snurrande ikon bredvid menyn Jobb, som anger att ett jobb pågår och hur många filer som bearbetas. Du kan markera ikonen om du vill visa mer information om det aktiva jobbet.

>[!NOTE]
>
>En lista över dina nyligen publicerade jobb finns också på sidan Senaste aktivitet. Välj **[!UICONTROL Recent]** i fältet Global navigering.

## Om sidan Jobb {#about-the-jobs-page}

Välj **[!UICONTROL Jobs]** i fältet Global navigering så att sidan Jobb öppnas. Som standard listas jobb med början från den senaste.

Jobb visas i följande kategorier på fliken Historik på sidan Jobb:

* **[!UICONTROL Job Type]**: En ikon anger jobbtypen: Överför och Publish är de vanligaste jobbtyperna.

* **[!UICONTROL Job Name]**: Jobbets namn. Namnet innehåller den användardefinierade delen av namnet samt datum och tid.

* **[!UICONTROL Started]**: När jobbet startades.

* **[!UICONTROL Total]**: Antalet överförda filer.

* **[!UICONTROL W (warnings)]**: Antalet varningar i jobbet (om sådana finns). Varningar indikerar problem med jobbet som inte påverkade det övergripande jobbslutförandet. Dessa varningar kan vanligtvis ignoreras eftersom de rapporterar om dolda filer. Till exempel innehåller `.DS_store` filer (Mac) och Thumbs.db-filer (Windows®) information om hur du visar bildfiler för användare. Varningsposter för dessa filer kan dock ignoreras eftersom de inte gäller hur dessa filer används i Adobe Dynamic Media Classic. Du kan dubbelklicka på ett jobbnamn för att få detaljerad information om varningar.

* **[!UICONTROL E (errors)]**: Visar antalet fel i jobbet (om sådana finns). Du kan dubbelklicka på ett jobbnamn för att få detaljerad information om fel.

* **[!UICONTROL Duration]**: Hur lång tid det tog att slutföra jobbet.

* **[!UICONTROL Status]**: Visar status för jobbet.

* **[!UICONTROL Destination]**: För överföringsjobb är målet företagets namn och mapp som filerna överfördes till. Den här kategorin gäller inte för jobb för publicering.

* **[!UICONTROL Submitted By]**: Listor som överförde resurserna.

>[!NOTE]
>
>Du kan avbryta pågående publicerings- och överföringsjobb genom att markera knappen **[!UICONTROL Cancel]** bredvid förloppsindikatorn.

## Ändra vyer på sidan Jobb {#changing-views-on-the-jobs-page}

Använd följande tekniker för att sortera jobb eller ändra vyn på fliken Historik på sidan Jobb:

* **[!UICONTROL Sorting]**: Välj ett kolumnnamn om du vill sortera listan efter en viss kolumn. Du kan välja växeln bredvid kolumnnamnet för att sortera i fallande eller stigande ordning.

* **[!UICONTROL Date Range]**: Välj menyn **[!UICONTROL Date Range]** och välj ett alternativ för att begränsa listan med jobb till aktuellt datum, föregående vecka eller föregående månad. Välj **[!UICONTROL Custom Date Range]** och ange sedan ett specifikt datumintervall.

* **[!UICONTROL Job Type]**: Välj menyn **[!UICONTROL Job Type]** och välj **[!UICONTROL Publish]** eller **[!UICONTROL Upload]** för att begränsa listan till publiceringsjobb eller överföringsjobb. Välj **[!UICONTROL All]** om du vill visa båda typerna av jobb.

* **[!UICONTROL Show]**: Gå till **[!UICONTROL Show]** > **[!UICONTROL My Jobs]** eller **[!UICONTROL Show]** > **[!UICONTROL All Jobs]** om du vill begränsa listan till jobb som du har beställt eller jobb som personer i ditt företag har beställt.

## Visa eller kopiera eller skriv ut en jobbdetaljrapport {#viewing-copying-or-printing-a-job-details-report}

Dubbelklicka på namnet på en rapport på jobbsidan så att sidan Jobbinformation öppnas. Den här sidan innehåller en sammanfattningsrapport om filerna i jobbet. Markera **[!UICONTROL View Detail]** så att du kan se en posts Adobe Dynamic Media Classic-ID, målsökväg och statusinformation. Om du har överfört en PDF- eller PostScript-fil som kräver teckensnitt som inte finns i Adobe Dynamic Media Classic visas en lista med de saknade teckensnitten i rapporten.

Du kan kopiera informationen till Urklipp.

1. Dubbelklicka på namnet på en rapport på sidan Jobs.
1. På sidan Jobbinformation väljer du **[!UICONTROL View Detail]** för att få en detaljerad rapport om en post.
1. Välj **[!UICONTROL Copy to Clipboard]**.

## Hantera återkommande överförings- och publiceringsjobb {#handling-recurring-upload-and-publish-jobs}

Återkommande överförings- och publiceringsjobb som du skapar på sidorna Överför och Publish visas på fliken Schemalagda på sidan Jobb. Du kan redigera och ta bort återkommande jobb på fliken Schemalagda.

Markera knappen Jobb i fältet Global navigering och välj fliken **[!UICONTROL Scheduled]** på sidan Jobb så att du kan redigera och ta bort återkommande jobb.

>[!NOTE]
>
>Du kan filtrera jobblistan på fliken **[!UICONTROL Scheduled]** med menyerna **[!UICONTROL Job Type]** och **[!UICONTROL Show]**. Välj en jobbtyp så att du kan begränsa listan till att publicera jobb av en viss typ. Välj ett **[!UICONTROL Show]**-alternativ så att du kan visa jobb som du har skapat eller jobb som har skapats av alla i ditt företag.

### Redigera, ta bort, pausa och återuppta återkommande jobb {#editing-deleting-pausing-and-resuming-recurring-jobs}

Välj ett återkommande jobb på sidan Jobb och följ dessa instruktioner om du vill redigera eller ta bort det:

* **Redigera ett återkommande jobb**: Markera knappen **[!UICONTROL Edit]** och ange schemainformation i dialogrutan Redigera schemalagt jobb. Om du vill att jobbet ska upprepas med valfritt intervall går du till **[!UICONTROL Repeat]** > **[!UICONTROL Custom]**.

Se [Skapa ett anpassat tidsintervall för överföring eller publiceringsjobb](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

* **Tar bort ett återkommande jobb**: Markera knappen **[!UICONTROL Delete]**.

* **Pausa (och återuppta) ett återkommande jobb**: Avmarkera en kryssruta i kolumnen Aktivt om du vill pausa ett jobb. Markera en kryssruta om du vill återuppta ett jobb som pausats.

### Skapa ett anpassat tidsintervall för överföring eller publiceringsjobb {#creating-a-custom-upload-or-publish-job-time-interval}

Om du vill skapa ett anpassat tidsintervall för en överföring (via FTP) eller ett publiceringsjobb går du till **[!UICONTROL Repeat]** > **[!UICONTROL Custom]** på sidan Överför eller Publish. Ange sedan siffror och jokertecken i rutan Regel som beskriver ett tidsintervall för överförings- eller publiceringsjobben som ska återkomma.

Syntaxen för att beskriva anpassade tidsintervall för överföring och publicering i rutan Regel är:

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

`0 15 10 * * ?` schemalägger till exempel ett jobb vid 10:15.00 varje dag.

I följande tabeller och listor beskrivs hur du beskriver ett tidsintervall i rutan Regel.

I den här tabellen visas tidsökningar, tillåtna värden och jokertecken som stöds:

| Tidsökningar | Tillåtna värden | Kommentar | Jokertecken stöds |
|--- |--- |--- |--- |
| Sekunder | 0-59 |  | `,: * /` |
| Minuter | 0-59 |  | `,: * /` |
| Timmar | 0-23 | Observera användningen av en 24-timmarsklocka. | `,: * /` |
| Dag i månaden | 1-31 | Du kan inte ange ett numeriskt värde för både&quot;dag i månaden&quot; och&quot;dag i veckan&quot;. Ett av dessa fält måste innehålla jokertecknet `?`. | `,: * / ? L C` |
| Månad | 1-12 eller jan, feb, mar, apr, maj, jun, jul, aug, sep, sep, okt, nov, dec | Värdena är skiftlägeskänsliga. | `,: * /` |
| Veckodag | Mån, Tue, Wed, Thu, Fri, Sat, Sun | Värdena är skiftlägeskänsliga. Du kan inte ange ett numeriskt värde för både&quot;dag i månaden&quot; och&quot;dag i veckan&quot;. Ett av dessa fält måste innehålla jokertecknet `?`. | `,: * / ? L C #` |
| År (valfritt) | Tom eller 1970-2099 |  | `,: * /` |


I den här tabellen beskrivs de jokertecken som är tillåtna i rutan Regel och hur du använder dem:

| Jokertecken | Namn | Vad det beskriver |
| --- | --- | --- |
| `*` | Asterisk | Alla värden (till exempel &quot;varje minut&quot;). |
| `?` | Frågetecken | Inget specifikt värde (till exempel &quot;någon minut inom den angivna timmen&quot;). |
| `,` | Komma | Andra värden (till exempel &quot;Måndag och onsdag&quot;). |
| `-` | Bindestreck | Värdeintervall (t.ex. &quot;Måndag till fredag&quot;). |
| `/` | Snedstreck | Ökningar (t.ex. &quot;var 15:e minut&quot;). |
| `L` | Versalt L | Sista&quot;dag i månaden&quot; eller&quot;veckodag&quot; (endast tillgängligt för dessa fält). Om månaden till exempel är januari, schemaläggs jobbet till den 31 januari med ett L-värde för fältet &quot;dag i månaden&quot;. I fältet Veckodag kan du ange det här tecknet enbart för att schemalägga jobbet på lördag. Du kan använda den med ett tal (till exempel `6L`) för att ange sista fredagen i månaden. Ange inte `L` med jokertecken för komma eller bindestreck. |
| `#` | Nummertecken | &quot;Nth&quot; veckodag i månaden (endast tillgängligt för fältet &quot;day of the week&quot;). Till exempel anger `6#3` i fältet &quot;veckodag&quot; den tredje fredagen i månaden. `6` betecknar &quot;fredag&quot; (den sjätte dagen i veckan) och `3` betecknar den tredje förekomsten i månaden. |
| `C` | # Versalt C | Första kalendern &quot;dag i månaden&quot; eller &quot;veckodag&quot; (endast tillgängligt för dessa fält). Om du till exempel anger värdet `1C` för &quot;dag i månaden&quot; schemaläggs den första dagen i kalendern som inträffar den femte eller senare. Om du anger `1C` för veckodagen schemaläggs den första dagen i kalendern som inträffar på eller efter söndag. |

Den här listan innehåller exempel på hur du beskriver tidsintervall i rutan Regel:

* `0 0 12 * * ?` : Ingen varje dag
* `0 15 10 ? * *` : 10:15 varje dag
* `0 0/5 14 * * ?`: Var femte minut mellan kl. 2:00 och kl. 2:55 varje dag
* `0 0/5 14,18 * * ?` : Var femte minut mellan kl. 2:00 och kl. 2:55 varje dag och var femte minut mellan kl. 6:00 och kl. 6:55 varje dag
* `0 10,44 14 ? 3` : ons kl. 2:10 och kl. 2:44 varje onsdag i mars
* `0 15 10 ? *` : mån-fre kl. 10.15 varje veckodag
* `0 15 10 20 * ?` : Klockan 10.15 den 20 i varje månad
* `0 15 10 L * ?` : Klockan 10:15 den sista dagen i varje månad
* `0 15 10 ? * 6L` : Klockan 10.15 den sista fredagen varje månad
* `0 15 10 * * 6#3` : Klockan 10.15 den tredje fredagen varje månad

## Använd ett överförings- eller publiceringsjobb som utlösare {#using-an-upload-or-publish-job-as-a-trigger}

När du överför resurser via FTP eller kör ett publiceringsjobb, kan du schemalägga ett efterföljande jobb att börja när överföringen är klar. (Om andra jobb är schemalagda att starta, köas jobbet som du schemalägger här bakom dem.) Det nya jobbet skickar ett meddelande till den adress som du anger så att koden på den platsen kan utlösas. Detta uppföljningsjobb får samma namn som det aktuella överföringsjobbet, men med prefixet _Pub.

Om du vill att ett överförings- eller publiceringsjobb ska utlösa ett annat jobb väljer du **[!UICONTROL Advanced]** på sidan Överför eller Publish. Ange sedan URL:en i textfältet HTTP-meddelande.
