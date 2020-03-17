---
title: Teckensnitt
seo-title: Teckensnitt
description: 'null'
seo-description: Lär dig hur du använder teckensnitt i Dynamic Media Classic.
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Teckensnitt{#fonts}

I vissa fall kräver Scene7 Publishing System att du överför en teckensnittsfil för att ange eller återge text i ett visst teckensnitt. Om du till exempel vill använda ett visst teckensnitt för text i ett mallager överför du teckensnittsfilen. Om du vill visa sidnummer för eCatalog Viewer i ett visst teckensnitt överför du teckensnittsfilen.

Dynamic Media Classic har stöd för följande teckensnittstyper:

* Alla TrueType-teckensnitt
* PostScript®-teckensnitt
* OpenType/TrueType-teckensnitt
* OpenType/PostScript-teckensnitt
* PhotoFonts

När en teckensnittsfil har överförts kan du ändra dess SPS-ID, teckensnittsnamn och typinformation på skärmen Redigera information.

>[!NOTE]
>
>Dynamic Media Classic rekommenderar att du överför alla teckensnittsformat (fet, kursiv, fet/kursiv och normal) om du tänker använda teckensnitt i mallager. Dynamic Media Classic behöver dessa teckensnittsformat för att bearbeta begäranden. Du bör även överföra alla PostScript-/Adobe Type 1-filer som är kopplade till ett teckensnitt eftersom vissa av teckensnitten innehåller detaljerad kerninginformation.

## Överför teckensnittsfiler {#uploading-font-files}

Överför teckensnittsfiler med samma tekniker som du använder för att överföra andra filer. Du kan lagra teckensnittsfiler i alla SPS-mappar. Se [Överföra filer](uploading-files.md#uploading_your_files).

## Redigera teckensnittsfilinformation {#editing-font-file-information}

Du kan ändra ID-namnet för ett teckensnitt och dess typinformation. Att redigera en teckensnittsfil kan vara praktiskt när du söker efter och gör det enklare att identifiera teckensnitt.

I panelen Bläddra markerar du den teckensnittsfil som du vill redigera i vyn Detalj och väljer Arkiv > Redigera info. Skärmen Redigera information öppnas. Välj följande alternativ och välj knappen Skicka.

**Teckensnittsnamn** Det här namnet identifierar teckensnittet när det publiceras.

**PostScript-namn** Det här namnet är det fullständiga PostScript-namnet för teckensnittet. Det anger vanligtvis bredden eller formatet.

**RTF-namn** Det här namnet visas på en snabbmeny i RTF-redigeraren där malltextlager skapas.

**Teckensnittsfamiljenamn** Det här namnet visar teckensnittsnamnet utan indikator för format, vikt eller teckensnittstyp.

**Teckensnittsformat** Alternativen är Normal, Fet, Kursiv och Fet-Kursiv.

**Teckensnittstyp** Alternativen är TrueType och Adobe Type 1. Om du anropar teckensnitten med ett annat namn kan du ange det.

**Typförkortning** Alternativen är följande:

**TTF** TrueType-teckensnittsfiler som används för PDF/PostScript-återgivning och bildvisning.

**AFM** Adobe PostScript-teckensnittsfiler som innehåller Adobe Font Metrics-information och används för bildvisning.

**PFM** Adobe PostScript-teckensnittsfiler som innehåller binär teckensnittsmätningsinformation.

**PFB** Adobe PostScript-teckensnittsfiler som innehåller binär teckensnittskonturinformation och används för PDF/PostScript-återgivning och bildvisning.
