---
title: Filteroefening
description: Leer hoe u het filter tussen modules gebruikt om alleen bepaalde typen bundels mogelijk te maken.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11040
thumbnail: KT1101.png
recommendations: noDisplay,catalog
exl-id: d2cec1ea-7ff9-48ae-8bfb-0c767d346079
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# Filteroefening

Leer hoe u het filter tussen modules gebruikt om alleen bepaalde typen bundels mogelijk te maken.

## Overzicht van oefening

Voeg een filter tussen de twee modules in het Buiten basistoewijzingsscenario toe om slechts projecten tot stand te brengen die een &quot;Rode&quot;projectkleur in het Csv- dossier hebben.

![&#x200B; het Beeld van Filters 1 &#x200B;](../12-exercises/assets/filters-walkthrough-1.png)

## Te volgen stappen

1. Maak een kloon van het scenario &quot;Buiten de basistoewijzing&quot; en noem dit scenario &quot;Het filter Mengheid gebruiken&quot;.

   **voeg een filter vóór Create Workfront projectenmodule toe om rode projecten slechts toe te staan om worden gecreeerd.**

   ![&#x200B; het Beeld van Filters 2 &#x200B;](../12-exercises/assets/filters-walkthrough-2.png)

1. Voeg een filter toe door op de stippellijn te klikken die de modules verbindt of door op de moersleutel te klikken en een filter instellen te selecteren.
1. Gebruik het veld Label om het filter Alleen rode projecten een naam te geven.
1. Wijs in het veld Voorwaarde het veld Projectkleur toe (kolom 3 in het CSV-bestand). Selecteer de operator Gelijk aan (hoofdlettergevoelig) en typ vervolgens &quot;rood&quot;.
1. Klik op OK.

   ![&#x200B; Beeld 3 van Filters &#x200B;](../12-exercises/assets/filters-walkthrough-3.png)

   **Test de filter en verifieer de resultaten.**

1. Klik op Opslaan om het scenario op te slaan en vervolgens eenmaal uit te voeren.
1. Klik op de uitvoeringscontrole voor het filter om te zien hoe elke bundel door het filter is gecontroleerd en of deze al dan niet is doorgegeven aan de module Workfront-projecten maken.

   ![&#x200B; Beeld 4 van Filters &#x200B;](../12-exercises/assets/filters-walkthrough-4.png)

1. Zoek de projecten die in uw Workfront-exemplaar zijn gemaakt.
