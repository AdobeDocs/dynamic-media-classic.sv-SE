---
title: Adobe Dynamic Media Classic - nu tillgängligt
seo-title: Adobe Dynamic Media Classic - nu tillgängligt
description: 'null'
seo-description: Läs mer om Dynamic Media Classic för datorer.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
translation-type: tm+mt
source-git-commit: 3f79517399e9f242149b66c1b71f6cca26bdb37d
workflow-type: tm+mt
source-wordcount: '1382'
ht-degree: 0%

---


# Ute nu: Skrivbordsappen Adobe Dynamic Media Classic {#dynamic-media-classic-desktop-app}

Dynamic Media Classic-användare har nu tillgång till en ny skrivbordsappsupplevelse som inte längre är beroende av Adobe Flash-teknik i webbläsaren.

Den nya appen finns nu för Windows och macOS.

>[!IMPORTANT]
>
>Vi rekommenderar att du installerar det nya datorprogrammet Adobe Dynamic Media Classic senast 1 oktober 2020. På så sätt får du en smidig övergång innan Adobe Flash Player tas bort den 31 december 2020. På den tiden kommer du inte längre att kunna logga in på webbläsarversionen av användargränssnittet Adobe Dynamic Media Classic, som heter Dynamic Media Classic i produkten.

Se Frågor och svar för den [nya Dynamic Media Classic-inloggningen.](/help/new-ui-2020.md)

## Systemkrav för datorprogrammet Adobe Dynamic Media Classic {#system-requirements-dmc-app}

Skrivbordsappen Adobe Dynamic Media Classic är kompatibel med följande operativsystem:
* macOS X 10.10 eller senare.
* Windows 7 eller senare.

## Korrigeringar i den senaste versionen, 20.20.2 {#latest-fixes-desktop-app}

* Ingen begränsning för hur många filer du kan överföra via skrivbordsappens användargränssnitt för både macOS och Windows.
* Du behöver inte logga ut från datorprogrammet för att växla mellan olika företag.
* Ctrl+V för inklistring fungerar nu i Windows.
* När en ny version av skrivbordsappen släpps i framtiden meddelas användarna via själva skrivbordsappen.

## Hämta och installera den senaste Adobe Dynamic Media Classic-datorappen på macOS eller Windows {#installation-dmc-app}

Se även:

