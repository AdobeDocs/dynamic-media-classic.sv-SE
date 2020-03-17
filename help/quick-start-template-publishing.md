---
title: '"Snabbstart: Mallpublicering"'
seo-title: '"Snabbstart: Mallpublicering"'
description: 'null'
seo-description: En introduktion och publicering med snabbstart till mall som hjälper dig att komma igång snabbt.
uuid: 101b6211-2421-4565-8635-944315a5c512
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: 03671fc1-ce3b-4fae-ad1f-53c99abcabde
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Snabbstart: Mallpublicering{#quick-start-template-publishing}

Med Adobe Dynamic Media Classic Web-to-Print kan du skapa professionellt varumärkesanpassat tryckmaterial som är enkelt för kunder, kunder och personal att anpassa och personalisera. Ni kan upprätthålla företagsinnehåll och varumärkesidentitet under hela publiceringsprocessen. Slutanvändare kan anpassa utskriftsinnehållet - men bara den del av innehållet som du låter dem anpassa. Personaliserade brevpapper, visitkort, affischer, gratulationskort, etiketter, checkar, presenter, kläder, kalendrar, scrapbooks och fotoalbum är exempel på skräddarsydda tryckprodukter som du kan leverera. Företag kan behålla en gemensam varumärkesidentitet i sin skylt som kan anpassas för olika regioner, franchise, butiker och filialkontor.

Du börjar med att designa en mall i Adobe Illustrator. Mallen definierar noggrant vad som är konstant och vad som är variabel - variabelkomponenterna är de som kan anpassas. När text i en Illustrator-fil till exempel har parametriserats kan slutanvändarna ange egen text. På samma sätt kan en bakgrundsfärg bytas ut mot en annan bakgrundsfärg när den har parametriserats som en variabelkomponent.

Dynamic Media Classic har två mallpubliceringsarbetsflöden, ett för grundläggande användningsområden och ett för avancerade användningsområden. De grundläggande användningsområdena är att skapa en design i Adobe Illustrator, överföra den till Dynamic Media Classic och definiera variabelelement med parametrar i SPS. För avancerade användningsområden krävs en mer heltäckande definition av variabilitet. Exempel på avancerade användningsområden är att skapa variabelelement i Adobe Illustrator, överföra filen till Dynamic Media Classic och ändra elementen direkt på XML-nivå med URL-anrop. Detta scenario anropas *`*DOM manipulation*`*.

>[!NOTE]
>
>Mer information om Dynamic Media Classic web-to-print-arbetsflöden, mallframtagning, parametrisering, DOM-manipulering med mera finns i handboken för web-to-print-arbetsflöde här: [www.adobe.com/go/learn_s7_webtoprint_en](https://www.adobe.com/go/learn_s7_webtoprint_en) . Ladda ned zip-filen till den lokala hårddisken och extrahera innehållet (självstudiekursen Dynamic Media Classic Web-To-PrintWorkflow och självstudiekurserna).

**Snabbstart**

Den här snabbstarten beskriver det grundläggande arbetsflödet för att använda Illustrator-filer för att skapa anpassningsbara tryckprodukter av hög kvalitet.

**1. Designa Illustrator-filen för mallpublicering**

Designa mallen i Illustrator. Om du vill använda den avancerade DOM-manipuleringsmetoden för att anpassa mallen definierar du s7:elementID:n för variabelelement i Illustrator.

Se [Skapa den inledande mallen i Illustrator](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator) och [DOM-redigering](dom-manipulation.md#dom_manipulation).

**2. Konvertera mallen till Dynamic Media Classic FXG och överför den till Scene7 Publishing System**

Adobe Creative Cloud-användare kan använda Adobe Illustrator-plugin-programmet för webb-till-tryck. Denna plugin konverterar mallar till Dynamic Media Classic FXG. Om en mall innehåller teckensnitt måste motsvarande teckensnittsfiler överföras till Scene7 Publishing System innan FXG-filen kan överföras.

Se [Överföra filer för mallpublicering](upload-files-template-publishing.md#upload_files_for_template_publishing).

**3. Visa, definiera eller förfina parametrar i Dynamic Media Classic**

På mallpubliceringens förhandsgransknings- och byggskärmar kan du definiera och förfina variabelelement via parametrar, förhandsgranska resultatet och testa resultatet. På dessa skärmar kan du:

* Skapa och ändra parametrar.
* Ange standardvärden för parameteregenskaper och attribut.
* Klicka på Kopiera URL för att kopiera förhandsvisnings-URL:en till Urklipp och förhandsgranska resultatet i ett webbläsarfönster.

Se [Parametrisera en mall i Dynamic Media Classic](parameterizing-template-scene7.md#parameterizing_a_template_in_scene7).

**4. Publicera FXG-mallen**

När du är klar med att definiera och testa parametrar och attribut publicerar du filen. När du publicerar din FXG-mall placeras den på de dynamiska mediabildsservrarna och URL:en aktiveras.

Glöm inte att publicera alla bilder och teckensnitt som är kopplade till FXG-mallen.

Se [Publicera FXG-mallar](dom-manipulation.md#publish_fxg_templates).

**5. Hämta URL**

Via sin URL är mallen nu klar att bäddas in på din webbplats så att slutanvändarna kan anpassa variabelt innehåll.

Se [Länka en FXG-mall till en webbsida](linking-fxg-template-web-page.md#linking_an_fxg_template_to_a_web_page).
