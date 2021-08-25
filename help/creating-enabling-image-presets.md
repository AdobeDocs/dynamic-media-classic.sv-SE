---
title: Skapa och aktivera bildförinställningar
description: Lär dig hur du skapar och aktiverar bildförinställningar i Dynamic Media Classic.
uuid: 62cfc6fa-da91-4c42-a3ed-10956384d633
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 84257b2a-681c-4fe9-a6e5-3633c1d61d8c
feature: Dynamic Media Classic,Samarbete,Bildförinställningar,Resurshantering
role: Admin,User
exl-id: 94c6c388-226b-4172-a6c7-a8dcf9c0f0cf
source-git-commit: 7be3f63bfadeafa71eeb2567f982f579ccb85975
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Skapa och aktivera bildförinställningar{#creating-and-enabling-image-presets}

När användare exporterar bildresurser med Media Portal kan de välja en bildförinställning i dialogrutan Exportera markerade resurser. En bildförinställning är en samling fördefinierade inställningar som ändrar storlek, bildkvalitet, format, upplösning och andra aspekter av en bilds utseende när den exporteras.

Administratörer för Media Portal kan skapa bildförinställningar som styr hur bilder formateras om när de exporteras. Bildförinställningar formaterar om bilderna enligt ditt företags specifikationer när användare exporterar bilder från Dynamic Media Classic. I stället för att bara formatera om bilder exporterar användarna dem till de exakta specifikationerna för en bildförinställning.

Följande begränsningar gäller när du exporterar bildresurser:

* Bredden x höjden måste vara mindre än eller lika med 100 MB per bild. Bilden får t.ex. inte överstiga 10 K x 10 K eller någon bildvariation under, t.ex. 8 K x 12 K.
* Det finns högst 1 GB total filstorlek per exportjobb.
* Du kan ha maximalt 500 totala resurser per exportjobb.

>[!NOTE]
>
>Dessa begränsningar gäller endast export av härledda bildresurser, inte export av överordnad filer.

Mer information om hur du skapar bildförinställningar finns i [Bildförinställningar](application-setup.md#image_presets).

Information om hur du gör det möjligt för användare att välja bildförinställningar när de exporterar filer finns i [Ange exportalternativ som är tillgängliga för Media Portal-användare](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

Om du vill välja vilka bildförinställningar som ska vara tillgängliga för medlemmarna i en grupp går du till [Välja åtkomstbehörigheter för bildförinställningar för en grupp](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).
