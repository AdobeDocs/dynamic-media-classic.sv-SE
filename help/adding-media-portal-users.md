---
title: Lägga till och hantera Media Portal-användare
seo-title: Lägga till och hantera Media Portal-användare
description: 'null'
seo-description: Lär dig hur du lägger till och hanterar Media Portal-användare
uuid: 96d4103c-6428-4ce1-b9e4-231599304f27
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 5e933045-ce1a-41b9-ba8b-2151c396b7a2
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Lägga till och hantera Media Portal-användare{#adding-and-managing-media-portal-users}

Som administratör kan du lägga till och hantera användare, bestämma om de ska kunna ändra lösenord, redigera användarinformation och överföra användarlistor. Dessa åtgärder utförs på skärmen Användaradministration. Du öppnar den här skärmen genom att klicka på **Inställningar** > **Programinställningar** > **Administrationsinställningar** > **Användaradministration**.

>[!NOTE]
>
>Innan du lägger till användare måste du konfigurera grupper för att administrera dem. Med Media Portal kan du inte lägga till en användare utan att tilldela användaren till en eller flera grupper. Mer information finns i [Skapa och hantera medieportalgrupper](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## Hantera lösenord för Media Portal {#handling-media-portal-passwords}

Användare, medarbetare och medverkande på Media Portal får ett välkomstmeddelande med ett lösenord när du registrerar dem. Administratörer kan bestämma om Media Portal-användare ska kunna ändra det här lösenordet.

1. Klicka på **Inställningar** > **Medieportalinställningar** > **Allmänna inställningar**.
1. På sidan Allmänna inställningar markerar eller avmarkerar du **Tillåt användare av Media Portal att ändra lösenord**.
1. Klicka på **Spara**.

>[!NOTE]
>
>Media Portal-användare som får ändra lösenord kan göra det genom att klicka på **Inställningar** > **Personliga inställningar** och ändra lösenord på skärmen Personliga inställningar.

## Lägga till en mediaportalanvändare {#adding-a-media-portal-user}

1. Klicka på **Inställningar** > **Programinställningar** > **Administrationsinställningar** > **Användaradministration**.
1. Klicka på **Lägg till** på sidan Användaradministration.
1. I dialogrutan Lägg till användare anger du användarens förnamn, efternamn och e-postadress på panelen Användarinformation och klickar sedan på **Nästa**.
1. På panelen Företag/Roll i listrutan Företag väljer du ett eller flera företag för användaren.
1. Välj en mediaportalsroll i rolllistan och klicka sedan på **Nästa**.

   Se Användarroller [i](media-portal-user-roles.md#media_portal_user_roles)Media Portal.

1. Markera en eller flera grupper på panelen Åtkomstgrupper.

   Se [Skapa och hantera medieportalgrupper](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

1. (Valfritt) Klicka på **E-postinställningar** för att välja e-postinställningar som inte är standardinställningarna.

   Se [Konfigurera välkomstmeddelandet för Media Portal-användare](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).

1. Klicka på **Lägg till användare**.

När du har lagt till en användare skickas ett välkomstmeddelande till användaren via Media Portal. Meddelandet innehåller ett tillfälligt lösenord och mediaportal-URL:en.

## Överföra en användarlista för Media Portal {#uploading-a-media-portal-user-list}

Om du har flera användare att lägga till kan du överföra en användarlista. Användarna läggs automatiskt till i det valda kontot.

Skapa användarlistan som en CSV-fil (kommaavgränsade värden) med användarinformationen. När listan har överförts läggs användarna i listan automatiskt till i kontot med sina angivna grupptilldelningar. Ett välkomstmeddelande skickas till varje ny användare, inklusive en länk till Media Portal och ett tillfälligt lösenord.

### Skapa CSV-filen {#creating-the-csv-file}

Skapa en CSV-fil (filename.csv) som överensstämmer med följande format och fält. Den första raden i filen måste innehålla de kolumnrubriker som anges i denna tabell. Du kan ordna kolumnerna efter behov. Alla kolumner är obligatoriska.

| Kolumnnamn | Beskrivning |
|--- |--- |
| Förnamn | Förnamnet. |
| Efternamn | Efternamnet. |
| E-post | En giltig e-postadress. |
| Lösenord | En skiftlägeskänslig lösenordssträng. |
| Användarroll | MediaPortalAdminMediaPortalUserMediaPortalContributorMediaPortalContributorAnvändare |
| Grupper | Lista över en eller flera kontogruppstilldelningar för varje användare, avgränsade med kommatecken. Du anger gruppen genom att ange kontonamnet som prefix, avgränsat med snedstreck (/). Exempel: PortalCo/IT, där PortalCo är kontot och IT är gruppen i PortalCo-kontot. |

I följande exempeltabell visas hur du utformar en CSV-fil:

| Förnamn | Efternamn | E-post | Lösenord | Användarroll | Grupper |
|--- |--- |--- |--- |--- |--- |
| Peter | Peterson | `petep@company.com` | välkommen | MediaPortalAdmin | PortalCo/IT, PortalCo/Admin |
| Kevin | Märken | `kevinm@myco.com` | välkommen | MediaPortalAnvändare | PortalCo/MktgGroup, PortalCo/test |


### Överför CSV-filen {#uploading-the-csv-file}

1. Öppna skärmen Inställningar för användaradministration.
1. Klicka på **Överför användarlista**.
1. I dialogrutan Välj fil som ska överföras markerar du CSV-filen och klickar sedan på **Öppna**.

Varje användare i listan läggs automatiskt till i de angivna grupperna. Ett välkomstmeddelande skickas till varje.

>[!NOTE]
Om CSV-filen inte har rätt format visas följande felmeddelande: &quot;Ett fel uppstod när den överförda CSV-filen bearbetades. Kontrollera om det finns giltiga data i filinnehållet.&quot; Om CSV-filen innehåller en befintlig IP- eller IPS-användare läggs användaren inte till i användarlistan.

## Generera en valbar lista med Media Portal-användare {#generating-a-selectable-list-of-media-portal-users}

Du kan visa namn och e-postadresser för Media Portal-användare i ett popup-fönster. Den här listan är användbar om du vill klippa ut och klistra in användarnamn och adresser för användning utanför Media Portal.

1. Klicka på **Inställningar** > **Programinställningar** > **Administrationsinställningar** > **Användaradministration**.
1. I listrutan **Efter användarroll** väljer du namnet på en användarroll för mediaportal och klickar på **Uppdatera** för att visa namnen på en klass av Media Portal-användare.
1. Klicka på **Popup-lista** för att öppna popup-fönstret. Du kan kopiera och klistra in den här listan.

## Konfigurera välkomstmeddelandet för användare av Media Portal {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

Du kan skicka ett välkomstmeddelande när du lägger till nya användare, medarbetare och medverkande på Media Portal. Du kan konfigurera det här e-postmeddelandet eller be Dynamic Media Classic att inte skicka det.

1. Välj **Inställningar** > **Programinställningar** > **Administrationsinställningar** > **Användaradministration**.
1. Klicka på **E-postinställningar** på skärmen Inställningar för användaradministration.
1. Ange någon av följande inställningar i dialogrutan E-postinställningar:

   **Skicka e-post** Avmarkera det här alternativet om du inte vill informera nya användare via e-post om att du har registrerat dem.

   **Standardlösenord** Ange ett tillfälligt lösenord för nya användare eller lämna fältet tomt om du vill att Dynamic Media Classic ska generera slumpmässiga lösenord. Användarna uppmanas att ändra lösenord första gången de loggar in.

   **Ersättnings-URL** Ange en annan URL än standardadressen om användarna öppnar Dynamic Media Classic via en annan URL.

## Andra användarhanteringsåtgärder {#other-user-management-tasks}

Med början på skärmen Inställningar för användaradministration kan du även göra följande:

**Filtrera och sortera användarlistan** Filtrera listan med Media Portal-användare för att hitta användare. Se Filtrera och sortera användarlistan.

**Ta bort användare** Ta bort en användare från listan. Se Ta bort en användare.

**Aktivera och inaktivera användare** Gör uppehåll i åtkomsten till mappar för en användare. Se Aktivera och inaktivera användare.

**Redigera användarinformation** Ange uppdaterad information om en användare. Se Redigera användarinformation.

**Skapa användardefinierade fält** Skapa anpassade, användardefinierade metadatafält som hjälper dig att ordna resurser i Scene7 Publishing System. Fälten kan också aktiveras eller inaktiveras vid behov.

Se [Användardefinierade fält](application-setup.md#user_defined_fields).