---
title: Vanliga frågor om uppgradering
description: Vanliga frågor och svar när du uppgraderar från [!DNL Adobe Dynamic Media Classic] datorprogrammet till [!DNL Dynamic Media] på [!DNL Adobe Experience Manager] Assets.
feature: Dynamic Media Classic
role: Admin,User
exl-id: 5c2e2937-fe4f-4b64-bee8-9572ca84695b
topic: Content Management
level: Intermediate
source-git-commit: 4601442c2d51d50a2712eee7fd8e5110b43fb2a0
workflow-type: tm+mt
source-wordcount: '1564'
ht-degree: 0%

---

# Frågor och svar om uppgradering från [!DNL Dynamic Media Classic] till [!DNL Dynamic Media]

## Allmän information

+++**Vad är [!DNL Dynamic Media] i [!DNL Adobe Experience Manager] Assets?**
[!DNL Dynamic Media] är nästa generations [!DNL Adobe Dynamic Media Classic] -funktioner (tidigare Scene7) i [!DNL Experience Manager] Assets. Lösningen kombinerar styrkan i resurshantering med multimedieleverans. Följande funktioner ingår:

* Ett användargränssnitt och en plattform för hantering av bilder och video.
* Innovativa marknadsföringsfunktioner.
* Adobe robusta och beprövade leveransplattform.
* Smidig enhetlighet med [!DNL Experience Manager] Assets.

+++

+++**Vilka är de viktigaste fördelarna med att uppgradera till [!DNL Dynamic Media]?**

* Collaboration och delad filsynkronisering med [!DNL Adobe Creative Cloud] program.
* Digital resurshantering på företagsnivå med:
   * stöd för robusta metadata
   * smart sökning
   * ljuslåda och samlingar
   * versionskontroll
   * säker resursdelning för användning av leverantörer, partners och franchisetagare
* Granska och godkänn arbetsflöden för resurser som bearbetas.
* Enkelt att använda och använda med det nya användargränssnittet.
* Skapa köpbara/interaktiva medieupplevelser med bilder och video som ökar konverteringsgraden och ökar användarnas engagemang och nöjdhet.
* Kombinera kampanjresurser med produktinformation så att ni kan effektivisera klickningen i kundvagnen.
* Skapa, justera, märk upp och distribuera enkelt interaktiva visningsprogram med WYSIWYG Viewer Designer.
* Leverera optimerade multimedielösningar till [!DNL Experience Cloud].
* Integrering med [!DNL Experience Cloud] för avancerad tillgångsanalys, målinriktning och återanvändning av resurser över alla kontaktytor för marknadsföring. Dessa kontaktytor omfattar [!DNL Adobe Campaign] för e-post, [!DNL Adobe Social] för sociala kanaler och [!DNL Experience Manager] webbplatser för responsiva webb- och mobilappar.

+++

+++**Använder [!DNL Dynamic Media] det befintliga Adobe CDN (Content Delivery Network)?**
Ja, [!DNL Dynamic Media] använder Adobe stabila leveransnätverk i toppskiktet.

* Berika multimedieleverantörer till Internet Retail 1000, nio år i rad.
* Stöd för 24/7/265, 99,95 % SLA.
* Beprövad infrastruktur som betjänar över 800 kunder över hela världen, 3,5 petabyte trafik per månad och över 500 miljoner tillgångar i ledning, 60 % ökning av trafiken per år.

+++

+++**Vad är [!DNL Dynamic Media Classic]? Byter Adobe namn på Adobe Scene7?**
Adobe har ändrat namnet på Adobe Scene7 till [!DNL Dynamic Media Classic] .

+++

## Uppgraderingsprocess och verktyg

+++**Vem är berättigad till uppgraderingsprogrammet?**
Kunder som för närvarande har [!DNL Dynamic Media Classic] (tidigare Scene7) och som också har [!DNL Experience Manager] .

+++

