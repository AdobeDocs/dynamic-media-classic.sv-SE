---
title: Vanliga frågor om uppgradering
description: Vanliga frågor och svar när du uppgraderar från [!DNL Adobe Dynamic Media Classic] datorprogram till [!DNL Dynamic Media] på [!DNL Adobe Experience Manager] Resurser.
feature: Dynamic Media Classic
role: Admin,User
exl-id: 5c2e2937-fe4f-4b64-bee8-9572ca84695b
topic: Content Management
level: Intermediate
source-git-commit: 1b90beb99b161b76da81403f5aed9755b3a92c8b
workflow-type: tm+mt
source-wordcount: '1550'
ht-degree: 0%

---

# Frågor och svar om uppgradering från [!DNL Dynamic Media Classic] till [!DNL Dynamic Media]

## Allmän information

+++**Vad är [!DNL Dynamic Media] in [!DNL Adobe Experience Manager] Resurser?**
[!DNL Dynamic Media] är nästa generations utveckling av [!DNL Adobe Dynamic Media Classic] (tidigare Scene7) i [!DNL Experience Manager] Resurser. Lösningen kombinerar styrkan i resurshantering med multimedieleverans. Följande funktioner ingår:

* Ett användargränssnitt och en plattform för hantering av bilder och video.
* Innovativa marknadsföringsfunktioner.
* Adobe och beprövad leveransplattform.
* Smidig enhetlighet med [!DNL Experience Manager] Resurser.

+++

+++**Vilka är de viktigaste fördelarna med att uppgradera till [!DNL Dynamic Media]?**

* Samarbete och delad filsynkronisering med [!DNL Adobe Creative Cloud] program.
* Hantering av digitala resurser på företagsnivå med robust stöd för metadata, smart sökning, ljuslåda och samlingar, versionskontroll och säker delning av resurser som kan användas av leverantörer, partners och franchisetes Granska och godkänn-arbetsflöden för material i process.
* Enkelt att använda och använda med det nya användargränssnittet.
* Skapa köpbara/interaktiva medieupplevelser med bilder och video som ökar konverteringsgraden och ökar användarnas engagemang och nöjdhet.
* Kombinera kampanjresurser med produktinformation så att ni kan effektivisera klick till kundvagn.
* Skapa, justera, märk upp och distribuera enkelt interaktiva visningsprogram med WYSIWYG Viewer Designer.
* Leverera optimerad multimedia för [!DNL Experience Cloud] lösningar.
* Integrering med [!DNL Experience Cloud] för avancerad materialanalys, målgruppsanpassning och återanvändning av resurser över alla kontaktytor för marknadsföring. Dessa kontaktytor inkluderar [!DNL Adobe Campaign] för e-post, [!DNL Adobe Social] för sociala kanaler, och [!DNL Experience Manager] Webbplatser för responsiva webb- och mobilappar.

+++

+++**Gör [!DNL Dynamic Media] använda det befintliga Adobe CDN (Content Delivery Network)?**
Ja, [!DNL Dynamic Media] använder Adobe, leveransnätverk i toppskiktet.

* Berika multimedieleverantörer till Internet Retail 1000, nio år i rad.
* Stöd för 24/7/265, 99,95 % SLA.
* Beprövad infrastruktur som betjänar över 800 kunder över hela världen, 3,5-petabyte trafik per månad och över 500 miljoner mediefiler i ledning, 60 % ökning av trafiken per år.

+++

+++**Vad är [!DNL Dynamic Media Classic]? Byter Adobe namn på Adobe Scene7?**
Adobe ändrade namnet på Adobe Scene7 till [!DNL Dynamic Media Classic].

+++

## Uppgraderingsprocess och verktyg

+++**Vilka har rätt att uppgradera?**
Aktuell [!DNL Dynamic Media Classic] (tidigare Scene7) kunder som också har [!DNL Experience Manager].

+++

