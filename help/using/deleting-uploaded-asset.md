---
title: Ta bort en överförd rasterbildsresurs
description: Lär dig hur du tar bort en överförd resurs i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: d845bcb2-f914-4727-8df2-049dc172f266
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 0%

---

# Ta bort en överförd resurs{#deleting-an-uploaded-asset}

Du kan använda parametern `delete` i det här formatet för att ta bort en resurs:

```as3
https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Följande är ett exempel på ett svar när en bildresurs tas bort:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content: Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>delete</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Delete request for1442564.tif</title> 
            <message>Your file was successfully deleted</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Du kan använda följande fält i URL-frågesträngen för att ta bort en resurs:

| URL-parameter | Obligatoriskt/valfritt | Värde |
| --- | --- | --- |
| `op` | Obligatoriskt | delete |
| `shared_secret` | Obligatoriskt | Nyckeln som är en delad hemlighet för företaget. |
| `image_name` | Obligatoriskt | Namnet på resursen som ska tas bort. |

<!-- <li>For Vector:fxg_name</li> -->

>[!IMPORTANT]
>
>Från och med 1 maj 2023 är UGC-resurser i Dynamic Media tillgängliga för användning upp till 60 dagar från överföringsdatumet. Efter 60 dagar tas resurserna bort.

>[!NOTE]
>
>Stöd för nya eller befintliga UGC-vektorbildresurser i Adobe Dynamic Media Classic upphörde den 30 september 2021.

**URL för exempelbild:**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg` -->
