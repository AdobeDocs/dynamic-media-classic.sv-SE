---
title: ICC-profiler
seo-title: ICC-profiler
description: 'null'
seo-description: Läs om ICC-profiler.
uuid: 708ff2ad-9a47-4e3e-b643-5b19648f726b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 44f1b4c4-6d7f-4e0f-84ce-11d26745e0f0
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# ICC-profiler{#icc-profiles}

En ICC-profil (International Color Consortium) är en fil som beskriver hur du korrekt konverterar bildfiler från en färgrymd till en annan. ICC-profiler hjälper dig att få rätt färger för dina bilder. Om du till exempel vill visa bilder som är utformade för utskrift på en datorskärm på rätt sätt kan du välja en ICC-profil. Den här profilen konverterar bilden till en annan färgrymd och ser till att färgerna visas korrekt online.

I Scene7 Publishing System kan du välja en ICC-profil för att konvertera bilder till en annan färgrymd när du överför bilderna. Alla vanliga Photoshop ICC-profiler är som standard tillgängliga i SPS. Om du vill visa namnen på färgprofiler på skärmen Överför väljer du menyn Färgprofil. Välj sedan Egen från > Till och välj ett ICC-profilnamn på menyerna Konverterad från och Konverterad till. Se [Bildredigeringsalternativ vid överföring](image-editing-options-upload.md#image-editing-options-at-upload).

Förutom att använda ICC-standardprofilerna kan du överföra andra ICC-profiler till SPS och göra dem tillgängliga för konvertering av färgrymd. Växla till vyn Detalj på panelen Bläddra om du vill undersöka profilklassen, färgrymdstypen och PCS-typen för en ICC-profil.

## Överför ICC-profiler {#uploading-icc-profiles}

Överför ICC-profiler med samma tekniker som du använder för att överföra filer. Du kan lagra ICC-profiler i alla SPS-mappar. Se [Överföra filer](uploading-files.md#uploading_your_files).

## Undersöka en ICC-profil {#examining-an-icc-profile}

Om du vill undersöka en ICC-profil markerar du den på panelen Bläddra och visar den i vyn Detalj. I detaljvyn finns den här informationen om ICC-profiler:

**Profilklass** ICC (International Color Consortium) definierar varje klass så att den omfattar en typ av program. Indataprofiler gäller till exempel enheter som digitalkameror och skannrar, och utdataprofiler gäller för skrivare.

**Färgrymdtyp** Detta är profilens&quot;indatafärgrymd&quot;, enligt ICC:n. Färgrymdtypen definierar antalet komponenter i färgrymden och tolkningen av dessa komponenter. RGB är till exempel en färgrymd med tre komponenter: röd, grön och blå. Färgrymdstypen definierar inte de särskilda färgegenskaperna för färgrymden (t.ex. de kromatoriska egenskaperna för primärfärgerna).

**PCS-typ** Den här PCS-typen är profilens utdatafärgrymd - profilens anslutningsmodell. En färgprofil kan till exempel konvertera RGB till PCS, som sedan konverterar den till CMYK.

För indata-, visnings- eller utdataprofiler som är användbara för att lägga till märkord i färger eller bilder är PCS-typen antingen XYZ eller Lab. Tolka den här profilen som motsvarande specifika färgrymd som definieras i ICC-specifikationen.