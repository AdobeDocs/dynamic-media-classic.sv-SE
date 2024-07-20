---
title: Dela resursändringar med kollegor i realtid
description: Lär dig hur du kan dela resursändringar med andra i realtid i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
topic: Administration, Collaboration
level: Intermediate
source-git-commit: 163eb32112ec6fbefd1dacf48212353ff3053d54
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# Dela resursändringar med kollegor i realtid{#sharing-asset-changes-with-peers-in-real-time}

Anta att du har flera kopior av Adobe Dynamic Media Classic som körs på datorer i samma företag. I sådana fall uppdateras följande åtgärder från alla Dynamic Media Classic-klienter i realtid med alla peer-klienter:

* Redigera en resurs (byggare, bildredigerare osv.)
* Byta namn på en resurs
* Ta bort en resurs
* Flytta en resurs
* Överför en eller flera resurser (både skrivbordsresurser och FTP)
* Skapa, ta bort eller byta namn på en mapp

När en ändring har gjorts i den ursprungliga klienten uppdateras alla peer-klienter som är signerade i samma företag med ändringen. Ändringar görs i peer-datorer utan meddelanden, såvida inte peer-datorn redigerar en resurs som ändras i någon av bildredigerarna eller byggarna.

När du loggade in uppmanades du att tillåta eller neka peer-uppdateringar. Du kan&quot;komma ihåg&quot; valet så att du bara får en fråga en gång. Ta bort den aktuella platsen från panelen P2P-nätverk i Globala inställningar för att ta bort ditt val.

Om du redigerade en resurs som har ändrats av en peer-dator uppmanas du att importera ändringen till byggaren eller redigeraren. Om du väljer **[!UICONTROL Yes]** ignoreras alla ändringar som gjorts i resursen och den uppdaterade resursen importeras. Om du väljer **[!UICONTROL No]** ändras resursen inte i byggaren eller redigeraren och eventuella ändringar som du har gjort sparas i den sessionen.

När du sparade resursen fick du ett meddelande om att det finns en nyare version och tillfrågades om du vill skriva över resursen med dina ändringar.
