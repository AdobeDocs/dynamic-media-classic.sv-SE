---
title: Överföra en bildresurs eller en vektorresurs
seo-title: Överföra en bildresurs eller en vektorresurs
description: 'null'
seo-description: Lär dig hur du överför en bildresurs eller en vektorresurs.
uuid: d0e4a754-8a49-4b0f-b202-e9003bdb8f20
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: de21dca9-99fe-4183-b647-debfe112fda4
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1536'
ht-degree: 0%

---


# Överföra en bildresurs eller en vektorresurs{#uploading-an-image-asset-or-a-vector-asset}

Innan du kan överföra en bildresurs måste du först begära en delad hemlig nyckel. Du använder den här delade hemliga nyckeln för att hämta en överföringstoken. Sedan använder du överföringstoken för att överföra bildresurser eller vektorresurser.

## Begär en delad-hemlig nyckel {#requesting-a-shared-secret-key}

Begär en *delad-hemlig nyckel* av [med Admin Console för att skapa ett supportärende.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) Begär en delad hemlig nyckel i ditt supportfall.

I e-postmeddelandet anger du det företagsnamn som du vill använda för att överföra bildresurser. När du har fått nyckeln från Dynamic Media Classic sparar du den lokalt för framtida bruk.

## Hämtar överföringstoken {#retrieving-the-upload-token}

*Överföringstoken* säkerställer att ingen kan använda samma delade hemliga nyckel för att överföra resurser. Den ser till att överföringen är giltig och kommer från en betrodd källa.

Överföringstoken är en alfanumerisk sträng som bara är tillgänglig under en viss tidsperiod. Använd följande URL:er, som ersätter din delade hemliga nyckel, för att hämta överföringstoken.

* Bild
   `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`I det här exemplet är nyckeln med delad hemlighet  `fece4b21-87ee-47fc-9b99-2e29b78b602`

* Vektor
   `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`I det här exemplet är nyckeln med delad hemlighet  `2d19f60e-890a-4e79-a1a5-9ac2875429b9`

Som standard upphör överföringstoken att gälla fem minuter (300 sekunder) efter att du har hämtat den. Om du vill ha mer tid tar du med `expires` i URL:en och den tid du behöver i sekunder. Följande exempelbild-URL hämtar till exempel en överföringstoken som är giltig i 1 800 sekunder:

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

Det lyckade svaret på bilder ser ut så här:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
        <serviceName>User Generated Content - Images</serviceName> 
        <version>1.0.0</version> 
        <operationName>get_uploadtoken</operationName> 
        <serviceStatus>SUCCESS</serviceStatus> 
        <title>Upload Token for fece4b21-87ee-47fc-9b99-2e29b78b602</title> 
        <message> 
            <uploadtoken>aa2a378a-cd25-4c80-994d-312094e0ef20_1800</uploadtoken> 
            <expiration_in_seconds>1800</expiration_in_seconds> 
        </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Spara överföringstoken lokalt för framtida förfrågningar.

Du kan använda följande fält i fråge-URL-strängen för att hämta en överföringstoken:

| URL-parameter | Obligatoriskt eller valfritt | Värde |
|--- |--- |--- |
| op | Obligatoriskt | get_uploadtoken |
| shared_secrets | Obligatoriskt | Den delade hemliga nyckeln för det företag som gör överföringen. |
| förfaller | Valfritt | Antal sekunder som överföringstoken är giltig. Standardvärdet är 300 sekunder om inget anges. |

**URL för exempelbild:**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

