---
title: Personliga inställningar
description: Alla användare kan ändra inställningarna på skärmen Personliga inställningar i Dynamic Media Classic.
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 1%

---


# Personliga inställningar {#personal-setup}

Alla användare kan ändra inställningarna på skärmen Personliga inställningar. Du öppnar skärmen Personliga inställningar genom att klicka på Inställningar > Personliga inställningar.

>[!NOTE]
>
>På skärmen Personliga inställningar visas vilken användarroll du har i Dynamic Media Classic: Företagsadministratör, administratör eller användare.

Inställningarna för personliga inställningar styr standardbeteendet för panelen Bläddra, hur du tar emot e-post och lösenordsinställningar. Kom ihåg att klicka på Spara när du har ändrat de här inställningarna.

## Min kontoinformation

Identifierar kontonamn, namn, användarnamn (e-postadress) och tilldelad användarroll.

### Skrivbordsversion

Klicka på Installera nu för att installera datorversionen av Dynamic Media Classic på den lokala hårddisken. Du kan också klicka på Installera om nu för att installera om skrivbordsversionen.

## Installera plugin-programmet på den lokala hårddisken

1. På sidan Personliga inställningar i Dynamic Media Classic, under Illustrator Plug-in för webb-till-utskrift, klickar du på **Hämta nu** för att hämta filen **Illustrator Plug-in för webb-till-utskrift.zip**.
1. Avkomprimera ZIP-filen till en tillfällig mapp.

   En Viktigt-fil finns i roten av den uppzippade filen och ger dig ytterligare information om plugin-programmet.

1. Beroende på vilket operativsystem du har gör du något av följande:

### Windows

| Om du kör | Gör detta |
|--- |--- |
| Adobe Illustrator 18 i Adobe Creative Cloud 2014 | <ul><li>Klicka på CC-2014 i roten för den uppzippade mappen.</li><li>Beroende på vilken bitversion av Adobe Illustrator du använder klickar du på win32 eller win64.</li><li>Klicka på Bibliotek > flame och kopiera sedan `aflame.dll` till den körbara Adobe Illustrator-mappen. Exempel, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Obs**: Den här exempelsökvägen är för 64-bitarsplatsen; 32-bitarsplatsen kan i stället ingå i Program Files (x86).  <br/><ul><li>Gå tillbaka till samma biblioteksmapp, klicka på flamingo och kopiera sedan `aflamingo.dll` till samma körbara Adobe Illustrator-mapp som du använde i föregående steg. </li><li>Gå tillbaka till mappen win32 eller win64 som du valde i steg 2 och kopiera sedan `AdobeS7FXGFileFormat.aip` till Adobe Illustrator plug-ins-mappen. Exempel, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Obs**: Den här exempelsökvägen är för 64-bitarsplatsen; 32-bitarsplatsen kan i stället ingå i Program Files (x86). |
| Adobe Illustrator 17 i Adobe Creative Cloud | <ul><li>Klicka på CC i roten i den uppzippade mappen. </li><li>Beroende på vilken bitversion av Adobe Illustrator du använder klickar du på win32 eller win64.</li><li> Kopiera `AdobeS7FXGFileFormat.aip` till Adobe Illustrator plugin-mapp. Exempel, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Obs**: Den här exempelsökvägen är för 64-bitarsplatsen; 32-bitarsplatsen kan i stället ingå i Program Files (x86). |
| Adobe Illustrator 16 i Adobe Creative Suite 6 | <ul><li>Klicka på 6.0 i roten för den uppzippade mappen. </li><li>Beroende på vilken bitversion av Adobe Illustrator du använder klickar du på win32 eller win64. </li><li>Kopiera Adobe7FXGFileFormat.aip till Adobe Illustrator plug-ins-mapp. Exempel, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Obs**: Den här exempelsökvägen är för 64-bitarsplatsen; 32-bitarsplatsen kan i stället ingå i Program Files (x86). |

### Mac

| Om du kör | Gör detta |
|--- |--- |
| Adobe Illustrator 18 i Adobe Creative Cloud 2014 | <ul><li>Klicka på CC-2014 > mac64 i roten för den uppzippade mappen.</li><li>Klicka på Bibliotek > flame och kopiera sedan mappen `aflame.framework` till Adobe Illustrator-paketinnehållsmappen. Exempel, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (Om du vill öppna Adobe Illustrator paketinnehållsmapp högerklickar du på ikonen Adobe illustrator CC 2014 och klickar på Visa paketinnehåll på snabbmenyn.)</li><li>Återgå till samma biblioteksmapp, klicka på `flamingo` och kopiera sedan `aflamingo.framework`-mappen till samma Adobe Illustrator-paketinnehållsmapp som du använde i föregående steg.</li><li>Gå tillbaka till mac64-mappen som du valde i steg 1 och kopiera sedan `AdobeS7FXGFileFormat.aip`-mappen till Adobe Illustrator plug-in-mapp. Exempel, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Illustrator 17 i Adobe Creative Cloud | <ul><li>Klicka på CC > mac64 i roten i den uppzippade mappen</li><li>Kopiera mappen `AdobeS7FXGFileFormat.aip` till Adobe Illustrator plug-in-mapp. Exempel, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Illustrator 16 i Adobe Creative Suite 6 | <ul><li>Klicka 6.0 > mac64 i roten för den uppzippade mappen</li><li>Kopiera mappen `AdobeS7FXGFileFormat.aip` till Adobe Illustrator plug-in-mapp. Exempel, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul> |

