---
title: Testa resurser innan du gör dem offentliga
seo-title: Testa resurser innan du gör dem offentliga
description: 'null'
seo-description: Lär dig hur du testar resurser innan du publicerar dem.
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 0%

---


# Testa resurser innan du gör dem offentliga {#testing-assets-before-making-them-public}

Säker testning hjälper er att definiera en säker testmiljö och bygga en robust B2B-lösning som bygger på en konfigurerbar uppsättning IP-adresser och intervall. Med den här funktionen kan du matcha dina Dynamic Media Classic-distributioner med arkitekturen för din innehållshantering och e-handelsplattform.

Med Säker testning kan du förhandsgranska testversionen av webbplatsen med opublicerat innehåll.

Du kanske föredrar att skapa en staging-miljö i stället för att göra resurserna tillgängliga för allmänheten av följande skäl:

* Förhandsgranska webbplatser innan den offentliga lanseringen (testwebbplatsen).
* Tjäna resurser som kräver begränsad åtkomst, till exempel e-kataloger som visar priser i B2B-webbprogram.
* Använd material bakom en brandvägg som en del av produktinformationshanteringssystemet, kundtjänstprogrammet, utbildningswebbplatsen osv.

>[!NOTE]
>
>Säker testning påverkar inte åtkomsten till Dynamic Media Classic. Dynamic Media Classic-säkerhet är konsekvent och kräver de vanliga autentiseringsuppgifterna för åtkomst till Dynamic Media Classic och relaterade webbtjänster.

## Så här fungerar säkra tester {#how-secure-testing-works}

De flesta företag använder internet bakom en brandvägg. Tillgång till Internet är möjlig via vissa vägar och vanligtvis via ett begränsat antal offentliga IP-adresser.

Från ditt företagsnätverk kan du ta reda på din offentliga IP-adress med hjälp av webbplatser som https://whatismyip.com eller begära den här informationen från din IT-organisation.

Med Säker testning skapar Dynamic Media Classic en dedikerad Image Server för testmiljöer eller interna program. Alla förfrågningar till den här servern kontrollerar den ursprungliga IP-adressen. Om den inkommande begäran inte finns i den godkända listan över IP-adresser returneras ett felsvar. Dynamic Media Classic Company Administrator konfigurerar den godkända listan med IP-adresser för företagets säkra testmiljö.

Eftersom platsen för den ursprungliga begäran måste bekräftas, dirigeras inte trafiken för tjänsten för säker testning via ett nätverk för innehållsdistribution, till exempel offentlig Dynamic Media Image Server-trafik. Begäranden till tjänsten för säker testning kan ha en något högre fördröjning än de offentliga Dynamic Media Image Servers.

Opublicerade resurser är omedelbart tillgängliga från tjänsterna för säker testning, utan att behöva publicera. Detta gör att du kan köra en förhandsvisning innan resurser publiceras på den offentliga bildservern.

***Obs **! Säker testning utnyttjar katalogservern som är konfigurerad med en intern publiceringskontext. Om ditt företag är konfigurerat att publicera till Säker testning bör du därför vara medveten om att överförda resurser i Dynamic Media Classic omedelbart blir tillgängliga på säkra testningstjänster. Den här funktionen är sann oavsett om resurserna har markerats för publicering vid överföring eller inte.*

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
* Standardvisningsprogram för multimedia i Dynamic Media Classic.
* Dynamic Media Classic OnDemand JSP-sidor.
* Statiskt innehåll, till exempel PDF-filer och progressivt levererade videor.
* HTTP-videoströmning.
* Progressiv videoströmning.

Följande tillgångstyper och funktioner stöds för närvarande inte:

* RTMP-videoströmning
* UGC-tjänster
* Webb-till-tryck
* Dynamic Media Classic Info eller e-katalogsökning

## Testa tjänsten Secure Testing {#testing-the-secure-testing-service}

Du bör testa tjänsten för säker testning för att kontrollera att den fungerar som förväntat.

**Förbered ditt konto**

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Kontakta teknisk support och begär att säker testning aktiveras för ditt konto.
1. I Dynamic Media Classic klickar du på **Inställningar** > **Publiceringsinställningar** > **Bildserver**.
1. På sidan Image Server Publish (Publicera kontext) väljer du **Test Image Serving**(Testa bildserver).
1. Klicka på **Lägg till** som klientadressfilter.
1. Markera kryssrutan om du vill aktivera (aktivera) adressen och ange sedan en IP-adress och nätmask i respektive textfält.
1. Upprepa de två föregående stegen för att lägga till fler IP-adresser. I annat fall fortsätter du till nästa steg.
1. Klicka på **Spara längst ned till vänster på sidan Image Server Publish**
1. Överför de önskade bilderna till ditt Dynamic Media Classic-konto.

   Se [Överföra filer](uploading-files.md#uploading_files).

1. Se till att vissa bilder är markerade för publicering och att andra är omarkerade och skicka sedan publiceringsjobbet.

   Se [Publicera](publishing-files.md#publishing_files).

1. Ange namnet på tjänsten för säker testning genom att klicka på **Inställningar** > **Programinställningar** > **Allmänna inställningar**.
1. På sidan Allmänna inställningar för programmet, under gruppen Servrar, hittar du namnet till höger om **Test Publish Context Server Name**.

Kontakta teknisk support om servernamnet saknas eller om URL:er till servern inte fungerar.

**Förbered webbplatsvarianter**

Du behöver två varianter av en webbplats som länkar de publicerade och opublicerade resurserna:

* Offentlig version: Länka resurser med din vanliga Dynamic Media Classic URL-syntax
* Mellanlagringsversion: Länka resurser med samma syntax men med namnet på platsen för säker testning

**Kör testerna**

Utför följande tester:

1. Kontrollera om resurser är synliga inifrån företagets nätverk.

   I det företagsnätverk som identifieras av det tidigare definierade IP-adressintervallet ska mellanlagringsversionen av webbplatsen visa alla bilder, oavsett om de är markerade för publicering eller inte. Det gör att du kan testa utan att oavsiktligt göra bilder tillgängliga innan du förhandsgranskar eller startar produkten.

   Bekräfta att den offentliga versionen av din webbplats visar publicerade resurser så som de har varit i Dynamic Media Classic tidigare.

1. Verifiera att icke-publicerade resurser (dvs. omärkta för publicering) är skyddade från åtkomst från tredje part utanför företagets nätverk.

   Få åtkomst till ditt nätverk utifrån (t.ex. från din hemdator eller via en 3G-anslutning) och kontrollera sedan att den offentliga versionen av webbplatsen visar alla publicerade resurser, men inget av det opublicerade innehållet.

   Bekräfta att mellanlagringsversionen inte visar någon resurs eftersom du använder tjänsten för säker testning från en ej godkänd IP-adress.

