---
title: Personliga inställningar
description: Alla användare kan ändra inställningarna på installationsskärmen för Adobe Dynamic Media Classic.
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
feature: Dynamic Media Classic
role: Admin,User
exl-id: a019f973-7647-466f-8af3-5312e9225e89
topic: Administration, Collaboration
level: Intermediate
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 0%

---

# Personliga inställningar {#personal-setup}

Alla användare kan ändra inställningarna på skärmen Personliga inställningar. Öppna skärmen Personliga inställningar på **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.

>[!NOTE]
>
>På skärmen Personliga inställningar visas vilken användarroll du har i Adobe Dynamic Media Classic: Företagsadministratör, administratör eller användare.

Inställningarna för personliga inställningar styr standardbeteendet för panelen Bläddra, hur du tar emot e-post och lösenordsinställningar. Kom ihåg att markera **[!UICONTROL Save]** när du har ändrat dessa inställningar.

## Min kontoinformation

Identifierar kontonamn, namn, användarnamn (e-postadress) och tilldelad användarroll.

## Skrivbord

* **Rensa bildcache** - Tar bort alla Adobe Dynamic Media-cachelagrade bildfiler från datorn.
* **Rensa resurscache** - Tar bort alla resursfiler i Adobe Dynamic Media från datorn.

Förutom att rensa bild- och resurscachen med skrivbordsappen kan du rensa cachen manuellt direkt från filsystemet. Navigera till följande beroende på operativsystem:

* macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Creative Suite-tillägg

**Så här installerar du Adobe Dynamic Media Creative Suite Extension:**

1. I Adobe Dynamic Media Classic går du till **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**, under Creative Suite Extension, markera **[!UICONTROL Download Now]** för att ladda ned `s7csxs.zxp` -fil.
1. Välj **[!UICONTROL Installation]** och **[!UICONTROL System Requirements]** länkar för mer information om tillägget.

<!--    A readme file is included at the root of the unzipped file to provide you with additional information about the extension.

1. Depending on your installed operating system, do one of the following: -->

<!-- #### Windows

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014.</li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li>Select libraries > flame, and then copy `aflame.dll` to Adobe Illustrator's executable folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead. <br/><ul><li>Return to the same libraries folder, select flamingo, and then copy `aflamingo.dll` to the same Adobe Illustrator executable folder that you used in the previous step. </li><li>Return to the win32 or win64 folder that you selected in step 2, and then copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64. </li><li>Copy AdobeS7FXGFileFormat.aip to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|

#### Mac

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014 > mac64.</li><li>Select libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator’s package contents folder, right-select on the Adobe illustrator CC 2014 icon and select Show Package Contents from context menu).</li><li>Return to the same libraries folder, select `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## Webbläsare

* **[!UICONTROL Thumbnail Size]** - Anger standardstorleken för miniatyrbilder i Stödrastervisning i panelen Bläddra.
* **[!UICONTROL Default Asset Library View]** - Avgör om resurserna i resursbiblioteket för uppsättningar visas som miniatyrer eller efter namn. Om du arbetar med stora mängder resurser i resursbiblioteket kan du visa resurserna efter namn. Om du till exempel skapar en stor e-katalog med många PDF-filer kan du visa resurserna efter namn för att göra listan kortare.
* **[!UICONTROL Default Browse Sort Order]** - Anger i vilken ordning resurser visas som standard på panelen Bläddra. Välj ett sorteringsvillkor på menyn och om du vill ha en stigande eller fallande sortering.
* **[!UICONTROL Default Browse Location]** - Gör att du kan ange att bläddringsplatsen ska vara standard, den senast öppnade mappen eller till en viss plats som du navigerar till och identifierar. Du kan också ange bläddringsplats för att sortera filerna och mapparna i stigande eller fallande ordning.
* **[!UICONTROL Default Browse View]** - Avgör om Stödrastervisning eller Listvy är standardvyn som du ser när du först öppnar panelen Bläddra.
* **[!UICONTROL Splash Screen Display]** - Avgör om du ser några välkomstskärmar, inklusive välkomstvälkomstskärmen.
* **[!UICONTROL Show ToolTips]** - Anger om verktygstips ska visas när du flyttar pekaren över knappar, menyer och navigeringslänkar. Verktygstips beskriver gränssnittsobjekt på skärmen.
* **[!UICONTROL Checkerboard Background]** - Visar ett schackbrädlager bakom bilder så att du enkelt kan se de genomskinliga områdena i en bild som har en alfakanal.
* **[!UICONTROL Show File Size]** - Visar filstorleken för en resurs när du bläddrar.
* **[!UICONTROL Include UDFs in Search]** - För att förbättra systemprestanda för de flesta metadatasökningar som du kör, avmarkerat (standard).

  Om de flesta av dina metadatasökningar har nytta av att inkludera användardefinierade fält kan du välja det här alternativet för att aktivera det. Du kan också använda Avancerad sökning för att få en mer riktad och snabbare sökupplevelse än att inkludera användardefinierade fält.

  Se [Använda avancerad sökning](searching-assets.md#conducting_an_advanced_search).

  Se även [Användardefinierade fält](application-setup.md#user_defined_fields).

* **[!UICONTROL Basic Search Type]** - Du kan välja mellan två alternativ: **[!UICONTROL Contains]** söker igenom hela strängen efter det angivna värdet, **[!UICONTROL StartsWith]** söker från början av strängen och returnerar resultat snabbare än **[!UICONTROL Contains]**. Båda alternativen åsidosätter standardinställningen som är inställd i **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Application General Settings]** av administratören.
* **[!UICONTROL Show Command Feedback]** - Välj att aktivera visning av kommandobegäranden till servern, avmarkera för att stänga av.
* **[!UICONTROL Show Dialog During Export]** - Välj det här alternativet om du vill visa en popup-dialogruta under en export. Om du avmarkerar (inaktiverar) det här alternativet kan du fortfarande gå till sidan Jobb för att hämta resultaten av din export.

## E-post

* **[!UICONTROL Email Options]** - Välj hur du vill att Adobe Dynamic Media Classic ska informera dig via e-post när överförings- och publiceringsjobben är slutförda. Du kan bara få meddelanden om slutförda jobb om varningar eller fel inträffar.
* **[!UICONTROL Email Scope]** - Avgör om du får alla jobbmeddelanden via e-post till ditt företag eller bara e-post om överförings- och publiceringsjobb som du initierar.
* **[!UICONTROL Email Types]** - Avgör om du får information när överföringsjobb och publiceringsjobb har slutförts.

## Språk

* **[!UICONTROL Preferred Language]** - Bestämmer vilket språk du vill använda för gränssnittet.

## Lösenord

* **[!UICONTROL Current Password]** - Ange lösenordet för ditt nuvarande lösenord.
* **[!UICONTROL New Password]** - Ange ett nytt, giltigt lösenord. Lösenordet måste uppfylla följande krav:
   * Var mellan 8 och 25 tecken lång.
   * Innehåller minst en gemen bokstav.
   * Innehåller minst en versal.
   * Innehåller minst en siffra.
   * Innehåller minst ett av följande specialtecken: `# $ & - _ : { }`
* **[!UICONTROL Re-Type Password]** - Ange det nya lösenordet igen för att bekräfta att du har angett det korrekt.
* **[!UICONTROL Password Expiration]** - Anger om ditt lösenord upphör att gälla efter 72 dagar som en säkerhetsåtgärd. Om du väljer Ja ombeds du skapa ett lösenord efter 72 dagar.
