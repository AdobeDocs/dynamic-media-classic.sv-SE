---
title: Personliga inställningar
description: Alla användare kan ändra inställningarna på skärmen Personliga inställningar i Dynamic Media Classic.
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
feature: Dynamic Media Classic
role: Administrator,Business Practitioner
exl-id: a019f973-7647-466f-8af3-5312e9225e89
translation-type: tm+mt
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 0%

---

# Personliga inställningar {#personal-setup}

Alla användare kan ändra inställningarna på skärmen Personliga inställningar. Du öppnar skärmen Personliga inställningar genom att klicka på Inställningar > Personliga inställningar.

>[!NOTE]
>
>På skärmen Personliga inställningar visas vilken användarroll du har i Dynamic Media Classic: Företagsadministratör, administratör eller användare.

Inställningarna för personliga inställningar styr standardbeteendet för panelen Bläddra, hur du tar emot e-post och lösenordsinställningar. Kom ihåg att klicka på Spara när du har ändrat de här inställningarna.

## Min kontoinformation

Identifierar kontonamn, namn, användarnamn (e-postadress) och tilldelad användarroll.

## Skrivbord

* **Rensa bildcache**  - Tar bort alla Adobe Dynamic Media-cachelagrade bildfiler från datorn.
* **Rensa resurscache**  - Tar bort alla Adobe Dynamic Media-cachelagrade resursfiler från datorn.

Förutom att rensa bild- och resurscachen med skrivbordsappen kan du rensa cachen manuellt direkt från filsystemet. Navigera till följande beroende på operativsystem:

* macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Creative Suite-tillägg

**Så här installerar du Adobe Dynamic Media Creative Suite Extension:**

1. I Dynamic Media Classic klickar du på **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**, under Creative Suite-tillägget, på **[!UICONTROL Download Now]** för att hämta `s7csxs.zxp`-filen.
1. Klicka på länkarna **[!UICONTROL Installation]** och **[!UICONTROL System Requirements]** om du vill ha mer information om tillägget.

<!--    A readme file is included at the root of the unzipped file to provide you with additional information about the extension.

1. Depending on your installed operating system, do one of the following: -->

<!-- #### Windows

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, click CC-2014.</li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64.</li><li>Click libraries > flame, and then copy `aflame.dll` to Adobe Illustrator's executable folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead. <br/><ul><li>Return to the same libraries folder, click flamingo, and then copy `aflamingo.dll` to the same Adobe Illustrator executable folder that you used in the previous step. </li><li>Return to the win32 or win64 folder that you selected in step 2, and then copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, click CC. </li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, click 6.0. </li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64. </li><li>Copy AdobeS7FXGFileFormat.aip to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|

#### Mac

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, click CC-2014 > mac64.</li><li>Click libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator’s package contents folder, right-click on the Adobe illustrator CC 2014 icon and click Show Package Contents from context menu).</li><li>Return to the same libraries folder, click `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, click CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, click 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## Webbläsare

* **Miniatyrstorlek**  - Anger standardstorleken för miniatyrbilder i stödrastervyn i panelen Bläddra.
* **Standardvy**  för resursbibliotek - Anger om resurserna i resursbiblioteket för uppsättningar ska visas som miniatyrer eller efter namn. Om du arbetar med stora mängder resurser i resursbiblioteket kan du visa resurserna efter namn. Om du till exempel skapar en stor e-katalog med många PDF-filer kan du visa resurserna efter namn för att göra listan kortare.
* **Standardordning**  för bläddringssortering - Anger i vilken ordning resurser visas som standard i panelen Bläddra. Välj ett sorteringsvillkor på menyn och om du vill ha en stigande eller fallande sortering.
* **Standardplats**  för bläddring - Här kan du ange bläddringsplatsen till standardplatsen, den senast bläddrade mappen eller till en specifik plats som du navigerar till och identifierar. Du kan också ange bläddringsplats för att sortera filerna och mapparna i stigande eller fallande ordning.
* **Standardvy**  för bläddring - Anger om stödrastervyn eller listvyn är standardvyn som du ser när du först öppnar panelen Bläddra.
* **Välkomstskärm**  - Anger om det visas några välkomstskärmar, inklusive välkomstvälkomstskärmen.
* **Visa verktygstips**  - Anger om verktygstips ska visas när du flyttar pekaren över knappar, menyer och navigeringslänkar. Verktygstips beskriver gränssnittsobjekt på skärmen.
* **Schackrutor**  - Visar ett schackrutigt lager bakom bilder så att du enkelt kan se de genomskinliga områdena i en bild som har en alfakanal.
* **Visa filstorlek**  - Visar filstorleken för en resurs när du bläddrar.
* **Inkludera användardefinierat fält i sökningen**  - Avmarkerat (standard) om du vill förbättra systemprestanda för de flesta metadatasökningar som du kör.

   Om de flesta av dina metadatasökningar har nytta av att inkludera användardefinierade fält kan du välja det här alternativet för att aktivera det. Du kan också använda Avancerad sökning för att få en mer riktad och snabbare sökupplevelse än att inkludera användardefinierade fält.

   Se [Avancerad sökning](searching-assets.md#conducting_an_advanced_search).

   Se även [Användardefinierade fält](application-setup.md#user_defined_fields).

* **Grundläggande sökningstyp**  - Du kan välja mellan två alternativ:  **[!UICONTROL Contains]** söker igenom hela strängen efter det angivna värdet,  **[!UICONTROL StartsWith]** söker från början av strängen och returnerar resultat snabbare än  **[!UICONTROL Contains]**. Båda alternativen åsidosätter standardinställningen som ställs in i **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Application General Settings]** av administratören.
* **Visa kommandofeedback** - Välj det här alternativet om du vill aktivera visning av kommandobegäranden på servern; avmarkera för att stänga av.
* **Visa dialogruta vid export**  - Välj det här alternativet om du vill visa en popup-dialogruta under en export. Om du avmarkerar (inaktiverar) det här alternativet kan du fortfarande gå till sidan Jobb för att hämta resultaten av din export.

## E-post

* **E-postalternativ**  - Välj hur du vill att Dynamic Media Classic ska informera dig via e-post när överföringen och publiceringen är klar. Du kan bara få meddelanden om slutförda jobb om varningar eller fel inträffar.
* **E-postomfång**  - Avgör om du får alla jobbmeddelanden för ditt företag eller bara e-post om överförings- och publiceringsjobb som du initierar.
* **E-posttyper**  - Avgör om du får information när överföringsjobb och publiceringsjobb har slutförts.

## Språk

* **Önskat språk**  - Anger vilket språk som ska användas för gränssnittet.

## Lösenord

* **Aktuellt lösenord**  - Ange lösenordet för ditt nuvarande lösenord.
* **Nytt lösenord**  - Ange ett nytt, giltigt lösenord. Lösenordet måste uppfylla följande krav:
   * Var mellan 8 och 25 tecken lång.
   * Innehåller minst en gemen bokstav.
   * Innehåller minst en versal.
   * Innehåller minst en siffra.
   * Innehåller minst ett av följande specialtecken: `# $ & - _ : { }`
* **Skriv lösenordet**  igen- Bekräfta att du har angett det korrekt genom att ange det nya lösenordet igen.
* **Lösenordets förfallodatum**  - Anger om ditt lösenord upphör att gälla efter 72 dagar som en säkerhetsåtgärd. Om du väljer Ja ombeds du skapa ett lösenord efter 72 dagar.
