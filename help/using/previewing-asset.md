---
title: Förhandsgranska en resurs
description: Lär dig hur du förhandsgranskar en resurs i Adobe Dynamic Media Classic.
uuid: 4a01be21-e37f-4d79-9220-f4e177e9179a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 17d0bfd6-fc62-4ed6-8a51-7ac1a6bb96cc
feature: Dynamic Media Classic,Asset Management,Viewers
role: User
exl-id: 7e6f652c-b197-4171-b11b-f532795f7cf2
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 0%

---

# Förhandsgranska en resurs{#previewing-an-asset}

Du kan använda Förhandsgranska för att se hur en digital resurs ser ut när den visas av en kund. I förhandsvisningen används det standardvisningsprogram som är tilldelat resursen. Standardvisningsprogram är konfigurerade i programinställningarna.

Se [Konfigurera standardvisningsprogram](application-setup.md#configuring_default_viewers).

Om du förhandsgranskar en mallresurs med parameterlager kan du ändra parametrar eller ändra bildförinställningen. Eftersom ändringarna infogas kan du visa resultatet direkt från samma förhandsgranskningsfönster.

Se även [Exempel på referensbibliotek för Adobe-visningsprogram](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

**Så här förhandsgranskar du en resurs:**

1. Gå till resursmapparna som innehåller resursen som du vill förhandsgranska i panelen Resursbibliotek på vänster sida.
1. Gör något av följande:

   * Ovanför fönstret Resurser, till höger om verktygsfältet, väljer du **[!UICONTROL Grid View]**.
   * Ovanför fönstret Resurser, till höger om verktygsfältet, väljer du **[!UICONTROL List View]**.
   * Ovanför fönstret Resurser, till höger om verktygsfältet, väljer du **[!UICONTROL Detail View]**.

1. Beroende på vilken vy du använder gör du något av följande:

   * I fönstret Resurser i stödrastervyn eller listvyn väljer du en enskild resurs och väljer sedan **[!UICONTROL Preview]** nära miniatyrbilden.
   * I verktygsfältet ovanför fönstret Resurser i stödrastervyn, listvyn eller detaljvyn väljer du **[!UICONTROL Preview]**.

## Förhandsgranska en resurs baserat på visningsprogrammets plattformstyp {#previewing-an-asset-based-on-viewer-platform-type}

Du kan använda visningsprogramlistan för att förhandsvisa hur en resurs visas på en viss typ av visningsprogramplattform, till exempel HTML5. Beroende på resurstypen och det tillhörande visningsprogram som du har valt att förhandsgranska, är inte alla plattformar tillgängliga i visningsprogramlistan.

Du kan också använda visningsprogramlistan för att kopiera en visningsprogramURL eller visa och kopiera visningsprogramkoden för inbäddning på dina webbsidor.

För en viss visningsprogramplattform kan du i visningsprogramlistefönstret se vilka enheter, som surfplattor och smarttelefoner, som ett visningsprogram är tillgängligt för.

**Så här förhandsgranskar du en resurs baserat på visningsprogrammets plattformstyp:**

1. Gå till resursmapparna som innehåller resursen som du vill förhandsgranska i panelen Resursbibliotek på vänster sida.
1. Gör något av följande:

   * Ovanför fönstret Resurser, till höger om verktygsfältet, väljer du **[!UICONTROL Grid View]**. I fönstret Resurser väljer du en enskild resurs och går sedan till under miniatyrbilden **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
   * Ovanför fönstret Resurser, till höger om verktygsfältet, väljer du **[!UICONTROL List View]**. I fönstret Resurser väljer du en enskild resurs och går sedan till höger om miniatyrbilden till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
   * Ovanför fönstret Resurser, till höger om verktygsfältet, väljer du **[!UICONTROL Detail View]**. På samma verktygsfält går du till **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

1. (Valfritt) Markera kolumnrubriken i fönstret Visningsprogramlista **[!UICONTROL Name]** eller **[!UICONTROL Platform type]** om du vill sortera kolumnen i stigande eller fallande ordning.
1. I fönstret Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Preview]** om du vill se hur resursen visas för ett valt visningsprogram och en viss plattformstyp.

   Stäng den förhandsgranskning som visas.

1. (Valfritt) I listrutan URL-kodning för att kopiera URL-generering i visningsprogramlistan längst ned väljer du den URL-kodning som du vill använda på resursens URL när den kopieras.
1. (Valfritt) Gör något av följande:

   * I fönstret Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Copy URL]** för ett valt visningsprogram och en viss plattformstyp.

     När du väljer **[!UICONTROL Copy URL]**, kopieras den associerade URL:en automatiskt till Urklipp.

   * I fönstret Visningsprogramlista, under kolumnen Åtgärder i tabellen, väljer du **[!UICONTROL Embed Code]**.

     När du väljer **[!UICONTROL Embed Code]**&#x200B;öppnas fönstret Bädda in kod där du kan granska visningsprogramkoden. Det är inte tillåtet att redigera koden i fönstret. Du kan också kopiera koden till Urklipp så att du kan klistra in den på dina webbsidor.

     Stäng den förhandsgranskning som visas.

