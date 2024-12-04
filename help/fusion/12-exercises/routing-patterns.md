---
title: Routeringspatronen
description: Verhoog uw concept van het verpletteren en de terugvalroutes zonder eigenlijk andere APIs te behandelen.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11044
thumbnail: KT11044.png
recommendations: noDisplay,catalog
exl-id: d8218115-5180-4e64-8ec1-d2d6afc88d23
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---

# Routeringspatronen

Verhoog uw concept van het verpletteren en de terugvalroutes zonder eigenlijk andere APIs te behandelen.

## Overzicht van oefening

Gebruik de Vastgestelde module van de Variabele om een aantal door veelvoudige wegen te verzenden om te zien hoe de filters en fallbacks zich wanneer het verpletteren gedragen.

![ Verpletterend patronenBeeld 1 ](../12-exercises/assets/routing-patterns-walkthrough-1.png)

## Te volgen stappen

1. Creeer een nieuw scenario en noem het &quot;Verpletterend patronen en fallbacks&quot;.
1. Voeg voor de trigger de module Variabele instellen toe. Zet &quot;Mijn Aantal&quot;voor de naam van de Variabele, verlaat de Veranderlijke levensduur als Één cyclus, en plaats het Variabele gebied aan &quot;75.&quot;

   ![ Verpletterend patroonbeeld 2 ](../12-exercises/assets/routing-patterns-walkthrough-2.png)

1. Voeg een andere module toe en kies de module van de Router. Kies voor beide paden het gereedschap Incrementele functie en klik op OK zonder voor beide paden wijzigingen aan te brengen.

   + Voor de eerste weg, creeer een filter, noem het &quot;minder dan 100,&quot;en plaats de voorwaarde aan [ Mijn Aantal ] minder dan 100.

   + Voor de tweede weg, creeer een filter, noem het &quot;minder dan 1000,&quot;en plaats de voorwaarde aan [ Mijn Aantal ] minder dan 1000. Gebruik de operator Numeriek voor beide.

   ![ Verpletterend patroonbeeld 3 ](../12-exercises/assets/routing-patterns-walkthrough-3.png)

   ![ Verpletterend patroonbeeld 4 ](../12-exercises/assets/routing-patterns-walkthrough-4.png)

1. Klik eenmaal op Uitvoeren en bekijk de bundel het pad &quot;Minder dan 100&quot;.
1. Wijzig vervolgens het veld voor de module Variabele instellen op 950 en voer de bewerking nogmaals uit. Kijk hoe het langs het tweede pad loopt.
1. Klik de router en voeg één meer weg toe. Voeg de het hulpmiddelmodule van de functie van de Toename toe. Klik voor het filter op het selectievakje &quot;De fallback-route&quot;. U ziet hoe de pijl die naar dat pad wijst, verandert in een invoegpunt. Dit geeft aan dat dit de fallbackroute is.

   ![ Verpletterend patroonbeeld 5 ](../12-exercises/assets/routing-patterns-walkthrough-5.png)

1. Wijzig het getal van de variabele Set in 9500 en voer het één keer uit. Omdat het aantal niet minder dan 100 of minder dan 1000 is, reist de bundel door de reserveroute.

Als u nog een pad toevoegt met een module voor het gereedschap Toename maar geen filter instelt, wat gebeurt er dan als u nogmaals op Uitvoeren klikt? Zal een bundel ooit de reserveroute met de vierde toegevoegde route gaan?

+ Nee, omdat zonder filterset elke bundel altijd dit pad omlaag gaat in plaats van de fallback-route.
