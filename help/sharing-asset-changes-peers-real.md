---
title: Dela resursändringar med kollegor i realtid
description: Lär dig hur du kan dela resursändringar med andra i realtid.
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be
feature: Dynamic Media Classic,Resurshantering,Samarbete
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Dela resursändringar med kollegor i realtid{#sharing-asset-changes-with-peers-in-real-time}

Om flera kopior av Dynamic Media Classic körs på en eller flera datorer i samma företag uppdateras följande åtgärder från alla Dynamic Media Classic-klienter i realtid med alla peer-klienter:

* Redigera en resurs (byggare, bildredigerare o.s.v.)
* Byta namn på en resurs
* Ta bort en resurs
* Flytta en resurs
* Överför en eller flera resurser (både skrivbordsresurser och FTP)
* Skapa, ta bort eller byta namn på en mapp

När en ändring har gjorts i den ursprungliga klienten uppdateras alla peer-klienter som är signerade i samma företag med ändringen. Ändringar görs i peer-datorer utan meddelanden, såvida inte peer-datorn redigerar en resurs som ändras i någon av bildredigerarna eller byggarna.

När du loggar in uppmanas du att tillåta eller neka peer-uppdateringar. Du kan&quot;komma ihåg&quot; valet så att du bara uppmanas en gång. Ta bort den aktuella platsen från panelen P2P-nätverk i Globala inställningar för att ta bort ditt val.

Om du redigerar en resurs som har ändrats av en peer-dator uppmanas du att importera ändringen till byggaren eller redigeraren. Om du väljer **[!UICONTROL Yes]** ignoreras alla ändringar som gjorts i resursen och den uppdaterade resursen importeras. Om du väljer **[!UICONTROL No]** ändras inte resursen i byggaren eller redigeraren och alla ändringar du har gjort sparas i den sessionen.

När du sparar resursen visas ett meddelande om att det finns en nyare version och du tillfrågas om du vill skriva över resursen med dina ändringar.
