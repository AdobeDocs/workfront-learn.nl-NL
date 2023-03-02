---
title: Een matrixrapport maken
description: Leer wanneer een matrixrapport nuttig kan zijn en hoe te om een matrixrapport in Workfront tot stand te brengen.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
kt: 8861
exl-id: e893d94a-e808-4bc1-bc6e-f46a5582b55d
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Een matrixrapport maken

In deze video leert u:

* Wanneer een matrixrapport nuttig kan zijn
* En hoe te om een matrixrapport te creëren

>[!VIDEO](https://video.tv.adobe.com/v/335156/?quality=12)

## Activiteit: Een matrixrapport maken

Creeer een matrixrapport dat toont hoeveel verzoeken er in elke status zijn, die door verzoekrij wordt gesorteerd. Zo krijgt u een snel overzicht van de hoeveelheid werk die binnenkomt en hoe goed u het bijhoudt.

U wilt dat de aanvraagrijen op de rijgroepen verschijnen. De status wordt weergegeven als kolomgroepen. Geef uw rapport de naam &quot;Verzoeken op status en Wachtrij aanvragen&quot;.

## Antwoord

1. Selecteren **[!UICONTROL Reports]** van de **[!UICONTROL Main Menu]**.
1. Klik op de knop **[!UICONTROL New Report]** en selecteert u **[!UICONTROL Issue]**.
1. Ga naar de **[!UICONTROL Groupings]** en klik op **[!UICONTROL Switch to Matrix Grouping]**.
1. Voor [!UICONTROL Row Groupings], selecteert u **[!UICONTROL Project]** > **[!UICONTROL Name]**.
1. Voor [!UICONTROL Column Grouping], selecteert u **[!UICONTROL Issue]** > **[!UICONTROL Status]**.

   ![Een beeld van het scherm om een nieuw punt tot stand te brengen rapporteert groepering](assets/matrix-report-groupings.png)

1. Ga naar de **[!UICONTROL Filters]** tab.
1. Om ervoor te zorgen u slechts verzoeken in actieve verzoekrijen ziet, voeg de volgende filterregels toe:

   * [!UICONTROL Project] > [!UICONTROL Status Equates With] > [!UICONTROL Equal] > [!UICONTROL Current]
   * [!UICONTROL Queue Definition] > [!UICONTROL Is Public] > [!UICONTROL Not Equal] > [!UICONTROL None] (Dit is hoe wij weten een project eigenlijk een verzoekrij is, door de Definitie van de Rij die aan één van de openbare opties wordt toegewezen.)

1. Klikken op **[!UICONTROL Save + Close]**. Wanneer ertoe aangezet voor een rapportnaam, typ in &quot;Verzoeken door Status en de Rij van het Verzoek.&quot;

   ![Een beeld van het scherm om een nieuw filter van het uitgifterapport tot stand te brengen](assets/matrix-report-filters.png)
