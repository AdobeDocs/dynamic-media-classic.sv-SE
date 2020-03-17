---
title: 'Arbeta i detaljvyn '
seo-title: 'Arbeta i detaljvyn '
description: 'null'
seo-description: Lär dig hur du arbetar i detaljvyn.
uuid: cb62f765-9b7f-4a53-8206-99afae2fb80d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eaa214ff-d1ef-4691-9148-d01bf243c810
translation-type: tm+mt
source-git-commit: 52f51c59bcc03444e5e751b7b33d20bed9aaaddb

---


# Arbeta i detaljvyn {#working-in-detail-view}

Du kan arbeta med och lära dig mer om en resurs genom att öppna den i detaljvyn. I detaljvyn ser du resursstorlek, attribut, derivat och metadata. Du kan också se om och när resursen publicerades och hämta URL:en för publicerade resurser. Beroende på resurstypen kan du förhandsgranska den i olika storlekar, zooma in den och utföra skärpeåtgärder, beskärningsåtgärder och andra formateringsåtgärder.

<!-- 

Comment Type: remark
Last Modified By: Rick Brough (rbrough@adobe.com)
Last Modified Date: 2018-06-14T13:52:46.623-0400

<p>as_detail_view_popup.png found in Downloads on local in folder "scene7-images"</p>

 -->

![Detaljvy](/help/assets/image_0.img.png)

>[!NOTE]
>
>Om du vill öppna mappen där resursen lagras kan du klicka på mappsökvägen högst upp på informationspanelen.

## Öppna en resurs i detaljvyn {#open-an-asset-in-detail-view}

Om du vill granska, förhandsgranska eller arbeta med en resurs kan du visa den i detaljvyn.

1. Gör något av följande i panelen Bläddra:

   * Dubbelklicka på resursen.
   * Markera resursen och klicka sedan på **[!UICONTROL Detail View]**.
   * Markera resursen och klicka sedan på **[!UICONTROL File > Details]**.

>[!NOTE]
>
>Du kan gå från resurs till resurs i samma mapp i detaljvyn genom att välja knappen Föregående resurs eller Nästa resurs. De här knapparna finns i det övre högra hörnet i vyn Detalj.

## Hämta information i detaljvyn {#getting-information-in-detail-view}

I detaljvyn finns information om en resurs eller fil. Den här informationen om ett objekt visas: mappen där den lagras, dess filnamn, det datum då objektet överfördes till Scene7 Publishing System och dess publiceringshistorik. Du kan också visa och redigera metadata och lägga till nyckelord för en resurs i detaljvyn.

Du kan hämta en resurs-URL i detaljvyn; URL:en är dock inte aktiv förrän du publicerar resursen. För bilder innehåller vyn Detalj även en lista över resurser och metadata som skapats, till exempel zoommål och bilduppsättningar.

## Arbeta med resurser i detaljvyn {#working-with-assets-in-detail-view}

I detaljvyn finns verktyg som du kan använda för att arbeta med den resurs du har öppnat. Vilka verktyg som är tillgängliga beror på vilken typ av resurs du arbetar med, men detaljvyn har alltid dessa funktioner:

* **objekt för publicering** Klicka på **[!UICONTROL Publish]** ikonen till vänster om namnet eller klicka på **[!UICONTROL File > Publish]** eller **[!UICONTROL File > Unpublish]**.

* **Byt namn på resursen** Välj namnet och ange ett nytt namn.

* **Redigera och lägga till metadata** Välj panelen Metadata och gör önskade ändringar. Se [Visa, lägga till och exportera metadata](/help/viewing-adding-exporting-metadata.md).

* **Redigera och lägga till nyckelord** Välj nyckelord och lägg till eller ta bort dem efter behov. Se [Lägga till eller redigera nyckelord](/help/viewing-adding-exporting-metadata.md).

* **Tar bort resursen** Klicka **[!UICONTROL File > Delete]**.

För diskreta filer - t.ex. bilder, bilduppsättningar och teckensnitt - kan du visa publicerings- och redigeringshistoriken och kontrollera jobbinformationen i detaljvyn.

Tabellen visar vilka ytterligare alternativ som är tillgängliga med olika typer av resurser i detaljvyn.

| Tillgångstyp | Redigera/justera | Förhandsgranska |
|--- |--- |--- |
| Bilder | Lägg till bildscheman Lägg till zoommål Beskär skärpa Skapa justerade vyer | Ja, Förinställningar för zoom och bild. |
| Skåp och fönster som täcker bilder | Nej | Miniatyrbild. |
| eCatalogs | Redigera | Ja. Info-panelen är också tillgänglig. |
| Teckensnitt | Redigera teckensnittsinformation | Nej. |
| FXG-filer | Redigera | Ja. |
| ICC-profiler | Redigera profilinformation | Nej. |
| Illustrator-filer | Nej (om det inte konverterats till FXG) | Nej. |
| Bilduppsättningar | Redigera | Ja. |
| InDesign-filer | Nej (om det inte konverterats till FXG) | Nej. |
| PDF-filer | Nej | Nej. |
| PSD-filer | Ja för enskilda lager | Ja för enskilda lager. |
| Rotationsset | Redigera | Ja. |
| SVG-filer | Nej | Nej. |
| Mallar | Redigera | Ja. |
| Videor | Nej | Ja. |
| Vinjetter och renderade vinjetteringar | Nej | Bilden visas. Du kan visa innehållet och strukturen för de återgivningsbara elementen i vinjetteringen i XML-format. |
| XML-filer | Nej | Innehållet visas. |
| ZIP-filer | Nej | Innehållet visas inte. |

>[!MORELIKETHIS]
>
>* [Visa, lägga till och exportera metadata](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)

