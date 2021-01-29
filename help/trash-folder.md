---
title: Hantera papperskorgen
description: Lär dig hur du hanterar papperskorgen.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---


# Hantera papperskorgen{#managing-the-trash-folder}

Objekt som du tar bort från Dynamic Media Classic flyttas till papperskorgen. De finns kvar i sju dagar i den här mappen tills de återställs eller tas bort permanent. Du kan undersöka borttagna objekt genom att markera papperskorgsikonen längst ned i resursbiblioteket och visa objekt i papperskorgen.

Alla användare kan återställa objekt i papperskorgen till de mappar som de togs bort från. Alla användare kan också tömma papperskorgen på allt innehåll.

Om du tar bort objekt från papperskorgen tas objekt bort permanent från Dynamic Media Classic; objekt som tas bort från papperskorgen kan inte längre återställas. Mer information om hur du konfigurerar meddelanden för företagsadministratörer när resurser ska tas bort automatiskt från papperskorgen finns i [Allmänna inställningar för program](application-setup.md#general_settings).

>[!NOTE]
>
>Resurser som har flyttats till papperskorgen är fortfarande registrerade i Dynamic Media Classic. Om du försöker överföra en fil som har samma namn som en borttagen fil i papperskorgen, behandlas den resurs som du vill överföra som en dubblettresurs i Dynamic Media Classic. Därför läggs ett tal till efter namnet.

## Om papperskorgen {#about-the-trash-folder}

Om du tar bort ett objekt i en mapp placeras objektet i papperskorgen. Följande händer när du tar bort ett objekt och flyttar det till papperskorgen:

* Objektet har tagits bort från dina Dynamic Media Classic-mappar, men det går inte att tilldela ett annat objekt dess ID medan det finns kvar i papperskorgen. Om du försöker överföra en resurs med samma namn som en fil i papperskorgen lägger Dynamic Media Classic till en siffra i resursens namn.
* Objektet kan inte publiceras. Även om objektet markerades för publicering när du tog bort det publiceras det inte.
* Objektet finns kvar i papperskorgen tills det återställs, sju dagar framåt eller någon väljer kommandot Töm papperskorgen. Efter sju dagar tas objektet bort permanent vid en automatisk rensning.

## Återställa resurser från papperskorgen {#restoring-assets-from-the-trash-folder}

Den som tagit bort en resurs behöver inte återställa den. alla kan återställa resurser från papperskorgen. Resurser som återställs placeras i de mappar som de har tagits bort från. Om de här mapparna inte längre finns återskapas de av Dynamic Media Classic och de återställda resurserna placeras i mapparna som du har skapat igen.

Följ de här stegen för att återställa resurser från papperskorgen till de mappar som de togs bort från:

1. Klicka på papperskorgen för att öppna papperskorgen.
1. Markera den eller de resurser som du vill återställa.
1. Välj Arkiv > Återställ från papperskorgen.

## Ta bort resurser permanent i papperskorgen {#permanently-deleting-assets-in-the-trash-folder}

När du tar bort resurser i papperskorgen tas resurserna bort permanent. Resurser tas automatiskt bort från papperskorgen efter sju dagar.

Om du vill ta bort resurser permanent från papperskorgen väljer du papperskorgen för att öppna papperskorgen. Ta sedan bort enskilda resurser eller ta bort alla resurser i mappen:

* **Ta bort enskilda** resurserMarkera de resurser som du vill ta bort permanent och klicka på  **[!UICONTROL File > Empty From Trash]**.

* **Tar bort alla** resurserKlicka  **[!UICONTROL File > Empty Trash]**.

>[!MORELIKETHIS]
>
>* [Ta bort resurser](moving-renaming-deleting-assets.md#delete_assets)

