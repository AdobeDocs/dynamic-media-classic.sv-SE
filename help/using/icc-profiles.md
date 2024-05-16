---
title: ICC-profiler (International Color Consortium)
description: Läs om ICC-profiler i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
topic: Administration, Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# ICC-profiler{#icc-profiles}

En ICC-profil (International Color Consortium) är en fil som beskriver hur du kan konvertera bildfiler från en färgrymd till en annan på ett korrekt sätt. ICC-profiler hjälper dig att få rätt färger för dina bilder. Om du till exempel vill visa bilder som är utformade för utskrift på en datorskärm på rätt sätt kan du välja en ICC-profil. Den här profilen konverterar bilden till en annan färgrymd och ser till att färgerna visas korrekt online.

I Adobe Dynamic Media Classic kan du välja en ICC-profil för att konvertera bilder till en annan färgrymd när du överför bilderna. Alla Photoshop ICC-standardprofiler är som standard tillgängliga i Adobe Dynamic Media Classic. Om du vill visa namnen på färgprofiler på skärmen Överför väljer du menyn Färgprofil. Välj sedan Egen från > Till och välj ett ICC-profilnamn på menyerna Konverterad från och Konverterad till.

Se [Alternativ för bildredigering vid överföring](image-editing-options-upload.md#image-editing-options-at-upload).

Förutom att använda ICC-standardprofilerna kan du överföra andra ICC-profiler till Adobe Dynamic Media Classic och göra dem tillgängliga för konvertering av färgrymd. Växla till detaljvyn på panelen Bläddra för att undersöka profilklassen, färgrymdstypen och PCS-typen för en ICC-profil.

## Överför ICC-profiler {#uploading-icc-profiles}

Överför ICC-profiler med samma tekniker som du använder för att överföra filer. Du kan spara ICC-profiler i alla Adobe Dynamic Media Classic-mappar.

Se [Överför dina filer](uploading-files.md#uploading_your_files).

## Undersök en ICC-profil {#examining-an-icc-profile}

Om du vill undersöka en ICC-profil markerar du den på panelen Bläddra och visar den i detaljvyn. I detaljvyn finns följande information om ICC-profiler:

* **[!UICONTROL Profile Class]**: ICC (International Color Consortium) definierar varje klass så att den omfattar en typ av program. Indataprofiler gäller till exempel enheter som digitalkameror och skannrar, och utdataprofiler gäller för skrivare.

* **[!UICONTROL Color Space Type]**: Det här talet är profilens&quot;indatafärgrymd&quot;, enligt ICC:n. Färgrymdtypen definierar antalet komponenter i färgrymden och tolkningen av dessa komponenter. RGB är till exempel en färgrymd med tre komponenter: röd, grön och blå. Färgrymdstypen definierar inte de särskilda färgegenskaperna för färgrymden (t.ex. de kromatoriska egenskaperna för primärfärgerna).

* **[!UICONTROL PCS Type]**: Den här PCS-typen är profilens utdatafärgrymd - profilens anslutningsmodell. En färgprofil kan till exempel konvertera RGB till PCS, som sedan konverterar den till CMYK.

För indata-, visnings- eller utdataprofiler som är användbara för att lägga till märkord i färger eller bilder är PCS-typen antingen XYZ eller Lab. Tolka den här profilen som motsvarande specifika färgrymd som definieras i ICC-specifikationen.
