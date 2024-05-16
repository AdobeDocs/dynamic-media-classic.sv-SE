---
title: Hämta information om diskanvändning
description: Lär dig hur du får information om diskanvändning i Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 337a4681-ac9a-40d9-82e8-1999bbed980c
topic: Administration, Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '91'
ht-degree: 0%

---

# Hämta information om diskanvändning {#get-disk-usage-information}

Du kan använda `disk_info` parameter för att hämta information om ett företags diskutrymmesanvändning, vilket visas i följande exempel:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=d03b7e0b-c9dc-4c6c-af0b-419beeea1c63
```

Ett exempelsvar ser ut så här:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content: Images</serviceName> 
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
| --- | --- | --- |
| op | Obligatoriskt | disk_info |
| shared_secrets | Obligatoriskt | Nyckeln som är en delad hemlighet för företaget |

Följande exempelkod hämtar diskinformation för 000Company:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```
