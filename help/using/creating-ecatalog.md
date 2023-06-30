---
title: Skapa en e-katalog
description: Lär dig hur du skapar en e-katalog i Adobe Dynamic Media Classic.
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
topic: Integrations, Development
level: Experienced
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '911'
ht-degree: 0%

---

# Skapa en e-katalog {#creating-an-ecatalog}

När du skapar en e-katalog måste du beställa sidorna, välja sidlayout och länka sidorna genom att rita bildscheman och ange överrullnings- och hypertextlänksdata. Du kan också anpassa innehållsförteckningen så att användarna ser sidnamn i stället för sidnummer i eCatalog Viewer.

## Skapa en e-katalog {#create}

Du kan inkludera bildfiler och PDF-filer i din eCatalog.

När du skapar en e-katalog **[!UICONTROL Publish after save]** påverkar uppsättningen och medlemmarna i uppsättningen på följande sätt:

| Alternativet Publicera efter spara är markerat innan du sparar? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
| --- | --- | --- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ange medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här skapar du en e-katalog:**

1. Börja skapa din e-katalog med någon av följande tekniker:

   * **Markera filerna först** - Markera filer på panelen Bläddra och gå sedan till **[!UICONTROL Build]** > **[!UICONTROL eCatalogs]**.

   * **Starta från eCatalog-skärmen** - Gå till **[!UICONTROL Build]** > **[!UICONTROL eCatalogs]**. Markera en mapp i resursbiblioteket och dra filer från mappen till fliken Ordna sidor på eCatalog-sidan.

     >[!NOTE]
     >
     >Om du vill visa objekten i resursbiblioteket efter namn i stället för efter miniatyrbild, väljer du alternativet Namn för standardvyn för resursbibliotek i Personliga inställningar.

1. Välj en övergripande layout för din eCatalog. Välj **[!UICONTROL 1 Up]** för enstaka sidor, **[!UICONTROL 2 Up]** för uppslag med dubbla sidor, eller **[!UICONTROL Custom]** för uppslag med fler än två sidor. I **[!UICONTROL Change eCatalog Layout]** väljer du **[!UICONTROL All Spreads]** alternativ och markera **[!UICONTROL OK]**.
1. Du kan också ändra layouten för enskilda sidor eller uppslag genom att markera dem och sedan välja **[!UICONTROL 1 Up]**, **[!UICONTROL 2 Up]**, eller **[!UICONTROL Custom]** -knappen. I **[!UICONTROL Change eCatalog Layout]** väljer du **[!UICONTROL Selected Spreads]** alternativ och markera **[!UICONTROL OK]**.
1. Ändra ordning på sidorna efter behov med någon av följande tekniker:

   * **Dra** - Dra en sida eller ett uppslag till en ny plats. Det lodräta strecket visar var sidan flyttas.

   * **Knappen Flytta till** - Markera en sida eller ett uppslag, markera **[!UICONTROL Move To]** och väljer sidan på menyn som du vill att sidan ska visas före.

   * **Sekvensnr** - I listvyn anger du sidnummer i fälten Sekvensnummer.

1. När du är klar ser du till att du ser till att **[!UICONTROL Publish after save]** är markerat (standard).
1. Välj **[!UICONTROL Save]**.
1. I dialogrutan Spara väljer du en mapp där din eCatalog ska lagras. I fältet Filnamn anger du namnet på rotationsuppsättningen.
1. Välj **[!UICONTROL Save]**.

   Du kan förhandsgranska din e-katalog genom att välja **[!UICONTROL Preview]**.

## Redigera en e-katalog {#editing-an-ecatalog}

Oavsett om du redigerar en publicerad uppsättning eller en opublicerad uppsättning kan du **[!UICONTROL Publish after save]** påverkar uppsättningen och medlemmarna i uppsättningen på följande sätt:

