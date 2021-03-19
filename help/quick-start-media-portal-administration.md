---
title: '"Snabbstart: Media Portal"'
description: En introduktion och en snabbstart till Media Portal som hjälper dig att komma igång snabbt med Media Portal-teknik och -administration.
uuid: 0dbd6146-b392-4e03-955b-0b323b654b9f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 1385a092-0b2c-4e05-ad1e-ce3685022300
feature: Dynamic Media Classic,Samarbete,Resurshantering
role: Administratör,Affärsledare
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 1%

---


# Snabbstart: Medieportal{#quick-start-media-portal}

Med Media Portal kan man enkelt skaffa, styra upp och distribuera godkänt material till externa partners och kanaler samt interna affärsanvändare. Den webbläsarbaserade, självbetjäningsmiljön ger Media Portal-användare administratörskontrollerad&quot;vy&quot; i Dynamic Media Classic-material så att de enkelt kan komma åt, söka, förhandsgranska och exportera mediefiler i företagsgodkända format.

Som administratör kan du styra hur användare visar, får åtkomst till och använder resurser i Media Portal. Dessutom kan ni anpassa Media Portal-gränssnittet så att det passar er webbplats och ert varumärke. Du kan ange teckensnitt, teckenfärg och teckensnittsstorlek samt inkludera märkeselement som logotyper i Media Portal-gränssnittet.

**Snabbstart**

Den här snabbstarten är utformad för att du snabbt ska komma igång med Media Portal-administration. I slutet av varje steg finns en korsreferens till ett ämne där du kan få mer information.

**1. Förstå användarroller i mediaportal**

Media Portal-användare har tre roller - användare, medarbetare och medarbetare. Varje roll kan utföra olika uppgifter. En medarbetare kan till exempel byta namn på och ta bort filer och mappar, men en användare kan inte göra det. Förstå de olika rollerna så att du förstår vilka ansvarsområden du ger dem när du lägger till användare.

Se [Användarroller för mediaportal](media-portal-user-roles.md#media_portal_user_roles).

**2. Skapa grupper för att hantera användare**

Grupper avgör vilka mappar och filer en användare har åtkomst till, vad användare kan göra i dessa mappar och filer och vilka bildförinställningar som är tillgängliga. Som administratör är din första uppgift att skapa grupper. För varje grupp bestämmer du vilka mappar, filer och medlemmar i gruppen Bildförinställningar som ska ha åtkomst. Bevilja även läs-, skriv- och borttagningsbehörigheter till gruppmedlemmarna. Dessa behörigheter avgör om medlemmar kan bläddra bland, redigera, byta namn på och ta bort mappar och filer som de har åtkomst till.

Se [Skapa och hantera medieportalgrupper](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

**3. Lägg till användare**

När du lägger till en användare tilldelar du användaren en roll (användare, medarbetare eller användarmedarbetare). Du kan även tilldela användaren till en eller flera grupper. Om du vill lägga till användare snabbare kan du överföra en användarlista i form av en CSV-fil. Nya användare får ett välkomstmeddelande och instruktioner om hur de loggar in på Media Portal.

Se [Lägga till och hantera Media Portal-användare](adding-media-portal-users.md#adding_and_managing_media_portal_users).

**4. Hantera FTP-konton**

Du kan ha separata FTP-konton som är kopplade till Media Portal och som är mappade till en viss mapp i ditt Dynamic Media Classic-konto. Den här typen av funktionalitet innebär att du kan tillåta användare att överföra digitala resurser till ditt konto med hjälp av separata FTP-konton.

Se [Hantera FTP-konton](ftp-accounts.md#managing_ftp_accounts).

>[!NOTE]
>
>Endast Media Portal-administratörer kan administrera dessa FTP-konton. Dessutom kan bara användare med rollen Medieportaldeltagare-Användare eller Medieportaldeltagare överföra filer.

Se [Användarroller för mediaportal](media-portal-user-roles.md#media_portal_user_roles).

**5. Ange exportalternativ**

Medieportalanvändare kan, när de exporterar filer, formatera om filerna och exportera överordnad originalfiler - om du ger dem tillstånd att göra det. Som administratör bestämmer du hur användare ska exportera filer.

Se [Ange vilka exportalternativ som är tillgängliga för Media Portal-användare](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

**6. Skapa bildförinställningar**

En bildförinställning är en samling fördefinierade inställningar som ändrar storlek, bildkvalitet, format, upplösning och andra aspekter av en bilds utseende när den exporteras. Du kan skapa bildförinställningar för att styra hur bilder formateras om när användare exporterar dem.

Se [Skapa och aktivera bildförinställningar](creating-enabling-image-presets.md#creating_and_enabling_image_presets).

**7. Skapa metadataförinställningar och användardefinierade metadatafält**

Metadata beskriver och identifierar en fil. används för att söka efter och ordna resurser. Du kan skapa metadataförinställningar för att vara säker på att metadata anges korrekt och att metadatafält som kräver data fylls i. En metadataförinställning är en fördefinierad uppsättning metadataposter. Du kan också skapa metadatafält som unikt beskriver de filer du arbetar med.

Se [Använda metadata på ett effektivare sätt](making-efficient-metadata.md#making_more_efficient_use_of_metadata).

**8. Anpassa skärmen Media Portal**

Med Media Portal-stilinställningarna kan du märka upp Media Portal-skärmen med företagets logotyp och färger. Använd formatinställningarna för att lägga din företagsstämpel på Media Portal.

Se [Anpassa skärmen Media Portal](customizing-media-portal-screen.md#customizing_the_media_portal_screen).