**Exempel på vektor-URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000`

**Tillåtna HTTP-metoder:** GET och POST

Du kan nu överföra en bildresurs.

Se [Överföra en bildresurs](uploading-image-asset-or-vector.md#uploading_an_image_asset).

## Överför en bildresurs {#uploading-an-image-asset}

När du har hämtat en överföringstoken som är giltig under en viss tid kan du överföra en bildresurs. Du överför resursen som en multipart-/formulärpost medan du skickar resten av värdena som en URL-frågesträng, vilket visas i det här exemplet:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

Fälten `upload_token` och `company_name` är obligatoriska.

Se [Hämta överföringstoken](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Se [Hämta en delad-hemlig nyckel](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

Du kan också skicka andra valfria värden som URL-frågesträngar, som i det här exemplet:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

Parametern `file_limit` anger gränsen för filstorlek i byte. Parametern `file_exts` anger de filnamnstillägg som tillåts för överföring. Båda dessa värden är valfria.

I programmet anges en global gräns för filstorlek och tillåtna filnamnstillägg. Om det du skickar i begäran är en delmängd av de globala gränserna respekteras det. De globala begränsningarna är följande:

| Global gräns | Värde |
|--- |--- |
| Filstorlek för alla klienter | 20 MB |
| Bildfilformat som stöds för överföring | BMP, GIF, JPG, PNG, PSD |

Med följande HTML-formulär kan en användare överföra en resurs. I formuläret uppmanas användaren att ange följande information:

* Ett företagsnamn.
* En överföringstoken.
* En gräns för filstorlek.
* En lista med filnamnstillägg.
* Om färgprofilen och filnamnet som är associerade med resursen ska bevaras eller inte.
* Om du vill använda Blockera bakgrund eller inte. Om du aktiverar Blockera bakgrund anger du hörn-, tolerans- och fyllningsmetod. Se Spara ur bakgrund i [Alternativ för bildredigering vid överföring](image-editing-options-upload.md#image-editing-options-at-upload).
* Namnet på filen som ska överföras

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

![]()

Du kan visa HTML-källkoden som är kopplad till formuläret ovan genom att klicka på följande länk:

[https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)

Högerklicka i webbläsarfönstret i Firefox och klicka sedan på **Visa sidkälla**. Koden visar motsvarande URL-frågesträng och den POST-metod som körs när användaren klickar på **Skicka**.

Om du vill visa XML-svaret i Internet Explorer klickar du på **Visa > Källa**. Om du vill visa XML-svar i Firefox klickar du på **Verktyg > Webbutvecklare > Sidkälla**. Firefox rekommenderas för visning av XML-svar.

Nedan följer ett exempelsvar från en slutförd överföring:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>upload</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Your file has been uploaded Successfully.</title> 
            <message> 
            <url>https://s7w2p1.scene7.com/is/image/ </url> 
            <path>000Company/ugc/1442564.tif</path> 
            <fullurl>https://s7w2p1.scene7.com/is/image/000Company/ugc/1442564.tif </fullurl> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

>[!NOTE]
>
>Den överförda resursen (JPG, GIF o.s.v.) konverteras till PTIFF-format och svaret skickar en direktlänk till den PTIFF-resursen.

Resursen är som vilken annan ImageServing-resurs som helst. du kan använda bearbetningsfrågor på den. Följande URL begär till exempel en resurs som är utsträckt till den angivna bredden och höjden.

```as3
https://s7w2p1.scene7.com/is/image/S7WebUGC/ugc/9536356.tif?&wid=800&hei=100&fit=stretch
```

Skicka resursen som ska överföras som en multipart-/formulärpost samtidigt som resten av värdena skickas som en URL-frågesträng. Du kan använda följande fält i URL-frågesträngen för att överföra en resurs:

| URL-parameter | Obligatoriskt eller valfritt | Värde |
|--- |--- |--- |
| op | Obligatoriskt | ladda upp |
| upload_token | Obligatoriskt | Överför token för den delade hemliga nyckeln som är associerad med företaget. |
| company_name | Obligatoriskt | Namnet på det företag som utför överföringen. |
| file_limit | Valfritt | Filstorleksgräns, i byte, för resursen. |
| file_exts | Valfritt | Lista över tillåtna tillägg för bildresursfilen. |
| preserve_color_profile | Valfritt | Bevarar inbäddad färgprofil när den överförda filen konverteras till PTIFF-format. Möjliga värden är true eller false. Standardvärdet är false. |
| preserve_filename | Valfritt | Bevarar filnamnet för den överförda resursen. Möjliga värden är true eller false. Standardvärdet är false. |

>[!NOTE]
>
>Du måste skicka resursen som ska överföras som det enda fältet i en begäran om flera POSTER.

**Exempel-URL:**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**Tillåten HTTP-metod:**

POST

### Hämta metadata för resurser för bilder {#getting-asset-metadata-for-images}

Du kan använda `image_info` för att hämta metadata för en resurs som du har överfört, vilket visas i följande exempel:

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Ett exempel på ett lyckat svar ser ut så här:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>image_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>More information on 1442564.tif</title> 
            <message> 
            File created on Tue Sep 08 19:02:04 CDT 2009, File Size = 243494 bytes 
            <imageFormat>Tiff</imageFormat> 
            <colorSpace>Rgb</colorSpace> 
            <width>686</width> 
            <height>457</height> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Du kan använda följande fält i URL-frågesträngen för att begära information om en resurs:

| URL-parameter | Obligatoriskt eller valfritt | Värde |
|--- |--- |--- |
| op | Obligatoriskt | image_info |
| shared_secrets | Obligatoriskt | Den delade hemliga nyckeln för företaget. |
| image_name | Obligatoriskt | Bildens namn. |

**Exempel-URL:**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Tillåten HTTP-metod:**

GET och POST

## Överför en vektorresurs {#uploading-a-vector-asset}

När du har hämtat en överföringstoken som är giltig under en viss tid kan du överföra en vektorresurs. Du överför resursen som en multipart-/formulärpost medan du skickar resten av värdena som en URL-frågesträng, vilket visas i det här exemplet:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

Fälten `upload_token` och `company_name` är obligatoriska.

Se [Hämta överföringstoken](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Se [Hämta en delad-hemlig nyckel](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

Du kan också skicka andra valfria värden som URL-frågesträngar, som i det här exemplet:

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

Parametern `file_limit` anger gränsen för filstorlek i byte. Parametern `file_exts` anger de filnamnstillägg som tillåts för överföring. Båda dessa värden är valfria.

I programmet anges en global gräns för filstorlek och tillåtna filnamnstillägg. Om det du skickar i begäran är en delmängd av de globala gränserna respekteras det. De globala begränsningarna är följande:

| Global gräns | Värde |
|--- |--- |
| Filstorlek för alla klienter | 20 MB |
| Vektorfilformat som stöds för överföring | AI, EPS, PDF (endast när PDF-filen tidigare har öppnats och sparats i Adobe Illustrator CS6) |

Med följande HTML-formulär kan en användare överföra en resurs. I formuläret uppmanas användaren att ange följande information:

* Ett företagsnamn.
* En överföringstoken.
* En gräns för filstorlek.
* En lista med filnamnstillägg.
* Om färgprofilen och filnamnet som är associerade med resursen ska bevaras eller inte.
* Om du vill använda Blockera bakgrund eller inte. Om du aktiverar Blockera bakgrund anger du hörn-, tolerans- och fyllningsmetod. Se Spara ur bakgrund i [Alternativ för bildredigering vid överföring](image-editing-options-upload.md#image-editing-options-at-upload).
* Namnet på filen som ska överföras

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

![]()

Följande HTML-kod visas när du högerklickar i webbläsarfönstret och sedan klickar på **Visa källa** för formuläret som visas i bilden. Koden visar motsvarande URL-frågesträng och den POST-metod som körs när användaren klickar på **Skicka**.

```as3
<body> 
<script language="javascript"> 
function uploadImage() 
{ 
document.image_upload.action="vector?op=upload&company_name="+document.image_upload.company_name.value+"&upload_token="+document.image_upload.upload_token.value+"&file_limit="+document.image_upload.file_limit.value+"&file_exts="+document.image_upload.file_exts.value; 
return true; 
} 
</script> 
<form method="POST" enctype="multipart/form-data" name="image_upload" id="image_upload" onSubmit="return uploadImage();"> 
<table> 
<tr><td colspan="2"><strong> UGC Vector Upload Test Page: </strong></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr><td><strong> Company Name</strong></td><td><input type="text" size="40" name="company_name"></td></tr> 
<tr><td><strong> Upload Token </strong></td><td><input type="text" size="40" name="upload_token"></td></tr> 
<tr><td><strong> File Size Limit (in bytes) </strong></td><td><input type="text" size="40" name="file_limit"> bytes</td></tr> 
<tr><td><strong> File Extensions allowed </strong></td><td><input type="text" size="40" name="file_exts"></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>File to upload: : </strong></td> 
<td><input name="filename" type="file" id="filename" size="58" maxlength="1024" /></td> 
</tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>Click Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

