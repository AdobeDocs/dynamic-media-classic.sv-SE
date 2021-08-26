---
title: Teckensnitt
description: Läs om hur du använder teckensnitt i Adobe Dynamic Media Classic.
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Teckensnitt{#fonts}

Ibland kräver Adobe Dynamic Media Classic att du överför en teckensnittsfil för att ange eller återge text i ett visst teckensnitt. Om du till exempel vill använda ett visst teckensnitt för text i ett mallager överför du teckensnittsfilen. Om du vill visa sidnummer för eCatalog Viewer i ett visst teckensnitt överför du teckensnittsfilen.

Adobe Dynamic Media Classic stöder följande teckensnittstyper:

* Alla TrueType-teckensnitt
* PostScript®
* OpenType/TrueType-teckensnitt
* OpenType-/PostScript-teckensnitt
* PhotoFonts

När en teckensnittsfil har överförts kan du ändra dess Adobe Dynamic Media Classic-ID, teckensnittsnamn och typinformation på skärmen Redigera information.

>[!NOTE]
>
>Adobe Dynamic Media Classic rekommenderar att du överför alla teckensnittsformat (fet, kursiv, fet/kursiv och normal) om du tänker använda teckensnitt i mallager. Adobe Dynamic Media Classic behöver dessa teckensnittsformat för att kunna bearbeta begäranden. Du bör även överföra alla PostScript-/Adobe Type1-filer som är kopplade till ett teckensnitt eftersom vissa av teckensnitten innehåller detaljerad kerninginformation.

## Överför teckensnittsfiler {#uploading-font-files}

Överför teckensnittsfiler med samma tekniker som du använder för att överföra andra filer. Du kan spara teckensnittsfiler i alla Adobe Dynamic Media Classic-mappar. Se [Överföra filer](uploading-files.md#uploading_your_files).

## Redigera teckensnittsfilinformation {#editing-font-file-information}

Du kan ändra ID-namnet för ett teckensnitt och dess typinformation. Att redigera en teckensnittsfil kan vara praktiskt när du söker efter och gör det enklare att identifiera teckensnitt.

I panelen Bläddra markerar du den teckensnittsfil som du vill redigera i detaljvyn och väljer Arkiv > Redigera information. Skärmen Redigera information öppnas. Välj följande alternativ och välj sedan **[!UICONTROL Submit]**.

* **[!UICONTROL Font Name]** - Det här namnet identifierar teckensnittet när det publiceras.

* **[!UICONTROL PostScript Name]** - Det här namnet är det fullständiga PostScript-namnet för teckensnittet. Det anger vanligtvis bredden eller formatet.

* **[!UICONTROL RTF Name]** - Det här namnet visas på en snabbmeny i RTF-redigeraren där malltextlager skapas.

* **[!UICONTROL Font Family Name]** - Det här namnet visar teckensnittsnamnet utan tecken på format, bredd eller teckensnittstyp.

* **[!UICONTROL Font Style]** - Alternativen är Normal, Fet, Kursiv och Fet-Kursiv.

* **[!UICONTROL Font Type]** - Alternativen är TrueType och Adobe Type 1. Om du anropar teckensnitten med ett annat namn kan du ange det.

* **[!UICONTROL Font Type Abbreviation]** - Alternativen är följande:

   * **[!UICONTROL TTF]** - TrueType-teckensnittsfiler som används för PDF/PostScript-återgivning och bildvisning.

   * **[!UICONTROL AFM]** - Adobe PostScript teckensnittsfiler som innehåller Adobe-teckensnittsmått och som används för bildvisning.

   * **[!UICONTROL PFM]** - Adobe PostScript teckensnittsfiler som innehåller binär teckensnittsmätningsinformation.

   * **[!UICONTROL PFB]** - Adobe PostScript teckensnittsfiler som innehåller binär teckensnittskonturinformation och används för PDF/PostScript-återgivning och bildvisning.
