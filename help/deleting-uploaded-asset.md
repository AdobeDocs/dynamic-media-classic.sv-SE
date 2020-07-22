---
title: Ta bort en överförd resurs
seo-title: Ta bort en överförd resurs
description: 'null'
seo-description: Lär dig hur du tar bort en överförd resurs.
uuid: edd2b688-c377-4be1-ba16-d2dd2e6f716d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: dd338c8c-06c6-44d5-8493-dc2087eeeafb
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '99'
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
            <serviceName>User Generated Content - Images</serviceName> 
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
|--- |--- |--- |
| op | Obligatoriskt | delete |
| shared_secrets | Obligatoriskt | Den delade hemliga nyckeln för företaget. |
| <ul><li>För bilder:bildnamn</li><li>För vektor:fxg_name</li></ul> | Obligatoriskt | Namnet på resursen som ska tas bort. |

**URL för exempelbild:**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Exempel på vektor-URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg`