1. I det nedre högra hörnet av fönstret Visningsprogramlista väljer du **[!UICONTROL Close]** för att gå tillbaka till skärmen Resurser.

## Förhandsvisa en bildresurs baserat på dess bildförinställning {#previewing-an-image-asset-based-on-its-image-preset}

Du kan förhandsgranska en bildresurs baserat på bildförinställningen för att ta reda på hur bilden ser ut när den levereras dynamiskt till webbplatsen eller programmet i olika storlekar.

En bildförinställning är en samling fördefinierade inställningar som ändrar storlek, bildkvalitet, format, upplösning och andra aspekter av en bilds utseende när den exporteras.

Se [Konfigurera bildförinställningar](setting-image-presets.md#setting_up_image_presets).

Se [Skapa och aktivera bildförinställningar](creating-enabling-image-presets.md#creating_and_enabling_image_presets).

**Så här förhandsvisar du en bildresurs baserat på dess bildförinställning:**

1. Gå till resursmapparna som innehåller den bildresurs som du vill förhandsgranska i panelen Resursbibliotek på vänster sida.
1. Gör något av följande:

   * Ovanför fönstret Resurser, till höger om verktygsfältet, väljer du **[!UICONTROL Grid View]**. I fönstret Resurser väljer du en enda bildresurs och går sedan till under miniatyrbilden **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.
   * Ovanför fönstret Resurser, till höger om verktygsfältet, väljer du **[!UICONTROL List View]**. I fönstret Resurser väljer du en enda bildresurs och går sedan till höger om miniatyrbilden till **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.
   * Ovanför fönstret Resurser, till höger om verktygsfältet, väljer du **[!UICONTROL Detail View]**. På samma verktygsfält går du till **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.

1. I fönstret Bildförinställningslista i tabellen markerar du namnet på en förinställningstyp vars bildresurs du vill förhandsgranska infogat i den högra rutan.
1. (Valfritt) I fönstret Bildförinställningslista i dialogrutan **[!UICONTROL URL Encoding for Copy URL Generation]** nedrullningsbar lista längst ned väljer du den URL-kodning som ska användas på bildresursens URL när den kopieras.
1. (Valfritt) I fönstret Bildförinställningslista i det övre högra hörnet av förhandsvisningsrutan väljer du **[!UICONTROL Copy URL]** för den valda förinställningstypen.

   När du väljer **[!UICONTROL Copy URL]**, kopieras den associerade URL:en automatiskt till Urklipp.

1. I det nedre högra hörnet av fönstret Bildförinställningslista väljer du **[!UICONTROL Close]** för att gå tillbaka till skärmen Resurser.
