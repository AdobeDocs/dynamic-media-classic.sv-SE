---
title: Adobe Dynamic Media Classic - nu tillgängligt
description: Läs mer om Dynamic Media Classic för datorer.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
source-git-commit: 9ff171590c65f55cef8c9e5a2b4e77ddbbfa6895
workflow-type: tm+mt
source-wordcount: '1772'
ht-degree: 0%

---

# Ute nu: Adobe Dynamic Media Classic-datorprogrammet {#dynamic-media-classic-desktop-app}

Dynamic Media Classic-användare har nu tillgång till en ny skrivbordsappsupplevelse som inte längre är beroende av Adobe Flash i webbläsaren.

Den nya appen finns nu för Windows® och macOS.

>[!IMPORTANT]
>
>Adobe rekommenderar att du installerar det nya Adobe Dynamic Media Classic-datorprogrammet senast 1 oktober 2020. På så sätt får du en smidig övergång innan Adobe Flash Player tas bort den 31 december 2020. Efter detta datum kan du inte logga in på webbläsarversionen av användargränssnittet Adobe Dynamic Media Classic, som heter Dynamic Media Classic i produkten.

Se Frågor och svar för [Ny inloggningsupplevelse i Dynamic Media Classic är nu tillgänglig.](/help/new-ui-2020.md)

## Systemkrav för datorprogrammet Adobe Dynamic Media Classic {#system-requirements-dmc-app}

Adobe Dynamic Media Classic är kompatibelt med följande operativsystem:

* macOS 10.10 eller senare.
* Windows® 7 eller senare.

>[!NOTE]
>
>Uppgraderingsmeddelanden i Dynamic Media Classic-datorprogrammet genereras inte för *mindre*-versioner. Kunder som drar nytta av korrigeringar i en mindre release kan uppgradera.

## Korrigeringar i den mindre versionen (20.21.2) {#minor-release}

* Känd begränsning i 20.21.1-listrutan Server är tom.
* I **[!UICONTROL Upload Job Options]** är standardvärdet för lagernamn under **[!UICONTROL Photoshop Options]** nu **[!UICONTROL Photoshop and Layer Name]**. Lager i PSD-filen överförs som separata bilder.
   * Det tidigare standardvärdet **[!UICONTROL Layer name]**, som namnger bilderna efter deras lagernamn eller lagernummer i PSD-filen. Lagernumret användes om lagernamnen i PSD-filen var Photoshop standardlagernamn.
   * Den nya standardinställningen **[!UICONTROL Photoshop and Layer Name]** namnger bilderna efter PSD-filen följt av lagernamnet eller lagernumret. Lagernumret används om lagernamnen i PSD-filen är Photoshop standardlagernamn.
   * Eftersom lagerbilder i Dynamic Media Classic nu har unika namn kommer inga uppdateringar att göras av befintliga PSD- eller mallar (som delar lagernamn i de ursprungliga PSD-filerna).
* Brutna miniatyrbilder av resurser.

## Korrigeringar i den senaste versionen (20.21.1) {#latest-fixes-desktop-app}

* Inloggningsproblem på grund av timeout, vilket resulterar i följande meddelande: *Den här användaren kan tilldelas gruppen eller grupperna utan behörighet. Kontakta administratören.*
* Förinställningar för visningsprogram dupliceras med varje felaktigt lösenordsförsök.
* Skrivbordsprogrammet slutar svara på grund av många resurser i rotmappen. (Fast i Windows®; arbeta som du vill i macOS.)

## Korrigeringar i föregående version (20.20.2) {#previous-version-fixes-desktop-app}

* Ingen begränsning för hur många filer du kan överföra via skrivbordsappens användargränssnitt för både macOS och Windows®.
* Du behöver inte logga ut från datorprogrammet för att växla mellan olika företag.
* Ctrl+V för inklistring fungerar nu i Windows®.
* När en ny version av datorprogrammet släpps i framtiden kommer användarna att meddelas via själva skrivbordsappen.

## Hämta och installera den senaste Adobe Dynamic Media Classic-datorappen på macOS eller Windows® {#installation-dmc-app}