+++**Hur startar jag uppgraderingsprocessen?**
Kontakta Adobe Account Team eller [mejla s7support@adobe.com](mailto:s7support@adobe.com) med ärenderaden `[!DNL Dynamic Media] Upgrade Program` .

+++

+++**Hur hanteras uppgraderingsprocessen?**
AGS (Adobe Global Services) hanterar uppgraderingen och behandlar den som ett serviceprojekt. Adobe erbjuder endast migrering av resurserna. Kunden, AGS eller Partner ansvarar för alla andra uppgraderingsaspekter och steg. På en sammanfattningsnivå innehåller en uppgraderingsplan följande:

* Tillhandahåll företag-/användarkonton.
* Replikera resurser från [!DNL Dynamic Media Classic] (tidigare Scene7) till [!DNL Dynamic Media]-komponenten i [!DNL Experience Manager] Assets (tillhandahålls av Adobe via ett automatiskt uppgraderingsverktyg).
* Konfigurera inställningar för bild och video.
* Ändra produktionsprocesserna och utbilda användare.

+++

+++**Hur lång tid tar uppgraderingen?**
Uppgraderingsprocessen varierar beroende på flera faktorer, bland annat, men inte begränsat till: antalet resurser och resursernas storlek. AGS eller Partner hanterar projekttidslinjen.

+++

+++**Hur kontrollerar jag uppgraderingens status?**
Uppgraderingsprocessen varierar beroende på flera faktorer, bland annat, men inte begränsat till: antalet resurser och resursernas storlek. AGS eller Partner hanterar projekttidslinjen.

+++

+++**Behöver du uppgradera till [!DNL Dynamic Media]?**
Uppgraderingsprocessen varierar beroende på flera faktorer, bland annat, men inte begränsat till: antalet resurser och resursernas storlek. AGS eller Partner hanterar projekttidslinjen.

+++

+++**Är det någon skillnad i licenskostnad?**
Kontakta Adobe Account Team för mer information om prissättningen.

+++

+++**Är uppgraderingen förknippad med några driftavbrott?**
Nej. [!DNL Dynamic Media Classic] fortsätter att fungera utan avbrott under uppgraderingsprocessen. När uppgraderingen är klar och innehållet har validerats fungerar alla användare exklusivt i [!DNL Dynamic Media]-komponenten i [!DNL Experience Manager] Assets.

+++

+++**Krävs alla steg i checklistan för uppgraderingsberedskap?**
Nej. Kontrolllistan [beredskap](/help/using/upgrade-readiness.md) innehåller obligatoriska och valfria steg för bästa praxis.

+++

+++**Måste jag uppgradera?**
Nej. Adobe stöder och underhåller fullt ut [!DNL Dynamic Media Classic] (kundbegärda felkorrigeringar, säkerhetskorrigeringar, plattformsskalbarhet och tillförlitlighet) nu och i framtiden.

Du kan uppgradera när du är redo att dra nytta av de nya funktionerna i [!DNL Dynamic Media].

+++

+++**Kan jag fortfarande använda [!DNL Dynamic Media Classic] (tidigare Adobe Scene7) efter att jag har uppgraderat till [!DNL Dynamic Media]?**
När du har uppgraderat till [!DNL Dynamic Media] bör du bara använda Dynamic Media för bild och video. Du kan bara fortsätta använda [!DNL Dynamic Media Classic] för funktioner som ännu inte är tillgängliga i [!DNL Dynamic Media], bland annat följande:

* Visual configurator (image author, image render).
* Bildmallar.
* eCatalogs.

+++

+++**Vilka verktyg tillhandahåller Adobe för att automatisera uppgraderingsprocessen?**
För den första starten av uppgraderingsprogrammet har Adobe verktyg som automatiskt kan flytta resurser från [!DNL Dynamic Media Classic] till [!DNL Dynamic Media] i [!DNL Experience Manager] Assets.

+++

