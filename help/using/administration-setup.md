---
title: Administrationsinställningar
description: Lär dig hur du ställer in administrationsdelen av Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
topic: Administration
level: Intermediate
source-git-commit: 5482f442b067fd4911a05351e88c5be130c0b76d
workflow-type: tm+mt
source-wordcount: '1850'
ht-degree: 0%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# Administrationsinställningar{#administration-setup}

Skärmerna Administrationsinstallationer används för att administrera Adobe Dynamic Media Classic-användare. Använd dessa skärmar för att göra det möjligt för användare att arbeta i Adobe Dynamic Media Classic och kommunicera via e-post med andra användare.

1. Gå till **Inställningar** > **Personliga inställningar** > **Administrationsinställningar** om du vill visa alternativen för administrationsinställningar.

## Användaradministration {#user-administration}

Alla Adobe Dynamic Media Classic-användare tilldelas en roll som avgör vilka behörigheter de har och vilka rättigheter de har för funktioner i Adobe Dynamic Media Classic. Administratörerna bestämmer vilka roller och ansvarsområden de har för de företag de är tilldelade.

Vanligtvis konfigurerar Adobe Dynamic Media Classic den första uppsättningen företag och tilldelar en företagsadministratör. Företagsadministratören konfigurerar och administrerar sedan Adobe Dynamic Media Classic-användare.

Adobe Dynamic Media Classic har stöd för flera användarroller. De här rollerna har åtkomst till företag som har konfigurerats för Adobe Dynamic Media Classic:

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Adobe Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe Dynamic Media Classic-användare** Kan komma åt företag som de har tilldelats. Det går inte att utföra några administrativa åtgärder.

**Adobe Dynamic Media Classic företagsadministratör** Kan endast visa och administrera egna företag. En företagsadministratör kan också utföra alla administrationsfunktioner, inklusive att lägga till administratörer och användare. En företagsadministratör kan lägga till en användare i DMC-företagets administratörskonton. (Den här rollen är standardanvändarrollen.)

När du har lagt till en användare skickar Adobe Dynamic Media Classic ett välkomstmeddelande till användaren. Meddelandet innehåller ett lösenord och Adobe Dynamic Media Classic URL.

### Lägga till en användare eller administratör {#adding-a-user-or-administrator}

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Välj **[!UICONTROL Add]**.
1. Ange namn och e-postadress för den användare eller administratör som du vill lägga till och välj sedan **[!UICONTROL Next]**.

   >[!NOTE]
   >
   >Apostrofen (`'`) tillåts inte i e-postadresser.

