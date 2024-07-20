---
title: Skapa en e-katalog
description: Lär dig skapa en e-katalog i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
topic: Integrations, Development
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '920'
ht-degree: 0%

---

# Skapa en e-katalog {#creating-an-ecatalog}

När du skapar en e-katalog måste du beställa sidorna, välja sidlayout och länka sidorna genom att rita bildscheman. Det kräver också att du anger rollover- och hypertextlänksdata. Du kan också anpassa innehållsförteckningen så att användarna ser sidnamn i stället för sidnummer i eCatalog Viewer.

## Skapa en e-katalog {#create}

Du kan inkludera bildfiler och PDF-filer i din eCatalog.

När du skapar en e-katalog påverkar alternativet **[!UICONTROL Publish after a save]** medlemmarna i uppsättningen och uppsättningen på följande sätt:

| Alternativet&quot;Publish after a save&quot; är valt innan du sparar? | Tillstånd för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
| --- | --- | --- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ställda medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här skapar du en e-katalog:**

1. Börja skapa din e-katalog med någon av följande tekniker:

   * **Markera filerna först**: Markera filerna på panelen Bläddra och gå sedan till **[!UICONTROL Build]** > **[!UICONTROL eCatalogs]**.

   * **Starta från e-katalogskärmen**: Gå till **[!UICONTROL Build]** > **[!UICONTROL eCatalogs]**. Välj en mapp i resursbiblioteket. Dra filer från mappen till fliken Ordna sidor på eCatalog-sidan.

     >[!NOTE]
     >
     >Om du vill visa objekten i resursbiblioteket efter namn i stället för efter miniatyrbild, väljer du alternativet Namn för standardvyn för resursbibliotek i Personliga inställningar.

1. Välj en övergripande layout för din eCatalog. Välj **[!UICONTROL 1 Up]** för enstaka sidor, **[!UICONTROL 2 Up]** för uppslag med dubbla sidor eller **[!UICONTROL Custom]** för uppslag med fler än två sidor. I dialogrutan **[!UICONTROL Change eCatalog Layout]** markerar du **[!UICONTROL All Spreads]**-alternativen och väljer **[!UICONTROL OK]**.
1. Du kan också ändra layouten för enskilda sidor eller uppslag genom att markera dem och sedan välja **[!UICONTROL 1 Up]**, **[!UICONTROL 2 Up]** eller **[!UICONTROL Custom]** . I dialogrutan **[!UICONTROL Change eCatalog Layout]** markerar du **[!UICONTROL Selected Spreads]**-alternativen och väljer **[!UICONTROL OK]**.
1. Ändra ordning på sidorna efter behov med någon av följande tekniker:

   * **Dra**: Dra en sida eller ett uppslag till en ny plats. Det lodräta strecket visar var sidan flyttas.

   * **Flytta till-knapp**: Markera en sida eller ett uppslag, markera **[!UICONTROL Move To]** och välj sidan på menyn som du vill att sidan ska visas före.

   * **Sekvens #**: I listvyn anger du sidnummer i fälten för sekvensnummer.

1. När du är klar ser du till att **[!UICONTROL Publish after a save]** är markerat (standard) nära sidans nedre högra hörn.
1. Välj **[!UICONTROL Save]**.
1. I dialogrutan Spara väljer du en mapp där din eCatalog ska lagras. I fältet Filnamn anger du namnet på rotationsuppsättningen.
1. Välj **[!UICONTROL Save]**.

   Du kan förhandsgranska din e-katalog genom att välja **[!UICONTROL Preview]** när du har sparat den.

## Redigera en e-katalog {#editing-an-ecatalog}

Oavsett om du redigerar en publicerad eller opublicerad uppsättning påverkar alternativet **[!UICONTROL Publish after a save]** medlemmarna i uppsättningen och uppsättningen på följande sätt:

| Har du redan publicerat? | Om du väljer&quot;Publish när du har sparat&quot; innan du sparar redigeringen? | Tillstånd för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
| --- | --- | --- | --- |
| Ja | Ja | Publicerad | Publicerad |
| Ja | Nej | Publicerad | Befintliga uppsättningsmedlemmar behåller sin publicerade status. Alla nya uppsättningsmedlemmar som du lägger till under redigeringen behåller sin publicerade eller opublicerade status. |
| Nej | Ja | Publicerad | Publicerad |
| Nej | Nej | Opublicerad | Befintliga uppsättningsmedlemmar och nya uppsättningsmedlemmar som du har lagt till under redigeringen behåller sina publicerade eller opublicerade tillstånd. |

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här redigerar du en e-katalog:**

1. Markera eCatalogs överrullningsknapp **[!UICONTROL Edit]**.
1. Gör önskade ändringar.
1. När du är klar med redigeringen kontrollerar du att **[!UICONTROL Publish after a save]** är markerat (standard) nära sidans nedre högra hörn.
1. Välj **[!UICONTROL Save]**, markera en lagringsmapp, ange ett namn för uppsättningen och välj sedan **[!UICONTROL Save]**.

## Ta bort en e-katalog

När du tar bort en uppsättning flyttas själva uppsättningen till papperskorgen. Medlemmarna (eller&quot;underordnade&quot;) i uppsättningen påverkas dock inte. De behåller i stället sitt befintliga publicerade eller opublicerade läge.

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här tar du bort en e-katalog:**

1. Markera en eller flera e-kataloger i Stödrastervisning, listvy eller detaljvy.
1. Gå till **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]** i det globala navigeringsfältet.

## Anpassa innehållsförteckningen {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic tillhandahåller standardsidnummer i din eCatalog på fliken Ordna sidor på skärmen eCatalog. För anpassade sidnamn kan du ändra de sidetiketter som utgör innehållsförteckningen. Vi rekommenderar att du byter namn på framsidan och baksidan. Försättsbladet kan t.ex. vara &quot;Omslag&quot; i stället för &quot;Sida 0-1&quot;.

Du kan skapa en anpassad innehållsförteckning för din eCatalog manuellt. Du kan också importera sidnamnen från en CSV-fil (endast Mac) eller en XML-fil.

>[!NOTE]
>
>Om du vill återställa standardsidrubrikerna väljer du **[!UICONTROL TOC Labels]** på fliken **[!UICONTROL Order Pages]** och sedan **[!UICONTROL Restore Defaults (All)]**.

### Ange sidnamn manuellt {#manually-entering-page-names}

Ange sidnamn manuellt en i taget genom att gå till fliken Ordna sidor på skärmen eCatalog. I sidnummerfältet anger du sedan ett namn för varje sida som du vill namnge.

### Importera sidnamn {#importing-page-names}

Du bör importera sidnamn om du har att göra med en e-katalog med många sidor. Du kan importera namnen från en tabbavgränsad fil eller XML-fil.

Innehållsförteckningsetiketten lagras i en bilds användardatafält. Formatera informationen som en lista med `name=<value>` ` pairs separated by two question marks "??" `. Om du till exempel vill ange en etikett för ett innehållsförteckningsfält med namnet `tocEN` anger du användardata för bilden till:

`tocEN=&lt;EN_page_label>`

Så här anger du separata etiketter för innehållsförteckningsfält med namnen `tocEN` och `tocFR`:

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

Om du vill importera sidnamn från en tabbavgränsad fil eller XML-fil markerar du knappen **[!UICONTROL TOC Labels]** och väljer **[!UICONTROL Import]**. I dialogrutan Överför metadata väljer du **[!UICONTROL Browse]** och importerar sedan CSV-filen (endast Mac) eller XML-filen som associerar varje sida med ett sidnamn.
