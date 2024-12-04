---
title: Buiten de basismapping
description: Leer hoe u met de formules van het deelvenster Toewijzing velden kunt bewerken of converteren die naar een module zijn verzonden.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11039
thumbnail: KT11039.png
recommendations: noDisplay,catalog
exl-id: 979d794d-b936-402e-b07c-71e999f40780
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Buiten de basismapping

Leer hoe u met de formules van het deelvenster Toewijzing velden kunt bewerken of converteren die naar een module zijn verzonden.

## Overzicht van oefening

Verander de projectnaam, de geplande begindatum, en de prioriteit van de Beyond Basis analyse oefeningen gebruikend de formules van het kaartpaneel.

![ voorbij Basis Afbeelding 1 van de Toewijzing ](../12-exercises/assets/beyond-basic-mapping-walkthrough-1.png)

## Te volgen stappen

**maak een kloon van uw Eerste scenario ontwerpscenario.**

1. Selecteer de optie Klonen rechts van het ontwerp van het Eerste scenario in de scenario-sectie, zoals hieronder wordt getoond. Geef deze de naam &quot;Buiten de basistoewijzing&quot;.

   ![ voorbij Basis Afbeelding 2 van de Toewijzing ](../12-exercises/assets/beyond-basic-mapping-walkthrough-2.png)

   **nu gaan wij het mappingpaneel in Create Workfront projectenmodule gebruiken om de projectnaam, geplande begindatum, en prioritaire gebieden te vormen.**

1. Klik op de module Workfront-projecten maken om de instellingen te bewerken. Gebruikend het kaartpaneel, verander het gebied van de Naam om &quot;[ Mijn Naam van het Project ] door [ Sponsor ] te zijn.&quot;

   + [ Mijn Naam van het Project ] is kolom 1 van de Parse module CSV en [ Sponsor ] is kolom 6. Het woord &quot;by&quot; wordt net tussen de twee getypt.

1. Ga daarna naar de Geplande Datum van het Begin en gebruik de formule addDays om 15 dagen aan het gebied toe te voegen, zoals die in de Beyond basiskaartafdrukvideo wordt beschreven.
1. Zoek het veld Prioriteit en schakel de knop Kaart rechtsboven in het veld in. Het keuzemenu verandert in een getal. Maak een if-instructie om een project als High(4)-prioriteit te labelen als de CSV-score voor bestandsvertrouwen lager is dan 100. Als dit niet het geval is, kan dit Normaal(2) zijn.

   + De betrouwbaarheidsscore is opgenomen in kolom 4.

   **op dit punt, zou uw kaartbord als dit moeten kijken:**

   ![ voorbij Basis Afbeelding 3 van de Toewijzing ](../12-exercises/assets/beyond-basic-mapping-walkthrough-3.png)

1. Klik op OK en vervolgens eenmaal op Uitvoeren.
1. Zoek het project in uw Workfront-exemplaar om te controleren of alles correct is toegewezen.
1. Sla uw scenario op.
