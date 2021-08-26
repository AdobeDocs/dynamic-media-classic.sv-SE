---
title: Hantera papperskorgen
description: Lär dig hur du hanterar papperskorgen.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Hantera papperskorgen{#managing-the-trash-folder}

Objekt som du tar bort från Adobe Dynamic Media Classic flyttas till papperskorgen. De borttagna filerna finns kvar i mappen i sju dagar tills de återställs eller tas bort permanent. Du kan granska borttagna objekt genom att klicka på ikonen **[!UICONTROL Trash]** längst ned i resursbiblioteket och visa objekt på papperskorgsmappens sida.

Alla användare kan återställa objekt i papperskorgen till de mappar som de togs bort från. Alla användare kan också tömma papperskorgen på allt innehåll.

Om du tar bort objekt från papperskorgen tas objekt bort permanent från Adobe Dynamic Media Classic; objekt som tas bort från papperskorgen kan inte längre återställas. Mer information om hur du konfigurerar meddelanden för företagsadministratörer när resurser ska tas bort automatiskt från papperskorgen finns i [Allmänna inställningar för program](application-setup.md#general_settings).

>[!NOTE]
>
>Resurser som har flyttats till papperskorgen registreras fortfarande i Adobe Dynamic Media Classic. Om du försöker överföra en fil som har samma namn som en borttagen fil i papperskorgen behandlas den resurs du vill överföra som en dubblettresurs i Adobe Dynamic Media Classic. Därför läggs ett tal till efter namnet.

## Om papperskorgen {#about-the-trash-folder}

Om du tar bort ett objekt i en mapp placeras objektet i papperskorgen. Följande händer när du tar bort ett objekt och flyttar det till papperskorgen:

* Objektet har tagits bort från dina Adobe Dynamic Media Classic-mappar, men det går inte att tilldela ett annat objekt dess ID medan det finns kvar i papperskorgen. Om du försöker överföra en resurs med samma namn som en fil i papperskorgen lägger Adobe Dynamic Media Classic till en siffra i resursens namn.
* Objektet kan inte publiceras. Även om objektet markerades för publicering när du tog bort det publiceras det inte.
* Objektet finns kvar i papperskorgen tills det återställs, sju dagar framåt eller någon väljer kommandot **[!UICONTROL Empty the Trash]**. Efter sju dagar tas objektet bort permanent vid en automatisk rensning.

## Återställa resurser från papperskorgen {#restoring-assets-from-the-trash-folder}

Den som tagit bort en resurs behöver inte återställa den. alla kan återställa resurser från papperskorgen. Resurser som återställs placeras i de mappar som de har tagits bort från. Om mapparna inte längre finns återskapas de i Adobe Dynamic Media Classic och de återställda resurserna placeras i mapparna som du har skapat igen.

Så här återställer du resurser från papperskorgen till de mappar som de togs bort från:

1. Klicka på ikonen **[!UICONTROL Trash]** längst ned på panelen Resursbibliotek för att öppna papperskorgen.
1. Markera den eller de resurser som du vill återställa.
1. Klicka på **[!UICONTROL File]** > **[!UICONTROL Restore from trash]**.

## Ta bort resurser i papperskorgen permanent {#permanently-deleting-assets-in-the-trash-folder}

När du tar bort resurser i papperskorgen tas resurserna bort permanent. Resurser tas automatiskt bort från papperskorgen efter sju dagar.

Om du vill ta bort resurser permanent från papperskorgen klickar du på ikonen **[!UICONTROL Trash]**. Gör något av följande på sidan Papperskorg:

* **Ta bort enskilda resurser** - Markera de resurser som du vill ta bort permanent och klicka sedan på  **[!UICONTROL File]** >  **[!UICONTROL Empty From Trash]**.

* **Tar bort alla resurser**  - Klicka  **[!UICONTROL File]** >  **[!UICONTROL Empty trash]**.

>[!MORELIKETHIS]
>
>* [Ta bort resurser](moving-renaming-deleting-assets.md#delete_assets)

