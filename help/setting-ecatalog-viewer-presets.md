---
title: Konfigurera förinställningar för eCatalog Viewer
description: Lär dig hur du ställer in förinställningar för visningsprogrammet för eCatalog.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
feature: Dynamic Media Classic,visningsprogram,visningsförinställningar,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Konfigurera förinställningar för eCatalog Viewer{#setting-up-ecatalog-viewer-presets}

eCatalog Viewer Presets avgör format, beteende och utseende för eCatalog-visningsprogram. I Dynamic Media Classic finns förinställningar för eCatalog Viewer, och du kan även skapa egna eCatalog Viewer-förinställningar om du är administratör.

Om du vill skapa en förinställning kan du börja från början eller börja med en förinställning för eCatalog Viewer som tillhandahållits av Dynamic Media Classic och spara den under ett nytt namn. Du kan skapa egna visningsförinställningar för eCatalog för att presentera utskrivet material i företagets färger och ställa in tonen.

Förinställningar för eCatalog Viewer ger många inställningar för att gå från sida till sida, zooma, söka och välja&quot;skal&quot;. Hur dessa kontroller ser ut och hur visningsprogrammet ser ut beror på vad du väljer bland förinställningarna för visningsprogrammet för eCatalog.

Följ de här stegen för att skapa en eCatalog Viewer-förinställning (du måste vara administratör):

1. Klicka på **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]** i fältet Global Navigation.
1. Skapa en visningsförinställning för eCatalog genom att starta en ny förinställning eller genom att starta från en befintlig visningsförinställning för eCatalog:

   * **Skapa en förinställning**  för eCatalog Viewer - klicka  **[!UICONTROL Add]**. I dialogrutan Lägg till visningsförinställning väljer du en plattform, väljer eCatalog Viewer och klickar sedan på **[!UICONTROL Add]**.

   * **Redigera en visningsförinställning**  för eCatalog - Välj en visningsförinställning för eCatalog och klicka sedan på Redigera. Klicka på **[!UICONTROL Save As]** när du har skapat förinställningen.

1. Ange ett namn för visningsförinställningen för eCatalog på skärmen Konfigurera visningsprogram.
1. Ange önskade alternativ på skärmen Konfigurera visningsprogram.

   Klicka på ikonen **[!UICONTROL Info Tip]** bredvid alternativet om du vill läsa dess beskrivning.

   På sidan Förhandsgranska visas visningsprogrammet när du uppdaterar och ändrar inställningar.

1. (Valfritt) I **[!UICONTROL Info Panel Settings]** kan alternativet **[!UICONTROL Information Server URL]** innehålla följande speciella tokens, som används av visningsprogrammet:

   | Token | Ersatt med | Anteckningar |
   |--- |--- |--- |
   | `$1$` | rollover_key-värde | Objektidentifieraren från `<area>`-elementet för kartan. |
   | `$2$` | frame | Sekvensnumret för den bildruta som visas i bilduppsättningen. |
   | `$3$` | imageroot | Det första sökvägselementet i det första objektet som anges i bildkommandot (vanligtvis bildkatalog-ID:t för den katalogpost som anger bilduppsättningen). |

1. (Valfritt) I rutan **[!UICONTROL Info Panel Settings]** skriver du den text som du vill ska visas om det uppstår ett fel i Dynamic Media Classic när information för ett bildschema hämtas. **[!UICONTROL Response Template]** Om systemet till exempel tar emot ett företagsnamn och ett eCatalog-namn, men ingen rollover-identifierare, visas det här meddelandet för användaren.

>[!NOTE]
>
>Om du vill använda den här svarsmallen i stället för mallen som är definierad i själva e-katalogen lägger du till `fmt=1` i slutet av informationsserverns URL. Exempel: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Klicka på **Spara**.
1. Klicka på Standard om du vill att den visningsförinställning för eCatalog som du skapade ska vara den som används för att visa e-kataloger på webbsidan.

Om du vill ta bort en visningsförinställning för eCatalog markerar du den på skärmen med visningsförinställningar och klickar på **[!UICONTROL Delete]**.

>[!MORELIKETHIS]
>
>* [Förinställningar för visningsprogram](application-setup.md#viewer_presets)

