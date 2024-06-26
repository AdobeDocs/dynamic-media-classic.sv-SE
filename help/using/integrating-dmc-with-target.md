---
title: Integrera Adobe Dynamic Media Classic med Adobe Target Standard/Premium
description: Lär dig integrera Adobe Dynamic Media Classic med Adobe Target Standard/Premium.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
topic: Integrations, Development
level: Experienced
source-git-commit: 914fde11270dc731a261da3305b29dd573584d93
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---

# Integrera Adobe Dynamic Media Classic med Adobe Target Standard/Premium {#integrating-dmc-with-target}

Innan du kan integrera [!DNL Adobe Dynamic Media Classic] med [!DNL Target Standard/Premium]måste du ange mål-URL:en i [!DNL Adobe Dynamic Media Classic] Skärmen Allmänna inställningar för programmet. Så här hämtar du mål-URL:en och anger den på sidan Allmänna inställningar för programmet:

1. I [!DNL Adobe Experience Cloud], logga in på [!DNL Target Standard/Premium] konto.
1. När du har loggat in kopierar du URL:en till och med i webbläsarens adressfält `.com`.

   Om *fiktiv* URL (URL-adresser innehåller alltid snedstreck, inte omvända snedstreck som i det här exemplet) i adressfältet är `https:\\www.myfictionalsite.com/categories/admin/home.do`, kopierar endast den här delen av *fiktiv* URL: `https:\\www.myfictionalsite.com`.

1. I [!DNL Adobe Dynamic Media Classic], gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]**.
1. På sidan Allmänna inställningar för programmet, i **[!UICONTROL Test&Target Server Name]** klistra in den URL som du kopierade i steg 2.
1. Välj **[!UICONTROL Close]**.