| Har du redan publicerat? | Alternativet Publicera efter spara är markerat innan du sparar redigeringen? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
| --- | --- | --- | --- |
| Ja | Ja | Publicerad | Publicerad |
| Ja | Nej | Publicerad | Befintliga uppsättningsmedlemmar behåller sin publicerade status. Alla nya uppsättningsmedlemmar som du lägger till under redigeringen behåller sin publicerade eller opublicerade status. |
| Nej | Ja | Publicerad | Publicerad |
| Nej | Nej | Opublicerad | Befintliga uppsättningsmedlemmar och nya uppsättningsmedlemmar som du har lagt till under redigeringen behåller sina publicerade eller opublicerade tillstånd. |

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här redigerar du en e-katalog:**

1. Välj eCatalogs rollover **[!UICONTROL Edit]** -knappen.
1. Gör önskade ändringar.
1. När du är klar med redigeringen, nära det nedre högra hörnet på sidan, ser du till att **[!UICONTROL Publish after save]** är markerat (standard).
1. Välj **[!UICONTROL Save]**, väljer en lagringsmapp, anger ett namn för uppsättningen och väljer **[!UICONTROL Save]**.

## Ta bort en e-katalog {#deleting-an-ecatalog}

När du tar bort en uppsättning flyttas själva uppsättningen till papperskorgen. Medlemmarna (eller &quot;barn&quot;) i uppsättningen påverkas dock inte. i stället behåller de sitt befintliga publicerade eller opublicerade läge.

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här tar du bort en e-katalog:**

1. Markera en eller flera e-kataloger i Stödrastervisning, listvy eller detaljvy.
1. På det globala navigeringsfältet går du till **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.

## Anpassa innehållsförteckningen {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic tillhandahåller standardsidnummer i din eCatalog på fliken Ordna sidor på skärmen eCatalog. För anpassade sidnamn kan du ändra de sidetiketter som utgör innehållsförteckningen. Vi rekommenderar att du byter namn på framsidan och baksidan. Försättsbladet kan t.ex. vara &quot;Omslag&quot; i stället för &quot;Sida 0-1&quot;.

Du kan skapa en anpassad innehållsförteckning för din eCatalog manuellt eller genom att importera sidnamnen från en CSV-fil (endast Mac) eller XML-fil.

>[!NOTE]
>
>Återställ standardsidrubrikerna på **[!UICONTROL Order Pages]** flik, välja **[!UICONTROL TOC Labels]** och sedan markera **[!UICONTROL Restore Defaults (All)]**.

### Ange sidnamn manuellt {#manually-entering-page-names}

Om du vill ange sidnamn manuellt, en åt gången, går du till fliken Ordna sidor på skärmen för eCatalog. I sidnummerfältet anger du sedan ett namn för varje sida som du vill namnge.

### Importera sidnamn {#importing-page-names}

Du bör importera sidnamn om du har att göra med en e-katalog med många sidor. Du kan importera namnen från en tabbavgränsad fil eller XML-fil.

Innehållsförteckningsetiketten lagras i en bilds fält för användardata. formatera dessa data som en lista över `name=<value>` ` pairs separated by two question marks “??” `. Du kan till exempel ange en etikett för ett innehållsförteckningsfält med namnet `tocEN`, ställer du in användardata för bilden på:

`tocEN=&lt;EN_page_label>`

Ange separata etiketter för innehållsförteckningsfält med namn `tocEN` och `tocFR`:

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

Om du vill importera fältet Användardata till en tabbavgränsad fil inkluderar du fältets användardata:

| IPSID | Användardata |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

Om du vill importera fältet Användardata till en XML-fil inkluderar du attributet `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Om du vill importera sidnamn från en tabbavgränsad fil eller XML-fil väljer du **[!UICONTROL TOC Labels]** och markera **[!UICONTROL Import]**. I dialogrutan Överför metadata väljer du **[!UICONTROL Browse]** och sedan importera CSV-filen (endast Mac) eller XML-filen som associerar varje sida med ett sidnamn.
