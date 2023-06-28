---
title: Rapporten maken met grafieken
description: Leer hoe grafieken de visualisatie van gegevens kunnen verbeteren en hoe u grafiekgereedschappen kunt gebruiken in Workfront.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
jira: KT-8860
exl-id: ea3b360b-1fbd-4d1a-b505-b75759d24e41
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Rapporten maken met grafieken

In deze video leert u:

* Hoe grafieken de visualisatie van gegevens kunnen verbeteren
* Workfront-grafiekgereedschappen gebruiken

>[!VIDEO](https://video.tv.adobe.com/v/335155/?quality=12&learn=on)

## Activiteit: Een diagram toevoegen aan een rapport

Het einde van het kwartaal nadert en u wilt zien hoe recent voltooide projecten zich aan hun budget hebben gekleed. Maak een rapport met de geplande kosten ten opzichte van de werkelijke kosten voor projecten. U wilt alleen projecten zien die in het laatste kwartaal zijn voltooid. Voeg een kleurengrafiek van de combinatiekolom toe gebruikend douanekleuren.

## Antwoord

1. Selecteren **[!UICONTROL Reports]** van de **[!UICONTROL Main Menu]**.
1. Klik op de knop **[!UICONTROL New Report]** en selecteert u **[!UICONTROL Project]**.
1. In de **[!UICONTROL Columns (View)]** tabblad, klikt u op **[!UICONTROL Add Column]**.
1. Selecteren [!UICONTROL Project] > [!UICONTROL Planned Cost] en vat deze kolom samen met **[!UICONTROL Sum]**.
1. Klikken **[!UICONTROL Add Column]** opnieuw.
1. Selecteren [!UICONTROL Project] > [!UICONTROL Actual Cost] en vat deze kolom samen met **[!UICONTROL Sum]**.

   ![Een beeld van het scherm om kolommen aan een rapport toe te voegen](assets/chart-report-columns.png)

1. In de **[!UICONTROL Groupings]** tab, stel het rapport in op groeperen op [!UICONTROL Project] > [!UICONTROL Name].

   ![Een beeld van het scherm om groepen aan een rapport toe te voegen](assets/chart-report-groupings.png)

1. In de **[!UICONTROL Filters]** twee filterregels toevoegen:

   * [!UICONTROL Project] > [!UICONTROL Status Equates With] > [!UICONTROL Complete]
   * [!UICONTROL Project] >[!UICONTROL  Actual Completion Date] > [!UICONTROL Last Quarter]

   ![Een afbeelding van het scherm om filters toe te voegen aan een rapport](assets/chart-report-filters.png)

1. In de **[!UICONTROL Chart]** tab, kiest u **[!UICONTROL Column]** voor het diagramtype.
1. Voor de [!UICONTROL Left (Y) Axis]kiest u [!UICONTROL Project] > [!UICONTROL Planned Cost].
1. Voor de [!UICONTROL Bottom (X) Axis]kiest u [!UICONTROL Project] > [!UICONTROL Name].
1. Klik op de knop **[!UICONTROL Combination Chart]** en selecteert u [!UICONTROL Project] > [!UICONTROL Actual Cost] in de **[!UICONTROL Value]** veld.
1. Klik op de pijl naast het kleurvak om het dialoogvenster [!UICONTROL Actual Cost] kleur. Selecteer een van de kleuren die wordt weergegeven of klik op het vak in de rechterbenedenhoek om het kleurenpalet weer te geven.
1. Klikken op **[!UICONTROL Save + Close]**. Wanneer ertoe aangezet voor een rapportnaam, noem het &quot;Gepland vs Ware Kosten door Project Voltooid Laatste Kwartaal.&quot;

   ![Een beeld van het scherm om een grafiek aan een rapport toe te voegen](assets/chart-report-chart.png)
