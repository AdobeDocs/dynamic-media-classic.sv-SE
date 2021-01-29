---
title: Skapa en mall
description: Lär dig hur du skapar en mall i Dynamic Media Classic.
uuid: c762224b-7c6c-4434-bada-c26570079645
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 8f7093da-d215-4337-ac95-69f0a5bf8648
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '3437'
ht-degree: 0%

---


# Skapa en mall {#creating-a-template}

Om du vill skapa en mall klickar du på Skapa > Grundläggande om mallar. Välj antingen Designer eller Developer. På den här sidan kan du lägga till bild- och textlager. Du kan också ändra ordning på lager, ändra storlek och position för lager och använda skugg- och glödeffekter på bilder och text.

>[!NOTE]
>
>Om du redigerar en mall som har skapats i en tidigare version av Dynamic Media Classic kan du få ett meddelande när du sparar med frågan&quot;Vill du lägga till ett arbetsytelager?&quot; Välj Nej om du inte vill lägga till ett nytt baslager. Om du av misstag väljer Ja tar du bort modifieringarna &quot;&amp;allowCanvasPrompt&quot; och &quot;&amp;layer=0&quot; i URL:en och trycker på Retur.

## Skapar den inledande mallen {#creating-the-initial-template}

När du skapar en malluppsättning påverkar alternativet **Publicera efter spara** uppsättningen och anger medlemmar på följande sätt:

| Alternativet Publicera efter spara är markerat innan du sparar? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
|--- |--- |--- |
| Ja | Publicerad | Publicerad |
| Nej | Opublicerad | Ange medlemmar behåller sitt publicerade eller opublicerade läge. |

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

Du kan skapa en mall från en befintlig mall. Öppna mallen, klicka på **Spara som** och ange ett nytt namn i dialogrutan Spara som.

**Skapa den inledande malluppsättningen**

1. Använd någon av följande metoder när du skapar mallen:

   **Markera PSD-filen eller bilderna** förstMarkera PSD-filen eller bilderna som du vill använda för mallen på panelen Bläddra och klicka sedan på Skapa > Mallgrunder.

   **Starta från** mallskärmenKlicka på Skapa > Grundläggande om mallar. Välj antingen Designer eller Developer.

1. I dialogrutan Ange storlek på arbetsyta anger du bredd- och höjdmått för mallen.
1. Markera en mapp i resursbiblioteket och dra PSD-filen eller bilderna som du vill använda för mallen till mallskärmen.
1. När du är klar ser du till att **Publicera efter spara** är markerat (standard) nära sidans nedre högra hörn.
1. Klicka på **Spara**.
1. Välj en mapp där du vill lagra mallen, ange ett namn för mallen och klicka på **Skicka**.

   Dynamic Media Classic förminskar bilder om det behövs för att de ska få plats på arbetsytan, området på mallskärmen för att definiera mallen.

## Redigera en malluppsättning {#editing-a-template-set}

Beroende på om du redigerar en publicerad uppsättning eller en opublicerad malluppsättning påverkar alternativet **Publicera efter spara** uppsättningen och ange medlemmar på följande sätt:

| Har du redan publicerat? | Alternativet Publicera efter spara är markerat innan du sparar redigeringen? | Status för uppsättning efter sparande | Tillstånd för angivna medlemmar efter att de har sparats |
|--- |--- |--- |--- |
| Ja | Ja | Publicerad | Publicerad |
| Ja | Nej | Publicerad | Befintliga uppsättningsmedlemmar behåller sin publicerade status.Alla nya uppsättningsmedlemmar som du lägger till under redigeringen behåller sin publicerade eller opublicerade status. |
| Nej | Ja | Publicerad | Publicerad |
| Nej | Nej | Opublicerad | Befintliga uppsättningsmedlemmar och nya uppsättningsmedlemmar som du har lagt till under redigeringen behåller sina publicerade eller opublicerade tillstånd. |

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

**Redigera en malluppsättning**

