---
title: Testa resurser innan du gör dem offentliga
description: Lär dig hur du testar resurser i Adobe Dynamic Media Classic innan du publicerar dem.
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 0%

---

# Testa resurser innan du gör dem offentliga {#testing-assets-before-making-them-public}

Säker testning hjälper er att definiera en säker testmiljö och bygga en robust B2B-lösning som bygger på en konfigurerbar uppsättning IP-adresser och intervall. Med den här funktionen kan ni matcha era Adobe Dynamic Media Classic-installationer med arkitekturen i ert innehållshanteringssystem och affärssystem.

Med Säker testning kan du förhandsgranska testversionen av webbplatsen med opublicerat innehåll.

Om du vill kan du skapa en staging-miljö i stället för att göra resurserna allmänt tillgängliga av följande skäl:

* Förhandsgranska webbplatser innan den offentliga lanseringen (testwebbplatsen).
* Tjäna resurser som kräver begränsad åtkomst, till exempel e-kataloger som visar priser i B2B-webbprogram.
* Använd material bakom en brandvägg som en del av produktinformationshanteringssystemet, kundtjänstprogrammet, utbildningswebbplatsen osv.

>[!NOTE]
>
>Säker testning påverkar inte åtkomsten till Adobe Dynamic Media Classic. Adobe Dynamic Media Classic säkerhet är konsekvent och kräver de vanliga inloggningsuppgifterna för åtkomst till Adobe Dynamic Media Classic och relaterade webbtjänster.

## Så här fungerar säkra tester {#how-secure-testing-works}

De flesta företag använder internet bakom en brandvägg. Tillgång till Internet är möjlig via vissa vägar och vanligtvis via ett begränsat antal offentliga IP-adresser.

I företagsnätverket kan du räkna ut din offentliga IP-adress med webbplatser som [https://www.whatismyip.com](https://www.whatismyip.com/) eller begär den här informationen från IT-avdelningen.

Med Secure Testing skapar Adobe Dynamic Media Classic en dedikerad Image Server för testmiljöer eller interna applikationer. Alla förfrågningar till den här servern kontrollerar den ursprungliga IP-adressen. Om den inkommande begäran inte finns i den godkända listan över IP-adresser returneras ett felsvar. Adobe Dynamic Media Classic företagsadministratör konfigurerar den godkända listan över IP-adresser för företagets säkra testmiljö.

Eftersom platsen för den ursprungliga begäran måste bekräftas, dirigeras inte trafiken för tjänsten för säker testning via ett nätverk för innehållsdistribution, t.ex. offentlig Dynamic Media Image Server-trafik. Begäranden till tjänsten för säker testning har en något högre fördröjning än de offentliga Dynamic Media Image-servrarna.

Opublicerade resurser är omedelbart tillgängliga från tjänsterna för säker testning, utan att behöva publicera. På så sätt kan du köra en förhandsvisning innan resurser publiceras på den offentliga bildservern.

>[!NOTE]
>
>Tjänster för säker testning använder katalogservern som är konfigurerad med en intern publiceringskontext. Om ditt företag är konfigurerat att publicera till Säker testning blir därför alla överförda resurser i Adobe Dynamic Media Classic omedelbart tillgängliga på säkra testningstjänster. Den här funktionen är sann oavsett om resurserna har markerats för publicering vid överföring.

Tjänster för säker testning stöder för närvarande följande resurstyper och funktioner:

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* Bilder.
* Vinjetter (renderingsserverbegäranden).
* Rendera serverförfrågningar (stöds, men måste begäras uttryckligen av kunden).
* Uppsättningar, inklusive bilduppsättningar, eCatalog, renderingsuppsättningar och medieuppsättningar.
* Adobe Dynamic Media Classic multimedievisningsprogram som standard.
* Adobe Dynamic Media Classic OnDemand JSP pages.
* Statiskt innehåll, till exempel PDF-filer och progressivt levererade videor.
* HTTP-videoströmning.
* Progressiv videoströmning.

Följande tillgångstyper och funktioner stöds för närvarande inte:

* Adobe Dynamic Media Classic Info- eller eCatalog-sökning
* RTMP-videoströmning
* Webb-till-tryck
* UGC-tjänster (användargenererat innehåll)

>[!IMPORTANT]
>
>Stöd för nya eller befintliga UGC-vektorbildresurser i Adobe Dynamic Media Classic upphörde den 30 september 2021.

## Testa tjänsten för säker testning {#testing-the-secure-testing-service}

Testa tjänsten Secure Testing så att du kan vara säker på att den fungerar som förväntat.

<!-- >[!NOTE]
>
>*If you do not mention any IPs under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Test Image Service]*** - If you add an IP only, that IP is able to call the assets and no other IP are allowed to make the calls. As long there is no IP mentioned under that section, all IPs are allowed to make the calls for the assets, and they show up. -->

