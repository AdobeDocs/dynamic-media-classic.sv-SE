---
title: Dela resursändringar med kollegor i realtid
seo-title: Dela resursändringar med kollegor i realtid
description: 'null'
seo-description: Lär dig hur du kan dela resursändringar med andra i realtid.
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Dela resursändringar med kollegor i realtid{#sharing-asset-changes-with-peers-in-real-time}

Om flera kopior av Dynamic Media Classic körs på en eller flera datorer i samma företag uppdateras följande åtgärder från alla Dynamic Media Classic-klienter i realtid med alla peer-klienter:

* Redigera en resurs (byggare, bildredigerare osv.)
* Byta namn på en resurs
* Ta bort en resurs
* Flytta en resurs
* Överför en eller flera resurser (både skrivbordsresurser och FTP)
* Skapa, ta bort eller byta namn på en mapp

När en ändring har gjorts i den ursprungliga klienten uppdateras alla peer-klienter som är inloggade på samma företag med ändringen. Ändringar görs i peer-datorer utan meddelanden, såvida inte peer-datorn redigerar en resurs som ändras i någon av bildredigerarna eller byggarna.

När du loggar in uppmanas du att tillåta eller neka peer-uppdateringar. Du kan&quot;komma ihåg&quot; valet så att du bara uppmanas en gång. Ta bort den aktuella platsen från panelen P2P-nätverk i Globala inställningar för att ta bort ditt val.

Om du redigerar en resurs som har ändrats av en peer-dator uppmanas du att importera ändringen till byggaren eller redigeraren. Om du väljer Ja ignoreras alla ändringar som gjorts i resursen och den uppdaterade resursen importeras. Om du väljer Nej ändras resursen inte i byggaren eller redigeraren och eventuella ändringar som du har gjort kvarstår under den sessionen.

När du sparar resursen visas ett meddelande om att det finns en nyare version och du tillfrågas om du vill skriva över resursen med dina ändringar.
