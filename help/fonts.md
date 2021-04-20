---
title: Teckensnitt
description: Lär dig hur du använder teckensnitt i Dynamic Media Classic.
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---


# Teckensnitt{#fonts}

I vissa fall kräver Dynamic Media Classic att du överför en teckensnittsfil för att ange eller återge text i ett visst teckensnitt. Om du till exempel vill använda ett visst teckensnitt för text i ett mallager överför du teckensnittsfilen. Om du vill visa sidnummer för eCatalog Viewer i ett visst teckensnitt överför du teckensnittsfilen.

Dynamic Media Classic stöder följande teckensnittstyper:

* Alla TrueType-teckensnitt
* PostScript®
* OpenType/TrueType-teckensnitt
* OpenType-/PostScript-teckensnitt
* PhotoFonts

När en teckensnittsfil har överförts kan du ändra dess Dynamic Media Classic-ID, teckensnittsnamn och typinformation på skärmen Redigera information.

>[!NOTE]
>
>Dynamic Media Classic rekommenderar att du överför alla teckensnittsformat (fet, kursiv, fet/kursiv och normal) om du tänker använda teckensnitt i mallager. Dessa teckensnittsformat behövs för att bearbeta begäranden i Dynamic Media Classic. Du bör även överföra alla PostScript/Adobe Type 1-filer som är kopplade till ett teckensnitt eftersom vissa av teckensnitten innehåller detaljerad kerninginformation.

## Överför teckensnittsfiler {#uploading-font-files}

Överför teckensnittsfiler med samma tekniker som du använder för att överföra andra filer. Du kan spara teckensnittsfiler i alla Dynamic Media Classic-mappar. Se [Överföra filer](uploading-files.md#uploading_your_files).

## Redigera teckensnittsfilinformation {#editing-font-file-information}

Du kan ändra ID-namnet för ett teckensnitt och dess typinformation. Att redigera en teckensnittsfil kan vara praktiskt när du söker efter och gör det enklare att identifiera teckensnitt.

I panelen Bläddra markerar du den teckensnittsfil som du vill redigera i vyn Detalj och väljer Arkiv > Redigera info. Skärmen Redigera information öppnas. Välj följande alternativ och välj knappen Skicka.

**Teckensnittsnamn** Det här namnet identifierar teckensnittet när det publiceras.

**PostScript-** namnDet här namnet är det fullständiga PostScript-namnet för teckensnittet. Det anger vanligtvis bredden eller formatet.

**RTF-** namnDet här namnet visas på en snabbmeny i RTF-redigeraren där malltextlager skapas.

**Teckensnittsfamilj** NamnDet här namnet visar teckensnittsnamnet utan indikator för format, vikt eller teckensnittstyp.

**Teckensnittsformat** Alternativen är Normal, Fet, Kursiv och Fet-Kursiv.

**Teckensnittstyp** Alternativen är TrueType och Adobe Type 1. Om du anropar teckensnitten med ett annat namn kan du ange det.

**Teckensnittstyp** FörkortningAlternativen är följande:

**TTFTrueType-** teckensnittsfiler som används för PDF/PostScript-återgivning och bildvisning.

**** AFMAdobe PostScript-teckensnittsfiler som innehåller Adobe Font Metrics-information och används för bildvisning.

**** PFMAdobe PostScript-teckensnittsfiler som innehåller binär teckensnittsmätningsinformation.

**** PFBAdobe PostScript-teckensnittsfiler som innehåller binär teckensnittskonturinformation och används för PDF/PostScript-återgivning och bildvisning.