+++**Fortsätter befintliga [!DNL Dynamic Media Classic] URL:er, API-integreringar och visningsprogram att fungera under och efter uppgraderingen?**
Ja. Du kan fortsätta använda publicerings- och leveransinfrastrukturen [!DNL Dynamic Media Classic] (tidigare Adobe Scene7) som den är i lösningen [!DNL Dynamic Media].

+++

+++**Måste jag uppdatera mina produktions-URL:er?**
Nej. Adobe fortsätter att använda publicerings- och leveransinfrastrukturen [!DNL Dynamic Media Classic] som den är i lösningen [!DNL Dynamic Media]. Fördelen med det här arbetssättet är att du inte behöver ändra några produktions-URL:er på dina webbsidor, vilket minimerar riskerna och arbetet med att migrera till [!DNL Dynamic Media].

+++

+++**Måste jag skriva om API-integreringar och andra automatiseringsskript?**
Nej. Adobe fortsätter att använda publicerings- och leveransinfrastrukturen [!DNL Dynamic Media Classic] som den är i lösningen [!DNL Dynamic Media]. Dessutom replikeras alla resurser till [!DNL Dynamic Media Classic]. Fördelen med den här metoden är att du inte behöver skriva om API-baserade integreringar eller automatiseringsskript, vilket minimerar riskerna och ansträngningarna med migrering till [!DNL Dynamic Media].

+++

+++**Måste jag göra ändringar eller utveckla om mina anpassade visningsprogram?**
Nej. Adobe fortsätter att använda publicerings- och leveransinfrastrukturen [!DNL Dynamic Media Classic] som den är i lösningen [!DNL Dynamic Media]. Fördelen med den här metoden är att du kan fortsätta använda dina anpassade visningsprogram, vilket minimerar riskerna och ansträngningen med migreringen till [!DNL Dynamic Media].
+++

+++**Hur migrerar jag mina inställningar (till exempel bildförinställningar, videokodningar) till [!DNL Dynamic Media]?**
Förinställningar och andra inställningar måste återskapas i [!DNL Dynamic Media] . Som en del av serviceprojektet kan Adobe Global Services eller Partner hjälpa till.

+++

+++**Hur konfigurerar jag användare och behörigheter (SSO- eller LDAP-alternativ)?**
Inställningarna måste återskapas i [!DNL Dynamic Media] . Som en del av serviceprojektet kan AGS eller Partner hjälpa till. Om du uppgraderar till [!DNL Dynamic Media] får du SSO/LDAP-integrering, vilket gör användarhanteringen mer effektiv. Dessutom har [!DNL Dynamic Media] robusta roller och behörigheter som styr användaråtkomst.

+++

+++**Kan jag fortfarande använda FTP för att överföra resurser i grupp/grupp?**
Ja. Du behöver inte ändra dina befintliga arbetsflöden för inmatning och kan fortsätta schemalägga FTP-baserade överföringar.

+++

+++**Vilka resurser finns för utbildning av nya användare?**
Utbildning erbjuds via ADLS (Adobe Digital Learning Services). [!DNL Dynamic Media]-funktioner beskrivs i två kurser: Hantera och leverera digitala Assets och Anpassa digitala Assets.

+++

+++**Är [!DNL Dynamic Media] tillgängligt för alla platser?**
Ja. Adobe har datacentraler i Nordamerika, Europa och Stillahavsområdet.

+++

+++**Hur länge kommer [!DNL Dynamic Media Classic] att finnas som en fristående produkt?**
Adobe stöder och underhåller fullt ut [!DNL Dynamic Media Classic] (kundefterfrågade felkorrigeringar, säkerhetskorrigeringar, plattformsskalbarhet och tillförlitlighet) nu och i framtiden.

+++

+++**Hur mycket lagringsutrymme ingår i [!DNL Dynamic Media]?**
Dynamic Media levereras med 60 GB lagringsutrymme. Du kan köpa ytterligare lagringsutrymme i block om 250 GB. Kontrollera avtalsinformationen så att du kan få aktuell lagringstilldelning.

+++