+++**Hur startar jag uppgraderingsprocessen?**
Kontakta Adobe Account Team eller [e-post s7support@adobe.com](mailto:s7support@adobe.com) med ämnesraden `[!DNL Dynamic Media] Upgrade Program`.

+++

+++**Hur hanteras uppgraderingsprocessen?**
Uppgraderingen hanteras av AGS (Adobe Global Services) och behandlas som ett serviceprojekt. Adobe kan endast migrera resurserna. Kunden, AGS eller Partner ansvarar för alla andra uppgraderingsaspekter och steg. På en sammanfattningsnivå innehåller en uppgraderingsplan följande:

* Tillhandahåll företag-/användarkonton.
* Replikera resurser från [!DNL Dynamic Media Classic] (tidigare Scene7) till [!DNL Dynamic Media] komponent i [!DNL Experience Manager] Resurser (tillhandahålls av Adobe via ett automatiserat uppgraderingsverktyg).
* Konfigurera inställningar för bild och video.
* Ändra produktionsprocesserna och utbilda användare.

+++

+++**Hur lång tid tar uppgraderingsprocessen?**
Uppgraderingsprocessen varierar beroende på flera faktorer, bland annat, men inte begränsat till: antalet resurser och resursernas storlek. AGS eller Partner hanterar projekttidslinjen.

+++

+++**Hur kontrollerar jag uppgraderingens status?**
Uppgraderingsprocessen varierar beroende på flera faktorer, bland annat, men inte begränsat till: antalet resurser och resursernas storlek. AGS eller Partner hanterar projekttidslinjen.

+++

+++**Krävs det några avtalsändringar att uppgradera till [!DNL Dynamic Media]?**
Uppgraderingsprocessen varierar beroende på flera faktorer, bland annat, men inte begränsat till: antalet resurser och resursernas storlek. AGS eller Partner hanterar projekttidslinjen.

+++

+++**Är det någon skillnad i licenskostnad?**
Kontakta Adobe Account Team för mer information om priser.

+++

+++**Har uppgraderingen några driftavbrott?**
Nej. [!DNL Dynamic Media Classic] fortsätter att fungera utan avbrott under uppgraderingsprocessen. När uppgraderingen är klar och innehållet har validerats arbetar alla användare uteslutande inom [!DNL Dynamic Media] komponent i [!DNL Experience Manager] Resurser.

+++

+++**Krävs alla steg i checklistan för uppgraderingsberedskap?**
Nej. The [checklista för beredskap](/help/using/upgrade-readiness.md) innehåller obligatoriska och valfria metodtips.

+++

+++**Måste jag uppgradera?**
Nej. Adobe fortsätter att stödja och upprätthålla fullt ut [!DNL Dynamic Media Classic] (kundefterfrågade felkorrigeringar, säkerhetskorrigeringar, plattformsskalbarhet och tillförlitlighet) nu och i framtiden.

Du kan uppgradera när du är redo att utnyttja de nya funktionerna i [!DNL Dynamic Media].

+++

+++**Kan jag fortsätta använda [!DNL Dynamic Media Classic] (tidigare Adobe Scene7) efter uppgradering till [!DNL Dynamic Media]?**
När du har uppgraderat till [!DNL Dynamic Media]bör du bara använda Dynamic Media för bild och video. Du kan fortsätta använda [!DNL Dynamic Media Classic] endast för funktioner som ännu inte är tillgängliga i [!DNL Dynamic Media] inklusive följande:

* Visual configurator (image author, image render).
* Bildmallar.
* eCatalogs.

+++

+++**Vilka verktyg tillhandahåller Adobe för att automatisera uppgraderingsprocessen?**
För uppgraderingsprogrammets första start har Adobe verktyg för att automatiskt flytta resurser från [!DNL Dynamic Media Classic] till [!DNL Dynamic Media] in [!DNL Experience Manager] Resurser.

+++

