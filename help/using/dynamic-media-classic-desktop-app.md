---
title: Adobe Dynamic Media Classic desktop
description: Läs mer om Adobe Dynamic Media Classic desktop-program som nu finns.
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
topic: Administration
level: Intermediate
source-git-commit: afc347201b13c3b91ec5e1bd3ac5304442772f8d
workflow-type: tm+mt
source-wordcount: '1903'
ht-degree: 0%

---

# Ute nu: Adobe Dynamic Media Classic datorprogram {#dynamic-media-classic-desktop-app}

Adobe Dynamic Media Classic-användare har nu tillgång till en ny datorappsupplevelse som inte längre är beroende av Adobe Flash i webbläsaren.

Den nya appen finns nu för Windows® och macOS.

>[!IMPORTANT]
>
>Adobe rekommenderar att du installerar den nya Adobe Dynamic Media Classic-appen senast 1 oktober 2020. På så sätt får du en smidig övergång innan Adobe Flash Player blir inaktuell den 31 december 2020. Efter detta datum kan du inte logga in på webbläsarversionen av Adobe Dynamic Media Classic användargränssnitt, som är märkt som Adobe Dynamic Media Classic i produkten.

Se Frågor och svar för [Ny inloggning från Adobe Dynamic Media Classic är nu tillgänglig.](/help/using/new-ui-2020.md)

## Systemkrav för Adobe Dynamic Media Classic datorprogram {#system-requirements-dmc-app}

Adobe Dynamic Media Classic-datorprogrammet är kompatibelt med följande operativsystem:

* macOS 10.10 eller senare.
* Windows® 7 eller senare.

Se de fullständiga systemkraven på [Systemkrav för Adobe Dynamic Media Classic-datorprogrammet](/help/using/system-requirements.md).

Uppgraderingsmeddelanden i Adobe Dynamic Media Classic-datorprogrammet genereras inte för *mindre*-versioner. Kunder som drar nytta av korrigeringar i en mindre release kan uppgradera.

## Fixed in the latest release (20.22.2) macOS only {#release-feb2022}

* macOS Monterey: Filöverföringssidan låses vid efterföljande överföringar. <!-- https://jira.corp.adobe.com/browse/ASSETS-7948 -->

## Korrigeringar i den senaste versionen (20.22.1) {#release-jan2022}

* När du redigerade en bild var knapparna **[!UICONTROL Save]** icke-funktionella.
* Knapparna **[!UICONTROL Close]**, **[!UICONTROL Save]** och **[!UICONTROL Save As]** inaktiveras i Set-redigerarna när du har bläddrat resurser på panelen **[!UICONTROL Add Assets]**.
* Knappen **[!UICONTROL Play]** i videouppdateringsvyn fungerade inte.
* Det gick inte att ange `d` och `e` i fälten **[!UICONTROL Username]** och **[!UICONTROL Password]** när macOS Monterey kördes.
* De återstående analys-API:erna flyttades till version 2.0.

## Korrigeringar i version 20.21.3 {#release-sept2021}

