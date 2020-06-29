---
title: Adobe Dynamic Media Classic - nu tillgängligt
seo-title: Adobe Dynamic Media Classic - nu tillgängligt
description: 'null'
seo-description: Läs mer om Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
translation-type: tm+mt
source-git-commit: 37f9a42b89ad1ade0aa7f8fc542b03c930bd9c27
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 0%

---


# Ute nu: Adobe Dynamic Media Classic {#dynamic-media-classic-desktop-app}

Dynamic Media Classic-användare har nu tillgång till en ny skrivbordsappsupplevelse som inte längre är beroende av Adobe Flash-teknik i webbläsaren.

Den nya appen finns nu för Windows och macOS.

>[!IMPORTANT]
>
>Vi rekommenderar att du installerar nya Adobe Dynamic Media Classic senast 1 oktober 2020. På så sätt får du en smidig övergång innan Adobe Flash Player är inaktuellt den 31 december 2020. På den tiden kommer du inte längre att kunna logga in på webbläsarversionen av Adobe Dynamic Media Classic-användargränssnittet, som heter Scene7 Publishing System i produkten.

Se Vanliga frågor och svar om inloggningen med [nya Dynamic Media Classic.](/help/new-ui-2020.md)

## Systemkrav för datorprogrammet Adobe Dynamic Media Classic {#system-requirements-dmc-app}

Adobe Dynamic Media Classic är kompatibelt med följande operativsystem:
* macOS X 10.10 eller senare.
* Windows 7 eller senare.

## Hämta och installera Adobe Dynamic Media Classic-datorprogrammet {#installation-dmc-app}

1. Avinstallera alla äldre versioner av Dynamic Media Classic-datorprogram på datorn.

1. Hämta det senaste installationsprogrammet för Adobe Dynamic Media Classic-datorprogrammet.

   * [macOS (.dmg) - Ladda ned.](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.dmg)
   * [Windows (.exe) - Ladda ned.](lhttp://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.exe)

1. Gör något av följande baserat på det installationsprogram du hämtade.

   * **För macOS** - Dra **[!UICONTROL Drag & drop to install]** och släpp det i **[!UICONTROL Adobe Dynamic Media Classic]** dialogrutan **[!UICONTROL Applications]**.

      ![Dra och släpp installation i macOS](/help/assets/dragondrop-install.png)

   * Tryck på ikonen Adobe Dynamic Media Classic i **[!UICONTROL Applications]** mappen.
   * Öppna Adobe Dynamic Media Classic-datorprogrammet genom **[!UICONTROL Open]** att trycka på i dialogrutan.

      ![Öppna hämtat program](/help/assets/open-dmclassicapp.png)

   * **För Windows** - Kör installationsprogrammets binärfil och följ instruktionerna på skärmen för att installera skrivbordsappen.

1. När du öppnar programmet visas den nya inloggningssidan för Adobe Dynamic Media Classic:

   ![Dynamic Media Classic-inloggning](/help/assets/dmclassic-login.png)

1. Använd samma inloggningsuppgifter som för webbläsaren när du loggar in på Adobe Dynamic Media Classic.

   Mer information om **[!UICONTROL Server]** hur du använder finns i följande mappning för produktionsmiljön:

   | Webbläsarens URL | Servernamn för skrivbordsapp |
   |---|---|
   | https://s7sps1.scene7.com/ | Produktion i Nordamerika |
   | https://s7sps3.scene7.com/ | EMEA-produktion (Europa, Mellanöstern och Afrika) |
   | https://s7sps5.scene7.com/ | APAC-produktion (Asien-Stillahavsområdet) |

1. När du publicerar användargränssnittet för inloggning kommer du att märka hur det fungerar i webbläsaren. Du kan utföra din dagliga aktivitet som vanligt nu i användargränssnittet för skrivbordsappen.

## Kända begränsningar i Dynamic Media Classic

**_Gäller endast Windows - finns det en begränsning av antalet filer som kan överföras via skrivbordsappens användargränssnitt?_**<br> Ja, högst 150 filer kan överföras åt gången via skrivbordsappens användargränssnitt.

**_Gäller Windows och macOS - Hur växlar jag mellan företag?_**<br> Så här byter du mellan företag:
* I appen Dynamic Media Classic väljer du det nya företaget i listrutan för företag.
* När popup-fönstret visas trycker du på **[!UICONTROL OK]** för att logga ut och stänga appen.

   ![Starta om appen för att använda det nya företaget](/help/assets/dmclassic-new-company.png)
* Starta om Dynamic Media Classic och logga sedan in som vanligt för att arbeta med det nya företaget.

## Tips och tricks

**_Jag kan inte se Media Cart-panelen på startsidan för Dynamic Media Classic._**<br> Tryck på **[!UICONTROL Setup > Personal Setup]** i Dynamic Media Classic. Kontrollera att alternativet **[!UICONTROL Show MediaPortal Features]** är markerat i webbläsaravsnittet. Tryck på **[!UICONTROL Save > Close]**.

**_Publiceringsläge (grön indikator) för en resurs återspeglas inte korrekt._**<br> I webbläsarens användargränssnitt krävdes en ominloggning till användargränssnittet för att se rätt publiceringstillstånd för resurserna. I skrivbordsappen har vi introducerat en **[!UICONTROL Refresh]** ikon i verktygsfältet till höger om **[!UICONTROL Select None]** knappen. Tryck på **[!UICONTROL Refresh]** ikonen för att visa den senaste statusen för alla resurser på den angivna sidan. Ingen ominloggning krävs som med webbläsargränssnittet.

![Ikonen](/help/assets/refresh-icon.png)Uppdatera *Uppdatera*

**_Jag ser inte gruppuppsättningsförinställningar som fungerar i skrivbordsappen._**<br> Tryck på **[!UICONTROL Upload > Job Options > Batch Set Presets]**. Kontrollera att relevant **[!UICONTROL Batch Set Preset]** är aktiverat. Klicka på **[!UICONTROL Save and Submit upload]**.
