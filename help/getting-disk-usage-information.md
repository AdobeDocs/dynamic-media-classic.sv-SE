---
title: Hämta information om diskanvändning
description: Lär dig hur du hämtar information om diskanvändning.
uuid: 01361693-53d0-4072-b7c3-f284631d28cf
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6763546d-83c4-42dc-879f-6bbfc8b56482
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '85'
ht-degree: 0%

---


# Hämta information om diskanvändning {#getting-disk-usage-information}

Du kan använda parametern `disk_info` för att hämta information om ett företags diskutrymmesanvändning, vilket visas i följande exempel:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=d03b7e0b-c9dc-4c6c-af0b-419beeea1c63
```

Ett exempelsvar ser ut så här:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>disk_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Disk Information for d03b7e0b-c9dc-4c6c-af0b-419beeea1c63</title> 
            <message>Total Space available = 1395402342400 bytes. Total Space used = 0 bytes.</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Du kan använda följande fält i URL-frågesträngen för att få information om diskanvändning:

| URL-parameter | Obligatoriskt/valfritt | Värde |
|--- |--- |--- |
| op | Obligatoriskt | disk_info |
| shared_secrets | Obligatoriskt | Den delade hemliga nyckeln för företaget |

Följande exempelkod hämtar diskinformation för 000Company:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```

