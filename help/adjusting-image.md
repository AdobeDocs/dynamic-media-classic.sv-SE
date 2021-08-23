---
title: Justera en bild
description: Läs om hur du justerar en bild i Dynamic Media Classic.
uuid: c052acd3-e8c1-4134-ad21-b9c41578097f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 47a23980-2886-4da3-ab2d-6cd50e00d188
feature: Dynamic Media Classic,Resurshantering
role: User
exl-id: 880ee6d0-cb0a-4d53-9056-f0b8b292136e
source-git-commit: 1d30c98b76ebe78ff60bae87bd112de7a577182d
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 0%

---

# Justera en bild{#adjusting-an-image}

I Dynamic Media Classic finns olika kommandon för att justera utseendet på en bild. Du kan vända, rotera, göra oskarpa, ändra färgbalansen och färglägga en bild. När du experimenterar med de här kommandona kan du se hur de påverkar bilden som du arbetar med.

Se även [Skapa ett alias för en bild](adjusting-image.md#creating_an_alias_for_an_image).

**Justera en bild:**

1. Markera bildens redigeringsknapp för överrullning och välj Justera, eller dubbelklicka på bilden i panelen Bläddra så att den öppnas i vyn Detalj.
1. Välj en storlek och en bildförinställning (längst ned i fönstret).
1. Använd kommandona till höger i fönstret Justera redigerare för att justera bilden:

   * Använd alternativen Vänd för att vända en bild vågrätt eller lodrätt.
   * Använd skjutreglaget Rotera för att rotera bilden. Du kan ange värden i fältet Rotera om du vill rotera en bild. Positiva värden roterar det medsols; negativa värden roterar det motsols.
   * Använd reglaget Oskärpa eller motsvarande ruta för att göra en bild oskarp. Ju högre värde, desto suddigare blir bilden.
   * Använd alternativen Kontrast, Intensitet, Mättnad, Nyans och Färgbalans för att justera färg och intensitet. Dessa effekter är kumulativa. Till exempel läggs ändringar i inställningarna för Magenta/Grönt till i ändringarna av nyansinställningarna.
   * Använd färgalternativen för att färglägga en bild samtidigt som skuggor och högdagrar bevaras. Ändringar av färgalternativen är också kumulativa. Välj **[!UICONTROL No Compensation]** på menyn Intensitet så att du inaktiverar automatisk intensitetskompensation. Ange kontrastvärdet 0 om du vill bevara det ursprungliga bildens kontrastintervall, eller ange ett kontrastintervall med ett värde som är större än 0. Värdet 100 maximerar kontrasten. Normala värden ligger i intervallet 30-70.

1. När du har justerat bilden gör du något av följande:

   * Välj **[!UICONTROL Save]**.

   * Om du vill ersätta originalbilden väljer du **[!UICONTROL Save As]**.

      Välj **[!UICONTROL Replace original]** i listrutan och välj sedan **[!UICONTROL Save]**.

   * Om du vill spara bilden som en ny överordnad bild väljer du **[!UICONTROL Save As]**.

      I listrutan  väljer du **[!UICONTROL Save as new master]**.
I listrutan **[!UICONTROL Folder Name]** väljer du den mapp där du vill spara den nya överordnad bilden.
Välj **[!UICONTROL Save]**.

   * Spara bilden som en annan vy av den överordnad bilden. du kan skapa ett alias för det. Välj **[!UICONTROL Save As]**.

      Välj **[!UICONTROL Save as another view of master]** i listrutan i dialogrutan **[!UICONTROL Save As]**.
I listrutan **[!UICONTROL Folder Name]** väljer du den mapp där du vill spara den nya överordnad bilden.
Välj **[!UICONTROL Save]**.

## Skapa ett alias för en bild {#creating-an-alias-for-an-image}

När du har justerat en bild kan du spara den som en annan vy av den överordnad bilden. Om du vill göra det kan du skapa ett alias för bilden med funktionen **[!UICONTROL Save as additional view of master]**.

**Så här skapar du ett alias för en bild:**

1. I Stödrastervisning eller listvy väljer du **[!UICONTROL Adjust]** i listrutan **[!UICONTROL Edit]** bredvid en bild som du vill skapa ett alias för.
1. Välj **[!UICONTROL Save As]** längst ned till höger på sidan.
1. Välj **[!UICONTROL Save as additional view of master]** i listrutan i dialogrutan **[!UICONTROL Save As]**.
1. I listrutan **[!UICONTROL Folder Name]** väljer du den mapp där du vill spara den utjämnade bilden.
1. I fältet **[!UICONTROL File Name]** skriver du namnet som du vill använda för aliaset.
1. Välj **[!UICONTROL Save]**.
