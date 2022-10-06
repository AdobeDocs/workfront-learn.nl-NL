---
title: Filters
description: Leer hoe u het filter tussen modules gebruikt om alleen bepaalde typen bundels mogelijk te maken.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11040
thumbnail: KT1101.png
source-git-commit: f367e016498d5c1814cab79e19e6e9001db2851f
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---


# Filters

Leer hoe u het filter tussen modules gebruikt om alleen bepaalde typen bundels mogelijk te maken.

## Overzicht van oefening

Voeg een filter tussen de twee modules in het Buiten basistoewijzingsscenario toe om slechts projecten tot stand te brengen die een &quot;Rode&quot;projectkleur in het Csv- dossier hebben.

![Filterafbeelding 1](../12-exercises/assets/filters-walkthrough-1.png)

## Te volgen stappen

1. Maak een kloon van het scenario &quot;Buiten de basistoewijzing&quot; en noem dit scenario &quot;Het filter Mengheid gebruiken&quot;.

   **Voeg een filter toe vóór de module Workfront-projecten maken om alleen rode projecten te maken.**

   ![Filterafbeelding 2](../12-exercises/assets/filters-walkthrough-2.png)

1. Voeg een filter toe door op de stippellijn te klikken die de modules verbindt of door op de moersleutel te klikken en een filter instellen te selecteren.
1. Gebruik het veld Label om het filter Alleen rode projecten een naam te geven.
1. Wijs in het veld Voorwaarde het veld Projectkleur toe (kolom 3 in het CSV-bestand). Selecteer de operator Gelijk aan (hoofdlettergevoelig) en typ vervolgens &quot;rood&quot;.
1. Klik op OK.

   ![Filterafbeelding 3](../12-exercises/assets/filters-walkthrough-3.png)

   **Test het filter en controleer de resultaten.**

1. Klik op Opslaan om het scenario op te slaan en vervolgens eenmaal uit te voeren.
1. Klik op de uitvoeringscontrole voor het filter om te zien hoe elke bundel door het filter is gecontroleerd en of deze al dan niet is doorgegeven aan de module Workfront-projecten maken.

   ![Filterafbeelding 4](../12-exercises/assets/filters-walkthrough-4.png)

1. Zoek de projecten die in uw Workfront-exemplaar zijn gemaakt.
