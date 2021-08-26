---
title: Integrera Adobe Dynamic Media Classic med Adobe Target Standard/Premium
description: Lär dig hur du integrerar Adobe Dynamic Media Classic med Adobe Target Standard/Premium.
uuid: d1c07a52-b058-4ae3-a31d-44c43dc27f65
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 3b4add18-4191-475e-a3a3-0184367a25fc
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# Integrera Adobe Dynamic Media Classic med Adobe Target Standard/Premium {#integrating-dmc-with-target}

Innan du kan integrera [!DNL Adobe Dynamic Media Classic] med [!DNL Target Standard/Premium] måste du ange mål-URL:en på skärmen för allmänna inställningar för [!DNL Adobe Dynamic Media Classic]-program. Så här hämtar du mål-URL:en och anger den på sidan Allmänna inställningar för programmet:

1. Logga in på ditt [!DNL Target Standard/Premium]-konto i [!DNL Adobe Experience Cloud].
1. När du har loggat in kopierar du URL:en till och med `.com` i webbläsarens adressfält.

   Om till exempel URL:en *fictional* (URL:er alltid innehåller snedstreck, inte omvända snedstreck som i det här exemplet) i adressfältet är `https:\\www.myfictionalsite.com/categories/admin/home.do`, kopierar du bara den här delen av URL:en för *fictional*: `https:\\www.myfictionalsite.com`.

1. I [!DNL Adobe Dynamic Media Classic] går du till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]**.
1. Klistra in den URL som du kopierade i steg 2 i fältet **[!UICONTROL Test&Target Server Name]** på sidan Allmänna inställningar för programmet.
1. Välj **[!UICONTROL Close]**.