1. Om du vill tilldela användaren en roll väljer du ett rollalternativ.

   Se [Adobe Dynamic Media Classic användarroller och behörigheter](administration-setup.md#user_administration).

1. Om du vill lägga till en användare till ett företag väljer du ett företagsnamn.
1. Om du vill lägga till användaren i en grupp (om du lägger till en Media Portal-användare eller -medarbetare) väljer du **[!UICONTROL Next]** och lägger till användaren.
1. Välj **[!UICONTROL Save]** för att slutföra användarkonfigurationen.

   När du har sparat en fråga om du vill lägga till en användare i ett annat företag. Välj **[!UICONTROL Add]** om du vill lägga till användaren i ett företag.

   Alla nya användare får ett slumpmässigt genererat lösenord. Användarna måste ändra lösenord första gången de loggar in på Adobe Dynamic Media Classic datorprogram.

   Nya användare får ett välkomstmeddelande när du har lagt till dem. I e-postmeddelandet finns ett tillfälligt lösenord och information om hur du loggar in på Adobe Dynamic Media Classic.

   Om användaren inte får välkomstmeddelandet ber du dem gå till Adobe Dynamic Media Classic inloggningssida (https://s7sps1.scene7.com) och välja **[!UICONTROL Forgot My Password]**. Lösenordet återställs och ett nytt e-postmeddelande skickas. Om användaren inte får e-postmeddelandet och inte finns i sin skräppostmapp kontaktar du teknisk support.

   När du lägger till nya Media Portal-användare kan du också gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL User Administration]**, markera **[!UICONTROL Upload User List]** och välja en CSV-fil som inte innehåller fler än 500 användare.

### Ta bort en användare {#delet-a-user}

Du kan ta bort användare från Adobe Dynamic Media Classic genom att göra dem ogiltiga. Ogiltiga användare tas bort från systemet och alla konton.

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Välj en användare i listan och välj sedan **[!UICONTROL Edit]**.
1. Avmarkera Giltig.
1. Välj **[!UICONTROL Save]**.

### Aktivera eller inaktivera användare {#activating-or-deactivating-users}

Användare som har inaktiverats har inte längre behörighet att ange kontot som visas högst upp på menyn Välj konton att komma åt.

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Markera eller avmarkera alternativet **[!UICONTROL Active]** bredvid användarens namn i användarlistan.

### Redigera användarinformation {#editing-user-information}

Vilken användarinformation du kan redigera beror på din roll som administratör och den tilldelade rollen för den användare vars information du vill redigera. Alternativ som är nedtonade (inte tillgängliga) går inte att redigera.

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Välj en användare i listan och välj sedan **[!UICONTROL Edit]**.
1. Markera den post i tabellen som visar det företag du försöker ändra behörigheter eller åtkomst för och välj sedan **[!UICONTROL Manage Company]**.
1. Välj användarroll.
1. Om du vill ändra användarens gruppmedlemskap (om du redigerar eller lägger till en Media Portal-användare eller -medarbetare) väljer du **[!UICONTROL Next]** och redigerar gruppmedlemskapet.
1. Välj **[!UICONTROL Save]**.

### Filtrera och sortera användarlistan {#filtering-and-sorting-the-user-list}

Du kan filtrera och sortera användarlistan för att hitta användare. Alla användare på alla konton som du administrerar visas i listan Användare, oavsett vilket konto som valts på menyn Välj konto för åtkomst.

Du kan använda följande tekniker för filtrering av användarlistor:

* **Filtrera efter grupp**: Välj menyn **[!UICONTROL By Group]** och välj ett alternativ för att begränsa listan till användare i en grupp.

* **Filtrera efter användarroll**: Välj menyn **[!UICONTROL By User Role]** och välj ett alternativ för att begränsa listan till användare eller administratörer av olika typer.

* **Filtrera efter fältnamn**: Välj **[!UICONTROL Enable Filter By Field]**. Välj sedan menyn **[!UICONTROL By Field Name]**, välj en kolumn för filtrering av listan, välj menyn Filtrera tecken och välj en bokstav. Listan filtreras på en av kolumnerna med den bokstav du väljer. Om du vill visa den fullständiga listan avmarkerar du alternativet **[!UICONTROL Enable Filter By Field]**.

* **Filtrera bort ogiltiga användare**: Avmarkera **[!UICONTROL Include Invalid]**. Sökresultaten visar endast användare som finns i systemet. Ogiltiga användare har tagits bort från systemet och de konton som du administrerar.

* **Sortera efter kolumnrubrik**: Välj en rubrik om du vill sortera alla användare efter status, i bokstavsordning efter förnamn, efternamn eller e-postadress. Eller sortera efter användarroll eller efter giltig/ogiltig status.

Om du har många användare kan du begränsa storleken på listan genom att välja menyn Maximal liststorlek och välja ett tal.

<!-- CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to an Adobe Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

You can link an Adobe IMS user identity to an Adobe Dynamic Media Classic IPS user account so you can use SSO (Single Sign On) to log on and launch Scene7 Publishing System from within Adobe Marketing Cloud.

1. Adobe should already have setup your account with an Adobe Marketing Cloud organization and linked it to your Scene7 Publishing System product context. If this setup is not yet done or you are unsure if it has been done, contact Adobe Customer Care.

   When the setup is complete, you can can log on to Adobe Marketing Cloud and link your Adobe Marketing Cloud identity to your Adobe Dynamic Media Classic user account by doing the following.

1. In Adobe Marketing Cloud, navigate to your account settings.
1. Select **Manage Organizations**.
1. Select **Link Account** or **Get Access**.
1. Select **Experience Manager**, and then type your credentials.

   Your credentials include your IPS company region, email address, and password.

1. Select **Link**.
1. When the link is set, you can launch Scene7 Publishing System from within Adobe Marketing Cloud, or you can launch it directly.

   Do one of the following:

    * To launch Adobe Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, select **Solutions** > **Experience Manager**. Under the Adobe Dynamic Media Classic card, select **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace "N" in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## Bandbredd och lagring {#bandwidth-storage}

Adobe Dynamic Media Classic-administratörer kan generera bandbredd, lagring och andra typer av rapporter för de företag de administrerar. Rapporterna finns på sidan Bandbredd och lagring.

Öppna den här sidan genom att gå till **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**. Expandera **[!UICONTROL Administration Setup]** och välj sedan **[!UICONTROL Bandwidth & Storage]**.

### Typ av rapporter {#types-of-reports}

I följande tabell beskrivs rapporter som du kan generera från sidan Bandbredd och lagring:

| Rapport | Information | Använd |
|:--- |:--- |:--- |
| Bandbredd | Bandbreddsanvändning av företag | Spåra bandbreddsanvändning per företag över specifika datumintervall för att fastställa trafikmönster. |
| Lagring | Lagringsanvändning | Spåra mängden data som överförts av företaget. |
| Bildinnehåll | Antalet bildbegäranden per typ | Spåra antalet begäranden och volymer för olika bildtyper. |
| Domän | Antalet URL-begäranden per domän | Spåra bildanvändningen baserat på domänen för bildbegäran för ett visst företag. (Adobe Dynamic Media Classic kan tillhandahålla mer än en domän per konto. Kontakta teknisk support om du vill ha mer information.) |
| Videoströmning | Bandbreddsanvändning för direktuppspelad video | Spåra direktuppspelad videoanvändning efter företag över vissa datumintervall för att fastställa trafikmönster. |
| Videoinnehåll | Spela upp olika videoklipp | Avgör vilka som är de mest visade och minst visade videoklippen. |

Rapporten Bildinnehåll innehåller information om begäranden för följande bildtyper:

* **Bildbegäran**: Begäran om bilder.

* **Miniatyrbildsbegäran**: Begäranden för färgruta eller alternativa bilder i visningsprogram.

* **Maskbegäran**: Förfrågningar om bilder som returnerar gråskalemasker.

* **Begäran om visningsprogrampanel**: Bildbegäranden som läses in av ett visningsprogram.

* **VNT-objektbegäran**: Bildåtergivningsbegäranden som returnerar en bild med angivna objekt i de begärda vinjetteringarna.

* **VNT-informationsbegäran**: Bildåtergivningsbegäranden som returnerar information om begärda vinjetter.

>[!NOTE]
>
>Videoströmningsrapporten gäller endast direktuppspelade videor. Det spårar inte visningen av progressiva videor.

### Generera en rapport {#generating-a-report}

Så här genererar du en rapport över bandbredd, lagring, bildinnehåll, domän, videoströmning eller videoinnehåll:

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.
1. Expandera Administrationsinställningar och välj sedan **[!UICONTROL Bandwidth & Storage]**.
1. Välj en flik: **[!UICONTROL Bandwidth]**, **[!UICONTROL Storage]**, **[!UICONTROL Image Content]**, **[!UICONTROL Domain]**, **[!UICONTROL Video Streaming]** eller **[!UICONTROL Video Content]**.

   Se [Typ av rapporter](administration-setup.md#types_of_reports).

### Visa data på olika sätt {#viewing-data-in-different-ways}

När du har genererat en rapport på sidan Bandbredd och lagring kan du välja alternativ för att visa information. Du kan välja hur informationen ska visas, visa information i ett diagram eller datarutnät och ange en tidsperiod för att hämta information. I datavyn kan du även sortera information och ordna om kolumner.

* **Visa data i ett diagram eller datarutnät**: Markera **[!UICONTROL Chart View]** om du vill visa data i ett diagram. Välj **[!UICONTROL Data View]** om du vill visa data i ett datarutnät.

* **Välj en rapportpresentationstyp**: På menyn Typ av rapport väljer du **[!UICONTROL Summary]**, **[!UICONTROL Daily]** eller **[!UICONTROL Monthly]** för att ordna data i sammanfattningsformat, per dag eller per månad. Det här alternativet finns inte i alla rapporter.

* **Ange en tidsperiod**: Välj alternativ för att definiera en tidsperiod för rapporten och välj sedan **[!UICONTROL Update]** efter att du har definierat en tidsperiod:

* **Fördefinierad tidsperiod**: Välj ett alternativ på menyn Fördefinierad rapport. Välj till exempel Sista månaden för att hämta data från föregående månad.

* **Anpassad tidsperiod**: Välj **[!UICONTROL Custom]** på menyn Fördefinierad rapport. Välj sedan ett datum på menyn **[!UICONTROL Start Month]** (eller **[!UICONTROL Start Date]**) och ett datum på menyn # av månader (eller # eller dagar). I Domän- och videoinnehållsrapporter kan du välja ett specifikt start- och slutdatum för att hämta rapportinformation.

* **Sortera data (endast datavyn)**: Sortera information i en kolumn. Markera kolumnrubriken. Välj igen om du vill sortera i fallande ordning.

* **Ordna om kolumner (endast datavyn)**: Dra rubriken om du vill flytta en kolumn till en annan plats i datarutnätet.

### Exportera och skriv ut rapporter {#exporting-and-printing-reports}

När du har genererat en rapport kan du exportera dess data för användning i kalkylblad och andra program. Du kan också skriva ut rapporter.

* **Exportera rapportdata**: Sortera och ordna data i datavyn efter behov. Öppna sedan menyn **[!UICONTROL Export]** och välj ett format: **[!UICONTROL Tab Delimited]**, **[!UICONTROL Comma Separated]** eller **[!UICONTROL HTML Formatted]**. Data kopieras till Urklipp i det format du väljer. Nu kan du klistra in data i ett kalkylblad eller program.

* **Skriv ut en rapport**: Välj **[!UICONTROL Print]**, välj önskade alternativ i dialogrutan Skriv ut och välj sedan **[!UICONTROL OK]**.

## Bildfel {#image-errors}

Adobe Dynamic Media Classic-administratörer kan generera bildfelsrapporter. En bildfelsrapport innehåller en lista med de 20 vanligaste bildfelen för det företag du är inloggad på under de senaste 24 timmarna. Så här genererar du en bildfelsrapport:

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.
1. Expandera Administrationsinställningar och välj sedan **[!UICONTROL Image Errors]**.
1. (Valfritt) Gör något av följande:

   * Om du vill sortera fel efter rubrikinformationen väljer du en rubrik. Som standard sorteras fel efter antal förekomster, från högst till lägst.
   * Flytta markören över svarsfältet för att se det specifika felmeddelandet.
   * Om du vill se länken till bilden eller referenswebbsidan för webbsidan, flyttar du markören över URL-fältet eller referensfältet.
   * Om du vill kopiera länken till den faktiska bilden väljer du **[!UICONTROL URL Copy URL]**. Du kan klistra in länken i ett webbläsarfönster för att gå till bilden och undersöka felet.
   * Om du vill kopiera länken till referenswebbsidan väljer du **[!UICONTROL Referrer Copy URL]**.

De fel som visas gäller det företag som du är inloggad på. Varje fel innehåller följande information:

* **Bild-ID**: ID för den felaktiga bilden.

* **Tid**: Tidsintervallet för den första gången som felet rapporterades till den senaste gången felet rapporterades, inom de senaste 24 timmarna.

* **Antal**: Antalet rapporterade fel i bilden.

* **Svar**: Det specifika felmeddelandet. Felen är antingen 4xx eller 5xx.

* **URL:er**: Visar URL:en till bilden på Adobe Dynamic Media Classic.

* **Referent**: Anger URL:en för den webbplats som den ursprungliga begäran kom från. Referenten kan vara vilken webbplats som helst som har en länk till bilden.

URL- och referenskolumnerna har en associerad Kopiera-URL för att förenkla testningen.
