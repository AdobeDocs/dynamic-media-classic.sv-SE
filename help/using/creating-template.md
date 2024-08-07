---
title: Skapa en mall
description: Lär dig skapa en mall i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 23ac1a0f-c90b-4250-ae36-93702fb5ebd9
topic: Content Management
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '3261'
ht-degree: 0%

---

# Skapa en mall

Om du vill skapa en mall går du till **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**. Välj antingen Designer eller Developer. På den här sidan kan du lägga till bild- och textlager. Du kan också ändra ordning på lager, ändra storlek och position för lager och använda skugg- och glödeffekter på bilder och text.

Se även utbildningsvideon [Mallgrunder](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS).

>[!NOTE]
>
>Om du redigerar en mall som har skapats i en tidigare version av Adobe Dynamic Media Classic blir du tillfrågad när du sparar&quot;Vill du lägga till ett arbetsytelager?&quot; Välj **[!UICONTROL No]** om du inte vill lägga till ett baslager. Om du råkar markera **[!UICONTROL Yes]** tar du bort modifieringarna `&allowCanvasPrompt` och `&layer=0` i URL:en och trycker på **[!UICONTROL Enter]** eller **[!UICONTROL Return]**.

## Skapa den ursprungliga mallen {#creating-the-initial-template}

När du skapar en malluppsättning påverkar alternativet **[!UICONTROL Publish after a save]** medlemmarna i uppsättningen och uppsättningen på följande sätt:

| **[!UICONTROL Publish after a save]** alternativ markerat innan du sparar? | Tillstånd för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
| --- | --- | --- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ställda medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

Du kan skapa en mall från en befintlig mall. Öppna mallen, markera **[!UICONTROL Save As]** och ange ett nytt namn i dialogrutan Spara som.

**Så här skapar du den ursprungliga mallen:**

1. Använd någon av följande metoder för att skapa en ursprunglig mall:

   * **Markera PSD eller bilder först**: På panelen Bläddra väljer du den eller de PSD-filer som du vill använda för mallen, går till **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**.

   * **Starta från mallskärmen**: Gå till **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**. Välj antingen Designer eller Developer.

1. Ange mallens bredd- och höjdmått i dialogrutan Ange storlek på arbetsyta.
1. Markera en mapp i resursbiblioteket och dra PSD-filen eller bilderna som du vill använda för mallen till mallskärmen.
1. När du är klar ser du till att **[!UICONTROL Publish after a save]** är markerat (standard) nära sidans nedre högra hörn.
1. Välj **[!UICONTROL Save]**.
1. Välj en mapp där du vill lagra mallen, ange ett namn för mallen och välj **[!UICONTROL Submit]**.

   Adobe Dynamic Media Classic förminskar bilder om det behövs för att de ska få plats på arbetsytan, området på mallskärmen för att definiera mallen.

## Redigera en malluppsättning {#editing-a-template-set}

Oavsett om du redigerar en publicerad uppsättning eller en opublicerad malluppsättning påverkar alternativet **[!UICONTROL Publish after a save]** medlemmarna i uppsättningen och uppsättningen på följande sätt:

| Har du redan publicerat? | **[!UICONTROL Publish after a save]** alternativ markerat innan du sparar redigeringen? | Tillstånd för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
| --- | --- | --- | --- |
| Ja | Ja | Publicerad | Publicerad |
| Ja | Nej | Publicerad | Befintliga uppsättningsmedlemmar behåller sin publicerade status. Alla nya uppsättningsmedlemmar som du lägger till under redigeringen behåller sin publicerade eller opublicerade status. |
| Nej | Ja | Publicerad | Publicerad |
| Nej | Nej | Opublicerad | Befintliga uppsättningsmedlemmar och nya uppsättningsmedlemmar som du har lagt till under redigeringen behåller sina publicerade eller opublicerade tillstånd. |

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här redigerar du en malluppsättning:**

1. I stödrastervyn bläddrar du till en malluppsättning och väljer **[!UICONTROL Edit]** nedanför bilden.
1. Ändra mallen efter behov.
1. När du är klar med redigeringen kontrollerar du att **[!UICONTROL Publish after a save]** är markerat (standard) nära sidans nedre högra hörn.
1. Välj **[!UICONTROL Save]**, markera en lagringsmapp, ange ett namn för uppsättningen och välj sedan **[!UICONTROL Save]**.

