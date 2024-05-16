---
title: Justera en bild
description: Lär dig justera en bild i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 880ee6d0-cb0a-4d53-9056-f0b8b292136e
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 0%

---

# Justera en bild{#adjusting-an-image}

I Adobe Dynamic Media Classic finns olika kommandon för att justera utseendet på en bild. Du kan vända, rotera, göra oskarpa, ändra färgbalansen och färglägga en bild. När du experimenterar med de här kommandona kan du se hur de påverkar bilden som du arbetar med.

Se även [Skapa ett alias för en bild](adjusting-image.md#creating_an_alias_for_an_image).

**Justera en bild:**

1. Markera bildens redigeringsknapp för överrullning och välj Justera, eller dubbelklicka på bilden i panelen Bläddra så att den öppnas i detaljvyn.
1. Välj en storlek och en bildförinställning (längst ned i fönstret).
1. Använda kommandona till höger i dialogrutan `Adjust Editor` så att du kan justera bilden:

   * Använd alternativen Vänd för att vända en bild vågrätt eller lodrätt.
   * Använd skjutreglaget Rotera för att rotera bilden. Du kan ange värden i fältet Rotera om du vill rotera en bild. Positiva värden roterar det medsols och negativa värden roterar det motsols.
   * Använd reglaget Oskärpa eller motsvarande ruta för att göra en bild oskarp. Ju högre värde, desto suddigare blir bilden.
   * Använd alternativen Kontrast, Intensitet, Mättnad, Nyans och Färgbalans för att justera färg och intensitet. Dessa effekter är kumulativa. Till exempel läggs ändringar i inställningarna för Magenta/Grönt till i ändringarna av nyansinställningarna.
   * Använd `Colorize` alternativ för att färglägga en bild samtidigt som skuggor och högdagrar bevaras. Ändringar av färgalternativen är också kumulativa. På menyn Intensitet väljer du **[!UICONTROL No Compensation]** så att du inaktiverar automatisk ljusstyrkekompensation. Ange kontrastvärdet 0 om du vill bevara det ursprungliga bildens kontrastintervall, eller ange ett kontrastintervall med ett värde som är större än 0. Värdet 100 maximerar kontrasten. Normala värden ligger i intervallet 30-70.

1. När du har justerat bilden gör du något av följande:

   * Välj **[!UICONTROL Save]**.

   * Om du vill ersätta originalbilden väljer du **[!UICONTROL Save As]**.

     Välj **[!UICONTROL Replace original]** och sedan markera **[!UICONTROL Save]**.

   * Om du vill spara bilden som en ny primär bild väljer du **[!UICONTROL Save As]**.

     Välj **[!UICONTROL Save as a new primary]**.
I **[!UICONTROL Folder Name]** väljer du den mapp där du vill spara den nya primära bilden.
Välj **[!UICONTROL Save]**.

   * Spara bilden som en annan vy av den primära bilden. du kan skapa ett alias för det. Välj **[!UICONTROL Save As]**.

     Från listrutan i dialogrutan **[!UICONTROL Save As]** väljer **[!UICONTROL Save as another view of primary]**.
I **[!UICONTROL Folder Name]** väljer du den mapp där du vill spara den nya primära bilden.
Välj **[!UICONTROL Save]**.

## Skapa ett alias för en bild {#creating-an-alias-for-an-image}

När du har justerat en bild kan du spara den som en annan vy av den primära bilden. Om du vill göra det kan du skapa ett alias för bilden med **[!UICONTROL Save as another view of the primary]** -funktion.

**Så här skapar du ett alias för en bild:**

1. I stödrastervyn eller listvyn i **[!UICONTROL Edit]** bredvid en bild som du vill skapa ett alias för väljer du **[!UICONTROL Adjust]**.
1. Välj i det nedre högra hörnet på sidan **[!UICONTROL Save As]**.
1. Från listrutan i dialogrutan **[!UICONTROL Save As]** väljer **[!UICONTROL Save as another view of primary]**.
1. I **[!UICONTROL Folder Name]** väljer du den mapp där du vill spara den utjämnade bilden.
1. I **[!UICONTROL File Name]** anger du namnet som du vill använda för aliaset.
1. Välj **[!UICONTROL Save]**.
