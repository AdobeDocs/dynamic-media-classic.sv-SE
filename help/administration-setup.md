---
title: Administrationsinställningar
description: Lär dig hur du ställer in administrationsdelen av Adobe Dynamic Media Classic.
uuid: 16ba9fed-b5c6-4991-83b3-8d7d7129013a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 3c9ee4ec-dd37-498d-98d6-1339b80177ff
feature: Dynamic Media Classic
role: Admin
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1845'
ht-degree: 0%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# Administrationsinställningar{#administration-setup}

Skärmerna Administrationsinstallationer används för att administrera Adobe Dynamic Media Classic-användare. Använd dessa skärmar för att göra det möjligt för användare att arbeta i Adobe Dynamic Media Classic och kommunicera via e-post med användare.

1. Gå till Administrationsinställningar **Inställningar** > **Personliga inställningar** > **Administrationsinställningar**.

## Användaradministration {#user-administration}

Alla Adobe Dynamic Media Classic-användare tilldelas en roll som avgör vilka behörigheter de har och vilka rättigheter de har för funktioner i Adobe Dynamic Media Classic. Administratörerna bestämmer vilka roller och ansvarsområden de har för de företag de är tilldelade.

Vanligtvis konfigurerar Adobe Dynamic Media Classic den första uppsättningen företag och tilldelar en företagsadministratör. Företagsadministratören ställer sedan in och administrerar Adobe Dynamic Media Classic-användare.

Adobe Dynamic Media Classic har stöd för flera användarroller. De här rollerna har åtkomst till företag som har konfigurerats för Adobe Dynamic Media Classic:

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Adobe Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe Dynamic Media Classic-användare** kan få tillgång till företag som de har tilldelats, kan inte utföra några administrativa uppgifter.

**Adobe Dynamic Media Classic företagsadministratör** Kan visa och administrera endast sina egna företag. En företagsadministratör kan också utföra alla administrationsfunktioner, inklusive att lägga till administratörer och användare. En företagsadministratör kan lägga till en användare i DMC-företagets administratörskonton. (Den här rollen är standardanvändarrollen.)

När du har lagt till en användare skickar Adobe Dynamic Media Classic ett välkomstmeddelande till användaren. Meddelandet innehåller ett lösenord och Adobe Dynamic Media Classic URL.

### Lägga till en användare eller administratör {#adding-a-user-or-administrator}

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Välj **[!UICONTROL Add]**.
1. Ange namn och e-postadress för den användare eller administratör som du vill lägga till och välj sedan **[!UICONTROL Next]**.

   >[!NOTE]
   >
   >apostrofen (`‘`) tillåts inte i e-postadresser.

