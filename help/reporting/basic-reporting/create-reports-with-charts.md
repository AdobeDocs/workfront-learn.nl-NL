---
title: Rapporten maken met grafieken
description: Grafieken verbeteren de gegevensvisualisatie door gegevensinzichten door klantgerichte filters, groeperingen, en gestapelde kolomformaten te organiseren, die analyse helderder en actiever maken.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
jira: KT-8860
last-substantial-update: 2025-05-06T00:00:00Z
exl-id: ea3b360b-1fbd-4d1a-b505-b75759d24e41
doc-type: video
source-git-commit: 1fafcafb173ceb4115612e1c33ca36564c7a6c3d
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 0%

---

# Rapporten maken met grafieken

De video legt uit hoe u grafieken kunt gebruiken om gegevens effectief te visualiseren, met name voor het bijhouden van projecttaken. &#x200B; Het toont het creëren van twee soorten rapporten in Workfront:

**Late Taken door het Rapport van het Project:**

* Begin met een lijstrapport en pas filters toe om slechts onvolledige, late taken in huidige projecten te tonen. &#x200B;
* Groepeer taken door projectnaam en creeer een cirkeldiagram om de distributie van late taken over projecten te visualiseren. &#x200B;
* Plaats de grafiek als standaardlusje voor gemakkelijke toegang. &#x200B;

**Taken door het Rapport van de Status van het Project en van de Voortgang:**

* Kopieer het eerste rapport en voeg een andere groepering voor de status van de taakvooruitgang toe.
* Verwijder filters om alle taken te omvatten, tonend hun vooruitgang tijdens projectuitvoering.
* Gebruik een gestapelde kolomgrafiek om het totale aantal taken per project, met stapels te tonen die verschillende vooruitgangsstatussen vertegenwoordigen.
* Pas indien nodig kleuren aan en sla het rapport op.

In de video wordt benadrukt hoe diagrammen als taart en gestapelde kolomgrafieken inzicht kunnen verschaffen in taakdistributie en projectprestaties, waardoor gebruikers projecten kunnen vergelijken en de taakvoortgang visueel kunnen begrijpen. &#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/335155/?quality=12&learn=on)

## Toetsen

* **de Grafieken verbeteren de Duidelijkheid van Gegevens**: Het visualiseren van gegevens met grafieken, zoals taart of kolomgrafieken, maakt het gemakkelijker om taakdistributie en projectvooruitgang te begrijpen in vergelijking met lijstrapporten. &#x200B;
* **Filtrerend voor Specifieke Inzichten**: Het toepassen van filters (b.v., onvolledige, late taken in huidige projecten) helpt zich op relevante gegevens voor gerichte analyse concentreren. &#x200B;
* **Groepering voor Betere Organisatie**: Het groeperen van taken door projectnaam of vooruitgangsstatus organiseert effectief gegevens, toelatend zinvolle vergelijkingen over projecten. &#x200B;
* **de Opties van de Aanpassing van de Grafiek**: De gebruikers kunnen grafiektypes (b.v., taart, kolom, bar) selecteren en kleuren aanpassen om met voorkeur of branding te richten. &#x200B;
* **gestapelde Grafieken van de Kolom voor Gedetailleerde Inzichten**: De gestapelde kolomgrafieken verstrekken een uitvoerige mening van taakvooruitgang binnen projecten, die zowel totale taken als hun status in één enkele visualisatie tonen.


## &quot;Rapporten maken met grafieken&quot;-activiteiten

### Activiteit 1: Een grafiek toevoegen aan een rapport

Het einde van het kwartaal nadert en u wilt zien hoe recent voltooide projecten zich aan hun budget hebben gekleed. Maak een rapport met de geplande kosten ten opzichte van de werkelijke kosten voor projecten. U wilt alleen projecten zien die in het laatste kwartaal zijn voltooid. Voeg een kleurengrafiek van de combinatiekolom toe gebruikend douanekleuren.

### Antwoord 1

1. Selecteer **[!UICONTROL Reports]** in het menu **[!UICONTROL Main Menu]** .
1. Klik op het menu **[!UICONTROL New Report]** en selecteer **[!UICONTROL Project]** .
1. Klik op het tabblad **[!UICONTROL Columns (View)]** op **[!UICONTROL Add Column]** .
1. Selecteer [!UICONTROL Project] > [!UICONTROL Planned Cost] en vat deze kolom samen met **[!UICONTROL Sum]** .
1. Klik nogmaals op **[!UICONTROL Add Column]** .
1. Selecteer [!UICONTROL Project] > [!UICONTROL Actual Cost] en vat deze kolom samen met **[!UICONTROL Sum]** .

   ![ een beeld van het scherm om kolommen aan een rapport toe te voegen ](assets/chart-report-columns.png)

1. Stel op het tabblad **[!UICONTROL Groupings]** het rapport in op groeperen met [!UICONTROL Project] > [!UICONTROL Name] .

   ![ een beeld van het scherm om groeperingen aan een rapport toe te voegen ](assets/chart-report-groupings.png)

1. Voeg op het tabblad **[!UICONTROL Filters]** twee filterregels toe:

   * [!UICONTROL Project] > [!UICONTROL Status Equates With] > [!UICONTROL Complete]
   * [!UICONTROL Project] >[!UICONTROL  Actual Completion Date] > [!UICONTROL Last Quarter]

   ![ een beeld van het scherm om filters aan een rapport toe te voegen ](assets/chart-report-filters.png)

1. Kies op het tabblad **[!UICONTROL Chart]** de optie **[!UICONTROL Column]** voor het diagramtype.
1. Kies [!UICONTROL Left (Y) Axis] bij [!UICONTROL Planned Cost] .
1. Kies [!UICONTROL Bottom (X) Axis] bij [!UICONTROL Name] .
1. Klik op de knop **[!UICONTROL Combination Chart]** en selecteer [!UICONTROL Actual Cost] in het veld **[!UICONTROL Value]** .
1. Selecteer Regel in het veld **[!UICONTROL Chart Type]** .
1. Klik op het kleurvak om de [!UICONTROL Actual Cost] -kleur te wijzigen. Selecteer een kleur.
1. Klik op **[!UICONTROL Save + Close]** . Wanneer ertoe aangezet voor een rapportnaam, noem het &quot;Gepland vs Ware Kosten door Project Voltooid Laatste Kwartaal.&quot;

   ![ een beeld van het scherm om een grafiek aan een rapport toe te voegen ](assets/chart-report-chart.png)
