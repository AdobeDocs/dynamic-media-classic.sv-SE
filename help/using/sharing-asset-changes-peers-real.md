---
title: Dela resursändringar med kollegor i realtid
description: Lär dig hur du kan dela resursändringar med andra i realtid i Adobe Dynamic Media Classic.
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
topic: Administration, Collaboration
level: Intermediate
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Dela resursändringar med kollegor i realtid{#sharing-asset-changes-with-peers-in-real-time}

Om flera kopior av Adobe Dynamic Media Classic körs på flera datorer i samma företag uppdateras följande åtgärder från alla Adobe Dynamic Media Classic-klienter i realtid med alla peer-klienter:

* Redigera en resurs (byggare, bildredigerare o.s.v.)
* Byta namn på en resurs
* Ta bort en resurs
* Flytta en resurs
* Överför en eller flera resurser (både skrivbordsresurser och FTP)
* Skapa, ta bort eller byta namn på en mapp

När en ändring har gjorts i den ursprungliga klienten uppdateras alla peer-klienter som är signerade i samma företag med ändringen. Ändringar görs i peer-datorer utan meddelanden, såvida inte peer-datorn redigerar en resurs som ändras i någon av bildredigerarna eller byggarna.

När du loggar in uppmanas du att tillåta eller neka peer-uppdateringar. Du kan&quot;komma ihåg&quot; valet så att du bara uppmanas en gång. Ta bort den aktuella platsen från panelen P2P-nätverk i Globala inställningar för att ta bort ditt val.

Om du redigerar en resurs som har ändrats av en peer-dator uppmanas du att importera ändringen till byggaren eller redigeraren. Om du väljer **[!UICONTROL Yes]**, tar byggaren eller redigeraren bort ändringar som gjorts i resursen och importerar den uppdaterade resursen. Om du väljer **[!UICONTROL No]**, är resursen oförändrad i byggaren eller redigeraren och alla ändringar som du har gjort kvarstår under den sessionen.

När du sparar resursen visas ett meddelande om att det finns en nyare version och du tillfrågas om du vill skriva över resursen med dina ändringar.