+++**Gör befintliga [!DNL Dynamic Media Classic] URL:er, API-integreringar och visningsprogram fortsätter att fungera under och efter uppgraderingen?**
Ja. Du kan fortsätta använda [!DNL Dynamic Media Classic] (tidigare Adobe Scene7) publicerings- och leveransinfrastruktur i [!DNL Dynamic Media] lösning.

+++

+++**Måste jag uppdatera mina URL:er?**
Nej. Adobe fortsätter att använda [!DNL Dynamic Media Classic] publicerings- och leveransinfrastruktur i [!DNL Dynamic Media] lösning. Fördelen med detta är att du inte behöver ändra några produktionswebbadresser på dina webbsidor, vilket minimerar riskerna och arbetet med att migrera till [!DNL Dynamic Media].

+++

+++**Måste jag skriva om API-integreringar och andra automatiseringsskript?**
Nej. Adobe fortsätter att använda [!DNL Dynamic Media Classic] publicerings- och leveransinfrastruktur i [!DNL Dynamic Media] lösning. Dessutom replikeras alla resurser till [!DNL Dynamic Media Classic]. Fördelen med detta är att du inte behöver skriva om några API-baserade integreringar eller automatiseringsskript, vilket minimerar riskerna och arbetet med att migrera till [!DNL Dynamic Media].

+++

+++**Måste jag göra ändringar eller utveckla om mina anpassade visningsprogram?**
Nej. Adobe fortsätter att använda [!DNL Dynamic Media Classic] publicerings- och leveransinfrastruktur i [!DNL Dynamic Media] lösning. Fördelen med detta är att du kan fortsätta att använda dina skräddarsydda visningsprogram, vilket minimerar riskerna och arbetet med att migrera till [!DNL Dynamic Media].
+++

+++**Hur migrerar jag mina inställningar (till exempel bildförinställningar, videokodning) till [!DNL Dynamic Media]?**
Förinställningar och andra inställningar måste återskapas i [!DNL Dynamic Media]. Som en del av serviceprojektet kan Adobe Global Services eller Partner hjälpa till.

+++

+++**Hur konfigurerar jag användare och behörigheter (SSO- eller LDAP-alternativ)?**
Inställningarna måste återskapas inom [!DNL Dynamic Media]. Som en del av serviceprojektet kan AGS eller Partner hjälpa till. Du uppgraderar dock till [!DNL Dynamic Media] ger SSO/LDAP-integrering, vilket gör användarhanteringen effektivare. Dessutom [!DNL Dynamic Media] har robusta roller och privilegier som styr åtkomsten till användarna.

+++

+++**Kan jag fortfarande använda FTP för att överföra resurser i grupp/grupp?**
Ja. Du behöver inte ändra dina befintliga arbetsflöden för inmatning och kan fortsätta schemalägga FTP-baserade överföringar.

+++

+++**Vilka resurser finns för att utbilda nya användare?**
Utbildning erbjuds via ADLS (Adobe Digital Learning Services). [!DNL Dynamic Media] finns i två kurser: Hantera och leverera digitala resurser och Anpassa digitala resurser.

+++

+++**Är [!DNL Dynamic Media] för alla länder?**
Ja. Adobe har datacentraler i Nordamerika, Europa och Asien-Stillahavsområdet.

+++

+++**Hur lång tid tar [!DNL Dynamic Media Classic] kommer du att existera som en fristående produkt?**
Adobe fortsätter att stödja och upprätthålla fullt ut [!DNL Dynamic Media Classic] (kundefterfrågade felkorrigeringar, säkerhetskorrigeringar, plattformsskalbarhet och tillförlitlighet) nu och i framtiden.

+++

+++**Hur mycket lagringsutrymme som [!DNL Dynamic Media]?**
Dynamic Media har 60 GB lagringsutrymme. Du kan köpa ytterligare lagringsutrymme i block om 250 GB. Kontrollera avtalsinformationen så att du kan få aktuell lagringstilldelning.

+++

