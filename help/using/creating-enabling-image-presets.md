---
title: Skapa och aktivera bildförinställningar
description: Lär dig hur du skapar och aktiverar bildförinställningar i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Image Presets,Asset Management
role: Admin,User
exl-id: 94c6c388-226b-4172-a6c7-a8dcf9c0f0cf
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Skapa och aktivera bildförinställningar{#creating-and-enabling-image-presets}

När användare exporterar bildresurser med Media Portal kan de välja en bildförinställning i dialogrutan Exportera markerade Assets. En bildförinställning är en samling fördefinierade inställningar. Dessa inställningar kan ändra storlek, bildkvalitet, format, upplösning och andra aspekter av en bilds utseende när den exporteras.

Administratörer för Media Portal kan skapa bildförinställningar som styr hur bilder formateras om när de exporteras. Bildförinställningar formaterar bilderna enligt ditt företags specifikationer när användare exporterar bilder från Adobe Dynamic Media Classic. I stället för att bara formatera om bilder exporterar användarna dem till de exakta specifikationerna för en bildförinställning.

Följande begränsningar gäller när du exporterar bildresurser:

* Bredden × höjden måste vara mindre än eller lika med 100 MB per bild. Bilden får t.ex. inte överstiga 10 K × 10 K eller någon bildvariation under, t.ex. 8 K × 12 K.
* Det finns högst 1 GB total filstorlek per exportjobb.
* Du kan ha maximalt 500 totala resurser per exportjobb.

>[!NOTE]
>
>Dessa begränsningar gäller endast export av härledda bildresurser, inte export av primära filer.

Mer information om hur du skapar bildförinställningar finns i [Bildförinställningar](application-setup.md#image_presets).

Information om hur du gör det möjligt för användare att välja bildförinställningar när de exporterar filer finns i [Ange exportalternativ som är tillgängliga för Media Portal-användare](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

Om du vill välja vilka bildförinställningar som ska vara tillgängliga för medlemmarna i en grupp går du till [Välja åtkomstbehörigheter för bildförinställningar för en grupp](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).
