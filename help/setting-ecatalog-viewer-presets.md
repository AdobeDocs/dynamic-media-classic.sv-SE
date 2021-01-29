---
title: Konfigurera förinställningar för eCatalog Viewer
description: Lär dig hur du ställer in förinställningar för visningsprogrammet för eCatalog.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 0%

---


# Konfigurera eCatalog Viewer-förinställningar{#setting-up-ecatalog-viewer-presets}

eCatalog Viewer Presets avgör format, beteende och utseende för eCatalog-visningsprogram. Dynamic Media Classic innehåller förinställningar för eCatalog-visningsprogrammet, och du kan även skapa egna förinställningar för eCatalog-visningsprogrammet om du är administratör.

Om du vill skapa en ny förinställning kan du börja från början eller börja med en förinställning för eCatalog Viewer som tillhandahållits av Dynamic Media Classic och spara den under ett nytt namn. Du kan skapa egna visningsförinställningar för eCatalog för att presentera utskrivet material i företagets färger och ställa in tonen.

Förinställningar för eCatalog Viewer ger många inställningar för att gå från sida till sida, zooma, söka och välja&quot;skal&quot;. Hur dessa kontroller ser ut och hur själva visningsprogrammet ser ut beror på vad du väljer bland förinställningarna för visningsprogrammet för eCatalog.

Så här skapar du en eCatalog Viewer-förinställning (du måste vara administratör):

1. Klicka på **Inställningar** > **Visningsförinställningar**.
1. Skapa en visningsförinställning för eCatalog genom att starta en ny förinställning eller genom att starta från en befintlig visningsförinställning för eCatalog:

   * **Skapa en**
förinställning för eCatalog ViewerKlicka på Lägg till. Välj en plattform, välj eCatalog Viewer och klicka sedan på 
**Lägg till**.

   * **Redigera en**
förinställning för eCatalog ViewerVälj en förinställning för eCatalog Viewer och klicka sedan på Redigera. Klicka på 
**Spara** som när du har skapat förinställningen.

1. Ange ett namn för visningsförinställningen för eCatalog på skärmen Konfigurera visningsprogram.
1. Ange önskade alternativ på skärmen Konfigurera visningsprogram.

   Klicka på ikonen för informationstips bredvid alternativet om du vill se dess beskrivning.

   Visningsprogrammet visas på förhandsgranskningsskärmen när du uppdaterar och ändrar inställningarna.

1. (Valfritt) I inställningarna på panelen Info kan URL-alternativet för informationsservern innehålla följande särskilda tokens, som används av visningsprogrammet:

   | Token | Ersatt med | Anteckningar |
   |--- |--- |--- |
   | `$1$` | rollover_key-värde | Objektidentifieraren från `<area>`-elementet för kartan. |
   | `$2$` | frame | Sekvensnumret för den bildruta som visas i bilduppsättningen. |
   | `$3$` | imageroot | Det första sökvägselementet i det första objektet som anges i bildkommandot (vanligtvis bildkatalog-ID:t för den katalogpost som anger bilduppsättningen). |

1. (Valfritt) I inställningarna för informationspanelen skriver du den text som du vill ska visas i rutan Svarsmall om ett fel uppstår när information för ett bildschema hämtas från Dynamic Media Classic. Om systemet till exempel tar emot ett företagsnamn och ett eCatalog-namn, men ingen rollover-identifierare, visas det här meddelandet för användaren.

>[!NOTE]
>
>Om du vill använda den här svarsmallen i stället för mallen som är definierad i själva eCatalog lägger du till&quot;fmt=1&quot; i slutet av informationsserverns URL. Exempel: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Klicka på **Spara**.
1. Klicka på Standard om du vill att den visningsförinställning för eCatalog som du skapade ska vara den som används för att visa e-kataloger på webbsidan.

Om du vill ta bort en visningsförinställning för eCatalog markerar du den på skärmen Förinställningar för visningsprogram och klickar på **Ta bort**.

>[!MORELIKETHIS]
>
>* [Förinställningar för visningsprogram](application-setup.md#viewer_presets)

