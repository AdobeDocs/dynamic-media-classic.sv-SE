---
title: Beredskap för uppgradering
description: En checklista för beredskap för uppgradering när du vill gå från  [!DNL Adobe Dynamic Media Classic] till [!DNL Dynamic Media] på [!DNL Adobe Experience Manager].
feature: Dynamic Media Classic
role: Admin,User
exl-id: 86537998-b7e9-449c-83eb-6fd04533a00f
topic: Administration, Migration
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---

# Checklista för beredskap för uppgradering

Använd följande checklista för att få hjälp med att förstå och förbereda en uppgradering från [!DNL Dynamic Media Classic] till [!DNL Dynamic Media].

|  | Uppgift | Beskrivning |
| :--- | :--- | --- |
| **Fas 1: Licensiering** | Kör kontrakt | Baserat på trafik och lagring arbetar Adobe-kontoteamet med dig för att gå över från licensen [!DNL Dynamic Media Classic] och förnya licensen [!DNL Dynamic Media]. |
| **Fas 2: Förberedelse** | Validera funktionsanvändning | Bekräfta att funktionerna som används i [!DNL Dynamic Media Classic] är tillgängliga i [!DNL Dynamic Media]. Se sidan [Funktionsjämförelse](/help/using/upgrade-feature-comparison.md). De nyckelfunktioner som ännu inte är tillgängliga i [!DNL Dynamic Media] är bland annat följande: <br> ・ Visual Configurator (Image Author, Image Render).<br> ・ bildmallar (1:1-mallar).<br> ・ e-kataloger.<br>Om ovanstående funktioner används kan uppgraderingen fortfarande utföras med antagandet att de funktionerna är tillgängliga via [!DNL Dynamic Media Classic]. |
|   | Identifiera resurser | Hitta och färdigställ material och förinställningar som ska användas för uppgradering. |
| **Fas 3: Miljö** | Uppgradera [!DNL Adobe Experience Manager] | Alla instanser av [!DNL Adobe Experience Manager] måste uppdateras till den senaste versionen. |
|   | Konfigurera [!DNL Dynamic Media] | Adobe Consulting eller Partner konfigurerar [!DNL Dynamic Media] med dina autentiseringsuppgifter. |
| **Fas 4: Uppgradera** | Replikera resurser | Under uppgraderingsprocessen replikeras [!DNL Dynamic Media Classic] angivna resurser till Dynamic Media. |
| **Fas 5: Administrativa inställningar** | Konfigurera användare och behörigheter | Skapa användare och tilldela behörigheter. |
|   | Konfigurera videokodningsprofiler | Skapa videokodningsprofiler. |
|   | Konfigurera förinställningar för visningsprogram | Skapa visningsförinställningar. |
|   | Ange bildförinställningar | Konfigurera bildförinställningar. |
| **Fas 6: Validering** | Validering | Verifiera användningsfall, resurser, länkar och API:er. |