+++**Vilka mått används för att mäta [!DNL Dynamic Media]-användningen?**
Sidvisningar per månad (PVM). Sidvy innebär en vy av ett e-postmeddelande eller en webbsida på en webbplats. Den innehåller även skärmvyer för applikationer, programskärmslägen, mobilwebbsidor och sidor för sociala nätverk. Sidvyer visas:

* Varje gång en webbsida läses in eller uppdateras
* När ett program läses in
* När innehåll återges
* Visas via ett öppnat eller visat e-postmeddelande

+++

+++**När kommer personaliserade media att vara tillgängliga med [!DNL Dynamic Media]?**
Adobe arbetar aktivt med att lägga till anpassade mediefunktioner i [!DNL Dynamic Media] . Mer information om när releasen ska komma.

+++

+++**Hur valideras resurser under uppgraderingen? Måste jag utföra manuell validering?**
Adobe utför en automatisk validering av alla resurser som flyttas till [!DNL Dynamic Media]. En allmän manuell validering av nyckelwebbplatser, sidor och upplevelser som drivs av [!DNL Dynamic Media] rekommenderas.

+++

+++**Finns det någon SLA för [!DNL Dynamic Media]?**
Ja. Kontakta Adobe Account Team för mer information.

+++

+++**Kan jag använda mitt eget CDN (Content Delivery Network) med [!DNL Dynamic Media]?**
Ja. Du kan använda ditt eget CDN med [!DNL Dynamic Media].

+++

+++**Har [!DNL Dynamic Media] de funktioner jag behöver så att jag kan uppgradera? Vilka funktioner är tillgängliga för [!DNL Dynamic Media] på [!DNL Experience Manager] Assets?**
Se sidan [ Funktionsjämförelse ](/help/using/upgrade-feature-comparison.md) där du kan läsa mer.

+++

+++**Vilka funktioner är fortfarande bara tillgängliga i [!DNL Dynamic Media Classic]? Kan jag fortfarande uppgradera?**
Kunder som behöver följande kan även fortsättningsvis ha tillgång till funktioner som kräver [!DNL Dynamic Media Classic] :

* Visual configurator (image author, image render).
* Bildmallar.
* eCatalogs.

Se även sidan [Funktionsjämförelse](/help/using/upgrade-feature-comparison.md) där du kan lära dig mer.

+++

+++**Vad händer med [!DNL Dynamic Media Classic] Media Portal-lösning?**
[!DNL Experience Manager] Brand Portal är ersättningserbjudandet för [!DNL Dynamic Media Classic] Media Portal.

+++

## Konsulttjänster

+++**Kan jag slutföra uppgraderingsprocessen själv?**
Nej. Samarbeta med er Adobe-representant och AGS för att göra uppgraderingen möjlig.

+++

+++**Hur ser tjänsteprojektet ut?**
Adobe samarbetar med er för att planera projektet. Adobe ansvarar för etablering och konfigurering av konton, replikering av resurser, testning och validering.

Kunderna är främst ansvariga för förändringshantering, inklusive utbildningsanvändare, redigeringsprocesser och utrullning av nya funktioner.

+++

## Support och utbildning

+++**Hur får jag support?**
Kundtjänst dygnet runt, alla dagar. [Kontakta teknisk support](https://experienceleague.adobe.com/sv?support-solution=General#support).

Telefon: 1-800-898-9743 (USA) | +44 (0)20 35641782 (Storbritannien) | +81-3-6743-9632 (Japan)

+++

+++**Var kan jag lära mig mer om betalda utbildningsalternativ?**
Se [ Adobe Digital Learning Services ](https://learning.adobe.com) .

Kontakta din Adobe Account Team-representant för anpassad eller individuell utbildning.

+++

## Ytterligare resurser

+++**Var kan jag läsa mer om [!DNL Dynamic Media] och dess funktioner?**
Mer information om [!DNL Dynamic Media] finns i [[!DNL Dynamic Media] mikrosite ](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/solutions.html) .

+++
