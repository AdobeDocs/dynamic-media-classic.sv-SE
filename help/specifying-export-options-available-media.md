---
title: Ange exportalternativ som är tillgängliga för Media Portal-användare
description: Lär dig hur du anger exportalternativ som är tillgängliga för Media Portal-användare.
uuid: 5258b8a4-0704-43cd-97d1-c9af2e4e298b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 9bfd95da-3714-4e38-98af-331a04c685f5
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: c27df6c2-76f4-441c-bd26-cee98203291e
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# Ange exportalternativ som är tillgängliga för Media Portal-användare {#specifying-export-options-available-to-media-portal-users}

Om administratören ger dem tillstånd kan Media Portal-användare formatera om bilder när de exporterar dem. De kan till exempel ändra storlek, filformat och bildkvalitet. Automatisk omformatering av bilder när de exporteras sparar tid genom att du inte behöver formatera om bilderna separat. Dessutom kan administratörer skapa en förinställning - ett i förväg fastställt urval av bildformatsinställningar. Du kan använda en förinställning när du exporterar bilder för att formatera om dem efter företagets specifikationer.

Följande två begränsningar gäller om du exporterar bildresurser som en användardefinierad konvertering eller om du exporterar överordnad originalbilder:

* Den komprimerade ZIP-exportfilen har en maximal filstorlek på 1 GB för exportjobbet.
* Du kan ha maximalt 500 totala resurser per exportjobb.

Se även [Exportera resurser från Adobe Dynamic Media Classic](exporting-assets-from-dmc.md#exporting-assets-from_dmc).

**Så här anger du exportalternativ som är tillgängliga för användare av Media Portal:**

1. Klicka på **[!UICONTROL Setup]** > **[!UICONTROL Image Presets]** i fältet Global Navigation.
1. Välj något av följande i fönstret Bildförinställningar:

   * **Aktivera användardefinierad konvertering**  - När det här alternativet är markerat kan användare välja andra från den  **[!UICONTROL Size]** nedrullningsbara listan i fönstret Exportera markerade resurser. Användarna kan sedan välja en måttenhet som pixlar eller centimeter och sedan ange önskad bredd och höjd. När de exporterar eller hämtar dessa filer formateras bildfilerna om.

      När du väljer **[!UICONTROL pixels]** i listrutan **[!UICONTROL Size]** får bildens bredd x-höjd inte överstiga 100 miljoner pixlar. Storleken är lika med 10 000 x 10 000 pixlar för en fyrkantig bild, eller ungefär 8 000 x 12 000 pixlar för en bild med 2x3-proportioner. Den här storleksbegränsningen gäller inte om du exporterar överordnad originalbilder.

      Avmarkera det här alternativet om du vill att användare ska hämta filer utan att formatera om dem när de hämtas.

   * **Aktivera Exportera original**  - Gör att du kan exportera överordnad originalbilder. I panelen **[!UICONTROL Export Selected Assets]** kan användarna öppna listrutan **[!UICONTROL Conversion]** och välja **[!UICONTROL Export Original]** för att exportera originalfilerna. Avmarkera det här alternativet om du vill tvinga användarna att välja en bildförinställning eller välja konverteringsalternativ när de exporterar bilder.

>[!MORELIKETHIS]
>
>* [Bildförinställningar](application-setup.md#image_presets)
>* [Välj åtkomstbehörighet för bildförinställning för en grupp](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)

