---
title: Skapa en e-katalog
seo-title: Skapa en e-katalog
description: 'null'
seo-description: Lär dig hur du skapar en e-katalog.
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '1005'
ht-degree: 0%

---


# Skapa en e-katalog{#creating-an-ecatalog}

När du skapar en e-katalog måste du beställa sidorna, välja sidlayout och länka sidorna genom att rita bildscheman och ange överrullnings- och hypertextlänksdata. Du kan också anpassa innehållsförteckningen så att användarna ser sidnamn i stället för sidnummer i eCatalog Viewer.

## Skapa en e-katalog {#create}

Du kan inkludera bildfiler och PDF-filer i din eCatalog.

När du skapar en e-katalog påverkar alternativet **Publicera efter spara** medlemmarna i uppsättningen och uppsättningen på följande sätt:

| Alternativet Publicera efter spara är markerat innan du sparar? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
|--- |--- |--- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ange medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) manuellt och [Avpublicera resurser](publishing-files.md#manually_unpublishing_assets)manuellt.

**Skapa en e-katalog**

1. Börja skapa din e-katalog med någon av följande tekniker:

   **Markera först** filerna i panelen Bläddra, markera filerna och klicka sedan på Skapa > eCatalogs.

   **Starta från eCatalog-skärmen** . Klicka på Skapa > eCatalogs. Markera en mapp i resursbiblioteket och dra filer från mappen till fliken Ordna sidor på eCatalog-sidan.

   ***Obs**! Om du vill visa objekten i resursbiblioteket efter namn i stället för efter miniatyrbild, väljer du alternativet Namn för standardvyn för resursbibliotek i Personliga inställningar. *

1. Välj en övergripande layout för din eCatalog. Klicka på uppåtknappen 1 för enstaka sidor, uppåtknappen 2 för uppslag med dubbla sidor eller knappen Egen för uppslag med fler än två sidor. Dialogrutan Ändra eCatalog-layout visas. Markera alternativen för alla uppslag och klicka på **OK**.
1. Du kan också ändra layouten för enskilda sidor eller uppslag genom att klicka på dem och sedan välja knappen 1 upp, 2 upp eller Egen. Dialogrutan Ändra eCatalog-layout visas. Markera alternativen för det markerade uppslaget och klicka på **OK**.
1. Ändra ordning på sidorna efter behov med någon av följande tekniker:

   **Dra** en sida eller ett uppslag till en ny plats. Det lodräta strecket visar var sidan flyttas.

   **Flytta till-knapp** Markera en sida eller ett uppslag, klicka på knappen Flytta till och välj den sida på menyn som du vill att sidan ska visas före.

   **Sekvens #** Ange sidnummer i fältet Sekvensnummer i listvyn.

1. När du är klar ser du till att **Publicera efter spara** är markerat (standard) nära sidans nedre högra hörn.
1. Klicka på **Spara**.
1. I dialogrutan Spara väljer du en mapp där din eCatalog ska lagras. I fältet Filnamn anger du namnet på rotationsuppsättningen.
1. Klicka på **Spara**.

   Du kan förhandsgranska din e-katalog när du har sparat den genom att klicka på **Förhandsgranska**.

## Redigera en e-katalog {#editing-an-ecatalog}

Beroende på om du redigerar en publicerad uppsättning eller en opublicerad uppsättning påverkar alternativet **Publicera efter spara** uppsättningen och ange medlemmar på följande sätt:

| Har du redan publicerat? | Alternativet Publicera efter spara är markerat innan du sparar redigeringen? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
|--- |--- |--- |--- |
| Ja | Ja | Publicerad | Publicerad |
| Ja | Nej | Publicerad | Befintliga uppsättningsmedlemmar behåller sin publicerade status.Alla nya uppsättningsmedlemmar som du lägger till under redigeringen behåller sin publicerade eller opublicerade status. |
| Nej | Ja | Publicerad | Publicerad |
| Nej | Nej | Opublicerad | Befintliga uppsättningsmedlemmar och nya uppsättningsmedlemmar som du har lagt till under redigeringen behåller sina publicerade eller opublicerade tillstånd. |

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) manuellt och [Avpublicera resurser](publishing-files.md#manually_unpublishing_assets)manuellt.

**Så här redigerar du en e-katalog**

1. Klicka på knappen **Redigera** överrullning för eCatalog.
1. Gör önskade ändringar.
1. När du är klar med redigeringen, nära det nedre högra hörnet på sidan, kontrollerar du att **Publicera efter spara** är markerat (standard).
1. Klicka på **Spara**, markera en lagringsmapp, ange ett namn för uppsättningen och klicka sedan på **Spara**.

## Ta bort en e-katalog {#deleting-an-ecatalog}

När du tar bort en uppsättning flyttas själva uppsättningen till papperskorgen. Medlemmarna (eller &quot;barn&quot;) i uppsättningen påverkas dock inte. i stället behåller de sitt befintliga publicerade eller opublicerade läge.

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) manuellt och [Avpublicera resurser](publishing-files.md#manually_unpublishing_assets)manuellt.

**Ta bort en e-katalog**

1. Markera en eller flera e-kataloger i Stödrastervisning, listvy eller detaljvy.
1. Klicka på **Arkiv** > **Ta bort** > **Ta bort** i det globala navigeringsfältet.

## Anpassa innehållsförteckningen {#customizing-the-table-of-contents-toc}

I Dynamic Media Classic finns standardsidnummer i din eCatalog på fliken Ordna sidor på skärmen eCatalog. För anpassade sidnamn kan du ändra de sidetiketter som utgör innehållsförteckningen. Vi rekommenderar att du byter namn på framsidan och baksidan. Försättsbladet kan t.ex. vara &quot;Omslag&quot; i stället för &quot;Sida 0-1&quot;.

Du kan skapa en anpassad innehållsförteckning för din eCatalog manuellt eller genom att importera sidnamnen från en CSV- (endast Mac) eller XML-fil.

>[!NOTE]
>
>Om du vill återställa standardsidrubrikerna klickar du på knappen för innehållsförteckningsetiketter på fliken Ordna sidor och väljer Återställ standardvärden (alla).

### Ange sidnamn manuellt {#manually-entering-page-names}

Om du vill ange sidnamn manuellt, en åt gången, går du till fliken Ordna sidor på skärmen för eCatalog. Klicka sedan i sidnummerfältet och ange ett namn. Ange ett namn för varje sida som du vill namnge.

### Importera sidnamn {#importing-page-names}

Du bör importera sidnamn om du har att göra med en e-katalog med många sidor. Du kan importera namnen från en tabbavgränsad fil eller XML-fil.

Innehållsförteckningsetiketten lagras i ett användardatafält för en bild. formatera dessa data som en lista över `name=<value>` ` pairs separated by two question marks “??” `. Om du till exempel vill ange en etikett för ett innehållsförteckningsfält med namnet tocEN anger du användardata för bilden till:

tocEN=&lt;EN_page_label>

Så här anger du separata etiketter för innehållsförteckningsfält med namnen tocEN och tocFR:

tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>

Om du vill importera fältet Användardata till en tabbavgränsad fil inkluderar du fältets användardata:

| IPSID | Användardata |
|--- |--- |
| `<image_IPS_ID>` | tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label> |

Om du vill importera fältet Användardata till en XML-fil inkluderar du attributet `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Om du vill importera sidnamn från en tabbavgränsad fil eller XML-fil markerar du knappen för innehållsförteckningsetiketter och väljer Importera. Dialogrutan Överför metadata visas. Klicka på knappen Bläddra och importera CSV-filen (endast Mac) eller XML-filen som associerar varje sida med ett sidnamn.