Plugin-programmet finns nu för användning i Adobe Illustrator.

### Webbläsare

* **Miniatyrstorlek**
   * Anger standardstorleken för miniatyrbilder i Stödrastervisning på panelen Bläddra.
* **Standardvy för resursbibliotek**
   * Avgör om resurserna i resursbiblioteket för uppsättningar visas som miniatyrer eller efter namn. Om du arbetar med stora mängder resurser i resursbiblioteket kan du visa resurserna efter namn. Om du till exempel skapar en stor e-katalog med många PDF-filer kan du visa resurserna efter namn för att göra listan kortare.
* **Standardordning för bläddringssortering**
   * Anger i vilken ordning som resurser visas som standard på panelen Bläddra. Välj ett sorteringsvillkor på menyn och om du vill ha en stigande eller fallande sortering.
* **Standardplats för bläddring**
   * Gör att du kan ange bläddringsplatsen till standardplatsen, den senast öppnade mappen eller till en specifik plats som du navigerar till och identifierar. Du kan också ange bläddringsplats för att sortera filerna och mapparna i stigande eller fallande ordning.
* **Standardvy för webbläsare**
   * Avgör om stödrastervyn eller listvyn är standardvyn som du ser när du först öppnar panelen Bläddra.
* **Välkomstskärm**
   * Avgör om du ser några välkomstskärmar, inklusive välkomstvälkomstvälkomstskärmen.
* **Visa verktygstips**
   * Avgör om verktygstips ska visas när du flyttar pekaren över knappar, menyer och navigeringslänkar. Verktygstips beskriver objekt på skärmen.
* **Schackrutor, bakgrund**
   * Visar ett schackbrädlager bakom bilder så att du enkelt kan se de genomskinliga områdena i en bild som har en alfakanal.
* **Visa filstorlek**
   * Visar filstorleken för en resurs när du bläddrar.
* **Inkludera användardefinierat fält i sökning**
   * Avmarkerat (standard) om du vill förbättra systemprestanda för de flesta metadatasökningar som du kör.

Om de flesta av dina metadatasökningar har nytta av att inkludera användardefinierade fält kan du välja det här alternativet för att aktivera det. Du kan också använda Avancerad sökning för att få en mer riktad och snabbare sökupplevelse än att inkludera användardefinierade fält.

Se [Avancerad sökning](searching-assets.md#conducting_an_advanced_search).

Se även [Användardefinierade fält](application-setup.md#user_defined_fields).

* **Grundläggande sökningstyp**
   * Välj en standardsöktyp, Innehåller eller Börjar med.
* **Visa funktioner för mediaportal**
   * Välj det här alternativet om du vill få tillgång till funktioner i Medieportalen, t.ex. Mediekortet.
* **Visa kommandofeedback**
   * Visa kommandobegäranden till servern.
* **Visa dialogrutan vid export**
   * Visar en dialogruta när du exporterar. Om du avmarkerar det här alternativet kan du fortfarande gå till sidan Jobb för att hämta resultatet av din export.

## E-post

* **E-postalternativ**
   * Välj hur du vill att Dynamic Media Classic ska informera dig via e-post när överförings- och publiceringsjobben har slutförts. Du kan bara få meddelanden om slutförda jobb om varningar eller fel inträffar.
* **E-postomfång**
   * Avgör om du får alla jobbmeddelanden via e-post till ditt företag eller bara e-post om överförings- och publiceringsjobb som du initierar.
* **E-posttyper**
   * Avgör om du får information när överföringsjobb och publiceringsjobb har slutförts.
* **Språk**
* **Önskat språk**
   * Anger språket för gränssnittet.
* **Lösenord**
* **Nytt lösenord**
   * Ange ett nytt, giltigt lösenord. Lösenordet måste uppfylla följande krav:
      * Var mellan 8 och 25 tecken lång
      * Innehåller minst en gemen bokstav
      * Innehåller minst en versal
      * Innehåller minst en siffra
      * Innehåller minst ett av följande specialtecken: #$&amp;-_:{}
* **Skriv lösenordet igen**
   * Ange det nya lösenordet igen för att bekräfta att du har angett det korrekt.
* **Lösenordets förfallodatum**
   * Fastställer om ditt lösenord upphör att gälla efter 72 dagar som en säkerhetsåtgärd. Om du väljer Ja ombeds du skapa ett nytt lösenord efter 72 dagar.