+++**Vilket mätvärde används för att mäta [!DNL Dynamic Media] användning?**
Sidvisningar per månad (PVM). Sidvy innebär en vy av ett e-postmeddelande eller en webbsida på en webbplats. Det innehåller även programskärmsvyer, programskärmslägen, mobilwebbsidor och sidor för sociala nätverk. Sidvyer visas varje gång en webbsida läses in eller uppdateras, ett program läses in eller när innehållet återges eller visas via ett öppet eller visat e-postmeddelande.

+++

+++**När kommer personaliserade medier att vara tillgängliga med [!DNL Dynamic Media]?**
Adobe arbetar aktivt för att lägga till anpassade mediefunktioner i [!DNL Dynamic Media]. Mer information om när releasen ska komma.

+++

+++**Hur valideras resurser under uppgraderingen? Måste jag utföra manuell validering?**
Adobe utför en automatisk validering av alla resurser som flyttas till [!DNL Dynamic Media]. En allmän manuell validering av viktiga webbplatser, sidor och upplevelser som bygger på [!DNL Dynamic Media] rekommenderas.

+++

+++**Finns det något SLA för [!DNL Dynamic Media]?**
Ja. Kontakta Adobe Account Team för mer information.

+++

+++**Kan jag använda mitt eget CDN (Content Delivery Network) med [!DNL Dynamic Media]?**
Ja. Du kan använda ditt eget CDN med [!DNL Dynamic Media].

+++

+++**Gör [!DNL Dynamic Media] har jag de funktioner jag behöver så att jag kan uppgradera? Vilka funktioner är tillgängliga med [!DNL Dynamic Media] på [!DNL Experience Manager] Resurser?**
Se [Funktionsjämförelse](/help/using/upgrade-feature-comparison.md) sida där du kan lära dig mer.

+++

+++**Vilka funktioner som fortfarande är tillgängliga i [!DNL Dynamic Media Classic]? Kan jag fortfarande uppgradera?**
Kunder som behöver följande kan även fortsättningsvis ha tillgång till [!DNL Dynamic Media Classic] motordrivna funktioner

* Visual configurator (image author, image render).
* Bildmallar.
* eCatalogs.

Se även [Funktionsjämförelse](/help/using/upgrade-feature-comparison.md) sida där du kan lära dig mer.

+++

+++**Vad händer med [!DNL Dynamic Media Classic] Media Portal-lösning?**
[!DNL Experience Manager] Brand Portal är ersättningserbjudandet för [!DNL Dynamic Media Classic] Media Portal.

+++

## Konsulttjänster

+++**Kan jag slutföra uppgraderingsprocessen själv?**
Nej. Samarbeta med er Adobe-representant och AGS för att se vad uppgraderingen omfattar.

+++

+++**Hur ser tjänsteprojektet ut?**
Adobe samarbetar med dig för att planera projektet. Adobe ansvarar för etablering och konfigurering av konton, replikering av resurser, testning och validering.

Kunderna är främst ansvariga för förändringshantering, inklusive utbildningsanvändare, redigeringsprocesser och utrullning av nya funktioner.

+++

## Support och utbildning

+++**Hur får jag support?**
Kundtjänst dygnet runt, alla dagar. [Kontakta teknisk support](https://experienceleague.adobe.com/?support-solution=General#support).

Telefon: 1-800-898-9743 (USA) | +44 (0)20 35641782 (Storbritannien) | +81-3-6743-9632 (Japan)

+++

+++**Var kan jag lära mig mer om betalda utbildningsalternativ?**
Se [Adobe Digital Learning Services](https://learning.adobe.com).

Kontakta din Adobe Account Team-representant för anpassad eller individuell utbildning.

+++

## Ytterligare resurser

+++**Var kan jag läsa mer om [!DNL Dynamic Media] och dess funktioner?**
Se [[!DNL Dynamic Media] mikrosite](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/solutions.html) om du vill veta mer om [!DNL Dynamic Media].

+++
