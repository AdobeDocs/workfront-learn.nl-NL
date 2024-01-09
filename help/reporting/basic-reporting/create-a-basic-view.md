---
title: Een basisweergave maken
description: Leer wat een mening is, hoe te om een mening tot stand te brengen, en hoe te om een mening met andere gebruikers in Workfront te delen.
activity: use
feature: Reports and Dashboards
thumbnail: 335148.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
last-substantial-update: 2023-06-20T00:00:00Z
jira: KT-8854
exl-id: ba3c0e10-dcf1-4a7b-bf11-ccfed9040e6d
doc-type: video
source-git-commit: d39151288d8b749940c5183063392ee471769445
workflow-type: tm+mt
source-wordcount: '642'
ht-degree: 1%

---

# Een basisweergave maken

In deze video leert u:

* Wat een weergave in Workfront
* Een weergave maken en wijzigen
* Een weergave delen met andere Workfront-gebruikers

>[!VIDEO](https://video.tv.adobe.com/v/335148/?quality=12&learn=on)

## Activiteit 1: Een taakstatusweergave maken

Als projectmanager, teamleider, of middelmanager, wilt u bijhouden hoe het taakwerk vordert. In deze weergave ziet u verschillende statusindicatoren voor een taak, allemaal in één rij van de lijst of het rapport.

Maak een taakweergave met de naam &quot;Taakstatusweergave&quot; met de volgende kolommen:

* [!UICONTROL Task Name]
* [!UICONTROL Assignments]
* [!UICONTROL Duration]
* [!UICONTROL Percent Complete]
* [!UICONTROL Status]
* [!UICONTROL Progress Status]
* [!UICONTROL Status Icons]

## Antwoord op activiteit 1

![Een afbeelding van het scherm om een taakstatusweergave te maken](assets/view-exercise.png)

1. Ga in een rapport van de taaklijst naar **[!UICONTROL View]** vervolgkeuzelijst en selecteert u **[!UICONTROL New View]**.
1. Geef de weergave de naam &#39;Taakstatusweergave&#39;.
1. Deze kolommen verwijderen: [!UICONTROL Pln Hrs], [!UICONTROL Predecessors], [!UICONTROL Start On], en [!UICONTROL Due On].
1. Klik op **[!UICONTROL Add Column]**.
1. In de [!UICONTROL Show in this column] veld, typ &quot;status&quot; en selecteer &quot;status&quot; onder het veld [!UICONTROL Task] veldbron.
1. Klikken **[!UICONTROL Add Column]** opnieuw.
1. In de [!UICONTROL Show in this column] veld, typt u &quot;status&quot; en selecteert u &quot;Voortgangsstatus&quot; onder het [!UICONTROL Task] veldbron.
1. Klikken **[!UICONTROL Add Column]** opnieuw.
1. In de [!UICONTROL Show in this column] veld, typt u &quot;status&quot; en selecteert u &quot;Statuspictogrammen&quot; onder de bron van het taakveld.
1. Klik op **[!UICONTROL Save]**.

Houd de muisaanwijzer boven de pictogrammen in het dialoogvenster [!UICONTROL Status Icons] om te zien wat ze vertegenwoordigen. Als ze grijs zijn, betekent dit dat de taak geen notities, documenten, goedkeuringsprocedures, enzovoort bevat. Als een pictogram in kleur verschijnt, is er minstens één van dat punt verbonden aan de taak. U kunt op de notitie- of documentpictogrammen klikken om naar dat item te gaan.

## Activiteit 2: Een mijlpaalweergave maken

Als u mijlpalen gebruikt, is deze mening de gemakkelijkste manier om mijlpalen door naam te zien en hen toe te voegen of uit te geven gebruikend in-lijn uitgeven.

Maak een taakweergave met de naam &quot;Weergave van mijlpaal&quot; met de volgende kolommen:

* [!UICONTROL Task Name]
* [!UICONTROL Assignments]
* [!UICONTROL Duration]
* [!UICONTROL Pln Hrs]
* [!UICONTROL Milestone: Name]
* [!UICONTROL Start On]
* [!UICONTROL Due On]
* [!UICONTROL Percent Complete]


## Antwoord op activiteit 2

![Een afbeelding van het scherm om een mijlpaalweergave te maken](assets/view-milestone-exercise-1.png)

1. Ga in een lijst met projecttaken naar de **[!UICONTROL View]** vervolgkeuzelijst en selecteert u **[!UICONTROL New View]**.
1. Geef uw weergave de naam &#39;Weergave van mijlpaal&#39;.
1. Klik op de knop [!UICONTROL Predecessors] te selecteren.
1. In de [!UICONTROL Show in this column] veld, klikt u op het X-pictogram in het dialoogvenster [!UICONTROL Task >> Predecessors] veld, typ vervolgens &quot;[!UICONTROL milestone name]&quot; en klik op &quot;[!UICONTROL Name]&quot; in de lijst.
1. Klik op **[!UICONTROL Save]**.

![Een afbeelding van een takenlijst met gebruik van een mijlpaalweergave](assets/view-milestone-exercise-2.png)

## Activiteit 3: Een type duur en een weergave met taakbeperkingen maken

Deze mening zal u toestaan om alle duurtypes en taakbeperkingen in uw project te onderzoeken en uit te geven.

Creeer een taakmening genoemd &quot;de types van Duur en de mening van taakbeperkingen&quot;met de volgende kolommen:

* [!UICONTROL Task Name]
* [!UICONTROL Assignments]
* [!UICONTROL Duration]
* [!UICONTROL Planned Duration]
* [!UICONTROL Pln Hrs]
* [!UICONTROL Predecessors]
* [!UICONTROL Start On]
* [!UICONTROL Due On]
* [!UICONTROL Duration Type]
* [!UICONTROL Task Constraint]
* [!UICONTROL Constraint Date]

Wijzig de [!UICONTROL Field Format] op de [!UICONTROL Start On] en [!UICONTROL Due On] kolommen waarin zowel de datum als de tijd worden weergegeven.

## Activiteit 3 Antwoord

![Een afbeelding van het scherm met de typen tijdsduur en de weergave met taakbeperkingen](assets/view-activity-3.png)

1. Ga in een lijst met projecttaken naar de **[!UICONTROL View]** vervolgkeuzelijst en selecteert u **[!UICONTROL New View]**.
1. Geef de weergave de naam &quot;Weergave Duur en taakbeperkingen&quot;.
1. Verwijder de [!UICONTROL % Complete] kolom.
1. Klik op **[!UICONTROL Add Column]**.
1. In de [!UICONTROL Show in this column] veld, type [!UICONTROL "duration"] Selecteer vervolgens [!UICONTROL "Planned Duration"] onder de [!UICONTROL Task] veldbron.
1. Deze kolom verplaatsen tussen de [!UICONTROL Duration] en de [!UICONTROL Pln Hrs] kolommen.
1. Klikken **[!UICONTROL Add Column]** opnieuw.
1. In de [!UICONTROL Show in this column] veld, type [!UICONTROL "duration type"] Selecteer vervolgens [!UICONTROL "Duration Type"] onder de [!UICONTROL Task] veldbron.
1. Klikken **[!UICONTROL Add Column]** opnieuw.
1. In de [!UICONTROL Show in this column] veld, type [!UICONTROL "constraint"] Selecteer vervolgens [!UICONTROL "Task Constraint"] onder de bron van het het gebiedsveld van de Taak.
1. Klikken **[!UICONTROL Add Column]** opnieuw.
1. In de [!UICONTROL Show in this column] veld, type [!UICONTROL "constraint"] Selecteer vervolgens [!UICONTROL "Constraint Date"] onder de bron van het het gebiedsveld van de Taak.
1. Selecteer de [!UICONTROL Start On] kolom, klik vervolgens op [!UICONTROL Advanced Options].
1. Onder de [!UICONTROL Field Format] vervolgkeuzelijst selecteren [!UICONTROL "10/17/60 3:00 AM"].
1. Selecteer de [!UICONTROL Due On] kolom, klik vervolgens op [!UICONTROL Advanced Options].
1. Onder de [!UICONTROL Field Format] vervolgkeuzelijst selecteren [!UICONTROL "10/17/60 3:00 AM"].
1. Klik op **[!UICONTROL Save]**.

## Activiteit 4: Een actieve statusweergave van een projectsjabloon maken

Iedereen die projectmalplaatjes beheert zal het zien van de actieve status (Waar of Onwaar) van elke malplaatje in een lijst waarderen. Nog beter - het veld is online bewerkbaar!

Creeer een mening van het projectmalplaatje genoemd &quot;Standaard+actieve status&quot;met de volgende kolommen:

* [!UICONTROL Name]
* [!UICONTROL Owner]
* [!UICONTROL Duration]
* [!UICONTROL Planned Hours]
* [!UICONTROL Planned Cost]
* [!UICONTROL Flags]
* [!UICONTROL Group Name]
* [!UICONTROL Is Active]


## Activiteit 4 Antwoord

![Een beeld van het scherm om een actieve de statusmening van het projectmalplaatje te tonen](assets/view-activity-4.png)

1. Ga in een lijst van het projectmalplaatje, naar **[!UICONTROL View]** vervolgkeuzelijst en selecteert u **[!UICONTROL New View]**.
1. Geef de weergave de naam Standaard+actieve status.
1. Klik op **[!UICONTROL Add Column]**.
1. In de [!UICONTROL Show in this column] veld, type &quot;is&quot; en selecteer &quot;Is Actief&quot; onder het veld [!UICONTROL Template] veldbron.
1. Klik op **[!UICONTROL Save View]**.
