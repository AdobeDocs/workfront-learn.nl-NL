---
title: Inleiding tot iteratoroefening
description: Leer hoe u apps van het type iteratie gebruikt en acties uitvoert op elke bundel van informatie.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11046
thumbnail: KT11046.png
exl-id: 8d751885-372a-4716-9542-079cc3d36caf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Inleiding tot iterators

Leer hoe u apps van het type iteratie gebruikt en acties uitvoert op elke bundel van informatie.

## Overzicht van oefening

Kijk naar een specifiek project in Workfront en bekijk dan alle taken binnen dat project. U zult de module van het verhogingshulpmiddel gebruiken om het aantal taken binnen het project te tellen. Tot slot zult u de Vastgestelde veranderlijke module gebruiken om het Aantal Kinderen van het Aantal Open Kwesties af te trekken om een numerieke waarde voor elk van de taakbundels te produceren.

![Inleiding tot iterators Image 1](../12-exercises/assets/introduction-to-iterators-walkthrough-1.png)

## Te volgen stappen

**Lees een project en verwante taken.**

1. Start een nieuw scenario. Noem het &quot;Inleiding aan herhaling.&quot;
1. Kies Workfront als de triggermodule. Een record lezen.
1. Kies Project bij Recordtype.
1. Kies Id, Naam en Beschrijving voor Output.
1. Op het gebied van identiteitskaart, zet projectidentiteitskaart van het project van ExhibitorsBooth van Northstar project van uw de testaandrijvingsinstantie van Workfront.
1. Wijzig de naam van deze module &#39;WF-projecten zoeken&#39;.
1. Voeg een andere Workfront-module toe om de taken met betrekking tot dit project te lezen. Kies de module Verwante records lezen.
1. Kies Project bij Recordtype.
1. Kies voor de bovenliggende record-id de id in de module Een record lezen.
1. Selecteer Taken bij Verzamelingen.
1. Selecteer voor Output de optie Id, Naam, Beschrijving, Aantal onderliggende items, Aantal geopende problemen en Werk.
1. Wijzig de naam van deze module &quot;De Taken van het Project lezen.&quot;
1. Sla het scenario op en klik vervolgens eenmaal op Uitvoeren om de uitvoer weer te geven.

   + Klik op de uitvoeringcontrole en u ziet één bundel als input (het project) en 28 bundels als output (de taken).

   **Telling- en procesherhaalde bundels.**

1. Voeg een andere module toe na Gelezen Verwante Verslagen. Kies een module voor de knoppen voor de functie Toename.

   + Laat het veld Een waarde opnieuw instellen op Nooit staan en klik op OK.

1. Wijzig de naam van deze module &quot;Aantal taken&quot;.
1. Voeg een module voor de variabele Set toe. Stel de naam van de variabele in op Willekeurig pad.
1. Trek in het veld Waarde variabele het aantal open onderliggende items af van het aantal open opTasks.

   **Het moet er als volgt uitzien:**

   ![Inleiding tot iterators Image 2](../12-exercises/assets/introduction-to-iterators-walkthrough-2.png)

1. Wijzig de naam van deze module Willekeurige wiskunde.
1. Sla het scenario op en klik eenmaal op Uitvoeren.

Workfront Fusion heeft 28 uitvoeringen uitgevoerd voor elk van de taken die door de module Read Related Records iterator zijn geproduceerd. Deze 28 bundels zullen door het scenario verder worden verwerkt tenzij een aggregator wordt toegevoegd om de lijn te sluiten.
