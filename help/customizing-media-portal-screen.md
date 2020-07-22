---
title: Anpassa skärmen Media Portal
seo-title: Anpassa skärmen Media Portal
description: 'null'
seo-description: Lär dig hur du anpassar mediaportalskärmen.
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---


# Anpassa skärmen Media Portal{#customizing-the-media-portal-screen}

Med formatinställningarna för Media Portal kan du märka upp Media Portal-skärmen med företagets logotyp och färger. Använd formatinställningarna för att lägga din företagsstämpel på Media Portal.

Du öppnar formatinställningarna genom att välja **Inställningar** > **Medieportalinställningar** > **Formatinställningar**. Spara inställningarna genom att klicka på **Spara** . Du kan klicka på **Återställ** om du vill återställa standardinställningarna. När du gör dina val visas hur alternativen ska se ut på panelen Förhandsvisa.

**Logotyp** Klicka på Bläddra och välj en bild i fönstret Välj logotypbild.

**Program** Skapa en övertoningsfärgblandning genom att göra val på menyerna Bakgrundsövertoningsfärger.

**Tree** Välj en överrullningsfärg (den färg som visas när du flyttar pekaren över ett objekt) och en markeringsfärg (den färg som visas när du markerar ett objekt).

**Dragspel** Välj bakgrundsfärger, en kantlinjestil och överrullning samt valda färger för dragspelsbilden som visas på skärmens högra sida i detaljvyn.

**Dragspelsrubrik** Välj om du vill skapa text i dragspelsrubrikens fetstil.

**Datagrid** Välj färger för rubrikraden i datarutnät.

**Varning** Välj en bakgrundsfärg för varningsmeddelanderutor.

**Förloppsindikator** Välj en färg för fältet som anger förloppet för överföringar och hämtningar.

För att Media Portal-användare ska kunna se de formatinställningar som du väljer måste de lägga `?company=(company name)` till den URL som de använder till sin Media Portal. Om du till exempel vill se formatinställningar kan du använda Media Portal-användare som har åtkomst till portalföretaget på följande plats:

`https://s7sps1.scene7.com/MediaPortal`

använder i stället följande URL:

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

Om du tar med företagsnamnet i URL:en kan Media Portal identifiera vilket företag en användare vill få åtkomst till och använda företagets formatinställningar utifrån detta.

Du kan lära dig mer om hur du kommunicerar URL-ändringar med Media Portal-användare och hur du konfigurerar ett välkomstmeddelande så att nya användare får rätt URL för Media Portal.

Se [Konfigurera välkomstmeddelandet för Media Portal-användare](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).
