---
title: Anpassa skärmen Media Portal
description: Lär dig hur du anpassar Media Portal-skärmen i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
topic: Collaboration, Content Management
level: Intermediate
source-git-commit: 00591bdbe721035e25d3dea245a2110f978d19aa
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Anpassa skärmen Media Portal{#customizing-the-media-portal-screen}

Med Media Portal-stilinställningarna kan du märka upp Media Portal-skärmen med företagets logotyp och färger. Använd formatinställningarna för att lägga företagets varumärke på Media Portal.

Gå till **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Style Settings]** om du vill komma åt formatinställningarna. Se till att du väljer **[!UICONTROL Save]** för att spara inställningarna när du har gjort dem. Du kan välja **[!UICONTROL Restore]** om du vill återställa standardinställningarna. När du gör dina val visas hur de visas på panelen Förhandsvisa.

* **[!UICONTROL Logo]**: Välj **[!UICONTROL Browse]** och välj sedan en bild i fönstret Välj logotypbild.

* **[!UICONTROL Application]**: Skapa en övertoningsfärgblandning genom att göra val på menyerna för bakgrundsövertoningsfärger.

* **[!UICONTROL Tree]**: Välj en överrullningsfärg och markeringsfärg.

* **[!UICONTROL Accordion]**: Välj bakgrundsfärger, en kantlinjestil och överrullning samt valda färger för dragspelet som visas på skärmens högra sida i detaljvyn.

* **[!UICONTROL Accordion Header]**: Välj om du vill skapa text i dragspelsrubrikens fetstil.

* **[!UICONTROL Datagrid]**: Välj färger för rubrikraden i datarutnätet.

* **[!UICONTROL Alert]**: Välj en bakgrundsfärg för varningsmeddelanderutor.

* **[!UICONTROL Progress Bar]**: Välj en färg för fältet som anger förloppet för överföringar och hämtningar.

För att Media Portal-användare ska kunna se de formatinställningar som du har valt måste de lägga till `?company=(company name)` till den URL som de använder till Media Portal. Om du till exempel vill se formatinställningar kan du använda Media Portal-användare som har åtkomst till PortalCo-företaget på följande plats:

`https://s7sps1.scene7.com/MediaPortal`

Använd följande URL i stället:

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

Om du tar med företagsnamnet i URL:en kan Media Portal identifiera vilket företag en användare vill få åtkomst till och använda företagets formatinställningar utifrån detta.

Du kan lära dig mer om hur du kommunicerar URL-ändringar med Media Portal-användare och hur du konfigurerar ett välkomstmeddelande så att nya användare får rätt URL för Media Portal.

Se [Konfigurera välkomstmeddelandet för Media Portal-användare](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).
