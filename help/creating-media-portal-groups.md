---
title: Skapa och hantera medieportalgrupper
description: Lär dig hur du skapar och hanterar medieportalgrupper.
uuid: 23f360e1-ddcb-491b-ab9f-428f3ac9c316
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 91524d36-b77a-4dc4-acba-a7bd85297e98
feature: Dynamic Media Classic,Samarbete,Resurshantering
role: Admin,User
exl-id: 0deb7133-b895-4c3f-8e5e-8604a6f2d16b
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 1%

---

# Skapa och hantera medieportalgrupper{#creating-and-managing-media-portal-groups}

** Grupper är utformade för att hjälpa dig att administrera Media Portal-användare. För att få åtkomst till en resurs måste användaren vara medlem i minst en grupp som har behörighet att få åtkomst till resursen. När du lägger till en användare tilldelar du användaren till en eller flera grupper. Då ger du användaren åtkomst till mappar som gruppen har tilldelats. Du kan också välja vilka bildförinställningar som är tillgängliga för en grupp.

## Använda grupper för att begränsa åtkomst till mappar, resurser och bildförinställningar {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

Om du vill ge åtkomstbehörighet på olika nivåer skapar du grupper. För varje grupp tilldelar du läs-, skriv- och borttagningsbehörigheter till olika mappar och resurser i mappar. Du bestämmer också vilka bildförinställningar som är tillgängliga för gruppen. Sedan tilldelar du användare till grupper. En användare kan vara medlem i mer än en grupp. Gruppkonceptet ger dig flexibilitet att tilldela åtkomst till begränsade uppsättningar av det totala innehållet.

Om du inte ger en gruppbehörighet till en resurs eller mapp ärver resursen eller mappen de behörigheter som du tilldelade den överordnade mappen (mappen ovanför den i mapphierarkin). Bevilja behörigheter till en överordnad mapp om du vill se till att alla dess underordnade mappar ärver samma behörigheter.

>[!NOTE]
>
>Användare kan tillhöra mer än en grupp. När en användare tillhör två grupper med olika åtkomstbehörigheter till en mapp får användaren den högsta åtkomstnivån.

## Lägga till en grupp {#adding-a-group}

1. Klicka på **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Groups]**.
1. Klicka på **[!UICONTROL Add]**.
1. Ange ett namn för gruppen i rutan Gruppnamn i dialogrutan Lägg till grupp och klicka sedan på **[!UICONTROL Add Group]**.
1. Om du vill kan du markera rutorna bredvid namnen på användarna som ska läggas till i den nya gruppen.
1. Om du vill ange åtkomstbehörigheter nu klickar du på fliken **[!UICONTROL Asset Access Permissions]** och anger sedan önskade alternativ.

   Se [Upprätta åtkomstbehörigheter för en grupp](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group).

1. Om du vill välja vilka bildförinställningar som är tillgängliga för gruppen klickar du på fliken **[!UICONTROL Image Preset Access Permissions]** och väljer Bildförinställningar som gruppen kan använda.

   Se [Välj åtkomstbehörighet för bildförinställningar för en grupp](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).

1. Klicka på **[!UICONTROL Close]**.

## Skapa åtkomstbehörigheter för en grupp {#establishing-asset-access-permissions-for-a-group}

1. Klicka på **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Groups]**.
1. Gör något av följande på sidan med grupplistan:

   * Om du vill lägga till en grupp och ange behörigheter klickar du på **[!UICONTROL Add]**. I dialogrutan Lägg till grupp anger du ett namn för gruppen, klickar på **[!UICONTROL Add Group]** och lägger till användare i gruppen.
   * Om du vill redigera en grupps behörigheter markerar du gruppen och klickar sedan på **[!UICONTROL Edit]**.

1. Klicka på fliken **[!UICONTROL Asset Access Permissions]** i dialogrutan Lägg till grupp eller Redigera grupp. Till höger på fliken finns rutor för att ange läs-, skriv- och borttagningsbehörigheter för mappar och resurser. Du kan expandera och komprimera mappar och undermappar i den vänstra rutan.
1. Om du vill tilldela rättigheter till mappar eller enskilda resurser markerar du mappen i den vänstra rutan. Mappinnehållet visas i den högra rutan. Tilldela sedan rättigheter för gruppen genom att markera rutorna för motsvarande filer eller mappar i den högra rutan.

   Den här tabellen mappar olika uppgifter till att läsa, skriva och ta bort behörigheter.

   | Uppgift | Läs | Skriv | Ta bort |
   |--- |--- |--- |--- |
   | Bläddra bland mappar och filer | X |  |  |
   | Redigera filer (beskära, öka skärpan, justera) |  | X |  |
   | Ändra filnamn |  | X |  |
   | Flytta filer till olika mappar |  | X |  |
   | Byt namn på filer |  | X |  |
   | Ta bort filer |  |  | X |

1. Klicka på **[!UICONTROL Close]**.

>[!NOTE]
>
>Åtkomsträttigheter fastställs när du markerar en ruta. När du tilldelar rättigheter till en mapp får dess undermappar och alla filer i den samma rättigheter som den överordnade mappen. Du kan dock ange olika behörigheter för enskilda undermappar och resursfiler.

## Välja åtkomstbehörighet för bildförinställning för en grupp {#choosing-image-preset-access-permissions-for-a-group}

Välj åtkomstbehörighet för bildförinställningar för en grupp om du vill ange vilka bildförinställningar som är tillgängliga för gruppmedlemmar när de exporterar resurser med Media Portal.

Se även [Ange vilka exportalternativ som är tillgängliga för Media Portal-användare](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

1. Klicka på **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Groups]**.
1. Gör något av följande på sidan med grupplistan:

   * Om du vill lägga till en grupp och ange vilka bildförinställningar som är tillgängliga för gruppen klickar du på **[!UICONTROL Add]**. I dialogrutan Lägg till grupp anger du ett namn för gruppen, klickar på **[!UICONTROL Add Group]** och lägger till användare i gruppen.
   * Om du vill redigera bildförinställningsalternativen för en grupp markerar du gruppen och klickar sedan på **[!UICONTROL Edit]**.

1. Klicka på fliken **[!UICONTROL Image Preset Access Permissions]** i dialogrutan Lägg till grupp eller Redigera grupp.
1. Om du vill ange vilka förinställningar som är tillgängliga för Media Portal-användare när de exporterar resurser markerar eller avmarkerar du Bildförinställningar.
1. Klicka på **[!UICONTROL Close]**.

## Redigera och ta bort grupper {#edit-and-delete-groups}

1. Klicka på **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Groups]**.
1. Markera en grupp på sidan Grupplista och redigera eller ta bort den.

   **Redigera en grupp** - Klicka  **[!UICONTROL Edit]** och välj sedan alternativ i dialogrutan Redigera grupp.

   **Ta bort en grupp** - klicka  **[!UICONTROL Delete]**.