1. I stödrastervyn bläddrar du till en malluppsättning och klickar sedan under bilden på **Redigera**.
1. Gör önskade ändringar i mallen.
1. När du är klar med redigeringen ser du till att **Publicera efter spara** är markerat (standard) nära sidans nedre högra hörn.
1. Klicka på **Spara**, markera en lagringsmapp, ange ett namn för uppsättningen och klicka sedan på **Spara**.

## Tar bort en mall {#deleting-a-template}

När du tar bort en malluppsättning flyttas själva uppsättningen till papperskorgen. Medlemmarna (eller &quot;barn&quot;) i uppsättningen påverkas dock inte. i stället behåller de sitt befintliga publicerade eller opublicerade läge.

Se även [Publicera resurser](publishing-files.md#manually_publishing_assets) och [Manuellt avpublicera resurser](publishing-files.md#manually_unpublishing_assets).

**Ta bort en mall**

1. Välj en eller flera mallar i Stödrastervisning, listvy eller detaljvy.
1. I det globala navigeringsfältet klickar du på **Arkiv** > **Ta bort** > **Ta bort**.

## Om mallfönstret {#understanding-the-template-screen}

På mallskärmen finns verktyg för att ändra och parametrisera lager.

Använd de här verktygen på mallskärmen för att skapa mallar:

**Panoreringsverktyg** Gör att du kan markera lager, flytta dem runt arbetsytan, ändra storlek på dem eller rotera dem.

**Textverktyget** Skapar ett textlager. Skapa ett textlager genom att dra på arbetsytan och ange sedan texten i lagret. Se Skapa ett textlager.

**FörhandsgranskningsknappÖppnar** förhandsgranskningsskärmen och visar mallen i ett zoomvisningsprogram. Du ser hur mallen ser ut för användare på din webbplats eller i ditt program.

**Knappen** ParametersammanfattningÖppnar fönstret Parametersammanfattning. Du kan se namnet på varje lager i en mall, och på varje lager, namnen på de parametrar som har aktiverats.

**Textredigeraren v4.3 och textredigeraren v4.2** Du kan välja att använda den senaste och mest avancerade textredigeraren, textredigeraren v4.3 eller den tidigare textredigeraren, v4.2. När du skapar nya mallar väljs textredigeraren v4.3 som standard. När du redigerar äldre mallar väljs textredigeraren v4.2 som standard. Textredigeraren v4.3 stöder för närvarande inte automatisk radbrytning, så när du redigerar äldre mallar som använder automatisk radbrytning bör du använda textredigeraren v4.2 för att behålla mallens återgivning helt intakt. Om den äldre mallen inte använder automatisk radbrytning kan du välja textredigeraren v4.3 för att utnyttja alla nya funktioner som den har, till exempel Öka marginaler, Minska marginaler, Ange text i versaler och Kopiera textpassning.

***Obs **! Textredigeraren v4.2 kommer till slut att tas bort som ett alternativ i Dynamic Media Classic, så vi rekommenderar att du använder textredigeraren 4.3 när det är möjligt. Alternativet Radbrytning kommer att införlivas i en framtida version av textredigeraren.*

**Designer och** utvecklareVälj det alternativ som bäst beskriver din roll.

**Arbetsyta** Definierar det totala tillgängliga området, i pixlar, för att definiera mallen. Standardstorleken är 300 x 300 pixlar. Lager placeras på arbetsytan.

**Lager-** listaVisar namnet på lagren i mallen. Om du vill markera ett lager markerar du lagrets namn i listan Lager. Listan Lager innehåller verktyg för att lägga till effekter i lager, ta bort lager, ordna om lager och parametrisera lager. Se Arbeta med lager.

**Lageregenskapsområde** Innehåller verktyg för att ändra bakgrundsfärg, opacitet, storlek och position för ett lager samt bakgrundsfärg, opacitet och storlek för arbetsytan. Du kan också justera skugg- och glödeffekter. Se Arbeta med lager.

## Skapar bildlager {#creating-image-layers}

1. Dra bilden från resursbiblioteket till arbetsytan.

   Bildens ID-namn visas i listan Lager.

>[!NOTE]
>
>Om det behövs krymper Dynamic Media Classic bilderna så att de får plats på arbetsytan när du skapar ett bildlager.

## Skapa ett textlager {#creating-a-text-layer}

1. Klicka på textverktyget.
1. Dra för att skapa en textruta på arbetsytan eller på en bild.
1. På textskärmen som öppnas lägger du till text genom att göra något av följande på fliken Förhandsgranska:

   * Skriv text i textrutan. Välj Kopiera anpassa text så att texten får plats i textrutan.
   * Klistra in text från Urklipp i textrutan.

1. Klicka på Använd och stäng sedan textskärmen.

### Formatera text {#format-text}

Så här formaterar du text i ett textlager:

1. Dubbelklicka på namnet på textrutan med den text du vill redigera i listan Lager. Textredigeraren öppnas.
1. Markera texten som du vill formatera i textrutan. Du kan markera all text, alla delar av texten samt enskilda tecken.
1. Ange något av dessa formateringsalternativ och klicka sedan på Använd.

   **** TeckensnittVälj ett teckensnitt på menyn Teckensnitt. Om ett teckensnitt som du vill använda inte visas på menyn kan du överföra det till Dynamic Media Classic. Se Teckensnitt.

   **TeckensnittsstorlekVälj en** teckenstorlek på menyn, skriv en specifik storlek i rutan eller klicka på upp- eller nedpilarna för att öka eller minska storleken med två punkter.

   **** FärgKlicka för att välja en textfärg.

   **Fet, Kursiv eller** UnderstrukenMarkera texten och klicka sedan på ikonen för den typ av formatering du vill använda för texten.

   **Versaler, Upphöjd eller** NedsänktMarkera texten och klicka sedan på ikonen för den typ av formatering du vill använda på texten.

   **** JusteringVälj en justeringsknapp för att vänsterjustera, centrera eller högerjustera text i textlagret.

   **Ange** TrackingType eller välj ett numeriskt värde som du vill justera avståndet mellan ord med.

   **** KerningType eller välj ett numeriskt värde som du vill justera avståndet mellan tecknen med.

   **Radavstånd** Ange eller välj ett numeriskt värde som du vill justera avståndet mellan raderna med.

   **Baslinje** ShiftType eller välj ett numeriskt värde som du vill flytta ett markerat tecken med uppåt eller nedåt i förhållande till den omgivande textens baslinje. Det här alternativet är särskilt användbart när du ställer in bråktal för hand eller justerar positionen för textbundna bilder.

>[!NOTE]
>
>Klicka på Ångra om du vill ångra den senaste åtgärden. Klicka på Gör om om du ångrar en åtgärd när du har klickat på Ångra.

### Formatera stycken {#format-paragraphs}

1. Dubbelklicka på namnet på textrutan med den text du vill redigera i listan Lager. Textredigeraren öppnas.
1. Markera stycket som du vill formatera.
1. Ange något av dessa formateringsalternativ och klicka sedan på Använd.

   **** JusteringKlicka för att ange justeringstypen: justera åt vänster, centrera, justera åt höger eller marginaljustera.

   **Justering av** styckeslutKlicka för att ange typ av justering för den sista raden i stycket: sista raden vänsterjusteras, sista raden i mitten, och sista raden justeras åt höger.

   **Radavstånd** Skriv eller välj ett numeriskt värde som du vill justera avståndet mellan alla rader i stycket med.

   **Öka indraget genom att dra in** allClick.

   **Ta bort** indragKlicka för att minska textens indrag.

   **Dra in första** radenAnge med hur mycket den första textraden ska dras in.

   **Avstånd före** styckeAnge hur mycket utrymme du vill ha ovanför den första textraden i stycket.

   **Avstånd efter** styckeAnge hur mycket utrymme du vill ha under den sista textraden i stycket.

   **Lodrät** justeringMarkera var du vill att texten ska visas lodrätt i textrutan: Överkant, Mitten, Nederkant.

   **TextorienteringVälj den** riktning som texten ska visas i: Höger till vänster eller vänster till höger.

### Justera egenskaper för textlager {#adjust-text-layer-properties}

1. Markera textrutan som du vill justera på skärmen Grundläggande om mallar.
1. Välj något av följande på panelen Lageregenskaper:

   **Krymp text (endast textredigeraren v4.2)** Välj det här alternativet om du vill krympa texten så att den passar i textrutan.

   **Radbyte (endast textredigeraren v4.2)** Välj ett radbrytningsalternativ för att ange om eller hur texten ska radbrytas:

   **Figursätt Texten** radbryts så att den passar i en textruta som är för liten vågrätt.

   **Ingen** radbrytning Texten radbryts inte när textrutan är för liten vågrätt, utan en del av texten tas bort.

   **NB Wrap**  (Nonbreaking wrap) Figursätter text så att den passar in i en textruta och bryter inte ord.

   **Placering** Anger textrutans plats på arbetsytan.

   **** UtfyllnadLägger till marginaler eller beskär lagerrektangeln. Ange antalet pixlar som ska läggas till eller tas bort för Vänster, Upptill, Underkant och Höger. Ange positiva tal för att lägga till en marginal. ange negativa tal som ska beskäras.

### Visa och redigera textkällkod {#view-and-edit-text-source-code}

Informationen på fliken Källa i textredigeraren är till för din referens. Redigera bara texten om du är bekant med att redigera källkod.

1. Dubbelklicka på namnet på textrutan med den text du vill redigera i listan Lager. Textredigeraren öppnas.
1. Klicka på fliken Källa i textredigeraren för att visa källkoden för texten.
1. Visa eller redigera texten efter behov.

   Ändringarna förblir intakta om du växlar fram och tillbaka mellan förhandsvisnings- och källvyn.

1. Klicka på Använd för att återge redigeringarna.

## Arbeta med lager {#working-with-layers}

Använd lagerlistan och området Lageregenskaper när du vill arbeta med lager. Du kan ordna om lager, ändra deras storlek och position, rotera lager och bestämma bakgrundsfärg, förgrundsfärg, opacitet och blandningsläge för ett lager.

Du kan också ändra storlek på arbetsytan, välja bakgrundsfärg och ändra opacitetsinställningen.

### Ändra ordning på lager {#reordering-layers}

Om du ändrar lagerordningen kan det påverka utseendet, särskilt när genomskinlighet eller övertryck används. Se till att du förhandsgranskar resultatet innan du implementerar ändringarna.

1. Använd någon av dessa tekniker för att ordna om lagren i en mall:

   * Markera ett lager i listan Lager. Klicka sedan på upp- eller nedknappen så många gånger som behövs för att placera den på rätt plats i listan.
   * Dra ett lager uppåt eller nedåt i listan Lager.

### Ändra storlek och position för lager och arbetsytan {#changing-the-size-and-position-of-layers-and-the-canvas}

Lagren måste vara tillräckligt små för att få plats på arbetsytan. Du kan ändra storlek på ett lager eller arbetsytan manuellt eller genom att ange mått för storlek. Du kan ändra positionen för ett lager manuellt eller genom att ange förskjutningsmått. Du kan också rotera ett lager.

>[!NOTE]
>
>Dynamic Media Classic rekommenderar att du skapar en bildförinställning som har exakt samma storlek som mallen. Genom att matcha storleken på förinställningen för bild med mallstorleken kan du vara säker på att mallens slutliga utdatastorlek och skärpealternativ ställs in korrekt. När du har skapat den här bildförinställningen kan du välja den på menyn Använd förinställning på skärmen Förhandsvisa mall. På skärmen visas hur bilden ser ut när den levereras från servern. Se [Konfigurera bildförinställningar](setting-image-presets.md#setting_up_image_presets).

**Ändra storlek på ett lager**

Om du vill ändra storlek på ett lager eller arbetsytan markerar du lagret eller arbetsytan i listan Lager och använder någon av följande tekniker:

**Ändra** storlek manuelltMarkera och dra i ett hörn på lagret eller arbetsytan. Med textlager kan du också dra en sida av lagret. Håll ned Skift-tangenten när du drar om du vill ändra storlek men behålla proportionerna (formen).

**Ange** mått för lagerstorlekAnge pixelmått i textrutorna B (bredd) och H (höjd) i området Lageregenskaper.

Förutom att ändra storlek på ett lager kan du lägga ut det. Om du vill göra det anger du en utfyllnadsmätning i rutan Vänster, Höger, Upptill och Nedtill i området Lageregenskaper. Utfyllnad lägger till en marginal i det aktuella lagret för att förskjuta den från omkretsen av dess baslager. Utfyllnaden är användbar om du lägger till en skugga eller yttre glöd och vill göra effekten mer synlig. Utfyllnad ökar storleken på ett lager och visar dess bakgrundsfärg i det utökade utfyllnadsområdet. Baslagret flyttar sig automatiskt i förhållande till lagrets nya storlek. Om det aktuella lagret till exempel är centrerat på baslagret flyttas det längre till höger om baslagret om du utökar lagrets vänstra sida.

**Ändra ett lagers position**

Om du vill ändra positionen för ett lager på arbetsytan markerar du lagrets namn i listan Lager och använder någon av följande tekniker:

**Ändra** position manuelltFlytta pekaren nära, men inte över, en lagergräns, och när du ser den fyrhövdade pilmarkören klickar du och börjar dra.

**Ange** mått för positionsförskjutningAnge förskjutningsmått för X och Y i textrutorna X och Y. Dessa mått representerar x-, y-förskjutningen för ankarpunkten i pixlar.

**Rotera ett lager**

I rutan Rotera visas vinkeln som lagret roterades till. Om du vill rotera ett lager markerar du lagrets namn i listan Lager och använder någon av följande tekniker:

**Manuellt** roteraFlytta markören nära ett hörn av lagret men inte över det. När du ser rotationsmarkören drar du i hörnet av lagret. Håll ned Skift medan du drar om du vill rotera i steg om 15 grader.

**Ange ett** gradmåttAnge antalet grader för att rotera lagret. Rotationen sker medurs; Om du vill rotera moturs anger du ett negativt tal.

**Dölja ett lager eller en lagereffekt**

Du kan dölja ett lager eller en lagereffekt genom att klicka på ögonikonen bredvid ett lagernamn eller effektnamn. Dolda lager visas inte i förhandsvisningar eller utdata. Lagerinformationen tas inte bort från URL:en. I stället läggs&quot;hide=1&quot; till i URL:en för att se att lagret för närvarande är dolt. Exempel:

layer=5&amp;src=is{PortalCo/title}&amp;pos=274,192&amp;effect=-1&amp;.effect=Drop Shadow&amp;blendmode

layer=5&amp;src=is{PortalCo/title}&amp;pos=274,192&amp;hide=1&amp;effect=-1&amp;.effect=Drop Shadow&amp;blendmode

### Bestämma bakgrundsfärg, opacitet och blandningsläge {#determining-the-background-color-opacity-and-blend-mode}

Om du vill välja bakgrundsfärg, opacitet och blandningsläge för ett lager eller arbetsytan markerar du lagret eller arbetsytan och använder följande tekniker:

**FörgrundsfärgKlicka** på knappen Förgrundsfärg och välj en färgruta om du vill ändra färgen på skuggan eller glöden. Du kan också ange en färgvärdesparameter i rutan. Bakgrundsfärgen används bara för lager som använder genomskinlighet. Det gäller till exempel ett delvis genomskinligt lager i en pristagg eller bakgrunden i ett textfält. Lager som består av en PSD-, TIFF- eller PNG-bild med genomskinlighet aktiverat kan ha genomskinliga bakgrunder.

**BakgrundsfärgKlicka** på knappen Bakgrundsfärg och välj en färgruta om du vill ändra färgen på de utfyllda områdena.

**** OpacitetDra opacitetsreglaget för att göra ett lager genomskinligt så att en del av den underliggande bilden syns igenom. Inställningen på 100 procent är helt ogenomskinlig. 0-inställningen är genomskinlig.

**BlandningslägeVälj ett** alternativ för att simulera ett av de blandningslägen som är tillgängliga i Photoshop. Alternativen är Normal, Lös upp, Ljusare, Mörkare, Multiplicera och Skärm. De här alternativen är tillgängliga för lager, inte för arbetsytan.

## Använda skugg- och glödeffekter på lager {#using-shadow-and-glow-effects-on-layers}

Du kan använda en skugga eller glöd på ett lager. Skugga eller glöd används i utkanten av lagret och sträcker sig inåt eller utåt, beroende på vilket skugg- eller glödalternativ du väljer. Om mallen har skapats med en PSD-fil med skugg- och glödeffekter kan du justera dessa effekter i Dynamic Media Classic.

När du har använt en skugg- eller glödeffekt kan du justera dess storlek, färg, opacitet och position i området Lageregenskaper på mallskärmen.

### Använda en skugg- eller glödeffekt på ett lager {#applying-a-shadow-or-glow-effect-to-a-layer}

Så här använder du en skugg- eller glödeffekt:

1. Markera ett lager i listan Lager.
1. Välj menyn Lägg till effekt och välj ett alternativ:

   **Skugga** Använder en skugga på lagrets nedre och högra sida.

   **Inre** skuggaAnvänder en skuggeffekt inuti lagrets alla kanter.

   **Yttre** glödAnvänder en glödeffekt runt lagrets alla kanter.

   **Inre** glödAnvänder en glödeffekt inuti lagrets alla kanter.

Ett effektnamn visas i listan Lager när du har använt en effekt. Om du vill ta bort en effekt markerar du effektens namn i listan Lager och klickar sedan på knappen Ta bort.

>[!NOTE]
>
>Ibland kan du inte se effekten av en skugga eller yttre glöd om det underliggande lagret inte är tillräckligt stort för att visas. Om du inte kan se skuggan eller glöden kan du lägga till utfyllnadsvärden i lagret eller ändra ordningen på lagret. Se [Ändra storlek och position för lager och arbetsytan](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas)och [Ändra ordning på lager](creating-template.md#reordering_layers).

### Justera en skugg- eller glödeffekt {#adjusting-a-shadow-or-glow-effect}

Om du vill justera en skugg- eller glödeffekt börjar du med att markera dess namn i listan Lager. Ändra sedan inställningarna under Lageregenskaper på mallskärmen:

**** FärgVälj knappen Färg och välj en färgruta om du vill ändra färgen på skuggan eller glöden. Du kan också ange en färgvärdesparameter i rutan.

**** OpacitetDra skjutreglaget för att bestämma hur intensiv effekten är. Mindre ogenomskinliga effekter är mer genomskinliga.

**BlandningslägeVälj ett** alternativ för att simulera ett av de blandningslägen som finns i Photoshop. Alternativen är Normal, Lös upp, Ljusare, Mörkare, Multiplicera och Skärm.

**** StorlekAnge mått i rutan X och Y om du vill förstora eller förminska skuggeffekten. Storleksalternativ är bara tillgängliga för inre skuggor och skuggor.

**** UtvidgaDra skjutreglaget för att utöka effekten inåt eller utåt.

**** OskärpaDra i skjutreglaget för att styra luddet vid effektens kanter. Effekter med mer oskärpa är mer luddade.

## Maskera lager {#masking-layers}

I lagerlistan finns en maskknapp som anger hur masken eller alfakanalen i ett lager ska användas. Med knappen Mask kan du använda effekten av ett bakgrundslager på ett visst lager eller på hela det överordnade lagret i mallen. Markera ett lager i listan Lager och välj knappen Mask för att bläddra igenom dessa lägen:

* Lagrets bakgrund är ogenomskinlig.
* Lagerinnehållet inverteras och lagrets bakgrund fylls med solid svart.
* Lagrets bakgrund är fylld med solid svart.