Se även:

* [Ladda ned och tyst installera den senaste Adobe Dynamic Media Classic-datorappen på Mac](#install-silent-mac-dmc-app)
* [Ladda ned och tyst installera den senaste Adobe Dynamic Media Classic-datorappen i Windows®](#install-silent-windows-dmc-app)

1. Avinstallera alla äldre versioner av Dynamic Media Classic-datorprogram på datorn.

1. Hämta det senaste installationsprogrammet för Adobe Dynamic Media Classic-datorprogrammet.

   * Den senaste versionen (20.21.2) finns här:

      * [macOS (.DMG) - Ladda ned](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
      * [Windows® (.EXE) - nedladdning](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)
   * Den tidigare versionen (20.21.1) finns på följande plats:

      * [macOS (.DMG) - Ladda ned](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.dmg)
      * [Windows® (.EXE) - nedladdning](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.exe)


<!--         * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. Gör något av följande baserat på det installationsprogram du hämtade.

   * **För macOS**  - Dra  **[!UICONTROL Drag & drop to install]** och släpp det i  **[!UICONTROL Adobe Dynamic Media Classic]** dialogrutan  **[!UICONTROL Applications]**.

      ![Dra och släpp installation i macOS](/help/assets/dragondrop-install1.png)

   * Tryck på ikonen Adobe Dynamic Media Classic i mappen **[!UICONTROL Applications]**.
   * I dialogrutan trycker du på **[!UICONTROL Open]** för att öppna Adobe Dynamic Media Classic-datorprogrammet.

      ![Öppna hämtat program](/help/assets/open-dmclassicapp1.png)

   * **För Windows**  - Kör installationsprogrammets binärfil och följ instruktionerna på skärmen för att installera skrivbordsappen.

1. När du öppnar programmet visas den nya inloggningssidan för Adobe Dynamic Media Classic:

   ![Dynamic Media Classic-inloggning](/help/assets/dmclassic-login1.png)

1. Om du vill logga in på datorprogrammet Adobe Dynamic Media Classic använder du samma inloggningsuppgifter som du använde när du loggade in på Dynamic Media Classic i webbläsaren.

   Mer information om hur du använder **[!UICONTROL Server]** finns i följande mappning för produktionsmiljön:

   | Webbläsarens URL | Servernamn för skrivbordsapp |
   |---|---|
   | https://s7sps1.scene7.com/ | Produktion i Nordamerika |
   | https://s7sps3.scene7.com/ | EMEA-produktion (Europa, Mellanöstern och Afrika) |
   | https://s7sps5.scene7.com/ | APAC-produktion (Asien-Stillahavsområdet) |

1. När du har loggat in kan du se hur webbläsargränssnittet fungerar. Du kan fortsätta din dagliga Dynamic Media Classic-aktivitet som vanligt i skrivbordsappen.

## Hämta och *tyst* installera den senaste Adobe Dynamic Media Classic-datorappen på macOS {#install-silent-mac-dmc-app}

Se även:

* [Hämta och installera den senaste Adobe Dynamic Media Classic-datorappen på Mac eller Windows®](#installation-dmc-app)
* [Ladda ned och tyst installera den senaste Adobe Dynamic Media Classic-datorappen i Windows®](#install-silent-windows-dmc-app)

Så här hämtar och *installerar du den senaste versionen av Adobe Dynamic Media Classic-datorprogrammet i macOS:*

1. Avinstallera alla äldre versioner av Dynamic Media Classic-datorprogram på datorn.

1. Ladda ned det senaste installationsprogrammet för Adobe Dynamic Media Classic för macOS.

   * [macOS (.DMG) - Ladda ned](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)

1. Montera den hämtade diskavbildningen (.DMG) på en monteringsplats med följande kommando:

   `hdiutil attach adobe-dynamic-media-classic-20.21.2.dmg -mountpoint <mount_point_path>`

1. Kopiera .APP-filen till **[!UICONTROL Applications]** med följande kommando:

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG - hdiutil detach <mount_point_path>
   ```

1. När du öppnar programmet visas den nya inloggningssidan för Adobe Dynamic Media Classic:

   ![Dynamic Media Classic-inloggning](/help/assets/dmclassic-login1.png)

1. Om du vill logga in på datorprogrammet Adobe Dynamic Media Classic använder du samma inloggningsuppgifter som du använde när du loggade in på Dynamic Media Classic i webbläsaren.

   Mer information om hur du använder **[!UICONTROL Server]** finns i följande mappning för produktionsmiljön:

   | Webbläsarens URL | Servernamn för skrivbordsapp |
   |---|---|
   | https://s7sps1.scene7.com/ | Produktion i Nordamerika |
   | https://s7sps3.scene7.com/ | EMEA-produktion (Europa, Mellanöstern och Afrika) |
   | https://s7sps5.scene7.com/ | APAC-produktion (Asien-Stillahavsområdet) |

## Hämta och *tyst* installera den senaste Adobe Dynamic Media Classic-datorappen i Windows® {#install-silent-windows-dmc-app}

Kommandot som du använder är för en grundläggande tyst MSI-installation. Installationsprogrammet för Dynamic Media Classic-datorprogrammet är dock ett MSI-installationsprogram för InstallScript som skapats med InstallShield. När du kör installationsprogrammet i inspelningsläge registreras all användarinteraktion i en svarsfil. Svarsfilen används sedan för en tyst installation enligt beskrivningen i [Köra installationer i tyst läge.](https://docs.revenera.com/installshield19helplib/helplibrary/SilentInstall.htm)

Se även:

* [Hämta och installera den senaste Adobe Dynamic Media Classic-datorappen på Mac eller Windows®](#installation-dmc-app)
* [Ladda ned och tyst installera den senaste Adobe Dynamic Media Classic-datorappen på macOS](#install-silent-mac-dmc-app)

Så här hämtar och *installerar du den senaste versionen av Adobe Dynamic Media Classic för Windows®:*

1. Avinstallera alla äldre versioner av Dynamic Media Classic-datorprogram på datorn.

1. Hämta det senaste installationsprogrammet för Adobe Dynamic Media Classic-datorprogrammet.

   * [Windows® (.EXE) - nedladdning](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)

1. Kör installationsprogrammet i postläge med följande kommando:

   `adobe-dynamic-media-classic-20.21.2.exe /r /f1"C:\Setup.iss"`

1. I GUI-installationsfönstret följer du stegen för att installera så att interaktioner/indata, som installationsplatsen, registreras i `Setup.iss`-filen.

1. Kopiera den skapade `Setup.iss`-filen och `adobe-dynamic-media-classic-20.21.2.exe` till en annan dator.

1. Kör följande kommando för en tyst installation:

   `adobe-dynamic-media-classic-20.21.2.exe /s /f1"C:\Setup.iss"`

   Information om kommandoradsparametrar finns på [Setup.exe och Update.exe Command-Line Parameters.](https://docs.revenera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. När du öppnar programmet visas den nya inloggningssidan för Adobe Dynamic Media Classic:

   ![Dynamic Media Classic-inloggning](/help/assets/dmclassic-login1.png)

1. Om du vill logga in på datorprogrammet Adobe Dynamic Media Classic använder du samma inloggningsuppgifter som du använde när du loggade in på Dynamic Media Classic i webbläsaren.

   Mer information om hur du använder **[!UICONTROL Server]** finns i följande mappning för produktionsmiljön:

   | Webbläsarens URL | Servernamn för skrivbordsapp |
   |---|---|
   | https://s7sps1.scene7.com/ | Produktion i Nordamerika |
   | https://s7sps3.scene7.com/ | EMEA-produktion (Europa, Mellanöstern och Afrika) |
   | https://s7sps5.scene7.com/ | APAC-produktion (Asien-Stillahavsområdet) |


## Videogenomgång om hur du använder Dynamic Media Classic Desktop App {#dmc-app-video-walk-through}

Titta på en [videogenomgång om hur du använder Dynamic Media Classic Desktop App](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media) (längd: 2 minuter (36 sekunder).

## Rensa bildcachen och resurscachen på datorn med skrivbordsappen {#clear-cache}

1. I Dynamic Media Classic-datorprogrammet trycker du **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]** i det övre högra hörnet.
1. Gör något av följande på sidan **[!UICONTROL Personal Setup]**, under rubriken **[!UICONTROL Desktop]**:
   * Om du vill ta bort alla Adobe Dynamic Media-cachelagrade bildfiler från datorn trycker du på **[!UICONTROL Clear Image Cache]** och sedan på **[!UICONTROL OK]**.
   * Om du vill ta bort alla cachelagrade resursfiler för Adobe Dynamic Media från datorn trycker du på **[!UICONTROL Clear Asset Cache]** och sedan på **[!UICONTROL OK]**.
1. Tryck på **[!UICONTROL Close]** längst ned till höger på sidan.

### Rensa bildcachen och resurscachen manuellt

Förutom att rensa bild- och resurscachen med skrivbordsappen kan du rensa cachen manuellt direkt från filsystemet.

1. Navigera till följande beroende på operativsystem:

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Känd begränsning i Dynamic Media Classic 20.21.1

* Listrutan **[!UICONTROL Server]** är tom efter uppdatering till Dynamic Media Classic för datorer 20.21.1 - scenario: Du installerar och loggar in på Dynamic Media Classic 20.20.1 eller 20.20.2 och stänger sedan programmet. Därefter uppdaterar du till Dynamic Media Classic 20.21.1. När du försöker logga in är listrutan **[!UICONTROL Server]** i dialogrutan **[!UICONTROL Sign in to your account]** tom. Du måste [rensa cacheminnet](#clear-cache) manuellt för att lösa problemet (se stegen ovan).

## Kända begränsningar i Dynamic Media Classic 20.20.1 (fast i 20.20.2)

**_Gäller endast Windows® - finns det en begränsning av antalet filer som kan överföras via skrivbordsappens användargränssnitt?_**<br>Ja, högst 150 filer kan överföras åt gången via skrivbordsappens användargränssnitt.

**_Gäller Windows® och macOS - Hur växlar jag mellan företag?_**<br>Så här byter du mellan företag:

* I appen Dynamic Media Classic väljer du det nya företaget i listrutan för företag.
* När popup-fönstret visas trycker du på **[!UICONTROL OK]** för att logga ut och stänga appen.

   ![Starta om appen om du vill använda det nya företaget](/help/assets/dmclassic-new-company1.png)

* Starta om Dynamic Media Classic och logga sedan in som vanligt för att arbeta med det nya företaget.

## Tips och tricks

**_Jag kan inte se Media Cart-panelen på startsidan för Dynamic Media Classic._**<br>Tryck på&#x200B;**[!UICONTROL Setup > Personal Setup]**i Dynamic Media Classic. Kontrollera att **[!UICONTROL Show MediaPortal Features]**är markerat i webbläsaravsnittet. Tryck på&#x200B;**[!UICONTROL Save > Close]**.

**_Publiceringsläge (grön indikator) för en resurs återspeglas inte korrekt._**<br>I webbläsarens användargränssnitt krävdes en ominloggning till användargränssnittet för att se rätt publiceringstillstånd för resurserna. I skrivbordsappen har Adobe introducerat en **[!UICONTROL Refresh]**-ikon i verktygsfältet till höger om knappen **[!UICONTROL Select None]**. Tryck på ikonen **[!UICONTROL Refresh]**för att visa den senaste statusen för alla resurser på den angivna sidan. Ingen ominloggning krävs som med webbläsargränssnittet.

![Ikon ](/help/assets/refresh-icon1.png)
*för uppdateringIkon för uppdatering*

**_Jag ser inte gruppuppsättningsförinställningar som fungerar i skrivbordsappen._**<br>Tryck på&#x200B;**[!UICONTROL Upload > Job Options > Batch Set Presets]**. Kontrollera att relevant **[!UICONTROL Batch Set Preset]**är aktiverat. Klicka på&#x200B;**[!UICONTROL Save and Submit upload]**.
