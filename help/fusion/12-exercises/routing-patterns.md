---
title: Routeringspatronen
description: Verhoog uw concept van het verpletteren en de terugvalroutes zonder eigenlijk andere APIs te behandelen.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11044
thumbnail: KT11044.png
source-git-commit: 8e07cde38ca939542a03dda2b520c90d1e3b5394
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Routeringspatronen

Verhoog uw concept van het verpletteren en de terugvalroutes zonder eigenlijk andere APIs te behandelen.

## Overzicht van oefening

Gebruik de Vastgestelde module van de Variabele om een aantal door veelvoudige wegen te verzenden om te zien hoe de filters en fallbacks zich wanneer het verpletteren gedragen.

![Patronen routeren, afbeelding 1](../12-exercises/assets/routing-patterns-walkthrough-1.png)

## Te volgen stappen

1. Creeer een nieuw scenario en noem het &quot;Verpletterend patronen en fallbacks&quot;.
1. Voeg voor de trigger de module Variabele instellen toe. Zet &quot;Mijn Aantal&quot;voor de naam van de Variabele, verlaat het leven van de Variabele als Één cyclus, en plaats het gebied van de Variabele aan &quot;75.&quot;

   ![Patroonpatroon, afbeelding 2](../12-exercises/assets/routing-patterns-walkthrough-2.png)

1. Voeg een andere module toe en kies de module van de Router. Kies voor beide paden het gereedschap Incrementele functie en klik op OK zonder voor beide paden wijzigingen aan te brengen.

   + Voor het eerste pad maakt u een filter, geeft u dit de naam &quot;Minder dan 100&quot; en stelt u de voorwaarde in op [Mijn nummer] Minder dan 100.

   + Voor het tweede pad maakt u een filter, geeft u dit de naam &quot;Minder dan 1000&quot; en stelt u de voorwaarde in op [Mijn nummer] Minder dan 1000. Gebruik de operator Numeriek voor beide.

   ![Patronen routeren, afbeelding 3](../12-exercises/assets/routing-patterns-walkthrough-3.png)

   ![Patronen routeren, afbeelding 4](../12-exercises/assets/routing-patterns-walkthrough-4.png)

1. Klik eenmaal op Uitvoeren en bekijk de bundel het pad &quot;Minder dan 100&quot;.
1. Wijzig vervolgens het veld voor de module Variabele instellen op 950 en voer de bewerking nogmaals uit. Kijk hoe het langs het tweede pad loopt.
1. Klik de router en voeg één meer weg toe. Voeg de het hulpmiddelmodule van de functie van de Toename toe. Klik voor het filter op het selectievakje &quot;De fallback-route&quot;. U ziet hoe de pijl die naar dat pad wijst, verandert in een invoegpunt. Dit geeft aan dat dit de fallbackroute is.

   ![Routeringspatronen, afbeelding 5](../12-exercises/assets/routing-patterns-walkthrough-5.png)

1. Wijzig het getal van de variabele Set in 9500 en voer het één keer uit. Omdat het aantal niet minder dan 100 of minder dan 1000 is, reist de bundel door de reserveroute.

Als u nog een pad toevoegt met een module voor het gereedschap Toename maar geen filter instelt, wat gebeurt er dan als u nogmaals op Uitvoeren klikt? Zal een bundel ooit de reserveroute met de vierde toegevoegde route gaan?

+ Nee, omdat zonder filterset elke bundel altijd dit pad omlaag gaat in plaats van de fallback-route.
