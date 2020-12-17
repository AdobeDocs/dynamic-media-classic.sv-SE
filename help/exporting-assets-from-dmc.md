---
title: Exportera resurser från Dynamic Media Classic
seo-title: Exportera resurser från Dynamic Media Classic
description: 'null'
seo-description: Lär dig hur du exporterar resurser från Dynamic Media Classic.
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---


# Exportera resurser från Dynamic Media Classic{#exporting-assets-from-dmc}

Du kan spara resurser som du har redigerat i Dynamic Media Classic på en lokal nätverksenhet. Exporterade resurser paketeras i en ZIP-fil för nedladdning eller sändning via e-post.

Den komprimerade ZIP-filen har en maximal filstorlek på 1 GB för exportjobbet. Tänk också på att du får högst 500 resurser totalt per exportjobb.

I Dynamic Media Classic registreras exportjobb på jobbskärmen.

**Exportera resurser från Dynamic Media Classic**

1. Markera de resurser som du vill exportera och klicka sedan på **Arkiv** > **Exportera**.
1. I fönstret Exportera markerade resurser klickar du på **Bildalternativ** och anger sedan något av följande alternativ (administratörer avgör vilka alternativ som är tillgängliga för användarna):

   * ****
FörinställningarDu kan också välja en bildförinställning för att formatera resursen när du exporterar den. Om du väljer en bildförinställning är de andra formateringsalternativen inte tillgängliga eftersom resursen använder de format som definieras i bildförinställningen.

   * ****
KonverteraKonvertera resursfilen eller originalbilden.

   * ****
StorlekDu kan välja en standardstorlek. Du kan också klicka på Annan i listrutan Storlek, välja önskad måttenhet och sedan ange bredd och höjd.

      Se även [Ange vilka exportalternativ som är tillgängliga för Media Portal-användare](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * ****
FormatVälj ett bildformat.

   * ****
FärgVälj RGB, CMYK eller Grå.

   * **UpplösningVälj**
72, 150 eller 300 ppi.

   * **Jobbnamn**
Du kan tilldela ett jobbnamn till exporten.

   * **Skicka e-post**
tillOm du vill kan du ange en e-postadress för att skicka resurserna via e-post. I e-postmeddelandet visas den URL där mottagaren kan gå för att hämta resurserna.

1. Klicka på **Exportera**.

Tre grundläggande exportåtgärder stöds:

* Originalfil (exportera originalfilen för resursen)
* Konvertera med förinställning (använd en bildförinställning för att formatera resursen)
* Konvertera utan förinställning (använd exportdialogrutan för att ange bildmodifierare)

Följande resurstyper kan inte exporteras. Alla andra bör generera en export.

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
* Postscript

Följande beteende uppstår när ett stort urval av olika tillgångstyper matas in i exportören:

* Alla resurstyper som inte kan exporteras tas bort från listan innan jobbet skickas
* Om en konvertering begärs exporteras alla typer som kan konverteras och alla andra som original