* Brutna miniatyrbilder för resurser som visas efter en viss inaktivitetsperiod i datorprogrammet.
* Skrivbordsappen slutar svara, vanligtvis efter Set-åtgärder.
* Automatiskt aktiverat begärandeautentisering och låsläge under **[!UICONTROL Test Image Serving]**.

  Se [Tjänsten Secure Testing](/help/using/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* Uppdaterad autentiseringsmekanism med Adobe Analytics. Relevant för nya integreringar eller om vissa Analytics-variabler måste uppdateras inifrån Dynamic Media Classic-datorprogrammet.

  Se [Logga in på Adobe Analytics](/help/using/log-analytics.md) för uppdaterade steg.

## Korrigeringar i version 20.21.2 {#minor-release}

* Känd begränsning i 20.21.1: listrutan **[!UICONTROL Server]** på inloggningsskärmen var tom.
* I **[!UICONTROL Upload Job Options]** är nu standardvärdet för lagernamn under **[!UICONTROL Photoshop Options]** **[!UICONTROL Photoshop and Layer Name]**. Lager i filen PSD överförs som separata bilder.
   * Det tidigare standardvärdet för **[!UICONTROL Layer name]**, som namngav bilderna efter deras lagernamn eller lagernummer i filen PSD. Lagernumret användes om lagernamnen i PSD-filen var Photoshop standardlagernamn.
   * Den nya standardinställningen **[!UICONTROL Photoshop and Layer Name]** namnger bilderna efter PSD-filen följt av lagernamnet eller lagernumret. Lagernumret används om lagernamnen i filen PSD är Photoshop standardlagernamn.
   * Eftersom lagerbilder i Adobe Dynamic Media Classic nu har unika namn kommer inga uppdateringar att göras av befintliga PSD eller mallar (som delar lagernamn i de ursprungliga PSD-filerna).
* Brutna miniatyrbilder av resurser.

## Korrigeringar i version 20.21.1 {#latest-fixes-desktop-app}

* Inloggningsproblem på grund av timeout som resulterar i följande meddelande: *Den här användaren kan tilldelas gruppen eller grupperna utan behörighet. Kontakta administratören.*
* Förinställningar för visningsprogram dupliceras med varje felaktigt lösenordsförsök.
* Skrivbordsprogrammet slutar svara på grund av många resurser i rotmappen. (Fast i Windows®; fungerar som du vill i macOS.)

## Korrigeringar i version 20.20.2 {#previous-version-fixes-desktop-app}

* Ingen begränsning för hur många filer du kan överföra via skrivbordsappens användargränssnitt för både macOS och Windows®.
* Du behöver inte logga ut från datorprogrammet för att växla mellan olika företag.
* Ctrl+V för inklistring fungerar nu i Windows®.
* När en ny version av datorprogrammet släpps i framtiden kommer användarna att meddelas via själva skrivbordsappen.

## Hämta och installera den senaste Adobe Dynamic Media Classic-appen på macOS eller Windows® {#installation-dmc-app}

Se även:

* [Ladda ned och tyst installera den senaste Adobe Dynamic Media Classic-appen på Mac](#install-silent-mac-dmc-app)
* [Hämta och tyst installera den senaste Adobe Dynamic Media Classic-appen på Windows](#install-silent-windows-dmc-app)

1. Avinstallera alla äldre versioner av Adobe Dynamic Media Classic-datorprogram på datorn.

1. Hämta det senaste installationsprogrammet för Adobe Dynamic Media Classic-datorprogrammet.

   * Den senaste versionen finns på följande webbplats:

      * [macOS (.DMG): Hämta](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)
      * [Windows (.EXE): Hämta](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

   * Den tidigare versionen finns på följande webbplats:

      * [macOS (.DMG): Hämta](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows® (.EXE): Hämta](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)

<!--         * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg) -->

<!--    * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows&reg; (.EXE): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. Gör något av följande beroende på vilket installationsprogram du har laddat ned.

   * **macOS** -I dialogrutan **[!UICONTROL Drag & drop to install]** drar du **[!UICONTROL Adobe Dynamic Media Classic]** och släpper den på **[!UICONTROL Applications]**.

     ![Dra och släpp installation på macOS](/help/using/assets/dragondrop-install1.png)

   * Tryck på ikonen Adobe Dynamic Media Classic i mappen **[!UICONTROL Applications]**.
   * Öppna Adobe Dynamic Media Classic-datorprogrammet genom att trycka på **[!UICONTROL Open]** i dialogrutan.

     ![Öppna hämtat program](/help/using/assets/open-dmclassicapp1.png)

   * **Windows** - Kör installationsprogrammets binärfil och följ instruktionerna på skärmen för att installera datorprogrammet.

1. När du öppnar programmet visas den nya Adobe Dynamic Media Classic Sign-in-sidan:

   ![Adobe Dynamic Media Classic-inloggning](/help/using/assets/dmclassic-login1.png)

1. Om du vill logga in på Adobe Dynamic Media Classic datorprogram använder du samma inloggningsuppgifter som du använde när du loggade in på Adobe Dynamic Media Classic i webbläsaren.

   Mer information om hur **[!UICONTROL Server]** ska användas finns i följande mappning för produktionsmiljön:

   | Server | Webbläsarens URL |
   | --- | --- |
   | NA Production (Nordamerika) | https://s7sps1.scene7.com/ |
   | EMEA-produktion (Europa, Mellanöstern och Afrika) | https://s7sps3.scene7.com/ |
   | APAC-produktion (Asien-Stillahavsområdet) | https://s7sps5.scene7.com/ |

1. När du har loggat in kan du se hur webbläsargränssnittet fungerar. Du kan fortsätta din dagliga Adobe Dynamic Media Classic-aktivitet som vanligt i skrivbordsappen.

## Hämta och *tyst* installera den senaste Adobe Dynamic Media Classic-datorappen på macOS {#install-silent-mac-dmc-app}

Se även:

* [Hämta och installera den senaste Adobe Dynamic Media Classic-appen på Mac eller Windows](#installation-dmc-app)
* [Hämta och tyst installera den senaste Adobe Dynamic Media Classic-appen på Windows](#install-silent-windows-dmc-app)

Så här hämtar och *tyst* installerar du den senaste versionen av Adobe Dynamic Media Classic-datorprogrammet på macOS:

1. Avinstallera alla äldre versioner av Adobe Dynamic Media Classic-datorprogram på datorn.

1. Hämta det senaste installationsprogrammet för Adobe Dynamic Media Classic-datorprogrammet för macOS.

   * [macOS (.DMG): Hämta](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)

1. Montera den hämtade diskavbildningen (.DMG) på en monteringsplats med följande kommando:

   `hdiutil attach adobe-dynamic-media-classic-20.22.2.dmg -mountpoint <mount_point_path>`

1. Kopiera APP-filen till **[!UICONTROL Applications]** med följande kommando:

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG: hdiutil detach <mount_point_path>
   ```

1. När du öppnar programmet visas den nya Adobe Dynamic Media Classic Sign-in-sidan:

   ![Adobe Dynamic Media Classic-inloggning](/help/using/assets/dmclassic-login1.png)

1. Om du vill logga in på Adobe Dynamic Media Classic datorprogram använder du samma inloggningsuppgifter som du använde när du loggade in på Adobe Dynamic Media Classic i webbläsaren.

   Mer information om hur **[!UICONTROL Server]** ska användas finns i följande mappning för produktionsmiljön:

   | Server | Webbläsarens URL |
   | --- | --- |
   | NA Production (Nordamerika) | https://s7sps1.scene7.com/ |
   | EMEA-produktion (Europa, Mellanöstern och Afrika) | https://s7sps3.scene7.com/ |
   | APAC-produktion (Asien-Stillahavsområdet) | https://s7sps5.scene7.com/ |

## Hämta och *tyst* installera den senaste Adobe Dynamic Media Classic-datorappen på Windows® {#install-silent-windows-dmc-app}

Kommandot som du använder är för en grundläggande tyst MSI-installation. Installationsprogrammet för Adobe Dynamic Media Classic-datorprogrammet är dock ett MSI-installationsprogram för InstallShield. När du kör installationsprogrammet i inspelningsläge registreras all användarinteraktion i en svarsfil. Den här svarsfilen används sedan för en tyst installation enligt beskrivningen i [Köra installationer i tyst läge](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/SilentInstall.htm).

Se även:

* [Hämta och installera den senaste Adobe Dynamic Media Classic-appen på Mac eller Windows](#installation-dmc-app)

* [Ladda ned och tyst installera den senaste Adobe Dynamic Media Classic-appen på macOS](#install-silent-mac-dmc-app)

Så här hämtar och *tyst* installerar du den senaste versionen av Adobe Dynamic Media Classic-datorprogrammet på Windows®:

1. Avinstallera alla äldre versioner av Adobe Dynamic Media Classic-datorprogram på datorn.

1. Hämta det senaste installationsprogrammet för Adobe Dynamic Media Classic-datorprogrammet.

   * [Windows® (.EXE): Hämta](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. Kör installationsprogrammet i postläge med följande kommando:

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. I GUI-installationsfönstret följer du stegen för att installera så att interaktioner/indata, som installationsplatsen, registreras i filen `Setup.iss`.

1. Kopiera den skapade `Setup.iss`-filen och `adobe-dynamic-media-classic-20.22.1.exe` till en annan dator.

1. Kör följande kommando för en tyst installation:

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   Information om kommandoradsparametrar finns på [Setup.exe och kommandoradsparametrarna Update.exe](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/IHelpSetup_EXECmdLine.htm?Highlight=Setup.exe%20and%20Update.exe%20Command-Line%20Parameters).

1. När du öppnar programmet visas den nya Adobe Dynamic Media Classic Sign-in-sidan:

   ![Adobe Dynamic Media Classic-inloggning](/help/using/assets/dmclassic-login1.png)

1. Om du vill logga in på Adobe Dynamic Media Classic datorprogram använder du samma inloggningsuppgifter som du använde när du loggade in på Adobe Dynamic Media Classic i webbläsaren.

   Mer information om hur **[!UICONTROL Server]** ska användas finns i följande mappning för produktionsmiljön:

   | Server | Webbläsarens URL |
   | --- | --- |
   | NA Production (Nordamerika) | https://s7sps1.scene7.com/ |
   | EMEA-produktion (Europa, Mellanöstern och Afrika) | https://s7sps3.scene7.com/ |
   | APAC-produktion (Asien-Stillahavsområdet) | https://s7sps5.scene7.com/ |

## Videogenomgång om hur du använder Adobe Dynamic Media Classic datorprogram {#dmc-app-video-walk-through}

Titta på en [videogenomgång om hur du använder Adobe Dynamic Media Classic-datorprogrammet](https://experienceleague.adobe.com/sv/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application#dynamic-media) (längd: 2 minuter 36 sekunder).

## Rensa bildcachen och resurscachen på datorn med datorprogrammet {#clear-cache}

1. I Adobe Dynamic Media Classic-datorprogrammet, i det övre högra hörnet, trycker du på **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.
1. Gör något av följande på sidan **[!UICONTROL Personal Setup]**, under rubriken **[!UICONTROL Desktop]**:
   * Om du vill ta bort alla Adobe Dynamic Media-cachelagrade bildfiler från datorn trycker du på **[!UICONTROL Clear Image Cache]** och sedan på **[!UICONTROL OK]**.
   * Om du vill ta bort alla cachelagrade resursfiler för Adobe Dynamic Media från datorn trycker du på **[!UICONTROL Clear Asset Cache]** och sedan på **[!UICONTROL OK]**.
1. Tryck på **[!UICONTROL Close]** i sidans nedre högra hörn.

### Rensa bildcachen och resurscachen manuellt

Förutom att rensa bild- och resurscachen med skrivbordsappen kan du rensa cachen manuellt direkt från filsystemet.

1. Navigera till följande beroende på operativsystem:

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Kända begränsningar i Adobe Dynamic Media Classic 20.21.1

* Listrutan **[!UICONTROL Server]** är tom efter uppdatering till Adobe Dynamic Media Classic datorprogram 20.21.1: Scenario: Du installerar och loggar in på Adobe Dynamic Media Classic 20.20.1 eller 20.20.2 och stänger sedan programmet. Uppdatera sedan till Adobe Dynamic Media Classic 20.21.1. När du försöker logga in är listrutan **[!UICONTROL Server]** i dialogrutan **[!UICONTROL Sign-in to your account]** tom. Du måste [rensa cachen](#clear-cache) manuellt för att kunna undvika problemet (se stegen ovan).

## Kända begränsningar i Adobe Dynamic Media Classic 20.20.1 (fast i 20.20.2)

**_Gäller endast Windows® - finns det en begränsning av antalet filer som kan överföras via skrivbordsappens användargränssnitt?_**<br>Ja, högst 150 filer kan överföras åt gången med hjälp av skrivbordsappens användargränssnitt.

**_Gäller Windows® och macOS - Hur växlar jag mellan företag?_**<br>Så här växlar du mellan företag:

* I appen Adobe Dynamic Media Classic väljer du det nya företaget i listrutan för företag.
* När popup-fönstret visas trycker du på **[!UICONTROL OK]** för att logga ut och stänga appen.

  ![Starta om appen](/help/using/assets/dmclassic-new-company1.png) om du vill använda det nya företaget

* Starta om Adobe Dynamic Media Classic och logga sedan in som vanligt för att arbeta med det nya företaget.

## Tips och tricks

**_Jag kan inte se Media Cart-panelen på Adobe Dynamic Media Classic landningssida._**<br>Tryck på&#x200B;**[!UICONTROL Setup > Personal Setup]**&#x200B;i Adobe Dynamic Media Classic. Kontrollera att **[!UICONTROL Show MediaPortal Features]**&#x200B;är markerat i webbläsaravsnittet. Tryck på&#x200B;**[!UICONTROL Save > Close]**.

**_Publish-tillstånd (grön indikator) för en resurs återspeglas inte korrekt._**<br>I webbläsarens användargränssnitt krävdes en ominloggning till användargränssnittet för att se rätt publiceringstillstånd för resurserna. I skrivbordsappen har Adobe introducerat en **[!UICONTROL Refresh]**-ikon i verktygsfältet till höger om knappen **[!UICONTROL Select None]**. Tryck på ikonen **[!UICONTROL Refresh]**&#x200B;för att visa den senaste statusen för alla resurser på den angivna sidan. Ingen ominloggning krävs som med webbläsargränssnittet.

![Ikonen Uppdatera](/help/using/assets/refresh-icon1.png)
*Ikonen Uppdatera*

**_Jag ser inte gruppuppsättningsförinställningar som fungerar i skrivbordsappen._**<br>Tryck på&#x200B;**[!UICONTROL Upload > Job Options > Batch Set Presets]**. Kontrollera att relevant **[!UICONTROL Batch Set Preset]**&#x200B;är aktiverat. Klicka på&#x200B;**[!UICONTROL Save and Submit upload]**.
