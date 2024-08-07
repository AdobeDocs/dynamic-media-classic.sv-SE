---
title: Lägga till och hantera Media Portal-användare
description: Lär dig hur du lägger till och hanterar Media Portal-användare i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 9590c53c-fd38-4bf2-b723-cd7369702364
topic: Administration
level: Intermediate
source-git-commit: bb229047c0c9b3855453ea15dcd1f9754bc65cef
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 0%

---

# Lägga till och hantera Media Portal-användare{#adding-and-managing-media-portal-users}

Som administratör kan du lägga till och hantera användare, bestämma om de ska kunna ändra lösenord, redigera användarinformation och överföra användarlistor. Dessa åtgärder utförs på skärmen Användaradministration. Navigera till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]** för att komma åt den här skärmen.

>[!NOTE]
>
>Innan du lägger till användare måste du konfigurera grupper för att administrera dem. Med Media Portal kan du lägga till en användare genom att tilldela användaren till en eller flera grupper. Mer information finns i [Skapa och hantera medieportalgrupper](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## Administration av lösenord för Media Portal {#handling-media-portal-passwords}

Användare, medarbetare och medverkande på Media Portal får ett välkomstmeddelande med ett lösenord när du registrerar dem. Administratörer kan bestämma om Media Portal-användare ska kunna ändra det här lösenordet.

1. Navigera till **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL General Settings]**.
1. Markera eller avmarkera **[!UICONTROL Allow Media Portal user to change Password]** på sidan Allmänna inställningar.
1. Välj **[!UICONTROL Save]**.

>[!NOTE]
>
>Medieportalanvändare som får ändra lösenord kan göra det genom att välja **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]** och ändra lösenord på skärmen Personliga inställningar.

## Lägg till en mediaportanvändare {#adding-a-media-portal-user}

