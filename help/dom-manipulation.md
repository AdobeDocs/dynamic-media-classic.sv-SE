---
title: DOM-manipulering
seo-title: DOM-manipulering
description: 'null'
seo-description: Lär dig mer om DOM-manipulering.
uuid: 275cd49d-2a55-41f9-80b0-e147d0cd2907
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: 890ca93e-3146-4347-864b-bd5e94037038
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# DOM-manipulering{#dom-manipulation}

DOM-redigering (Document Object Model) är en teknik som används för att redigera en designfil genom att direkt ändra dess XML-kod. DOM-manipulering ger dig större kontroll över variabla designelement, inklusive ändring av deras innehåll och utseende, kan du till och med skapa nya element vid behov.

Med Dynamic Media Classic kan du ändra DOM för en dynamisk Media Classic FXG-mall med hjälp av URL-kommandon när mallen har publicerats. Designelementen i FXG-mallen ändras genom att du skickar kommandon via webbadressen. På så sätt kan du dynamiskt ändra och lägga till attribut till bilder.

Om du vill använda DOM-manipulering skapar du s7:elementID:n i Illustrator-filen innan du konverterar den till en Dynamic Media Classic FXG-fil och överför den till SPS.

>[!NOTE]
>
>När du använder DOM-ändringskommandon måste alla värden som skickas vara URL-kodade.

>[!NOTE]
>
>Illustrator Plug-in for Web-to-Print (för konvertering av Illustrator-filer) konverteras till FXG 2.0. Mer information om den här specifikationen finns på [www.adobe.com/go/learn_s7_fxg2_en](https://www.adobe.com/go/learn_s7_fxg2_en).

## Skapa s7:element-ID:n i Illustrator-filer {#creating-s-elementids-in-illustrator-files}

Om du vill använda DOM-manipulering med en design som har skapats i Illustrator skapar du s7:elementID:n i Illustrator-designen. Om du skapar s7:elementID:n kan designelement ändras med URL-kommandon när mallen har publicerats.

### Skapa s7:elementID:n för DOM-redigering av text {#creating-s-elementids-for-dom-manipulation-of-text}

Om du vill skapa ett s7:elementID för DOM-redigering av ett textobjekt öppnar du panelen Lager i Illustrator. I textlagret som innehåller variabeltext ger du lagret ett s7:elementID. Om du vill göra det anger du bokstäverna `id` (för identifiering), kolon ( `:`) och ett namn. Nedan följer exempel på textlagernamn för s7:elementID:

`id:BirthdayBoyName`

`id:DateofBirth`

`id:EnterFirstNameHer`

### Skapa s7:elementID:n för DOM-manipulering av objekt {#creating-s-elementids-for-dom-manipulation-of-objects}

Skapa s7:elementID:n för objekt när du vill att slutanvändarna ska kunna ändra objektens attribut. Objekt kan utgöra hela textramar, bilder och bilder. En färgbakgrund är ett exempel på ett objektelements-ID. När säsongerna förändras kan slutanvändaren byta ut bakgrundsfärgen i en affisch så att affischen passar säsongen.

Skapa ett separat lager för objektet innan du skapar ett s7:element-ID för ett objekt i Illustrator.

Så här skapar du ett s7:elementID för ett objekt i Illustrator:

1. Markera objektet.
1. Klicka på **Fönster** > **Lager**.
1. På panelen Lager ger du objektlagret ett s7:elementID. Om du vill göra det anger du bokstäverna `id` (för identifiering), kolon ( `:`) och beskrivning för att identifiera elementet. Nedan följer exempel på objektlagernamn för s7:elementID:

   `id:BackgroundColor`

   `id:RotationPercentage`

   `id:JacketJPG`

## Publicera FXG-mallar {#publish-fxg-templates}

När du publicerar din FXG-mall placeras den på de dynamiska Media Classic-servrarna, där den är tillgänglig för din webbplats och ditt program. Under publiceringsprocessen aktiverar Scene7 Publishing System de URL:er du behöver för webbplatsen eller tillämpningen.

>[!NOTE]
>
>Om du vill använda din FXG-mall publicerar du allt innehåll som ingår i mallen, inklusive teckensnitt och bilder. Om du inte inkluderar alla nödvändiga filer visas ett felmeddelande när du publicerar.

### Markera FXG-mallar för publicering {#mark-fxg-templates-for-publish}

Mallar och deras supportfiler måste markeras för publicering för att de ska kunna placeras på dynamiska mediabildsservrar.

1. I panelen Bläddra väljer du FXG-mallen tillsammans med bilder, bilder och teckensnitt som används.
1. Klicka på **Markera för publicering**.

### Publicera din FXG-mall {#publish-your-fxg-template}

1. Klicka på **Publicera** i fältet Global navigering.
1. Välj alternativet Vid och ange eventuellt ett namn för publiceringsjobbet.
1. Klicka på **Starta publicering**.

### Visa indikator för textspill {#text-overflow-indicator-display}

En *textflödesindikator* visar när texten överskrider det tilldelade utrymmet i en textram (eller i den sista textramen för kopplad text). Indikatorn är en röd ruta med ett plustecken. Indikatorer för textspill i SPS är alltid aktiverade.

Indikatorer för textspill styrs med `markOverflowingTextFrame` modifieraren. Använd modifieraren på följande sätt:

| Modifierare/värden | Beskrivning |
|--- |--- |
| markOverflowingTextFrame=0,1 | Värdet 1 gör att textflödesindikatorer visas. Standardvärdet är 0. (Även om standardvärdet är 0 är fortsättningssymbol för text i SPS alltid aktiverat.) Observera att modifieraren markOverflowingTextFrame är skiftlägeskänslig. |

>[!MORELIKETHIS]
>
>* [Definiera variabilitet: Parameterisering kontra DOM-manipulering](defining-variability-parameterization-versus-dom.md#defining_variability_parameterization_versus_dom_manipulation)
>* [Publicering](publishing-files.md#publishing_files)

