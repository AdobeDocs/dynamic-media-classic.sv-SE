---
title: 'Snabbstart: Medieportal'
description: En introduktion och en snabbstart till Media Portal som hjälper dig att komma igång snabbt med Media Portal-teknik och -administration i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: bff613c8-a93b-4cca-94db-8cad1cc36296
topic: Collaboration, Content Management
level: Beginner
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# Snabbstart: Medieportal{#quick-start-media-portal}

Med Media Portal kan man enkelt skaffa, kontrollera och distribuera godkända mediefiler till externa partners och kanaler samt interna användare i ett företag. Den webbläsarbaserade, självbetjäningsmiljön ger Media Portal-användare administratörskontrollerad&quot;vy&quot; av Adobe Dynamic Media Classic-material så att de enkelt kan komma åt, söka, förhandsgranska och exportera mediefiler i företagsgodkända format.

Som administratör kan du styra hur användare visar, får åtkomst till och använder resurser i Media Portal. Dessutom kan du anpassa Media Portal-gränssnittet så att det passar webbplatsen och varumärket. Du kan ange teckensnitt, teckenfärg, teckenstorlek och inkludera märkeselement som logotyper i Media Portal-gränssnittet.

Se följande utbildningsvideor:

* [Översikt över medieportalen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/544_mp_overview1_converted%20renamed_Done-AVS)

* [Demo av mediaportal ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/545_mp_tour1_user_converted%20renamed_Done-AVS)

* [Demo av mediaportal 2](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/546_mp_tour2_admin_converted%20renamed_Done-AVS)

Följande snabbstart är utformad för att du snabbt ska komma igång med Media Portal-administration. I slutet av varje steg väljer du ämneslänken om du vill veta mer.

## 1. Förstå användarroller i Media Portal

Media Portal-användare har tre roller: användare, medarbetare och medarbetare. Varje roll kan utföra olika uppgifter. En medarbetare kan till exempel byta namn på och ta bort filer och mappar, men en användare kan inte göra det. Förstå de olika rollerna så att du förstår vilka ansvarsområden du ger dem när du lägger till användare.

Se [Användarroller för mediaportal](media-portal-user-roles.md#media_portal_user_roles).

## 2. Skapa grupper för att hantera användare

Grupper avgör vilka mappar och filer en användare har åtkomst till, vad användare kan göra i de mapparna och filerna och vilka bildförinställningar som är tillgängliga. Som administratör är din första uppgift att skapa grupper. För varje grupp bestämmer du vilka mappar, filer och medlemmar i gruppen Bildförinställningar som ska ha åtkomst. Bevilja även läs-, skriv- och borttagningsbehörigheter till gruppmedlemmarna. Dessa behörigheter avgör om medlemmar kan bläddra bland, redigera, byta namn på och ta bort mappar och filer som de har åtkomst till.

Se [Skapa och hantera medieportalgrupper](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## 3. Lägg till användare

När du lägger till en användare tilldelar du användaren en roll (användare, medarbetare eller användarmedarbetare). Du kan också tilldela användaren till en eller flera grupper. Om du vill lägga till användare snabbare kan du överföra en användarlista i form av en CSV-fil. Nya användare får ett välkomstmeddelande och instruktioner om hur de loggar in på Media Portal.

Se [Lägga till och hantera Media Portal-användare](adding-media-portal-users.md#adding_and_managing_media_portal_users).

## 4. Hantera FTP-konton

Du kan ha separata FTP-konton som är kopplade till Media Portal. De kan mappas till en viss mapp på ditt Adobe Dynamic Media Classic-konto. Den här typen av funktionalitet innebär att du kan tillåta användare att överföra digitala resurser till ditt konto med hjälp av separata FTP-konton.

Se [Hantera FTP-konton](ftp-accounts.md#managing_ftp_accounts).

>[!NOTE]
>
>Endast Media Portal-administratörer kan administrera dessa FTP-konton. Dessutom kan bara användare med rollen Medieportaldeltagare-Användare eller Medieportaldeltagare överföra filer.

Se [Användarroller för mediaportal](media-portal-user-roles.md#media_portal_user_roles).

## 5. Ange exportalternativ

Medieportalanvändare kan, när de exporterar filer, formatera om filerna och exportera ursprungliga primära filer - om du ger dem behörighet att göra det. Som administratör bestämmer du hur användare ska exportera filer.

Se [Ange tillgängliga exportalternativ för Media Portal-användare](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

## 6. Skapa bildförinställningar

En bildförinställning är en samling fördefinierade inställningar. Dessa inställningar kan ändra storlek, bildkvalitet, format, upplösning och andra aspekter av en bilds utseende när den exporteras. Du kan skapa bildförinställningar för att styra hur bilder formateras om när användare exporterar dem.

Se [Skapa och aktivera bildförinställningar](creating-enabling-image-presets.md#creating_and_enabling_image_presets).

## 7. Skapa metadataförinställningar och användardefinierade metadatafält

Metadata beskriver och identifierar en fil. Det används för att söka efter och ordna resurser. Du kan skapa metadataförinställningar för att vara säker på att du anger metadata korrekt och att alla metadatafält som kräver data fylls i. En metadataförinställning är en fördefinierad uppsättning metadataposter. Du kan också skapa metadatafält som unikt beskriver de filer du arbetar med.

Se [Använda metadata mer effektivt](making-efficient-metadata.md#making_more_efficient_use_of_metadata).

## 8. Anpassa sidan Media Portal

Med Media Portal-formatinställningar kan du märka upp Media Portal-sidan med företagets logotyp och färger. Använd formatinställningarna för att lägga företagets varumärke på Media Portal.

Se [Anpassa sidan Media Portal](customizing-media-portal-screen.md#customizing_the_media_portal_screen).
