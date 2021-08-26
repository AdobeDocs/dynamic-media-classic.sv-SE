---
title: Hantera innehållsvariationer
description: Läs om hur du hanterar innehållsvariationer i Adobe Dynamic Media Classic.
uuid: 1e40a526-02f8-41d9-886f-6d094546bc13
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: aa129b0e-fc73-4fc2-a894-4560b3f46c4f
feature: Dynamic Media Classic
role: User
exl-id: 65b8c314-7ec1-417f-8a7b-aa13762072a1
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 0%

---

# Hantera innehållsvariationer{#managing-content-variations}

Använd malluppsättningar för att hantera det sätt på vilket resursvariationer publiceras.

Skapa en malluppsättning för att hantera varianter av en mall. Du kan styra vilken variation som används utan att ändra koden på webbplatsen. Med den här metoden kan innehållshanterare rotera innehåll utan att IT-avdelningen behöver ändra en webbadress i webbkoden.

Universella URL:er används för att visa mallvariationen som visas på sidan, baserat på den ordning som de listas i uppsättningen. Mallen högst upp i malluppsättningslistan publiceras alltid.

Du kan använda valfri URL för bildförinställningar i listan. URL:er för bildförinställningar fungerar som universella URL:er. Det kan finnas mer än en URL för bildförinställning.

1. Gå till **[!UICONTROL Build]** > **[!UICONTROL Template Sets]**.
1. Välj en mall i verktyget och välj sedan **[!UICONTROL Add/Preview]**.
1. Ändra mallegenskaperna och välj **[!UICONTROL Save As]** om du vill skapa en annan version.
1. Skriv ett namn och välj sedan **[!UICONTROL Save]**.

   Både resursen och mallen måste publiceras.

1. Gå till sidan Detalj för att hämta en kopia-URL från avsnittet URL:er.

Du kan flytta en mall i mallordningen (till exempel högst upp i listan) genom att dra den till dess nya plats. Publicera igen för att skicka den nya ordern.

>[!NOTE]
>
>Om det behövs rensar du cacheminnet för att se ändringarna. Ändringen visas bara på webbplatsen när ändringen har gått igenom cachecykeln.
