---
title: Exportera resurser från Adobe Dynamic Media Classic
description: Lär dig exportera resurser från Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Exportera resurser från Adobe Dynamic Media Classic{#exporting-assets-from-dmc}

Du kan spara resurser som du har redigerat i Adobe Dynamic Media Classic på en lokal nätverksenhet. Exporterade resurser paketeras i en ZIP-fil för nedladdning eller sändning via e-post.

Den komprimerade ZIP-filen har en maximal filstorlek på 1 GB för exportjobbet. Du får dessutom högst 500 totala resurser per exportjobb.

Adobe Dynamic Media Classic sparar uppgifter om exportering av jobb på jobbskärmen.

**Så här exporterar du resurser från Adobe Dynamic Media Classic:**

1. Markera de resurser som du vill exportera och gå sedan till **[!UICONTROL File]** > **[!UICONTROL Export]**.
1. I fönstret Exportera markerade resurser klickar du på **[!UICONTROL Image Options]** och ange sedan något av följande alternativ (administratörer avgör vilka alternativ som är tillgängliga för användarna):

   * **[!UICONTROL Presets]**: Om du vill kan du välja en bildförinställning för att formatera resursen när du exporterar den. Om du väljer en bildförinställning är de andra formateringsalternativen inte tillgängliga eftersom resursen använder de format som definieras i bildförinställningen.

   * **[!UICONTROL Conversion]**: Konvertera resursfilen eller originalbilden.

   * **[!UICONTROL Size]**: Du kan välja en standardstorlek. Du kan också välja **[!UICONTROL Other]** från **[!UICONTROL Size]** väljer du önskad måttenhet och anger sedan bredd och höjd.

     Se även [Ange exportalternativ som är tillgängliga för Media Portal-användare](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * **[!UICONTROL Format]**: Välj ett bildformat.

   * **[!UICONTROL Color]**: Välj RGB, CMYK eller Grå.

   * **[!UICONTROL Resolution]**: Välj 72 ppi, 150 ppi eller 300 ppi.

   * **[!UICONTROL Job Name]**: Du kan tilldela ett jobbnamn till exporten.

   * **[!UICONTROL Send Email To]**: Valfritt. Ange en e-postadress om du tänker skicka resurserna via e-post. I e-postmeddelandet visas den URL där mottagaren kan gå för att hämta resurserna.

1. Välj **[!UICONTROL Export]**.

Tre grundläggande exportåtgärder stöds:

* Originalfil (exportera originalfilen för resursen)
* Konvertera med förinställning (använd en bildförinställning för att formatera resursen)
* Konvertera utan förinställning (använd exportdialogrutan för att ange bildmodifierare)

Följande resurstyper kan inte exporteras. Alla andra genererar en export.

* Bilduppsättningar
* Återgivningsuppsättningar
* Snurra uppsättningar
* Medieuppsättningar
* Uppsättningar med flera bithastigheter
* eCatalogs

Dessutom kan mallar inte exporteras som&quot;originalfil&quot;.

Du kan använda konvertering för att exportera följande resurstyper:

* Bilder
* Mallar
* Justerade bilder
* PDF (genererar konverterade sidor)
* PostScript®

Följande beteende uppstår när ett stort urval av olika tillgångstyper matas in i exportören:

* Alla resurstyper som inte kan exporteras tas bort från listan innan jobbet skickas
* Om en konvertering begärs exporteras alla typer som kan konverteras och alla andra som original