1. Om du vill tilldela användaren en roll väljer du ett rollalternativ.

   Se [Adobe Dynamic Media Classic användarroller och -behörigheter](administration-setup.md#user_administration).

1. Om du vill lägga till en användare till ett företag väljer du ett företagsnamn.
1. Om du vill lägga till användaren i en grupp (om du lägger till en Media Portal-användare eller -medarbetare) väljer du **[!UICONTROL Next]** och lägga till användaren.
1. Välj **[!UICONTROL Save]** för att slutföra användarinställningarna.

   När du har sparat en fråga om du vill lägga till en användare i ett annat företag. Välj **[!UICONTROL Add]** om du vill lägga till användaren i ett företag.

   Alla nya användare får ett slumpmässigt genererat lösenord. -användare måste ändra lösenord första gången de loggar in på Adobe Dynamic Media Classic-datorprogrammet.

   Nya användare får ett välkomstmeddelande när du har lagt till dem. I e-postmeddelandet finns ett tillfälligt lösenord och information om hur du loggar in på Adobe Dynamic Media Classic.

   Om användaren inte får välkomstmeddelandet kan du be dem gå till inloggningssidan för Adobe Dynamic Media Classic (https://s7sps1.scene7.com) och välja **[!UICONTROL Forgot My Password]**. Lösenordet återställs och ett nytt e-postmeddelande skickas. Om användaren inte får e-postmeddelandet och inte finns i sin skräppostmapp kontaktar du teknisk support.

   När du lägger till nya Media Portal-användare kan du även gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL User Administration]** väljer **[!UICONTROL Upload User List]** och väljer en CSV-fil som inte innehåller fler än 500 användare.

### Ta bort en användare {#deleting-a-user}

Du kan ta bort användare från Adobe Dynamic Media Classic genom att göra dem ogiltiga. Ogiltiga användare tas bort från systemet och alla konton.

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Välj en användare i listan och välj sedan **[!UICONTROL Edit]**.
1. Avmarkera Giltig.
1. Välj **[!UICONTROL Save]**.

### Aktivera eller inaktivera användare {#activating-or-deactivating-users}

Användare som har inaktiverats har inte längre behörighet att ange kontot som visas högst upp på menyn Välj konton att komma åt.

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. I användarlistan markerar eller avmarkerar du **[!UICONTROL Active]** bredvid användarens namn.

### Redigera användarinformation {#editing-user-information}

Vilken användarinformation du kan redigera beror på din roll som administratör och den tilldelade rollen för den användare vars information du vill redigera. Alternativ som är nedtonade (inte tillgängliga) går inte att redigera.

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Välj en användare i listan och välj sedan **[!UICONTROL Edit]**.
1. Markera den post i tabellen som visar det företag du försöker ändra behörigheter eller åtkomst för och välj sedan **[!UICONTROL Manage Company]**.
1. Välj användarroll.
1. Om du vill ändra användarens gruppmedlemskap (om du redigerar eller lägger till en Media Portal-användare eller -medarbetare) väljer du **[!UICONTROL Next]** och redigera gruppmedlemskapet.
1. Välj **[!UICONTROL Save]**.

### Filtrera och sortera användarlistan {#filtering-and-sorting-the-user-list}

Du kan filtrera och sortera användarlistan för att hitta användare. Alla användare på alla konton som du administrerar visas i listan Användare, oavsett vilket konto som valts på menyn Välj konto för åtkomst.

Du kan använda följande tekniker för filtrering av användarlistor:

* **Filtrera efter grupp** - Välj **[!UICONTROL By Group]** och välj ett alternativ för att begränsa listan till användare i en grupp.

* **Filtrera efter användarroll** - Välj **[!UICONTROL By User Role]** och välj ett alternativ som begränsar listan till användare eller administratörer av olika typer.

* **Filtrera efter fältnamn** - Välj **[!UICONTROL Enable Filter By Field]**. Välj sedan **[!UICONTROL By Field Name]** väljer du en kolumn för filtrering av listan, väljer menyn Filtertecken och väljer en bokstav. Listan filtreras på en av kolumnerna med den bokstav du väljer. Om du vill se hela listan avmarkerar du **[!UICONTROL Enable Filter By Field]** alternativ.

* **Filtrera bort ogiltiga användare** - Avmarkera **[!UICONTROL Include Invalid]**. Sökresultaten visar endast användare som finns i systemet. Ogiltiga användare har tagits bort från systemet och de konton som du administrerar.

* **Sortera efter kolumnrubrik** - Välj en rubrik om du vill sortera alla användare efter status, i bokstavsordning efter förnamn, efternamn eller e-post, efter användarroll eller efter giltig/ogiltig status.

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

      Replace “N” in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## Bandbredd och lagring {#bandwidth-storage}

Adobe Dynamic Media Classic-administratörer kan generera bandbredd, lagring och andra typer av rapporter för de företag de administrerar. Rapporterna finns på sidan Bandbredd och lagring.

Öppna den här sidan genom att gå till **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**. Expandera **[!UICONTROL Administration Setup]** och sedan markera **[!UICONTROL Bandwidth & Storage]**.

### Typ av rapporter {#types-of-reports}

I följande tabell beskrivs rapporter som du kan generera från sidan Bandbredd och lagring:

| Rapport | Information | Använd |
|:--- |:--- |:--- |
| Bandbredd | Bandbreddsanvändning | Spåra bandbreddsanvändning per företag över specifika datumintervall för att fastställa trafikmönster. |
| Lagring | Lagringsanvändning | Spåra mängden data som överförts av företaget. |
| Bildinnehåll | Antalet bildbegäranden per typ | Spåra antalet begäranden och volymer för olika bildtyper. |
| Domän | Antalet URL-begäranden per domän | Spåra bildanvändningen baserat på domänen för bildbegäran för ett visst företag. (Adobe Dynamic Media Classic kan tillhandahålla mer än en domän per konto. Kontakta teknisk support om du vill ha mer information.) |
| Videoströmning | Bandbreddsanvändning för direktuppspelad video | Spåra direktuppspelad videoanvändning efter företag över vissa datumintervall för att fastställa trafikmönster. |
| Videoinnehåll | Spela upp tid för olika videoklipp | Avgör vilka som är de mest visade och minst visade videoklippen. |

Rapporten Bildinnehåll innehåller information om begäranden för följande bildtyper:

* **Bildbegäran** - Begäranden om bilder.

* **Begäran om miniatyrbild** - Begär färgrutor eller alternativa bilder i visningsprogram.

* **Maskbegäran** - Förfrågningar till bilder som returnerar gråskalemasker.

* **Begäran om visningsruta** - Bildbegäranden som läses in av ett visningsprogram.

* **Förfrågan om värdeobjekt** - Begäran om bildåtergivning som returnerar en bild med angivna objekt i de begärda vinjetteringarna.

* **Förfrågan om värdeinformation** - Begäran om bildåtergivning som returnerar information om begärda vinjetter.

>[!NOTE]
>
>Videoströmningsrapporten gäller endast direktuppspelade videor. Visningen av progressiva videor spåras inte.

### Generera en rapport {#generating-a-report}

Så här genererar du en rapport över bandbredd, lagring, bildinnehåll, domän, videoströmning eller videoinnehåll:

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.
1. Expandera Administrationsinställningar och välj sedan **[!UICONTROL Bandwidth & Storage]**.
1. Välj en flik: **[!UICONTROL Bandwidth]**, **[!UICONTROL Storage]**, **[!UICONTROL Image Content]**, **[!UICONTROL Domain]**, **[!UICONTROL Video Streaming]**, eller **[!UICONTROL Video Content]**.

   Se [Typ av rapporter](administration-setup.md#types_of_reports).

### Visa data på olika sätt {#viewing-data-in-different-ways}

När du har genererat en rapport på sidan Bandbredd och lagring kan du välja alternativ för att visa information. Du kan välja hur informationen ska visas, visa information i ett diagram eller datarutnät och ange en tidsperiod för att hämta information. I datavyn kan du även sortera information och ordna om kolumner.

* **Visa data i ett diagram eller datarutnät** - Välj **[!UICONTROL Chart View]** för att se data i ett diagram, välj **[!UICONTROL Data View]** för att visa data i ett datarutnät.

* **Välj en rapportpresentationstyp** - Välj **[!UICONTROL Summary]**, **[!UICONTROL Daily]**, eller **[!UICONTROL Monthly]** för att organisera data i sammanfattningsform, per dag eller per månad. Det här alternativet finns inte i alla rapporter.

* **Ange en tidsperiod** - Välj alternativ för att definiera en tidsperiod för rapporten och välj sedan **[!UICONTROL Update]** efter att du har definierat en tidsperiod:

* **Fördefinierad tidsperiod** - Välj ett alternativ på menyn Fördefinierad rapport. Välj till exempel Sista månaden för att hämta data från föregående månad.

* **Anpassad tidsperiod** - På menyn Fördefinierad rapport väljer du **[!UICONTROL Custom]**. Välj sedan ett datum på **[!UICONTROL Start Month]** (eller **[!UICONTROL Start Date]**) och ett datum på menyn # of Months (eller # or Days). I Domän- och videoinnehållsrapporter kan du välja ett specifikt start- och slutdatum för att hämta rapportinformation.

* **Sortera data (endast datavyn)** - Om du vill sortera information i en kolumn markerar du kolumnens rubrik. Välj igen om du vill sortera i fallande ordning.

* **Ordna om kolumner (endast datavyn)** - Om du vill flytta en kolumn till en annan plats i datarutnätet drar du i rubriken.

### Exportera och skriv ut rapporter {#exporting-and-printing-reports}

När du har genererat en rapport kan du exportera dess data för användning i kalkylblad och andra program. Du kan också skriva ut rapporter.

* **Exportera rapportdata** - Sortera och ordna data efter behov i datavyn. Öppna sedan **[!UICONTROL Export]** och välj ett format: **[!UICONTROL Tab Delimited]**, **[!UICONTROL Comma Separated]**, eller **[!UICONTROL HTML Formatted]**. Data kopieras till Urklipp i det format du väljer. Nu kan du klistra in data i ett kalkylblad eller program.

* **Skriva ut en rapport** - Välj **[!UICONTROL Print]** väljer du önskade alternativ i dialogrutan Skriv ut och väljer sedan **[!UICONTROL OK]**.

## Bildfel {#image-errors}

Adobe Dynamic Media Classic-administratörer kan generera bildfelsrapporter. En bildfelsrapport innehåller en lista med de 20 vanligaste bildfelen för det företag du är inloggad på under de senaste 24 timmarna. Så här genererar du en bildfelsrapport:

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.
1. Expandera Administrationsinställningar och välj sedan **[!UICONTROL Image Errors]**.
1. (Valfritt) Gör något av följande:

   * Om du vill sortera fel efter rubrikinformationen väljer du en rubrik. Som standard sorteras fel efter antal förekomster, från högst till lägst.
   * Flytta markören över svarsfältet för att se det specifika felmeddelandet.
   * Om du vill se länken till bildens eller hänvisarens webbsida för du markören över URL-fältet eller referensfältet.
   * Om du vill kopiera länken till den faktiska bilden väljer du **[!UICONTROL URL Copy URL]**. Du kan klistra in länken i ett webbläsarfönster för att gå till bilden och undersöka felet.
   * Om du vill kopiera länken till referenswebbsidan väljer du **[!UICONTROL Referrer Copy URL]**.

De fel som visas gäller det företag som du är inloggad på. Varje fel innehåller följande information:

* **Bild-ID** - ID för den felaktiga bilden.

* **Tid** - Tidsintervallet för den första gången som felet rapporterades till den senaste gången felet rapporterades, under de senaste 24 timmarna.

* **Antal** - Antalet fel som rapporterats i bilden.

* **Svar** - Det specifika felmeddelandet. Fel är antingen 4xx eller 5xx.

* **URL:er** - Visar URL:en till bilden på Adobe Dynamic Media Classic.

* **Referent** - Anger URL:en för den webbplats som den ursprungliga begäran kom från. Referenten kan vara vilken webbplats som helst som har en länk till bilden.

URL- och referenskolumnerna har en associerad Kopiera-URL för att förenkla testningen.
