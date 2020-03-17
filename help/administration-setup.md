---
title: Administrationsinställningar
seo-title: Administrationsinställningar
description: 'null'
seo-description: Lär dig hur du ställer in administrationsdelen för Dynamic Media Classic.
uuid: 16ba9fed-b5c6-4991-83b3-8d7d7129013a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
discoiquuid: 3c9ee4ec-dd37-498d-98d6-1339b80177ff
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Administrationsinställningar{#administration-setup}

Administrationsinstallationsskärmarna används för att administrera användare av Scene7 Publishing System. Använd dessa skärmar för att göra det möjligt för användare att arbeta i Scene7 Publishing System och kommunicera via e-post med användare.

1. Om du vill visa alternativen för administrationsinställningar klickar du på **Inställningar** > **Personliga inställningar** > **Administrationsinställningar**.

## Användaradministration {#user-administration}

Alla Dynamic Media Classic-användare tilldelas en roll som bestämmer deras behörigheter och åtkomsträttigheter till funktioner i Scene7 Publishing System. Administratörerna bestämmer vilka roller och ansvarsområden de har för de företag de är tilldelade.

Dynamic Media Classic konfigurerar vanligtvis den första uppsättningen företag och tilldelar en företagsadministratör. Företagsadministratören konfigurerar och administrerar sedan användare av Scene7 Publishing System.

Scene7 Publishing System har stöd för tre användarroller. Alla tre rollerna har åtkomst till företag som har konfigurerats för Scene7 Publishing System:

**SPS Administrator** Kan visa och administrera alla funktioner i Scene7 Publishing System, samt konfigurera företag och lägga till administratörer och användare.

**Företagsadministratör** Kan endast visa och administrera egna företag. En företagsadministratör kan också utföra alla administrationsfunktioner, inklusive att lägga till administratörer och användare. En företagsadministratör kan lägga till en användare i SPS-företagets administratörskonton. (Den här rollen är standardanvändarrollen.)

**SPS-användare** har tillgång till företag som de har tilldelats, kan inte utföra några administrativa uppgifter.

När du har lagt till en användare skickar Scene7 Publishing System ett välkomstmeddelande till användaren. Meddelandet innehåller ett lösenord och Scene7 Publishing System-URL:en.

### Lägga till en användare eller administratör {#adding-a-user-or-administrator}

1. Klicka på Inställningar > Programinställningar > Administrationsinställningar > Användaradministration.
1. Klicka på Lägg till.
1. Ange namn och e-postadress för den användare eller administratör som du vill lägga till och klicka sedan på Nästa.

   >[!NOTE]
   >
   >Apostrofen (&quot;) tillåts inte i e-postadresser.

1. Välj ett rollalternativ för att tilldela användaren en roll.

   Se [Dynamic Media Classic-användarroller och -behörigheter](administration-setup.md#user_administration).

1. Välj ett företagsnamn om du vill lägga till en användare i ett företag.
1. Om du vill lägga till användaren i en grupp (om du lägger till en Media Portal-användare eller -medarbetare) klickar du på Nästa och lägger till användaren.
1. Klicka på Spara för att slutföra användarinställningarna.

   När du har sparat en fråga om du vill lägga till en användare i ett annat företag. Klicka på Lägg till om du vill lägga till användaren i ett företag.

   Alla nya användare får ett slumpmässigt genererat lösenord. -användare måste ändra lösenord första gången de loggar in på Scene7 Publishing System.

   Nya användare får ett välkomstmeddelande när du har lagt till dem. E-postmeddelandet innehåller ett tillfälligt lösenord och förklarar hur du loggar in på Scene 7 Publishing System.

   Om användaren inte får välkomstmeddelandet ber du dem gå till SPS-inloggningssidan (https://s7sps1.scene7.com) och klicka på Har du glömt mitt lösenord. Lösenordet återställs och ett nytt e-postmeddelande skickas. Om användaren inte får e-postmeddelandet och inte finns i sin skräppostmapp kontaktar du teknisk support.

   När du lägger till nya Media Portal-användare kan du även gå till Inställningar > Programinställningar > Användaradministration, klicka på Överför användarlista och välja en CSV-fil som inte innehåller fler än 500 användare.

### Ta bort en användare {#deleting-a-user}

Du kan ta bort användare från Scene7 Publishing System genom att göra dem ogiltiga. Ogiltiga användare tas bort från systemet och alla konton.

1. Klicka på **Inställningar** > **Programinställningar** >**Administrationsinställningar** > **Användaradministration**.
1. Markera en användare i listan och klicka sedan på **Redigera**.
1. Avmarkera Giltig.
1. Klicka på **Spara**.

### Aktivera eller inaktivera användare {#activating-or-deactivating-users}

Användare som har inaktiverats har inte längre behörighet att ange kontot som visas högst upp på menyn Välj konton att komma åt.

1. Klicka på **Inställningar** > **Programinställningar** >**Administrationsinställningar** > **Användaradministration**.
1. Markera eller avmarkera alternativet Aktiv bredvid användarens namn i användarlistan.

### Redigera användarinformation {#editing-user-information}

Vilken användarinformation du kan redigera beror på din roll som administratör och den tilldelade rollen för den användare vars information du vill redigera. Alternativ som är nedtonade (inte tillgängliga) går inte att redigera.

1. Gå till **Inställningar** > **Programinställningar**>**Administrationsinställningar** > **Användaradministration**.
1. Markera användaren och klicka på **Redigera**.
1. Markera den post i tabellen som visar det företag du försöker ändra behörigheter eller åtkomst för och klicka sedan på länken Hantera företag.
1. Välj användarroll.
1. Om du vill ändra användarens gruppmedlemskap (om du redigerar eller lägger till en Media Portal-användare eller -medarbetare) klickar du på Nästa och redigerar gruppmedlemskapet.
1. Klicka på **Spara**.

### Filtrera och sortera användarlistan {#filtering-and-sorting-the-user-list}

Du kan filtrera och sortera användarlistan för att hitta användare. Alla användare på alla konton som du administrerar visas i listan Användare, oavsett vilket konto som valts på menyn Välj konto för åtkomst.

Du kan använda följande filtertekniker för användarlistor:

**Filtrera efter grupp** Välj menyn Efter grupp och välj ett alternativ för att begränsa listan till användare i en grupp.

**Filtrera efter användarroll** Välj menyn Efter användarroll och välj ett alternativ för att begränsa listan till användare eller administratörer av olika typer.

**Filtrera efter fältnamn** Välj alternativet Aktivera filter efter fält. Välj sedan menyn Efter fältnamn, välj en kolumn för filtrering av listan, välj menyn Filtertecken och välj en bokstav. Listan filtreras på en av kolumnerna med den bokstav du väljer. Avmarkera alternativet Aktivera filter efter fält för att se hela listan.

**Filtrera bort ogiltiga användare** Avmarkera alternativet Inkludera ogiltiga. Sökresultaten visar endast användare som finns i systemet. Ogiltiga användare har tagits bort från systemet och de konton du administrerar.

**Sortera efter kolumnrubrik** Klicka på en rubrik om du vill sortera alla användare efter status, i bokstavsordning efter förnamn, efternamn eller e-post, efter användarroll eller efter giltig/ogiltig status.

Om du har många användare kan du begränsa storleken på listan genom att välja menyn Maximal liststorlek och välja ett tal.

### Länka en IMS-användaridentitet till ett Dynamic Media Classic IPS-användarkonto {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

Du kan länka en Adobe IMS-användaridentitet till ett Dynamic Media Classic IPS-användarkonto så att du kan använda enkel inloggning (Single Sign On) för att logga in och starta Scene7 Publishing System inifrån Adobe Marketing Cloud.

1. Adobe bör redan ha konfigurerat ditt konto hos en Adobe Marketing Cloud-organisation och länkat det till produktsammanhanget för Scene7 Publishing System. Om installationen inte är klar än eller om du är osäker på om den är klar kontaktar du Adobes kundtjänst.

   När konfigurationen är klar kan du logga in på Adobe Marketing Cloud och länka din Adobe Marketing Cloud-identitet till ditt Dynamic Media Classic-användarkonto genom att göra följande.

1. Navigera till dina kontoinställningar i Adobe Marketing Cloud.
1. Klicka på **Hantera organisationer**.
1. Klicka på **Länka konto** eller **Få åtkomst**.
1. Välj **Experience Manager** och ange dina autentiseringsuppgifter.

   Dina autentiseringsuppgifter inkluderar din region för IPS-företaget, e-postadress och lösenord.

1. Klicka på **Länka**.
1. När länken är angiven kan du starta Scene7 Publishing System inifrån Adobe Marketing Cloud eller starta det direkt.

   Gör något av följande:

   * Om du vill starta Dynamic Media Classic inifrån Adobe Marketing Cloud klickar du på **Lösningar** > **Experience Manager** till vänster i Adobe Marketing Cloud. Klicka på **Starta** under Dynamic Media Classic-kortet.
   * Om du vill logga in på Scene7 Publishing System direkt med dina IMS-inloggningsuppgifter använder du följande webbplats:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Ersätt&quot;N&quot; i ovanstående sökväg med numret för IPS-företagsregionen. Det vill säga N = 1 för Nordamerika, 3 för EMEA, eller 5 för JAPAC.

## Bandbredd och lagring {#bandwidth-storage}

SPS-administratörer kan generera bandbredd, lagring och andra typer av rapporter för de företag de administrerar. Rapporterna är tillgängliga på skärmen Bandbredd och lagring.

Om du vill öppna den här skärmen klickar du på Inställningar > Personliga inställningar. Expandera Administrationsinställningar och klicka sedan på Bandbredd och lagring.

### Typ av rapporter {#types-of-reports}

I följande tabell beskrivs rapporter som du kan generera från skärmen Bandbredd och lagring:

| Rapport | Information | Använd |
|:--- |:--- |:--- |
| Bandbredd | Bandbreddsanvändning | Spåra bandbreddsanvändning per företag över specifika datumintervall för att fastställa trafikmönster. |
| Lagring | Lagringsanvändning | Spåra mängden data som överförts av företaget. |
| Bildinnehåll | Antalet bildbegäranden per typ | Spåra antalet begäranden och volymer för olika bildtyper. |
| Domän | Antalet URL-begäranden per domän | Spåra bildanvändningen baserat på domänen för bildbegäran för ett visst företag. (Dynamic Media Classic kan tillhandahålla mer än en domän per konto. Kontakta teknisk support om du vill ha mer information.) |
| Videoströmning | Bandbreddsanvändning för direktuppspelad video | Spåra direktuppspelad videoanvändning efter företag över vissa datumintervall för att fastställa trafikmönster. |
| Videoinnehåll | Spela upp tid för olika videoklipp | Avgör vilka som är de mest visade och minst visade videoklippen. |


Rapporten Bildinnehåll innehåller information om begäranden för följande bildtyper:

**Begäran** om avbildningar.

**Begär** miniatyrbilder för att begära färgrutor eller alternativa bilder i visningsprogram.

**Maskbegäran** begär bilder som returnerar gråskalemasker.

**Bildbegäranden** för visningsprogrammets panel läses in av ett visningsprogram.

**Förfrågningar om bildåtergivning från Vnt-objekt** som returnerar en bild med angivna objekt i de begärda vinjetteringarna.

**Vnt Info begär** bildåtergivning som returnerar information om de begärda vinjetterna.

>[!NOTE]
>
>Videoströmningsrapporten gäller endast direktuppspelade videor. Visningen av progressiva videor spåras inte.

### Generera en rapport {#generating-a-report}

Så här genererar du en rapport över bandbredd, lagring, bildinnehåll, domän, videoströmning eller videoinnehåll:

1. Välj Inställningar > Personliga inställningar.
1. Expandera Administrationsinställningar och klicka sedan på Bandbredd och lagring.
1. Klicka på en flik: Bandbredd, lagring, bildinnehåll, domän, videoströmning eller videoinnehåll.

   Se [Rapporttyper](administration-setup.md#types_of_reports).

### Visa data på olika sätt {#viewing-data-in-different-ways}

När du har genererat en rapport på sidan Bandbredd och lagring kan du välja alternativ för att visa information. Du kan välja hur informationen ska visas, visa information i ett diagram eller datarutnät och ange en tidsperiod för att hämta information. I datavyn kan du även sortera information och ordna om kolumner.

**Visa data i ett diagram eller datarutnät** Klicka på alternativet Diagramvy om du vill visa data i ett diagram. Klicka på alternativet Datavy om du vill visa data i ett datarutnät.

**Välj en rapportpresentationstyp** På menyn Typ av rapport väljer du Sammanfattning, Dagligen eller Månad för att ordna data i sammanfattningsform, per dag eller per månad. Det här alternativet finns inte i alla rapporter.

**Ange en tidsperiod** Välj alternativ för att definiera en tidsperiod för rapporten och klicka sedan på Uppdatera när du har definierat en tidsperiod:

**Fördefinierad tidsperiod** Välj ett alternativ på menyn Fördefinierad rapport. Välj till exempel Sista månaden för att hämta data från föregående månad.

**Anpassad tidsperiod** Välj Anpassad på menyn Fördefinierad rapport. Välj sedan ett datum på menyn Startmånad (eller Startdatum) och ett datum på menyn # av månader (eller # eller Dagar). I Domän- och videoinnehållsrapporter kan du välja ett specifikt start- och slutdatum för att hämta rapportinformation.

**Sortera data (endast datavyn)** Om du vill sortera information i en kolumn klickar du på kolumnens rubrik. Klicka igen om du vill sortera i fallande ordning.

**Ordna om kolumner (endast datavyn)** Om du vill flytta en kolumn till en annan plats i datarutnätet drar du rubriken.

### Exportera och skriva ut rapporter {#exporting-and-printing-reports}

När du har genererat en rapport kan du exportera dess data för användning i kalkylblad och andra program. Du kan också skriva ut rapporter.

**Exportera rapportdata** Sortera och ordna data i datavyn efter behov. Öppna sedan menyn Exportera och välj ett format: Tabbavgränsad, kommaseparerad eller HTML-formaterad. Data kopieras till Urklipp i det format du väljer. Nu kan du klistra in data i ett kalkylblad eller program.

**Skriva ut en rapport** Klicka på Skriv ut, välj önskade alternativ i dialogrutan Skriv ut och klicka sedan på OK.

## Bildfel {#image-errors}

SPS-administratörer kan generera bildfelsrapporter. En bildfelsrapport innehåller en lista med de 20 vanligaste bildfelen för det företag du är inloggad på under de senaste 24 timmarna. Följ de här stegen för att generera en bildfelsrapport:

1. Klicka på Inställningar > Personliga inställningar.
1. Expandera Administrationsinställningar och klicka sedan på Bildfel.
1. (Valfritt) Gör något av följande:

   * Klicka på en rubrik om du vill sortera fel efter rubrikinformationen. Som standard sorteras fel efter antal förekomster, från högst till lägst.
   * Flytta markören över svarsfältet för att se det specifika felmeddelandet.
   * Flytta markören över URL-fältet eller referensfältet för att se länken till bilden eller referenswebbsidan.
   * Klicka på URL-kopieringens URL för att kopiera länken till den faktiska bilden. Du kan klistra in länken i ett webbläsarfönster för att gå till bilden och undersöka felet.
   * Klicka på URL för refererarkopia för att kopiera länken till referenswebbsidan.

De fel som visas gäller det företag du är inloggad på. Varje fel innehåller följande information:

**Bild-ID** för den felaktiga bilden.

**Tid** Tidsintervallet för den första gången som felet rapporterades till den senaste gången felet rapporterades, under de senaste 24 timmarna.

**Antal** fel som rapporterats i bilden.

**Svar** Det specifika felmeddelandet. Fel är antingen 4xx eller 5xx.

**URL:er** Visar URL:en till bilden på Scen 7.

**Referent** Anger URL:en för den webbplats som den ursprungliga begäran kom från. Referenten kan vara vilken webbplats som helst som har en länk till bilden.

URL- och referenskolumnerna har en associerad Kopiera-URL för att förenkla testningen.