### Förbered ditt konto

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Kontakta Adobe kundtjänst och begär att de aktiverar säker testning på ditt konto.
1. I Adobe Dynamic Media Classic går du till **[!UICONTROL Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]**.
1. På sidan Image Server Publish (Image Server Publish) i **[!UICONTROL Publish Context]** nedrullningsbar lista, välja **[!UICONTROL Test Image Serving]**.
1. För klientadressfiltret väljer du **[!UICONTROL Add]**.
1. Markera kryssrutan så att adressen är aktiverad (påslagen) och skriv sedan en IP-adress och nätmask i respektive textfält.

   >[!NOTE]
   >
   >Om du lägger till en enda IP-adress och nätmask kan den adressen göra tillgångsanrop. Andra IP-adresser och nätmasker som du lägger till har dock inte rätt att göra resursanrop. Överväg därför att inaktivera (inaktivera) kryssrutan i steget ovan för att inaktivera möjligheten att ange en IP-adress och nätmask. Om man gör det på ett så effektivt sätt kan *alla* IP-adresser för att göra tillgångsanrop, och de visas alla.

1. Gör något av följande:
   * Upprepa de två föregående stegen om du måste lägga till fler IP-adresser.
   * Fortsätt till nästa steg.
1. Längst ned till vänster på Image Server Publish-sidan väljer du **[!UICONTROL Save]**
1. Ladda upp bilderna till ditt Adobe Dynamic Media Classic-konto.

   Se [Överför filer](uploading-files.md#uploading_files).

1. Se till att vissa bilder är markerade för publicering och att andra är omarkerade och skicka sedan publiceringsjobbet.

   Se [Publicera filer](publishing-files.md#publishing_files).

1. Bestäm namnet på tjänsten för säker testning genom att gå till **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]**.
1. På sidan Allmänna inställningar för programmet, under gruppen Servrar, söker du efter namnet till höger om **[!UICONTROL Test Publish Context Server Name]**.

Kontakta Adobe Care om servernamnet saknas eller om URL:erna till inte fungerar.

### Förbered webbplatsvarianter

Du behöver två varianter av en webbplats som länkar de publicerade och opublicerade resurserna:

* Offentlig version - Länka resurser med din traditionella Adobe Dynamic Media Classic URL-syntax.
* Mellanlagringsversion - Länka resurser med samma syntax men med namnet på platsen för säker testning.

### Kör testerna

Utför följande tester:

1. Kontrollera om resurser är synliga inifrån företagets nätverk.

   I företagsnätverket som identifieras av det tidigare definierade IP-adressintervallet visar mellanlagringsversionen av webbplatsen alla bilder, oavsett om de är markerade för publicering eller inte. Därför kan du testa utan att oavsiktligt göra bilder tillgängliga innan du förhandsgranskar eller startar produkten.

   Bekräfta att den offentliga versionen av din webbplats visar publicerade resurser så som de har varit med Adobe Dynamic Media Classic tidigare.

1. Verifiera att icke-publicerade resurser (dvs. omärkta för publicering) är skyddade från åtkomst från tredje part utanför företagets nätverk.

   Få åtkomst till ditt nätverk utifrån (t.ex. från din hemdator eller via en 3G-anslutning) och kontrollera sedan att den offentliga versionen av webbplatsen visar alla publicerade resurser, men inget av det opublicerade innehållet.

   Bekräfta att mellanlagringsversionen inte visar någon resurs eftersom du använder tjänsten för säker testning från en ej godkänd IP-adress.