* [Hämta och installera den senaste Adobe Dynamic Media Classic-datorappen på Mac eller Windows](#installation-dmc-app)
* [Ladda ned och tyst installera den senaste Adobe Dynamic Media Classic-datorappen i Windows](#install-silent-windows-dmc-app)

1. Avinstallera alla äldre versioner av Dynamic Media Classic-datorprogram på datorn.

1. Ladda ned det senaste installationsprogrammet för Adobe Dynamic Media Classic.

   >[!NOTE]
   >
   >Användare som redan har installerat GA-versionen bör *avinstallera* den från det lokala Windows-systemet innan de installerar den senaste versionen. Eller så kan användarna helt enkelt *ersätta* den installerade GA-versionen i sina lokala macOS-system med den senaste versionen. Nya användare bör installera den senaste versionen direkt.

   Den senaste versionen är 20.20.2 och finns på följande sida:

   * [macOS (.DMG) - Ladda ned.](http://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
   * [Windows (.EXE) - Ladda ned.](http://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe)

   GA-versionen (General Availability) var 20.20.1, tillgänglig på följande sida:

   * [macOS (.DMG) - Ladda ned.](http://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.1.dmg)
   * [Windows (.EXE) - Ladda ned.](http://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.1.exe)




1. Gör något av följande baserat på det installationsprogram du hämtade.

   * **För macOS** - Dra **[!UICONTROL Drag & drop to install]** och släpp det i **[!UICONTROL Adobe Dynamic Media Classic]** dialogrutan **[!UICONTROL Applications]**.

      ![Dra och släpp installation i macOS](/help/assets/dragondrop-install1.png)

   * Tryck på ikonen Adobe Dynamic Media Classic i **[!UICONTROL Applications]** mappen.
   * Öppna Adobe Dynamic Media Classic-datorprogrammet genom **[!UICONTROL Open]** att trycka på i dialogrutan.

      ![Öppna hämtat program](/help/assets/open-dmclassicapp1.png)

   * **För Windows** - Kör installationsprogrammets binärfil och följ instruktionerna på skärmen för att installera skrivbordsappen.

1. När du öppnar programmet visas den nya inloggningssidan för Adobe Dynamic Media Classic:

   ![Logga in med Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Använd samma inloggningsuppgifter som för webbläsaren för att logga in på Adobe Dynamic Media Classic.

   Mer information om **[!UICONTROL Server]** hur du använder finns i följande mappning för produktionsmiljön:

   | Webbläsarens URL | Servernamn för skrivbordsapp |
   |---|---|
   | https://s7sps1.scene7.com/ | Produktion i Nordamerika |
   | https://s7sps3.scene7.com/ | EMEA-produktion (Europa, Mellanöstern och Afrika) |
   | https://s7sps5.scene7.com/ | APAC-produktion (Asien-Stillahavsområdet) |

1. När du publicerar användargränssnittet för inloggning kommer du att märka hur det fungerar i webbläsaren. Du kan utföra din dagliga aktivitet som vanligt nu i skrivbordsappens användargränssnitt.

## Ladda ned och *tyst* installera den senaste Adobe Dynamic Media Classic-datorappen på macOS {#install-silent-mac-dmc-app}

Se även:

* [Hämta och installera den senaste Adobe Dynamic Media Classic-datorappen på Mac eller Windows](#installation-dmc-app)
* [Ladda ned och tyst installera den senaste Adobe Dynamic Media Classic-datorappen i Windows](#install-silent-windows-dmc-app)

Så här hämtar och ** installerar du den senaste versionen av datorprogrammet Adobe Dynamic Media Classic i macOS:

1. Avinstallera alla äldre versioner av Dynamic Media Classic-datorprogram på datorn.

1. Ladda ned det senaste installationsprogrammet för Adobe Dynamic Media Classic för macOS.

   * [macOS (.DMG) - Ladda ned.](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.2.dmg)

1. Montera den hämtade diskavbildningen (.DMG) på en monteringsplats med följande kommando:

   `hdiutil attach adobe-dynamic-media-classic-20.20.2.dmg -mountpoint <mount_point_path>`

1. Kopiera APP-filen till **[!UICONTROL Applications]** med följande kommando:

   `rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
Unmount DMG - hdiutil detach <mount_point_path>`

1. När du öppnar programmet visas den nya inloggningssidan för Adobe Dynamic Media Classic:

   ![Logga in med Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Använd samma inloggningsuppgifter som för webbläsaren för att logga in på Adobe Dynamic Media Classic.

   Mer information om **[!UICONTROL Server]** hur du använder finns i följande mappning för produktionsmiljön:

   | Webbläsarens URL | Servernamn för skrivbordsapp |
   |---|---|
   | https://s7sps1.scene7.com/ | Produktion i Nordamerika |
   | https://s7sps3.scene7.com/ | EMEA-produktion (Europa, Mellanöstern och Afrika) |
   | https://s7sps5.scene7.com/ | APAC-produktion (Asien-Stillahavsområdet) |

## Hämta och *tyst* installera den senaste Adobe Dynamic Media Classic-datorappen i Windows {#install-silent-windows-dmc-app}

Kommandot som du använder är för en grundläggande tyst MSI-installation. Installationsprogrammet för det dynamiska Media Classic-datorprogrammet är dock ett installationsprogram för InstallScript MSI som skapats med InstallShield. När du kör installationsprogrammet i inspelningsläge registreras all användarinteraktion i en svarsfil. Svarsfilen används sedan för en tyst installation enligt beskrivningen i [Köra installationer i tyst läge.](https://docs.flexera.com/installshield19helplib/helplibrary/SilentInstall.htm)

Se även:

* [Hämta och installera den senaste Adobe Dynamic Media Classic-datorappen på Mac eller Windows](#installation-dmc-app)
* [Ladda ned och tyst installera den senaste Adobe Dynamic Media Classic-datorappen i Windows](#install-silent-windows-dmc-app)

Så här hämtar och ** installerar du den senaste versionen av Adobe Dynamic Media Classic för Windows:

1. Avinstallera alla äldre versioner av Dynamic Media Classic-datorprogram på datorn.

1. Ladda ned det senaste installationsprogrammet för Adobe Dynamic Media Classic.

   * [Windows (.EXE) - Ladda ned.](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.2.exe)

1. Kör installationsprogrammet i postläge med följande kommando:

   `adobe-dynamic-media-classic-20.20.2.exe /r /f1"C:\Setup.iss"`

1. I GUI-installationsfönstret följer du stegen för att installera så att interaktioner/indata, som installationsplatsen, registreras i `Setup.iss` filen.

1. Kopiera den skapade `Setup.iss` filen och `adobe-dynamic-media-classic-20.20.2.exe` till en annan dator.

1. Kör följande kommando för en tyst installation:

   `adobe-dynamic-media-classic-20.20.2.exe /s /f1"C:\Setup.iss"`

   Information om kommandoradsparametrar finns på [Setup.exe och Update.exe Command-Line Parameters.](https://docs.flexera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. När du öppnar programmet visas den nya inloggningssidan för Adobe Dynamic Media Classic:

   ![Logga in med Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Använd samma inloggningsuppgifter som för webbläsaren för att logga in på Adobe Dynamic Media Classic.

   Mer information om **[!UICONTROL Server]** hur du använder finns i följande mappning för produktionsmiljön:

   | Webbläsarens URL | Servernamn för skrivbordsapp |
   |---|---|
   | https://s7sps1.scene7.com/ | Produktion i Nordamerika |
   | https://s7sps3.scene7.com/ | EMEA-produktion (Europa, Mellanöstern och Afrika) |
   | https://s7sps5.scene7.com/ | APAC-produktion (Asien-Stillahavsområdet) |


## Videogenomgång med Dynamic Media Classic Desktop App

Titta på en [video om hur du använder Dynamic Media Classic Desktop App](https://docs.adobe.com/content/help/en/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html) (längd: 2 minuter (36 sekunder).

## Kända begränsningar i Dynamic Media Classic 20.20.1 (åtgärdat i 20.20.2)

**_Gäller endast Windows - finns det en begränsning av antalet filer som kan överföras via skrivbordsappens användargränssnitt?_**<br>Ja, högst 150 filer kan överföras åt gången via skrivbordsappens användargränssnitt.

**_Gäller Windows och macOS - Hur växlar jag mellan företag?_**<br>Så här byter du mellan företag:
* I appen Dynamic Media Classic väljer du det nya företaget i listrutan.
* När popup-fönstret visas trycker du på **[!UICONTROL OK]** för att logga ut och stänga appen.

   ![Starta om appen för att använda det nya företaget](/help/assets/dmclassic-new-company1.png)
* Starta om Dynamic Media Classic och logga sedan in som vanligt för att arbeta med det nya företaget.

## Tips och tricks

**_Jag kan inte se Media Cart-panelen på startsidan för Dynamic Media Classic._**<br>Tryck på&#x200B;**[!UICONTROL Setup > Personal Setup]**i Dynamic Media Classic. Kontrollera att alternativet **[!UICONTROL Show MediaPortal Features]**är markerat i webbläsaravsnittet. Tryck på&#x200B;**[!UICONTROL Save > Close]**.

**_Publiceringsläge (grön indikator) för en resurs återspeglas inte korrekt._**<br>I webbläsarens användargränssnitt krävdes en ominloggning till användargränssnittet för att se rätt publiceringstillstånd för resurserna. I skrivbordsappen har vi introducerat en **[!UICONTROL Refresh]**ikon i verktygsfältet till höger om **[!UICONTROL Select None]**knappen. Tryck på&#x200B;**[!UICONTROL Refresh]**ikonen för att visa den senaste statusen för alla resurser på den angivna sidan. Ingen ominloggning krävs som med webbläsargränssnittet.

![Ikonen](/help/assets/refresh-icon1.png)Uppdatera *Uppdatera*

**_Jag ser inte gruppuppsättningsförinställningar som fungerar i skrivbordsappen._**<br>Tryck på&#x200B;**[!UICONTROL Upload > Job Options > Batch Set Presets]**. Kontrollera att relevant **[!UICONTROL Batch Set Preset]**är aktiverat. Klicka på&#x200B;**[!UICONTROL Save and Submit upload]**.