Om du vill visa XML-svaret i Internet Explorer klickar du på **Visa** > **Källa**. Om du vill visa XML-svar i Firefox klickar du på **Visa** > **Sidkälla**. Firefox rekommenderas för visning av XML-svar.

Nedan följer ett exempelsvar från en slutförd överföring:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
    <scene7> 
    <user_generated_content> 
    <response> 
    <serviceName>User Generated Content -Vector</serviceName> 
    <version>1.0.0</version> 
    <operationName>upload</operationName> 
    <serviceStatus>SUCCESS</serviceStatus> 
    <title>Your file has been uploaded Successfully.</title> 
    <message> 
    <url>https://s7w2p1.scene7.com/is/agm</url> 
    <path>W2PTest/ugc/8875744.fxg</path> 
    <fullurl> 
        https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg 
    </fullurl> 
</message> 
</response> 
</user_generated_content> 
</scene7>
```

>[!NOTE]
>
>Den överförda resursen (AI, EPS, PDF osv.) konverteras till FXG-format och svaret skickar en direktlänk till den aktuella FXG-resursen.

Resursen är som alla andra webb-till-tryck-resurser. du kan använda bearbetningsfrågor på den. Följande URL konverterar till exempel en FXG-resurs till en bild med storleken 500 × 500 png.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

Skicka resursen som ska överföras som en multipart-/formulärpost samtidigt som resten av värdena skickas som en URL-frågesträng. Du kan använda följande fält i URL-frågesträngen för att överföra en resurs:

| URL-parameter | Obligatoriskt eller valfritt | Värde |
|--- |--- |--- |
| op | Obligatoriskt | ladda upp |
| upload_token | Obligatoriskt | Överför token för den delade hemliga nyckeln som är associerad med företaget. |
| company_name | Obligatoriskt | Namnet på det företag som utför överföringen. |
| file_limit | Valfritt | Filstorleksgräns, i byte, för resursen. |
| file_exts | Valfritt | Lista över tillåtna tillägg för resursfilen. |

>[!NOTE]
>
>Du måste skicka resursen som ska överföras som det enda fältet i en begäran om flera POSTER.

**Exempel-URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**Tillåten HTTP-metod:**

POST
