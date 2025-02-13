---
title: Basisweergaveactiviteiten maken
description: Praktijk die basismeningen met geleidelijke instructies creeert.
activity: use
feature: Reports and Dashboards
thumbnail: 335148.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
last-substantial-update: 2023-06-20T00:00:00Z
jira: KT-8854
hidefromtoc: true
source-git-commit: 915b28bbbf138fa84dce6d1915387fbe22c63362
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 1%

---

# Basisweergaveactiviteiten maken

Praktijk die basismeningen met geleidelijke instructies creeert.

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

![ een beeld van het scherm om een mening van de taakstatus tot stand te brengen ](assets/view-exercise.png)

1. Ga in een takenlijstrapport naar de vervolgkeuzelijst **[!UICONTROL View]** en selecteer **[!UICONTROL New View]** .
1. Geef de weergave de naam &#39;Taakstatusweergave&#39;.
1. Verwijder de volgende kolommen: [!UICONTROL Pln Hrs], [!UICONTROL Predecessors], [!UICONTROL Start On] en [!UICONTROL Due On] .
1. Klik op **[!UICONTROL Add Column]**.
1. Typ in het veld [!UICONTROL Show in this column] &quot;status&quot; en selecteer &quot;Status&quot; onder de veldbron van [!UICONTROL Task] .
1. Klik nogmaals op **[!UICONTROL Add Column]** .
1. Typ in het veld [!UICONTROL Show in this column] &quot;status&quot; en selecteer &quot;Voortgangsstatus&quot; onder de veldbron van [!UICONTROL Task] .
1. Klik nogmaals op **[!UICONTROL Add Column]** .
1. Typ in het veld [!UICONTROL Show in this column] &quot;status&quot; en selecteer vervolgens &quot;Statuspictogrammen&quot; onder de bron van het taakveld.
1. Klik op **[!UICONTROL Save]**.

Houd de muisaanwijzer boven elk pictogram in de kolom [!UICONTROL Status Icons] om te zien wat de pictogrammen vertegenwoordigen. Als ze grijs zijn, betekent dit dat de taak geen notities, documenten, goedkeuringsprocedures, enzovoort bevat. Als een pictogram in kleur verschijnt, is er minstens één van dat punt verbonden aan de taak. U kunt op de notitie- of documentpictogrammen klikken om naar dat item te gaan.

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

![ een beeld van het scherm om een milestone mening ](assets/view-milestone-exercise-1.png) te creëren

1. Ga in een lijst met projecttaken naar de vervolgkeuzelijst **[!UICONTROL View]** en selecteer **[!UICONTROL New View]** .
1. Geef uw weergave de naam &#39;Weergave van mijlpaal&#39;.
1. Klik op de kolom [!UICONTROL Predecessors] om deze te selecteren.
1. Klik in het veld [!UICONTROL Show in this column] op het X-pictogram in het veld [!UICONTROL Task >> Predecessors] , typ &quot;[!UICONTROL milestone name]&quot; en klik op &quot;[!UICONTROL Name]&quot; in de lijst.
1. Klik op **[!UICONTROL Save]**.

![ een beeld van een taaklijst gebruikend een milestone mening ](assets/view-milestone-exercise-2.png)

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

Wijzig [!UICONTROL Field Format] in de kolommen [!UICONTROL Start On] en [!UICONTROL Due On] om zowel de datum als de tijd weer te geven.

## Activiteit 3 Antwoord

![ een beeld van het scherm dat de duurtypes en de mening van taakbeperkingen toont ](assets/view-activity-3.png)

1. Ga in een lijst met projecttaken naar de vervolgkeuzelijst **[!UICONTROL View]** en selecteer **[!UICONTROL New View]** .
1. Geef de weergave de naam &quot;Weergave Duur en taakbeperkingen&quot;.
1. Verwijder de kolom [!UICONTROL % Complete] .
1. Klik op **[!UICONTROL Add Column]**.
1. Typ in het veld [!UICONTROL Show in this column] [!UICONTROL "duration"] en selecteer [!UICONTROL "Planned Duration"] onder de veldbron van [!UICONTROL Task] .
1. Verplaats deze kolom tussen de kolommen [!UICONTROL Duration] en [!UICONTROL Pln Hrs] .
1. Klik nogmaals op **[!UICONTROL Add Column]** .
1. Typ in het veld [!UICONTROL Show in this column] [!UICONTROL "duration type"] en selecteer [!UICONTROL "Duration Type"] onder de veldbron van [!UICONTROL Task] .
1. Klik nogmaals op **[!UICONTROL Add Column]** .
1. Typ in het veld [!UICONTROL Show in this column] [!UICONTROL "constraint"] en selecteer [!UICONTROL "Task Constraint"] onder de bron van het taakveld.
1. Klik nogmaals op **[!UICONTROL Add Column]** .
1. Typ in het veld [!UICONTROL Show in this column] [!UICONTROL "constraint"] en selecteer [!UICONTROL "Constraint Date"] onder de bron van het taakveld.
1. Selecteer de kolom [!UICONTROL Start On] en klik op [!UICONTROL Advanced Options] .
1. Selecteer onder de vervolgkeuzelijst [!UICONTROL Field Format] de optie [!UICONTROL "10/17/60 3:00 AM"] .
1. Selecteer de kolom [!UICONTROL Due On] en klik op [!UICONTROL Advanced Options] .
1. Selecteer onder de vervolgkeuzelijst [!UICONTROL Field Format] de optie [!UICONTROL "10/17/60 3:00 AM"] .
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

![ een beeld van het scherm om een actieve de statusmening van het projectmalplaatje te tonen ](assets/view-activity-4.png)

1. Ga in een lijst met projectsjablonen naar de vervolgkeuzelijst **[!UICONTROL View]** en selecteer **[!UICONTROL New View]** .
1. Geef de weergave de naam Standaard+actieve status.
1. Klik op **[!UICONTROL Add Column]**.
1. Typ in het veld [!UICONTROL Show in this column] &quot;is&quot; en selecteer &quot;Is actief&quot; onder de veldbron van [!UICONTROL Template] .
1. Klik op **[!UICONTROL Save View]**.
