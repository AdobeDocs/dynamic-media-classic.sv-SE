---
title: Överföra en rasterbildsresurs
description: Lär dig hur du överför en rasterbildsresurs till Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: 2ef78fe6-1e7c-4f48-86da-137ddaa55bbf
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '1002'
ht-degree: 0%

---

# Överföra en rasterbildsresurs {#uploading-an-image-asset-or-a-vector-asset}

Innan du kan överföra en bildresurs måste du först begära en delad hemlig nyckel. Du använder den här delade hemliga nyckeln för att hämta en överföringstoken. Du använder sedan överföringstoken för att överföra rasterbildsresurser.

>[!IMPORTANT]
>
>Från och med 1 maj 2023 kommer UGC-resurser i Dynamic Media att vara tillgängliga för användning upp till 60 dagar från överföringsdatumet. Efter 60 dagar tas resurserna bort.

>[!NOTE]
>
>Stöd för nya eller befintliga UGC-vektorresurser i Adobe Dynamic Media Classic upphörde den 30 september 2021.

## Begär en delad hemlig nyckel {#requesting-a-shared-secret-key}

Begär en *delad-hemlig nyckel* av [med Admin Console för att skapa ett supportärende.](https://helpx.adobe.com/se/enterprise/using/support-for-experience-cloud.html) I fallet med teknisk support begär du en delad-hemlig nyckel.

I e-postmeddelandet anger du det företagsnamn som du vill använda för att överföra bildresurser. När du har fått nyckeln från Adobe Dynamic Media Classic sparar du den lokalt för framtida bruk.

## Hämta överföringstoken {#retrieving-the-upload-token}

*Överföringstoken* ser till att ingen kan använda samma delade hemliga nyckel för att överföra resurser. Den ser till att överföringen är giltig och kommer från en betrodd källa.

Överföringstoken är en alfanumerisk sträng som bara är tillgänglig under en viss tidsperiod. Använd följande URL:er och ersätt din delade hemliga nyckel så att du kan hämta överföringstoken.

* Rasterbild
  `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`I det här exemplet är nyckeln med delad hemlighet `fece4b21-87ee-47fc-9b99-2e29b78b602`

<!-- * Vector
  `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`In this example, the shared-secret key is `2d19f60e-890a-4e79-a1a5-9ac2875429b9` -->

Som standard upphör överföringstoken att gälla fem minuter (300 sekunder) efter att du har hämtat den. Om du vill ha mer tid tar du med `expires` i URL:en och den tid du behöver i sekunder. Följande exempelbild-URL hämtar till exempel en överföringstoken som är giltig i 1 800 sekunder:

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

Svaret för bilder ser ut ungefär som följande:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
        <serviceName>User Generated Content: Images</serviceName> 
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
| --- | --- | --- |
| op | Obligatoriskt | get_uploadtoken |
| shared_secrets | Obligatoriskt | Den delade hemliga nyckeln för det företag som gör överföringen. |
| förfaller | Valfritt | Antal sekunder som överföringstoken är giltig. Standardvärdet är 300 sekunder om inget anges. |

**URL för exempelrasterbild:**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000` -->

**Tillåtna HTTP-metoder:**
`GET` och `POST`

Du kan nu överföra en bildresurs.

Se [Överför en bildresurs](uploading-image-asset-or-vector.md#uploading_an_image_asset).

## Överföra en rasterbildsresurs {#uploading-an-image-asset}

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

I programmet anges en global gräns för filstorlek och tillåtna filnamnstillägg. Om det du skickade i begäran är en delmängd av de globala begränsningarna, respekteras det. De globala begränsningarna är följande:

| Global gräns | Värde |
| --- | --- |
| Filstorlek för alla klienter | 20 MB |
| Bildfilformat som stöds för överföring | BMP, GIF, JPG, PNG, PSD, TIFF |

I följande HTML-formulär kan en användare överföra en resurs. I formuläret uppmanas användaren att ange följande information:

* Ett företagsnamn.
* En överföringstoken.
* En gräns för filstorlek.
* En lista med filnamnstillägg.
* Anger om färgprofilen och filnamnet som är associerade med resursen ska bevaras.
* Om en blockerad bakgrund ska användas. Om du aktiverar Blockera bakgrund anger du hörn-, tolerans- och fyllningsmetod.
Se Blockera bakgrund i [Alternativ för finjustering av bilder vid överföring](image-editing-options-upload.md#image-editing-options-at-upload).
* Namnet på filen som ska överföras.

Du kan visa källkoden för HTML som är kopplad till formuläret ovan genom att välja [https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)

Högerklicka i webbläsarfönstret i Firefox och välj sedan **[!UICONTROL View Page Source]**. Koden visar motsvarande URL-frågesträng och den POST som körs när användaren väljer **[!UICONTROL Submit]**.

Om du vill visa XML-svaret i Internet Explorer går du till **[!UICONTROL View]** > **[!UICONTROL Source]**. Om du vill visa XML-svaret i Firefox går du till **[!UICONTROL Tools]** > **[!UICONTROL Browser Tools]** > **[!UICONTROL Web Developer Tools]**. Firefox rekommenderas för visning av XML-svar.

Nedan följer ett exempelsvar från en slutförd överföring:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content: Images</serviceName> 
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
>Den överförda resursen (JPG, GIF och så vidare) konverteras till PTIFF-format och svaret skickar en direkt länk till den PTIFF-resursen.

Resursen är som vilken annan ImageServing-resurs som helst. Du kan använda bearbetningsfrågor på den. Följande URL begär till exempel en resurs som är utsträckt till den angivna bredden och höjden.

```as3
https://s7w2p1.scene7.com/is/image/S7WebUGC/ugc/9536356.tif?&wid=800&hei=100&fit=stretch
```

Skicka resursen som ska överföras som en multipart-/formulärpost samtidigt som resten av värdena skickas som en URL-frågesträng. Du kan använda följande fält i URL-frågesträngen för att överföra en resurs:

| URL-parameter | Obligatoriskt eller valfritt | Värde |
| --- | --- | --- |
| `op` | Obligatoriskt | ladda upp |
| `upload_token` | Obligatoriskt | Överför en token för den delade hemliga nyckeln som är associerad med företaget. |
| `company_name` | Obligatoriskt | Namnet på det företag som utför överföringen. |
| `file_limit` | Valfritt | Filstorleksgräns i byte för resursen. |
| `file_exts` | Valfritt | Lista över tillåtna tillägg för bildresursfilen. |
| `preserve_colorprofile` | Valfritt | Bevarar inbäddad färgprofil när den överförda filen konverteras till PTIFF-format. Möjliga värden är true eller false. Standardvärdet är false. |
| `preserve_filename` | Valfritt | Bevarar filnamnet för den överförda resursen. Möjliga värden är true eller false. Standardvärdet är false. |

>[!NOTE]
>
>Du måste skicka resursen som ska överföras som det enda fältet i en begäran om flera POSTER.

**Exempel-URL:**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**Tillåten HTTP-metod:**

POST

### Hämta metadata för bildobjekt {#getting-asset-metadata-for-images}

Du kan använda `image_info` för att hämta metadata för en resurs som du har överfört, vilket visas i följande exempel:

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Ett exempel på ett lyckat svar ser ut ungefär så här:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content: Images</serviceName> 
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
| --- | --- | --- |
| `op` | Obligatoriskt | image_info |
| `shared_secret` | Obligatoriskt | Nyckeln som är delad hemlighet för företaget. |
| `image_name` | Obligatoriskt | Bildens namn. |

**Exempel-URL:**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Tillåten HTTP-metod:**

GET och POST

<!-- ## Upload a vector asset {#uploading-a-vector-asset}

>[!IMPORTANT]
>
>Support for new or existing UGC vector image assets in Adobe Dynamic Media Classic end on September 30, 2021.

After you retrieve an upload token that is valid for a specific amount of time, you can upload a vector asset. You upload the asset as a multipart/form post while sending the rest of the values as a URL query string, as shown in this example:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

The `upload_token` and `company_name` fields are required.

See [Retrieve the upload token](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

See [Retrieve a shared-secret key](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

You can also send other optional values as URL query strings, as in this example:

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

The `file_limit` parameter specifies the file-size limit in bytes. The `file_exts` parameter specifies the filename extensions that are allowed for upload. Both of these values are optional.

A global limit is set in the application for the file size limit and the filename extensions allowed. If what you send in the request is a subset of the global limits, it is honored. The global limits are the following:

| Global limit | Value |
| --- | --- |
| File size for all clients | 20 MB |
| Supported vector file formats for upload | AI, EPS, PDF (only when the PDF is previously opened and saved in Adobe Illustrator CS6) |

The following HTML form lets a user upload an asset. The form asks the user to enter the following information:

* A company name.
* An upload token.
* A file size limit.
* A list of filename extensions.
* Whether to preserve the color profile and file name associated with the asset.
* Whether to use Knockout Background. If you enable Knockout Background, set the Corner, Tolerance, and Fill Method.
See Knockout Background in [Image fine-tuning options at upload](image-editing-options-upload.md#image-editing-options-at-upload).
* The name of the file to upload.

The following HTML code is displayed when you right-click in the browser window, and then select **[!UICONTROL View Source]** for the form shown in the example. The code shows the corresponding URL query string and the POST method that are run when the user selects **[!UICONTROL Submit]**.

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
<td><strong>Select Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

To view the XML response in Internet Explorer, go to **[!UICONTROL View]** > **[!UICONTROL Source]**. To view XML response in Firefox, go to **[!UICONTROL Tools]** > **[!UICONTROL Browser Tools]** > **[!UICONTROL Page Source]**. Firefox is recommended for viewing XML responses.

The following is a sample response from a successful upload:

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
>The uploaded asset (AI, EPS, PDF so on) is converted to the FXG format and the response sends a direct link to that FXG asset.

The asset is like any other Web-to-print resource; you apply processing queries to it. For example, the following URL converts an FXG resource into a 500x500 png image.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

Send the asset to upload as a multipart/form post while sending the rest of the values as a URL query string. You can use the following fields in the URL query string to upload an asset:

| URL Parameter | Required or Optional | Value |
| --- | --- | --- |
| `op` | Required | upload |
| `upload_token` | Required | Upload token for the shared-secret key associated with the company. |
| `company_name` | Required | Name of the company performing the upload. |
| `file_limit` | Optional | File size limit, in bytes, for the asset. |
| `file_exts` | Optional | List of allowable extensions for the asset file. |

>[!NOTE]
>
>You are required to send the asset to be uploaded as the only field in a multipart POST request.

**Sample URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**Allowed HTTP method:**

POST
 -->