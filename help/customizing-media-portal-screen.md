---
title: Anpassa skärmen Media Portal
description: Lär dig hur du anpassar mediaportalskärmen.
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
feature: Dynamic Media Classic,Samarbete,Resurshantering
role: Administrator,Business Practitioner
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
translation-type: tm+mt
source-git-commit: 4e79c98b92dfa4e1a9890ed8a291cdf564126466
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Anpassa skärmen Media Portal{#customizing-the-media-portal-screen}

Med formatinställningarna för Media Portal kan du märka upp Media Portal-skärmen med företagets logotyp och färger. Använd formatinställningarna för att lägga företagets varumärke på Media Portal.

Välj **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Style Settings]** för att komma åt formatinställningarna. Kontrollera att du klickar på **[!UICONTROL Save]** för att spara inställningarna när du har gjort dem. Du kan klicka på **[!UICONTROL Restore]** om du vill återställa standardinställningarna. När du gör dina val visas hur alternativen ska se ut på panelen Förhandsvisa.

* **Logotyp** - Klicka  **[!UICONTROL Browse]** och välj en bild i fönstret Välj logotypbild.

* **Program**  - Skapa en övertoningsfärgblandning genom att göra val på menyerna Bakgrundsövertoningsfärger.

* **Träd**  - Välj en överrullningsfärg (den färg som visas när du flyttar pekaren över ett objekt) och en markeringsfärg (den färg som visas när du markerar ett objekt).

* **Dragspelspanel**  - Välj bakgrundsfärger, en kantlinjestil samt överrullning och valda färger för dragspelsbilden som visas på skärmens högra sida i detaljvyn.

* **Dragspelsrubrik**  - Välj om du vill skapa text i dragspelsrubrikens fetstil.

* **Datagrid**  - Välj färger för rubrikraden i datarutnät.

* **Varning**  - Välj en bakgrundsfärg för varningsmeddelanderutor.

* **Förloppsindikator**  - Välj en färg för fältet som anger förloppet för överföringar och hämtningar.

För att Media Portal-användare ska kunna se de formatinställningar som du har valt måste de lägga till `?company=(company name)` till den URL som de kommer åt Media Portal med. Om du till exempel vill se formatinställningar kan du använda Media Portal-användare som har åtkomst till portalföretaget på följande plats:

`https://s7sps1.scene7.com/MediaPortal`

Använd följande URL i stället:

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

Om du tar med företagsnamnet i URL:en kan Media Portal identifiera vilket företag en användare vill få åtkomst till och använda företagets formatinställningar utifrån detta.

Du kan lära dig mer om hur du kommunicerar URL-ändringar med Media Portal-användare och hur du konfigurerar ett välkomstmeddelande så att nya användare får rätt URL för Media Portal.

Se [Konfigurera välkomstmeddelandet för Media Portal-användare](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).
