---
title: Konfigurera förinställningar för eCatalog Viewer
description: Lär dig hur du ställer in förinställningar för eCatalog Viewer i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
topic: Integrations, Development
level: Experienced
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# Konfigurera förinställningar för eCatalog Viewer{#setting-up-ecatalog-viewer-presets}

eCatalog Viewer Presets avgör format, beteende och utseende för eCatalog-visningsprogram. Adobe Dynamic Media Classic tillhandahåller eCatalog Viewer-förinställningar och du kan även skapa egna eCatalog Viewer-förinställningar om du är administratör.

Om du vill skapa en förinställning kan du börja från början eller börja med en förinställning för eCatalog Viewer som tillhandahållits av Adobe Dynamic Media Classic och spara den under ett nytt namn. Du kan skapa egna visningsförinställningar för eCatalog för att presentera utskrivet material i företagets färger och ställa in tonen.

Förinställningar för eCatalog Viewer ger många inställningar för att gå från sida till sida, zooma, söka och välja&quot;skal&quot;. Hur dessa kontroller ser ut och hur visningsprogrammet ser ut beror på vad du väljer bland förinställningarna för visningsprogrammet för eCatalog.

Följ de här stegen för att skapa en eCatalog Viewer-förinställning (du måste vara administratör):

1. I fältet Global Navigation går du till **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.
1. Skapa en visningsförinställning för eCatalog genom att starta en ny förinställning eller genom att starta från en befintlig visningsförinställning för eCatalog:

   * **Skapa en förinställning för eCatalog Viewer**: Välj **[!UICONTROL Add]**. I dialogrutan Lägg till visningsförinställning väljer du en plattform, väljer eCatalog Viewer och sedan **[!UICONTROL Add]**.

   * **Redigera en förinställning för eCatalog Viewer**: Välj en visningsförinställning för eCatalog och välj sedan **[!UICONTROL Edit]**. Välj **[!UICONTROL Save As]** när du har skapat förinställningen.

1. På `Configure Viewer` anger du ett namn för visningsförinställningen för eCatalog.
1. På `Configure Viewer` anger du önskade alternativ.

   välj **[!UICONTROL Info Tip]** -ikonen bredvid alternativet om du vill läsa dess beskrivning.

   På sidan Förhandsgranska visas visningsprogrammet när du uppdaterar och ändrar inställningar.

1. (Valfritt) I dialogrutan **[!UICONTROL Info Panel Settings]**, **[!UICONTROL Information Server URL]** kan innehålla följande speciella tokens som används av användaren:

   | Token | Ersatt med | Anteckningar |
   | --- | --- | --- |
   | `$1$` | rollover_key-värde | Objektidentifieraren från `<area>` kartelementet. |
   | `$2$` | frame | Sekvensnumret för den bildruta som visas i bilduppsättningen. |
   | `$3$` | bildrot | Det första sökvägselementet i det första objektet som anges i bildkommandot (vanligtvis bildkatalog-ID:t för den katalogpost som anger bilduppsättningen). |

1. (Valfritt) I dialogrutan **[!UICONTROL Info Panel Settings]**, i **[!UICONTROL Response Template]** skriver du den text som du vill ska visas om Adobe Dynamic Media Classic stöter på ett fel när information hämtas för en bildschema. Om systemet till exempel tar emot ett företagsnamn och ett eCatalog-namn, men ingen rollover-identifierare, visas det här meddelandet för användaren.

>[!NOTE]
>
>Om du vill använda den här svarsmallen i stället för mallen som är definierad i själva e-katalogen lägger du till `fmt=1` till slutet av informationsserverns URL. Till exempel: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Välj **[!UICONTROL Save]**.
1. Välj **[!UICONTROL Default]** så att den visningsförinställning för eCatalog som du skapade används för att visa e-kataloger på webbsidan.

Om du vill ta bort en visningsförinställning för eCatalog markerar du den på skärmen med visningsförinställningar och väljer **[!UICONTROL Delete]**.

>[!MORELIKETHIS]
>
>* [Förinställningar för visningsprogram](application-setup.md#viewer_presets)
