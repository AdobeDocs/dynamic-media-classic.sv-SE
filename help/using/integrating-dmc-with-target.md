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

Innan du kan integrera [!DNL Adobe Dynamic Media Classic] med [!DNL Target Standard/Premium] måste du ange mål-URL:en på skärmen [!DNL Adobe Dynamic Media Classic] Allmänna inställningar för program. Så här hämtar du mål-URL:en och anger den på sidan Allmänna inställningar för programmet:

1. Logga in på ditt [!DNL Adobe Experience Cloud]-konto i [!DNL Target Standard/Premium].
1. När du har loggat in kopierar du URL:en till och med `.com` i webbläsarens adressfält.

   Om till exempel URL:en *fictional* (URL:er-sökvägar alltid innehåller snedstreck, inte omvända snedstreck som i det här exemplet) i adressfältet är `https:\\www.myfictionalsite.com/categories/admin/home.do` kopierar du bara den här delen av URL:en *fictional* : `https:\\www.myfictionalsite.com`.

1. Gå till [!DNL Adobe Dynamic Media Classic] > **[!UICONTROL Setup]** i **[!UICONTROL Application Setup]**.
1. Klistra in den URL som du kopierade i steg 2 i fältet **[!UICONTROL Test&Target Server Name]** på sidan Allmänna inställningar för programmet.
1. Välj **[!UICONTROL Close]**.