1. Navigera till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Välj **Lägg till** på sidan Användaradministration.
1. I dialogrutan **[!UICONTROL `Add User`]** anger du användarens förnamn, efternamn och e-postadress på panelen Användarinformation och väljer sedan **[!UICONTROL Next]**.
1. På panelen Företag/Roll i listrutan Företag väljer du ett eller flera företag för användaren.
1. I rolllistan väljer du en mediaportalroll och sedan **[!UICONTROL Next]**.

   Se [Användarroller för mediaportal](media-portal-user-roles.md#media_portal_user_roles).

1. Markera en eller flera grupper på panelen Åtkomstgrupper.

   Se [Skapa och hantera medieportalgrupper](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

1. (Valfritt) Välj **[!UICONTROL Email Settings]** om du vill välja andra e-postinställningar än standardinställningarna.

   Se [Konfigurera välkomstmeddelandet för Media Portal-användare](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).

1. Välj **[!UICONTROL Add User]**.

När du har lagt till en användare skickas ett välkomstmeddelande till användaren via Media Portal. Meddelandet innehåller ett tillfälligt lösenord och mediaportal-URL:en.

## Överför en användarlista för Media Portal {#uploading-a-media-portal-user-list}

Om du har flera användare att lägga till kan du överföra en användarlista. Användarna läggs automatiskt till i det valda kontot.

Skapa användarlistan som en CSV-fil (kommaavgränsade värden) som innehåller användarinformationen. När listan har överförts läggs användarna i listan automatiskt till i kontot med sina angivna grupptilldelningar. Ett välkomstmeddelande skickas till varje ny användare, inklusive en länk till Media Portal och ett tillfälligt lösenord.

### Skapa CSV-filen {#create-the-csv-file}

Skapa en CSV-fil (filename.csv) som överensstämmer med följande format och fält. Den första raden i filen måste innehålla kolumnrubrikerna i tabellen. Du kan ordna kolumnerna efter behov. Alla kolumner är obligatoriska.

| Kolumnnamn | Beskrivning |
|--- |--- |
| Förnamn | Förnamnet. |
| Efternamn | Efternamnet. |
| E-post | En giltig e-postadress. |
| Lösenord | En skiftlägeskänslig lösenordssträng. |
| Användarroll | MediaPortalAdminMediaPortalUserMediaPortalContributorMediaPortalContributorAnvändare |
| Grupper | Lista över en eller flera kontogruppstilldelningar för varje användare, avgränsade med kommatecken. Du anger gruppen genom att ange kontonamnet som prefix, avgränsat med snedstreck (/). Exempel: PortalCo/IT, där PortalCo är kontot och IT är gruppen i PortalCo-kontot. |

I följande exempelkalkylblad visas hur du utformar en CSV-fil:

| Förnamn | Efternamn | E-post | Lösenord | Användarroll | Grupper |
|--- |--- |--- |--- |--- |--- |
| Prairie | Kat | `prairiek@company.com` | välkommen | MediaPortalAdmin | PortalCo/IT, PortalCo/Admin |
| Rick | Brough | `rickb@myco.com` | välkommen | MediaPortalAnvändare | PortalCo/MktgGroup, PortalCo/test |

### Överför CSV-filen {#uploading-the-csv-file}

1. Öppna skärmen Inställningar för användaradministration.
1. Välj **[!UICONTROL Upload User List]**.
1. I dialogrutan Välj fil som ska överföras markerar du CSV-filen och väljer sedan **[!UICONTROL Open]**.

Varje användare i listan läggs automatiskt till i de angivna grupperna. Ett välkomstmeddelande skickas till varje.

>[!NOTE]
>
>Om CSV-filen inte har rätt format visas följande felmeddelande: &quot;Ett fel uppstod när den överförda CSV-filen bearbetades. Kontrollera om det finns giltiga data i filinnehållet.&quot; Om CSV-filen innehåller en befintlig IP- eller IPS-användare läggs användaren inte till i användarlistan.

## Generera en valbar lista med Media Portal-användare {#generating-a-selectable-list-of-media-portal-users}

Du kan visa namn och e-postadresser för Media Portal-användare i ett popup-fönster. Den här listan är användbar om du vill klippa ut och klistra in användarnamn och adresser för användning utanför Media Portal.

1. Navigera till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. I listrutan **[!UICONTROL By User Role]** väljer du namnet på en användarroll för Media Portal och väljer **[!UICONTROL Refresh]** för att visa namnen på en klass av Media Portal-användare.
1. Välj **[!UICONTROL Popup List]**. Kopiera och klistra in listan.

## Konfigurera e-postmeddelandet med välkomstmeddelanden för Media Portal-användare {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

Du kan skicka ett välkomstmeddelande när du lägger till nya användare, medarbetare och medverkande på Media Portal. Du kan konfigurera det här e-postmeddelandet eller be Adobe Dynamic Media Classic att inte skicka det.

1. Navigera till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**.
1. Välj **[!UICONTROL Email Settings]** på skärmen Inställningar för användaradministration.
1. Ange någon av följande inställningar i dialogrutan E-postinställningar:

   * **[!UICONTROL Send Email]**: Avmarkera det här alternativet om du vill informera nya användare via e-post om att du har registrerat dem.

   * **[!UICONTROL Default Password]**: Ange ett tillfälligt lösenord för nya användare eller lämna fältet tomt om du vill att Adobe Dynamic Media Classic ska generera slumpmässiga lösenord. Användarna uppmanas att ändra lösenord första gången de loggar in.

   * **[!UICONTROL Replacement URL]**: Ange en annan URL än standardadressen om dina användare öppnar Adobe Dynamic Media Classic via en annan URL.

## Andra användarhanteringsåtgärder {#other-user-management-tasks}

Med början på skärmen Inställningar för användaradministration kan du även göra följande:

* **[!UICONTROL Filter and sort the user list]**: Filtrera listan med Media Portal-användare för att hitta användare.

* **[!UICONTROL Delete users]**: Ta bort en användare från listan.

* **[!UICONTROL Activate and deactivate users]**: Gör så att en användare inte kan komma åt mappar.

* **[!UICONTROL Edit user information]**: Ange aktuell information om en användare.

* **[!UICONTROL Create user-defined fields]**: Skapa anpassade, användardefinierade metadatafält så att de kan hjälpa dig att ordna resurser i Adobe Dynamic Media Classic. Fälten kan också aktiveras eller inaktiveras vid behov.

Se [Användardefinierade fält](application-setup.md#user_defined_fields).