## Ta bort en mall

När du tar bort en malluppsättning flyttas själva uppsättningen till papperskorgen. Medlemmarna (eller&quot;underordnade&quot;) i uppsättningen påverkas dock inte. De behåller i stället sitt befintliga publicerade eller opublicerade läge.

Se även [Publicera resurser manuellt](publishing-files.md#manually_publishing_assets) och [Avpublicera resurser manuellt](publishing-files.md#manually_unpublishing_assets).

**Så här tar du bort en mall:**

1. I Stödrastervisning, listvy eller detaljvy väljer du en eller flera mallar.
1. Gå till **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]** i det globala navigeringsfältet.

## Förstå mallskärmen {#understanding-the-template-screen}

På mallskärmen finns verktyg för att ändra och parametrisera lager.

Använd de här verktygen på mallskärmen så att du kan skapa mallar:

* **[!UICONTROL Pan]**: Gör att du kan markera lager, flytta dem runt arbetsytan, ändra storlek på dem eller rotera dem.

* **[!UICONTROL Text]**: Skapar ett textlager. Skapa ett textlager genom att dra på arbetsytan och ange sedan texten i lagret. Se [Skapa ett textlager](#creating-a-text-layer).

* **[!UICONTROL Preview]**: Öppnar förhandsgranskningsskärmen och visar mallen i ett zoomvisningsprogram. Du ser hur mallen ser ut för användare på din webbplats eller i ditt program.

* **[!UICONTROL Parameter Summary]** Öppnar fönstret Parametersammanfattning. Du kan se namnet på varje lager i en mall, och på varje lager, namnen på de parametrar som har aktiverats.

* **[!UICONTROL Text Editor v4.3 and Text Editor v4.2]**: Använd den senaste och mest funktionsrika textredigeraren. Du kan välja att använda textredigeraren v4.3 eller den tidigare textredigeraren, textredigeraren v4.2. När du skapar mallar väljs textredigeraren v4.3 som standard. När du redigerar äldre mallar väljs textredigeraren v4.2 som standard. Textredigeraren v4.3 stöder för närvarande inte automatisk radbrytning, så när du redigerar äldre mallar som använder automatisk radbrytning bör du använda textredigeraren v4.2 för att behålla mallens återgivning helt intakt. Om den äldre mallen inte använder automatisk radbrytning kan du välja textredigeraren v4.3 för att utnyttja alla nya funktioner som den har. Du kan till exempel öka marginalerna, minska marginalerna, ange text i versaler och kopiera textpassning.

  >[!NOTE]
  >
  >Textredigeraren v4.2 planeras att tas bort som ett alternativ i Adobe Dynamic Media Classic. Vi rekommenderar att du använder textredigeraren 4.3 när det är möjligt. Alternativet **[!UICONTROL Word Wrap]** kommer att införlivas i en framtida version av textredigeraren.

* **[!UICONTROL Designer and Developer]**: Välj det alternativ som bäst beskriver din roll.

* **[!UICONTROL Canvas]**: Definierar det totala tillgängliga området, i pixlar, för att definiera mallen. Standardstorleken är 300 × 300 pixlar. Lager placeras på arbetsytan.

* **[!UICONTROL Layers list]**: Visar namnet på lagren i mallen. Markera ett lager genom att markera lagrets namn i listan Lager. Listan Lager innehåller verktyg för att lägga till effekter i lager, ta bort lager, ordna om lager och parametrisera lager. Se [Arbeta med lager](#working-with-layers).

* **[!UICONTROL Layer Properties area]**: I det här området finns verktyg för att ändra bakgrundsfärg, opacitet, storlek och position för ett lager. Du kan också ändra bakgrundsfärg, opacitet och storlek för arbetsytan. Du kan också justera skugg- och glödeffekter. Se [Arbeta med lager](#working-with-layers).

## Skapa bildlager {#creating-image-layers}

1. Dra bilden från resursbiblioteket till arbetsytan.

   Bildens ID-namn visas i listan Lager.

   >[!NOTE]
   >
   >Om det behövs krymper Adobe Dynamic Media Classic bilderna så att de får plats på arbetsytan när du skapar ett bildlager.

## Skapa ett textlager {#creating-a-text-layer}

1. Välj verktyget **[!UICONTROL Text]**.
1. Dra för att skapa en textruta på arbetsytan eller på en bild.
1. På textskärmen som öppnas lägger du till text genom att göra något av följande på fliken Förhandsgranska:

   * Skriv text i textrutan. Välj Kopiera anpassa text så att texten får plats i textrutan.
   * Klistra in text från Urklipp i textrutan.

1. Välj **[!UICONTROL Apply]** och stäng sedan textskärmen.

### Formatera text {#format-text}

Så här formaterar du text i ett textlager:

1. Dubbelklicka på namnet på textrutan med den text du vill redigera i listan Lager. Textredigeraren öppnas.
1. Markera texten som du vill formatera i textrutan i textredigeraren. Du kan markera all text, alla delar av texten eller enskilda tecken.
1. Ange något av följande formateringsalternativ och välj sedan **[!UICONTROL Apply]**.

   * **[!UICONTROL Font]**: Välj ett teckensnitt på teckensnittsmenyn. Om ett teckensnitt som du vill använda inte visas på menyn kan du överföra det till Adobe Dynamic Media Classic. Se Typsnitt.

   * **[!UICONTROL Font Size]**: Välj en teckensnittsstorlek på menyn, ange en specifik storlek i rutan eller markera **[!UICONTROL Up]** - eller **[!UICONTROL Down]** -pilarna för att öka eller minska storleken med två punkter.

   * **[!UICONTROL Color]**: Välj en färg för texten.

   * **[!UICONTROL Bold]**, **[!UICONTROL Italic]** eller **[!UICONTROL Underline]**: Markera texten och markera sedan ikonen för den typ av formatering som du vill använda på texten.

   * **[!UICONTROL All Caps]**, **[!UICONTROL Superscript]** eller **[!UICONTROL Subscript]**: Markera texten och markera sedan ikonen för den typ av formatering som du vill använda på texten.

   * **[!UICONTROL Alignment]**: Välj en justeringsknapp för att vänsterjustera, centrera eller högerjustera text i textlagret.

   * **[!UICONTROL Tracking]**: Ange eller markera ett numeriskt värde som du vill justera avståndet mellan ord med.

   * **[!UICONTROL Kerning]**: Ange eller markera ett numeriskt värde som du vill justera avståndet mellan tecknen med.

   * **[!UICONTROL Line Spacing]**: Ange eller välj ett numeriskt värde som du vill justera avståndet mellan raderna med.

   * **[!UICONTROL Baseline Shift]**: Ange eller markera ett numeriskt värde som du vill flytta ett markerat tecken uppåt eller nedåt i förhållande till den omgivande textens baslinje. Det här alternativet är särskilt användbart när du ställer in bråktal för hand eller justerar positionen för textbundna bilder.

>[!NOTE]
>
>Välj **[!UICONTROL Undo]** om du vill ångra den senaste åtgärden. Välj **[!UICONTROL Redo]** om du ångrar en åtgärd när du har valt **[!UICONTROL Undo]**.

### Formatera stycken {#format-paragraphs}

1. Dubbelklicka på namnet på textrutan med den text du vill redigera i listan Lager. Textredigeraren öppnas.
1. Markera stycket som du vill formatera.
1. Ange något av följande formateringsalternativ och välj sedan **[!UICONTROL Apply]**.

   * **[!UICONTROL Alignment]**: Ange justeringstypen genom att klicka på **[!UICONTROL Align left]**, **[!UICONTROL Align center]**, **[!UICONTROL Align right]** eller **[!UICONTROL Justify]**.

   * **[!UICONTROL End of Paragraph Justification]**: Välj det här alternativet om du vill ange justeringstypen för den sista raden i stycket: den sista raden vänsterjusteras, den sista raden centreras och den sista raden högerjusteras.

   * **[!UICONTROL Line Spacing]**: Ange eller markera ett numeriskt värde som du vill justera avståndet mellan alla rader i stycket med.

   * **[!UICONTROL Indent All]**: Välj det här alternativet om du vill öka textindraget.

   * **[!UICONTROL Remove Indent]**: Välj det här alternativet om du vill minska textens indrag.

   * **[!UICONTROL Indent First Line]**: Ange hur mycket du vill dra in den första textraden med.

   * **[!UICONTROL Space Before Paragraph]**: Ange hur mycket utrymme du vill ha ovanför den första textraden i stycket.

   * **[!UICONTROL Space After Paragraph]**: Ange hur mycket utrymme du vill ha under den sista textraden i stycket.

   * **[!UICONTROL Vertical Align]**: Välj var du vill att texten ska visas lodrätt i textrutan: Överkant, Mitten, Nederkant.

   * **[!UICONTROL Text Direction]**: Välj i vilken riktning du vill att texten ska visas: höger-till-vänster eller vänster-till-höger.

### Justera egenskaper för textlager {#adjust-text-layer-properties}

1. Markera textrutan som du vill justera på skärmen Grundläggande om mallar.
1. Välj något av följande på panelen Lageregenskaper:

   * **[!UICONTROL Shrink Text (Text Editor v4.2 only)]**: Välj det här alternativet om du vill krympa texten så att den passar i textrutan.

   * **[!UICONTROL Word Wrap (Text Editor v4.2 only)]**: Om du vill ange om eller hur texten ska radbrytas väljer du ett radbrytningsalternativ:

   * **[!UICONTROL Wrap]**: Radbryter texten så att den får plats i en textruta som är för liten vågrätt.

   * **[!UICONTROL No Wrap]**: Figursätter inte texten när textrutan är för liten vågrätt, utan klipper i stället av en del av texten.

   * **[!UICONTROL Nonbreaking Wrap]**: Radbryter text så att den får plats i en textruta, och bryter inte ord.

   * **[!UICONTROL Position]**: Anger textrutans plats på arbetsytan.

   * **[!UICONTROL Padding]**: Lägger till marginaler eller beskär lagerrektangeln. Ange antalet pixlar som du vill lägga till eller ta bort för Vänster, Upptill, Underkant och Höger. Ange positiva tal om du vill lägga till en marginal eller negativa tal i beskärningen.

### Visa och redigera textkällkod {#view-and-edit-text-source-code}

Du kan referera till informationen på fliken Source i textredigeraren. Redigera bara texten om du är bekant med att redigera källkod.

1. Dubbelklicka på namnet på textrutan med den text du vill redigera i listan Lager. Textredigeraren öppnas.
1. Visa källkoden för texten i textredigeraren genom att välja fliken **[!UICONTROL Source]** i textredigeraren.
1. Visa eller redigera texten efter behov.

   Ändringarna förblir intakta om du växlar fram och tillbaka mellan förhandsgransknings- och Source-vyn.

1. Välj **[!UICONTROL Apply]** om du vill återge redigeringarna.

## Arbeta med lager {#working-with-layers}

Använd lagerlistan och området Lageregenskaper när du vill arbeta med lager. Du kan ordna om lager, ändra deras storlek och position, rotera lager och bestämma bakgrundsfärg, förgrundsfärg, opacitet och blandningsläge för ett lager.

Du kan också ändra storlek på arbetsytan, välja bakgrundsfärg och ändra opacitetsinställningen.

### Ordna om lager {#reordering-layers}

Om du ändrar lagerordningen kan det påverka utseendet, särskilt när genomskinlighet eller övertryck används. Se till att du förhandsgranskar resultatet innan du implementerar ändringarna.

1. Använd någon av dessa tekniker för att ordna om lagren i en mall:

   * Markera ett lager i listan Lager. Välj sedan **[!UICONTROL Up]** eller **[!UICONTROL Down]** så många gånger som behövs för att placera den på rätt plats i listan.
   * Dra ett lager uppåt eller nedåt i listan Lager.

### Ändra storlek och position för lager och arbetsytan {#changing-the-size-and-position-of-layers-and-the-canvas}

Lagren måste vara tillräckligt små för att få plats på arbetsytan. Du kan ändra storlek på ett lager eller arbetsytan manuellt eller genom att ange mått för storlek. Du kan ändra positionen för ett lager manuellt eller genom att ange förskjutningsmått. Du kan också rotera ett lager.

>[!NOTE]
>
>Adobe Dynamic Media Classic rekommenderar att du skapar en bildförinställning som har exakt samma storlek som mallen. Genom att matcha storleken på förinställningen för bild med mallstorleken kan du vara säker på att mallens slutliga utdatastorlek och skärpealternativ ställs in korrekt. När du har skapat den här bildförinställningen kan du välja den på menyn Använd förinställning på skärmen Förhandsvisa mall. På skärmen visas hur bilden ser ut när den levereras från servern. Se [Konfigurera bildförinställningar](setting-image-presets.md#setting_up_image_presets).

* **Ändra storlek på ett lager**: Om du vill ändra storlek på ett lager eller arbetsytan markerar du lagret eller arbetsytan i listan Lager och använder någon av följande tekniker:

* **Ändra storlek manuellt**: Markera och dra i ett hörn på lagret eller arbetsytan. Med textlager kan du också dra en sida av lagret. Håll ned Skift-tangenten när du drar om du vill ändra storleken men behålla proportionerna (formen).

* **Ange mått för lagerstorlek**: Ange pixelmått i textrutorna B (bredd) och H (höjd) i området Lageregenskaper.

Förutom att ändra storlek på ett lager kan du lägga ut det. Om du vill göra det anger du en utfyllnadsmätning i rutan Vänster, Höger, Upptill och Nedtill i området Lageregenskaper. Utfyllnad lägger till en marginal i det aktuella lagret för att förskjuta den från omkretsen av dess baslager. Utfyllnaden är användbar om du lägger till en skugga eller yttre glöd och vill göra effekten mer synlig. Utfyllnad ökar storleken på ett lager och visar dess bakgrundsfärg i det utökade utfyllnadsområdet. Baslagret flyttar sig automatiskt i förhållande till lagrets nya storlek. Om det aktuella lagret till exempel är centrerat på baslagret flyttas det längre till höger om baslagret om du utökar lagrets vänstra sida.

* **Ändra position för ett lager**: Om du vill ändra position för ett lager på arbetsytan markerar du lagrets namn i listan Lager och använder någon av följande tekniker:

* **Ändra position manuellt**: Flytta pekaren nära, men inte över, en lagergräns, och när du ser den fyrhövdade pilmarkören markerar du och börjar dra.

* **Ange förskjutningsmått för position**: Ange förskjutningsmått för X och Y i textrutorna X och Y. Dessa mått representerar x-, y-förskjutningen för ankarpunkten i pixlar.

* **Rotera ett lager**: Rutan Rotera visar vinkeln som lagret roterades till. Om du vill rotera ett lager markerar du lagrets namn i listan Lager och använder någon av följande tekniker:

* **Rotera** manuellt: Flytta markören nära, men inte över, ett hörn av lagret. När du ser rotationsmarkören drar du i hörnet av lagret. Håll ned Skift medan du drar om du vill rotera i steg om 15 grader.

* **Ange ett gradmått**: Ange hur många grader lagret ska roteras. Rotationen är medsols. Om du vill rotera moturs anger du ett negativt tal.

**Dölj ett lager eller en lagereffekt:**

Du kan dölja ett lager eller en lagereffekt genom att markera ögonikonen bredvid ett lagernamn eller effektnamn. Dolda lager visas inte i förhandsvisningar eller utdata. Lagerinformationen tas inte bort från URL:en. I stället läggs `hide=1` till i URL:en för att notera att lagret är dolt. Till exempel:

`layer=5&src=is{PortalCo/title}&pos=274,192&effect=-1&.effect=Drop Shadow&blendmode`

`layer=5&src=is{PortalCo/title}&pos=274,192&hide=1&effect=-1&.effect=Drop Shadow&blendmode`

### Bestämma bakgrundsfärg, opacitet och blandningsläge

Om du vill välja bakgrundsfärg, opacitet och blandningsläge för ett lager eller arbetsytan markerar du lagret eller arbetsytan och använder följande tekniker:

* **Förgrundsfärg**: Markera **[!UICONTROL Foreground Color]** och välj en färgruta om du vill ändra färgen på skuggan eller glöden. Du kan också ange en färgvärdesparameter i rutan. Bakgrundsfärgen används bara för lager som använder genomskinlighet. Det gäller till exempel ett delvis genomskinligt lager i en pristagg eller bakgrunden i ett textfält. Lager som består av en PSD-, TIFF- eller PNG-bild med genomskinlighet aktiverat kan ha genomskinliga bakgrunder.

* **Bakgrundsfärg**: Markera **[!UICONTROL Background Color]** och välj en färgruta om du vill ändra färgen på de utfyllda områdena.

* **Opacitet**: Dra opacitetsreglaget för att göra ett lager genomskinligt så att en del av den underliggande bilden syns igenom. Inställningen på 100 procent är ogenomskinlig och 0 är genomskinlig.

* **Blandningsläge**: Välj ett alternativ om du vill simulera ett av de blandningslägen som är tillgängliga i Photoshop. Alternativen är Normal, Lös upp, Ljusare, Mörkare, Multiplicera och Skärm. De här alternativen är tillgängliga för lager, inte för arbetsytan.

## Använd skugg- och glödeffekter på lager {#using-shadow-and-glow-effects-on-layers}

Du kan använda en skugga eller glöd på ett lager. Skuggan eller glöden gäller för lagrets omkrets och sträcker sig inåt eller utåt, beroende på vilket skugg- eller glödalternativ du väljer. Om mallen har skapats med en PSD-fil med skugg- och glödeffekter kan du justera dessa effekter i Adobe Dynamic Media Classic.

När du har använt en skugg- eller glödeffekt kan du justera dess storlek, färg, opacitet och position i området Lageregenskaper på mallskärmen.

### Använda en skugg- eller glödeffekt på ett lager {#applying-a-shadow-or-glow-effect-to-a-layer}

1. Markera ett lager i listan Lager.
1. Välj menyn **[!UICONTROL `Add Effect`]** och välj ett alternativ:

   * **[!UICONTROL Drop Shadow]**: Använder en skugga på lagrets nedre och högra sida.

   * **[!UICONTROL Inner Shadow]**: Använder en skuggeffekt inuti alla kanter i lagret.

   * **[!UICONTROL Outer Glow]**: Använder en glödeffekt runt alla kanter i lagret.

   * **[!UICONTROL Inner Glow]**: Använder en glödeffekt inuti alla kanter i lagret.

Ett effektnamn visas i listan Lager när du har använt en effekt. Om du vill ta bort en effekt markerar du dess namn i listan Lager och väljer sedan **[!UICONTROL Delete]**.

>[!NOTE]
>
>Ibland kan du inte se effekten av en skugga eller yttre glöd om det underliggande lagret inte är tillräckligt stort för att kunna visa det. Om du inte kan se skuggan eller glöden kan du lägga till utfyllnadsvärden i lagret eller ändra ordningen på lagret. Se [Ändra storlek och position för lager och arbetsytan](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) och [Ändra ordning på lager](creating-template.md#reordering_layers).

### Justera en skugg- eller glödeffekt {#adjusting-a-shadow-or-glow-effect}

Om du vill justera en skugg- eller glödeffekt börjar du med att markera dess namn i listan Lager. Ändra sedan inställningarna under Lageregenskaper på mallskärmen:

* **[!UICONTROL Color]**: Välj knappen Färg och välj en färgruta om du vill ändra färgen på skuggan eller glöden. Du kan också ange en färgvärdesparameter i rutan.

* **[!UICONTROL Opacity]**: Dra i skjutreglaget för att bestämma hur intensiv effekten är. Mindre ogenomskinliga effekter är mer genomskinliga.

* **[!UICONTROL Blend Mode]**: Välj ett alternativ om du vill simulera ett av de blandningslägen som är tillgängliga i Photoshop. Alternativen är Normal, Lös upp, Ljusare, Mörkare, Multiplicera och Skärm.

* **[!UICONTROL Size]**: Ange mått i rutan X och Y för att förstora eller förminska skuggeffekten. Storleksalternativ är bara tillgängliga för inre skuggor och skuggor.

* **[!UICONTROL Grow]**: Dra skjutreglaget för att utöka effekten inåt eller utåt.

* **[!UICONTROL Blur]**: Dra i skjutreglaget för att styra luddet vid effektens kanter. Effekter med mer oskärpa är mer luddade.

## Maskeringslager {#masking-layers}

I lagerlistan finns en maskknapp som anger hur masken eller alfakanalen i ett lager ska användas. Med knappen Mask kan du använda effekten av ett bakgrundslager på ett visst lager eller på hela det överordnade lagret i mallen. Markera ett lager i lagerlistan och välj **[!UICONTROL Mask]** för att bläddra igenom dessa lägen:

* Lagrets bakgrund är ogenomskinlig.
* Lagerinnehållet inverteras och lagrets bakgrund fylls med solid svart.
* Lagrets bakgrund är fylld med solid svart.
