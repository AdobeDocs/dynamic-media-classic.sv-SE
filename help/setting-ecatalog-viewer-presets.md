---
title: Konfigurera förinställningar för eCatalog Viewer
seo-title: Konfigurera förinställningar för eCatalog Viewer
description: 'null'
seo-description: Lär dig hur du ställer in förinställningar för visningsprogrammet för eCatalog.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Konfigurera förinställningar för eCatalog Viewer{#setting-up-ecatalog-viewer-presets}

eCatalog Viewer Presets avgör format, beteende och utseende för eCatalog-visningsprogram. Dynamic Media Classic innehåller förinställningar för eCatalog Viewer och du kan skapa egna förinställningar för eCatalog Viewer om du är administratör.

Om du vill skapa en ny förinställning kan du börja från början eller börja med en dynamisk Media Classic-förinställning för eCatalog Viewer och spara den under ett nytt namn. Du kan skapa egna visningsförinställningar för eCatalog för att presentera utskrivet material i företagets färger och ställa in tonen.

Förinställningar för eCatalog Viewer ger många inställningar för att gå från sida till sida, zooma, söka och välja&quot;skal&quot;. Hur dessa kontroller ser ut och hur själva visningsprogrammet ser ut beror på vad du väljer bland förinställningarna för visningsprogrammet för eCatalog.

Så här skapar du en eCatalog Viewer-förinställning (du måste vara administratör):

1. Klicka på **Inställningar** > **Visningsförinställningar**.
1. Skapa en visningsförinställning för eCatalog genom att starta en ny förinställning eller genom att starta från en befintlig visningsförinställning för eCatalog:

   * **Skapa en eCatalog Viewer-förinställning** genom att klicka på Lägg till. I dialogrutan Lägg till visningsförinställning väljer du en plattform, väljer eCatalog Viewer och klickar sedan på **Lägg till**.

   * **Redigera en eCatalog Viewer-förinställning** Välj en visningsförinställning för eCatalog och klicka sedan på Redigera. Klicka på **Spara som** när du har skapat förinställningen.

1. Ange ett namn för visningsförinställningen för eCatalog på skärmen Konfigurera visningsprogram.
1. Ange önskade alternativ på skärmen Konfigurera visningsprogram.

   Klicka på ikonen för informationstips bredvid alternativet om du vill se dess beskrivning.

   Visningsprogrammet visas på förhandsgranskningsskärmen när du uppdaterar och ändrar inställningarna.

1. (Valfritt) I inställningarna på panelen Info kan URL-alternativet för informationsservern innehålla följande särskilda tokens, som visningsprogrammet ersätter:

   | Token | Ersatt med | Anteckningar |
   |--- |--- |--- |
   | `$1$` | rollover_key-värde | Objektidentifieraren från kartans `<area>` element. |
   | `$2$` | frame | Sekvensnumret för den bildruta som visas i bilduppsättningen. |
   | `$3$` | imageroot | Det första sökvägselementet i det första objektet som anges i bildkommandot (vanligtvis bildkatalog-ID:t för den katalogpost som anger bilduppsättningen). |

1. (Valfritt) I inställningarna för informationspanelen skriver du den text som du vill ska visas i rutan Svarsmall om det uppstår ett fel när information för ett bildschema hämtas. Om systemet till exempel tar emot ett företagsnamn och ett eCatalog-namn, men ingen rollover-identifierare, visas det här meddelandet för användaren.

>[!NOTE]
>
>Om du vill använda den här svarsmallen i stället för mallen som är definierad i själva eCatalog lägger du till&quot;fmt=1&quot; i slutet av informationsserverns URL. Exempel: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Klicka på **Spara**.
1. Klicka på Standard om du vill att den visningsförinställning för eCatalog som du skapade ska vara den som används för att visa e-kataloger på webbsidan.

Om du vill ta bort en visningsförinställning för eCatalog markerar du den på skärmen med visningsförinställningar och klickar på **Ta bort**.

>[!MORELIKETHIS]
>
>* [Förinställningar för visningsprogram](application-setup.md#viewer_presets)
