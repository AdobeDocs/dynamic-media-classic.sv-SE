---
title: Anpassa skärmen Media Portal
description: Lär dig hur du anpassar Media Portal-skärmen i Adobe Dynamic Media Classic.
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
topic: Collaboration, Content Management
level: Intermediate
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Anpassa skärmen Media Portal{#customizing-the-media-portal-screen}

Med formatinställningarna för Media Portal kan du märka upp Media Portal-skärmen med företagets logotyp och färger. Använd formatinställningarna för att lägga företagets varumärke på Media Portal.

Gå till **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Style Settings]**. Se till att du väljer **[!UICONTROL Save]** om du vill spara inställningarna när du har gjort dem. Du kan välja **[!UICONTROL Restore]** för att återställa standardinställningarna. När du gör dina val visas hur de visas på panelen Förhandsvisa.

* **[!UICONTROL Logo]** - Välj **[!UICONTROL Browse]** och välj sedan en bild i fönstret Välj logotypbild.

* **[!UICONTROL Application]** - Skapa en övertoningsfärgblandning genom att göra val på menyerna Bakgrundsövertoningsfärger.

* **[!UICONTROL Tree]** - Välj en överrullningsfärg (den färg som visas när du flyttar pekaren över ett objekt) och en markeringsfärg (den färg som visas när du markerar ett objekt).

* **[!UICONTROL Accordion]** - Välj bakgrundsfärger, kantlinjeformat, överrullning och valda färger för dragspelet som visas på skärmens högra sida i detaljvyn.

* **[!UICONTROL Accordion Header]** - Välj om du vill skapa text i dragspelsrubrikens fetstil.

* **[!UICONTROL Datagrid]** - Välj färger för rubrikraden i datarutnätet.

* **[!UICONTROL Alert]** - Välj en bakgrundsfärg för varningsmeddelanderutor.

* **[!UICONTROL Progress Bar]** - Välj en färg för fältet som anger förloppet för överföringar och nedladdningar.

För att Media Portal-användare ska kunna se de formatinställningar som du har valt måste de lägga till `?company=(company name)` till den URL som de använder för att komma åt Media Portal. Om du till exempel vill se formatinställningar kan du använda Media Portal-användare som har åtkomst till portalföretaget på följande plats:

`https://s7sps1.scene7.com/MediaPortal`

Använd följande URL i stället:

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

Om du tar med företagsnamnet i URL:en kan Media Portal identifiera vilket företag en användare vill få åtkomst till och använda företagets formatinställningar utifrån detta.

Du kan lära dig mer om hur du kommunicerar URL-ändringar med Media Portal-användare och hur du konfigurerar ett välkomstmeddelande så att nya användare får rätt URL för Media Portal.

Se [Konfigurera e-postmeddelandet med välkomstmeddelanden för Media Portal-användare](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).
