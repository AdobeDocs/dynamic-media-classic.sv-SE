---
title: Hantera papperskorgen
description: Lär dig hur du hanterar papperskorgen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Hantera papperskorgen{#managing-the-trash-folder}

Objekt som du tar bort från Adobe Dynamic Media Classic flyttas till papperskorgen. Dessa borttagna objekt finns kvar i mappen i sju dagar tills de återställs eller tas bort permanent. Du kan undersöka borttagna objekt genom att markera ikonen **[!UICONTROL Trash]** längst ned i resursbiblioteket och visa objekt på sidan Papperskorg.

Alla användare kan återställa objekt i papperskorgen till de mappar som de togs bort från. Alla användare kan också tömma papperskorgen på allt innehåll.

Om du tar bort objekt från papperskorgen tas objekt från Adobe Dynamic Media Classic bort permanent. Objekt som tas bort från papperskorgen kan inte längre återställas. Mer information om hur du konfigurerar meddelanden för företagsadministratörer när resurser ska tas bort automatiskt från papperskorgen finns i [Allmänna inställningar för program](application-setup.md#general_settings).

>[!NOTE]
>
>Assets som har flyttats till papperskorgen är fortfarande registrerade i Adobe Dynamic Media Classic. Anta till exempel att du försöker överföra en fil som har samma namn som en borttagen fil i papperskorgen. Adobe Dynamic Media Classic behandlar den resurs som du vill överföra som en dubblettresurs. I så fall läggs ett tal till efter namnet.

## Om papperskorgen {#about-the-trash-folder}

Om du tar bort ett objekt i en mapp placeras objektet i papperskorgen. Följande händer när du tar bort ett objekt och flyttar det till papperskorgen:

* Objektet tas bort från din Adobe Dynamic Media Classic-mapp, men det går inte att tilldela det till en annan resurs medan det finns kvar i papperskorgen. Om du försöker överföra en resurs med samma namn som en fil i papperskorgen lägger Adobe Dynamic Media Classic till ett nummer i resursens namn.
* Objektet kan inte publiceras. Även om objektet markerades för publicering när du tog bort det publiceras det inte.
* Objektet finns kvar i papperskorgen tills det återställs, sju dagar framåt eller någon väljer kommandot **[!UICONTROL Empty the Trash]**. Efter sju dagar tas objektet bort permanent vid en automatisk rensning.

## Återställ resurser från papperskorgen {#restoring-assets-from-the-trash-folder}

Den som har tagit bort en resurs behöver inte återställa den. Alla kan återställa resurser från papperskorgen. Assets som återställs placeras i de mappar som de har tagits bort från. Om mapparna inte längre finns återskapas de av Adobe Dynamic Media Classic och de återställda resurserna placeras i de mappar som du har skapat igen.

Så här återställer du resurser från papperskorgen till de mappar som de togs bort från:

1. Längst ned på panelen Resursbibliotek väljer du ikonen **[!UICONTROL Trash]** för att öppna papperskorgen.
1. Markera den eller de resurser som du vill återställa.
1. Gå till **[!UICONTROL File]** > **[!UICONTROL Restore from trash]**.

## Ta bort resurser i papperskorgen permanent {#permanently-deleting-assets-in-the-trash-folder}

När du tar bort resurser i papperskorgen tas resurserna bort permanent. Assets tas automatiskt bort från papperskorgen efter sju dagar.

Du kan ta bort resurser permanent från papperskorgen genom att markera ikonen **[!UICONTROL Trash]**. Gör något av följande på sidan Papperskorg:

* **Tar bort enskilda resurser**: Du kan ta bort resurser permanent. Markera de resurser som du vill ha och klicka sedan på **[!UICONTROL File]** > **[!UICONTROL Empty From Trash]**.

* **Tar bort alla resurser**: Gå till **[!UICONTROL File]** > **[!UICONTROL Empty trash]**.

>[!MORELIKETHIS]
>
>* [Ta bort resurser](moving-renaming-deleting-assets.md#delete_assets)
