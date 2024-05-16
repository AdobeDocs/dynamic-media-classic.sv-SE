---
title: Beredskap för uppgradering
description: En checklista för beredskap för uppgradering när du vill gå vidare från [!DNL Adobe Dynamic Media Classic] till [!DNL Dynamic Media] på [!DNL Adobe Experience Manager].
feature: Dynamic Media Classic
role: Admin,User
exl-id: 86537998-b7e9-449c-83eb-6fd04533a00f
topic: Administration, Migration
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# Checklista för beredskap för uppgradering

Använd följande checklista för att förstå och förbereda en uppgradering från [!DNL Dynamic Media Classic] till [!DNL Dynamic Media].

|  | Uppgift | Beskrivning |
| :--- | :--- | --- |
| **Fas 1: Licensiering** | Kör kontrakt | Adobe-kontoteamet arbetar tillsammans med er utifrån trafik och lagring för att gå över från [!DNL Dynamic Media Classic] licens att förnya på [!DNL Dynamic Media] licens. |
| **Fas 2: Förberedelse** | Validera funktionsanvändning | Bekräfta funktionerna som används i [!DNL Dynamic Media Classic] är tillgängliga i [!DNL Dynamic Media]. Se [Funktionsjämförelse](/help/using/upgrade-feature-comparison.md) sida. Viktiga funktioner som ännu inte är tillgängliga i [!DNL Dynamic Media] inkludera följande:<br>・ Visual Configurator (Image Author, Image Render).<br>・ Bildmallar (1:1-mallar).<br>・ eCatalogs.<br>Om funktionerna ovan används kan uppgraderingen fortfarande utföras under förutsättning att de funktionerna är tillgängliga via [!DNL Dynamic Media Classic]. |
|   | Identifiera resurser | Hitta och färdigställ material och förinställningar som ska användas för uppgradering. |
| **Fas 3: Miljö** | Uppgradera [!DNL Adobe Experience Manager] | Alla förekomster av [!DNL Adobe Experience Manager] måste uppdateras till den senaste versionen. |
|   | Inställningar [!DNL Dynamic Media] | Konsult- eller partnerkonfigurationer för Adobe [!DNL Dynamic Media] med dina uppgifter. |
| **Fas 4: Uppgradera** | Replikera resurser | Under uppgraderingsprocessen kan du [!DNL Dynamic Media Classic] resurser replikeras till Dynamic Media. |
| **Fas 5: Administrativ installation** | Konfigurera användare och behörigheter | Skapa användare och tilldela behörigheter. |
|   | Konfigurera videokodningsprofiler | Skapa videokodningsprofiler. |
|   | Konfigurera förinställningar för visningsprogram | Skapa förinställningar för visningsprogram. |
|   | Ange bildförinställningar | Konfigurera bildförinställningar. |
| **Fas 6: Validering** | Validering | Verifiera användningsfall, resurser, länkar och API:er. |
