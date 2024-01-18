---
title: Arbeta i detaljvyn
description: Lär dig hur du arbetar i detaljvyn i Adobe Dynamic Media Classic.
uuid: cb62f765-9b7f-4a53-8206-99afae2fb80d
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eaa214ff-d1ef-4691-9148-d01bf243c810
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 618ae6a4-6f60-4a80-b197-a9d35b3c47af
topic: Content Management
level: Intermediate
source-git-commit: ae7d0c6d3047d68ed3da4187ef516dc51c95de30
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# Arbeta i detaljvyn{#working-in-detail-view}

Du kan arbeta med och lära dig mer om en resurs genom att öppna den i detaljvyn. I detaljvyn ser du resursstorlek, attribut, derivat och metadata. Du ser också om och när resursen publicerades och du kan hämta URL:en för publicerade resurser. Beroende på resurstypen kan du förhandsgranska den i olika storlekar, zooma in den och utföra skärpeåtgärder, beskärningsåtgärder och andra formateringsåtgärder.

<!-- 

Comment Type: remark
Last Modified By: Rick Brough (rbrough@adobe.com)
Last Modified Date: 2018-06-14T13:52:46.623-0400

<p>as_detail_view_popup.png found in Downloads on local in folder "scene7-images"</p>

 -->

![Detaljvy](/help/using/assets/image_0.img.png)
*Detaljvy med panelen Resursbibliotek dold från vyn till vänster.*

>[!NOTE]
>
>Om du vill öppna den mapp där resursen lagras kan du markera mappsökvägen högst upp på informationspanelen.

## Öppna en resurs i detaljvyn {#open-an-asset-in-detail-view}

Om du vill granska, förhandsgranska eller arbeta med en resurs kan du visa den i detaljvyn.

1. Gör något av följande i panelen Bläddra:

   * Markera resursen. I Adobe Dynamic Media Classic övre högra hörn väljer du **[!UICONTROL Detail View]** ikon .
   * Dubbelklicka på resursen.
   * Markera resursen och gå sedan till **[!UICONTROL File]** > **[!UICONTROL Details]**.

>[!NOTE]
>
>Du kan gå från resurs till resurs i samma mapp i detaljvyn genom att välja **[!UICONTROL Previous Asset]** eller **[!UICONTROL Next Asset]**. De här knapparna finns i det övre högra hörnet i detaljvyn.

## Hämta information i detaljvyn {#getting-information-in-detail-view}

I detaljvyn finns information om en resurs eller fil. Här visas information om ett objekt: mappen där det lagras, dess filnamn, datumet då objektet överfördes till Adobe Dynamic Media Classic och dess publiceringshistorik. Du kan också visa och redigera metadata och lägga till nyckelord för en resurs i detaljvyn.

Du kan hämta en resurs-URL i detaljvyn, men URL:en är inte aktiv förrän du publicerar resursen. För bilder innehåller detaljvyn även en lista med resurser och metadata som skapats, t.ex. zoommål och bilduppsättningar.

## Arbeta med resurser i detaljvyn {#working-with-assets-in-detail-view}

I detaljvyn finns verktyg som du kan använda för att arbeta med resursen som du har öppnat. Vilka verktyg som är tillgängliga beror på vilken typ av resurs du arbetar med, men detaljvyn har alltid dessa funktioner:

* **objekt för publicering** - Välj **[!UICONTROL Publish]** till vänster om namnet, eller gå till **[!UICONTROL File]** > **[!UICONTROL Publish]** eller **[!UICONTROL File]** > **[!UICONTROL Unpublish]**.

* **Byt namn på resursen** - Markera namnet och ange ett nytt namn.

* **Redigera och lägga till metadata** - Välj panelen Metadata och ändra efter behov. Se [Visa, lägga till och exportera metadata](/help/using/viewing-adding-exporting-metadata.md).

* **Redigera och lägga till nyckelord** - Välj Nyckelord och lägg till eller ta bort dem efter behov. Se [Lägga till eller redigera nyckelord](/help/using/viewing-adding-exporting-metadata.md).

* **Ta bort resursen** - Gå till **[!UICONTROL File]** > **[!UICONTROL Delete]**.

För diskreta filer - t.ex. bilder, bilduppsättningar och teckensnitt - kan du visa publicerings- och redigeringshistorik och kontrollera jobbinformation i detaljvyn.

Tabellen visar vilka andra alternativ som är tillgängliga med olika typer av resurser i detaljvyn.

| Tillgångstyp | Redigera/justera | Förhandsgranska |
| --- | --- | --- |
| Bilder | Lägg till bildscheman<br>Lägg till zoommål<br>Beskär<br>Skärpa<br>Skapa justerade vyer | Ja, förinställningar för zoomning och bild |
| Skåp och fönster som täcker bilder | Nej | Miniatyrbild |
| eCatalogs | Redigera | Ja<br>Informationspanelen är också tillgänglig |
| Typsnitt | Redigera teckensnittsinformation | Nej |
| FXG-filer | Redigera | Ja |
| ICC-profiler | Redigera profilinformation | Nej |
| Illustrator-filer | Nej (om det inte konverterats till FXG) | Nej |
| Bilduppsättningar | Redigera | Ja |
| InDesign | Nej (om det inte konverterats till FXG) | Nej |
| PDF-filer | Nej | Nej |
| PSD-filer | Ja för enskilda lager | Ja för enskilda lager |
| Rotationsset | Redigera | Ja |
| SVG-filer | Nej | Nej |
| Mallar | Redigera | Ja |
| Videor | Nej | Ja |
| Vinjetter och renderade vinjetteringar | Nej | Bilden visas<br>Du kan visa innehållet och strukturen för vinjettens återgivningsbara element i XML-format |
| XML-filer | Nej | Innehållet visas |
| ZIP-filer | Nej | Innehållet visas inte |

>[!MORELIKETHIS]
>
>* [Visa, lägga till och exportera metadata](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
