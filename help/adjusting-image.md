---
title: Justera en bild
description: Lär dig hur du justerar en bild i Adobe Dynamic Media Classic.
uuid: c052acd3-e8c1-4134-ad21-b9c41578097f
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 47a23980-2886-4da3-ab2d-6cd50e00d188
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 880ee6d0-cb0a-4d53-9056-f0b8b292136e
source-git-commit: 972e5d4f468f14bd40e970c989465a639fd5e6fb
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Justera en bild{#adjusting-an-image}

I Adobe Dynamic Media Classic finns olika kommandon för att justera utseendet på en bild. Du kan vända, rotera, göra oskarpa, ändra färgbalansen och färglägga en bild. När du experimenterar med de här kommandona kan du se hur de påverkar bilden som du arbetar med.

Se även [Skapa ett alias för en bild](adjusting-image.md#creating_an_alias_for_an_image).

**Justera en bild:**

1. Markera bildens redigeringsknapp för överrullning och välj Justera, eller dubbelklicka på bilden i panelen Bläddra så att den öppnas i detaljvyn.
1. Välj en storlek och en bildförinställning (längst ned i fönstret).
1. Använd kommandona till höger i fönstret Justera redigerare för att justera bilden:

   * Använd alternativen Vänd för att vända en bild vågrätt eller lodrätt.
   * Använd skjutreglaget Rotera för att rotera bilden. Du kan ange värden i fältet Rotera om du vill rotera en bild. Positiva värden roterar det medsols; negativa värden roterar det motsols.
   * Använd reglaget Oskärpa eller motsvarande ruta för att göra en bild oskarp. Ju högre värde, desto suddigare blir bilden.
   * Använd alternativen Kontrast, Intensitet, Mättnad, Nyans och Färgbalans för att justera färg och intensitet. Dessa effekter är kumulativa. Till exempel läggs ändringar i inställningarna för Magenta/Grönt till i ändringarna av nyansinställningarna.
   * Använd färgalternativen för att färglägga en bild samtidigt som skuggor och högdagrar bevaras. Ändringar av färgalternativen är också kumulativa. På menyn Intensitet väljer du **[!UICONTROL No Compensation]** så att du inaktiverar automatisk intensitetskompensation. Ange kontrastvärdet 0 om du vill bevara det ursprungliga bildens kontrastintervall, eller ange ett kontrastintervall med ett värde som är större än 0. Värdet 100 maximerar kontrasten. Normala värden ligger i intervallet 30-70.

1. När du har justerat bilden gör du något av följande:

   * Välj **[!UICONTROL Save]**.

   * Om du vill ersätta originalbilden väljer du **[!UICONTROL Save As]**.

      Välj **[!UICONTROL Replace original]** och sedan markera **[!UICONTROL Save]**.

   * Om du vill spara bilden som en ny primär bild väljer du **[!UICONTROL Save As]**.

      Välj **[!UICONTROL Save as new master]**.
I **[!UICONTROL Folder Name]** väljer du den mapp där du vill spara den nya primära bilden.
Välj **[!UICONTROL Save]**.

   * Spara bilden som en annan vy av den primära bilden. du kan skapa ett alias för det. Välj **[!UICONTROL Save As]**.

      I **[!UICONTROL Save As]** väljer du **[!UICONTROL Save as another view of master]**.
I **[!UICONTROL Folder Name]** väljer du den mapp där du vill spara den nya primära bilden.
Välj **[!UICONTROL Save]**.

## Skapa ett alias för en bild {#creating-an-alias-for-an-image}

När du har justerat en bild kan du spara den som en annan vy av den primära bilden. Om du vill göra det kan du skapa ett alias för bilden med **[!UICONTROL Save as additional view of master]** -funktion.

**Så här skapar du ett alias för en bild:**

1. I stödrastervyn eller listvyn i **[!UICONTROL Edit]** bredvid en bild som du vill skapa ett alias för väljer du **[!UICONTROL Adjust]**.
1. Välj **[!UICONTROL Save As]**.
1. I **[!UICONTROL Save As]** väljer du **[!UICONTROL Save as additional view of master]**.
1. I **[!UICONTROL Folder Name]** väljer du den mapp där du vill spara den utjämnade bilden.
1. I **[!UICONTROL File Name]** anger du namnet som du vill använda för aliaset.
1. Välj **[!UICONTROL Save]**.
