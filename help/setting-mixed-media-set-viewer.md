---
title: Konfigurera en visningsförinställning för blandad medieuppsättning
description: Lär dig hur du ställer in en visningsförinställning för en blandad medieuppsättning i Adobe Dynamic Media Classic.
uuid: d5bf1840-e453-445d-bebc-84889b29f3c8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
discoiquuid: 8029aad8-d696-4d7c-99e2-3b08edb68181
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: d41b30e7-994a-43f3-8698-7dbfc36305ae
source-git-commit: e47c22508230adbb1ece323be0c1413a3f27ad89
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# Konfigurera en visningsförinställning för blandad medieuppsättning{#setting-up-a-mixed-media-set-viewer-preset}

Visningsförinställningarna för den blandade medieuppsättningen avgör formatet, beteendet och utseendet på huvudvisningsprogrammet. När du konfigurerar en förinställning anger du vilka andra visningsprogram du vill ska visas i visningsprogrammet för blandade media. Om du t.ex. har inkluderat en bilduppsättning i din uppsättning med blandade media anger du en förinställning för bilduppsättningsvisningsprogrammet för visningsprogrammet för den blandade medieuppsättningen.

Du kan välja att ta med alla eller vissa communityfunktioner i visningsprogrammet för den blandade medieuppsättningen. Med funktionen Bädda in läggs en länk till visningsprogrammet som gör att användarna kan kopiera den kod som krävs för att visa visningsprogrammet på en extern sida (till exempel en blogg, en webbplats eller en social nätverksplats). Länkfunktionen tillhandahåller URL:en till visningsprogrammet, så att användare kan länka tillbaka till det här visningsprogrammet. Besöksfunktionen tillhandahåller en länk till den webbplats du anger.

1. Gå till **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]** i fältet Global Navigation.
1. Gör något av följande på sidan Förinställningar för visningsprogram:

   * Välj **[!UICONTROL Add]** om du vill skapa en förinställning. I dialogrutan Lägg till visningsförinställning väljer du en plattform, väljer **[!UICONTROL Mixed Media Set Viewer]** och sedan **[!UICONTROL Add]**.
   * Om du vill redigera en förinställning för visningsprogrammet för blandad medieuppsättning markerar du den och väljer **[!UICONTROL Edit]**.

1. Skriv ett namn i rutan Förinställningsnamn för visningsprogrammet för den blandade medieuppsättningen på sidan för Configuration Viewer.
1. Ange **[!UICONTROL Tabs]** eller **[!UICONTROL No Tabs]**. Flikar separerar objekt efter typ, t.ex. videoklipp, färgrutor och snurra uppsättningar. När du inte anger några flikar visas alla objekt på en rad i förhandsgranskningsfönstret.
1. I rutan **[!UICONTROL Name]** anger du ett namn för det visningsprogram som du vill lägga till.

   Om du till exempel lägger till en färgruteuppsättning i den blandade medieuppsättningen skriver du `Swatch Set A`.

1. Välj vilken typ av resurs du vill visa på menyn Visare, t.ex. Uppsättningar med färgrutor.
1. Välj en förinställning för den valda resurstypen på menyn Förinställning.

   Om du till exempel lägger till en färgruteuppsättning väljer du **[!UICONTROL SwatchSet1-Colors]**.

1. Välj **[!UICONTROL Add]**.

   Den nya visningsförinställningen visas i listan.

1. Upprepa steg 6-9 för alla visningsprogramförinställningar som du vill lägga till.
1. Om du vill redigera förinställningslistan gör du något av följande:

   * Om du vill ta bort en förinställning från listan markerar du den och väljer **[!UICONTROL Delete]**.
   * Om du vill ändra ordning på förinställningarna i listan markerar du en förinställning och väljer den blå pilen **[!UICONTROL Up]** eller **[!UICONTROL Down]**.

1. Om du vill lägga till communityfunktioner (Bädda in, Länk, Besök) i visningsprogrammet anger du alternativ för något av följande:

   * **E-post**  - Välj  **[!UICONTROL On]** om du vill aktivera en e-postknapp i visningsprogrammet. När användare väljer knappen E-post när de visar uppsättningen öppnas ett e-postmeddelande med länken till uppsättningen.

   * **Bädda in**  - Välj  **[!UICONTROL Live]**. I rutan Bädda in knappetikett skriver du det namn som du vill ska visas i visningsprogrammet för knappen Bädda in. Om du vill kan du markera **[!UICONTROL Browse]** för att hitta och välja ett anpassat skal för knappen.

   * **Länk**  - Välj  **[!UICONTROL Live]**. Skriv det namn som du vill ska visas i visningsprogrammet för knappen Länk i rutan Länkknappsetikett. Om du vill kan du markera **[!UICONTROL Browse]** för att hitta och välja ett anpassat skal för knappen.

   * **Besök**  - Välj  **[!UICONTROL Live]**. I rutan Besök knappetikett skriver du det namn som du vill ska visas i visningsprogrammet för knappen Besök. I rutan Besök URL skriver du URL-adressen till den webbplats som du vill öppna när du klickar på länken.

1. Ange andra alternativ efter behov. Om du vill visa en beskrivning av ett alternativ väljer du ikonen Tips för information bredvid alternativet.

   På sidan Förhandsgranska visas visningsprogrammet när du uppdaterar och ändrar inställningar.

1. Välj **[!UICONTROL Save]**.

>[!MORELIKETHIS]
>
>* [Skapa och redigera visningsförinställningar](application-setup.md#adding_and_editing_viewer_presets)

