---
title: Geavanceerde samenvoeging
description: Begrijp hoe te om groeperingen te gebruiken wanneer het groeperen. (Moet tussen 60 en 160 tekens lang zijn, maar is 49 tekens)
feature: Workfront Fusion
role: User
level: Beginner
kt: 11048
thumbnail: KT11048.png
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---


# Geavanceerde samenvoeging

Begrijp hoe te om groeperingen te gebruiken wanneer het groeperen.

## Overzicht van oefening

Bel een webservice om details over meerdere landen te retourneren en de totale bevolking van alle landen, gegroepeerd per subregio, te identificeren.

![Geavanceerd aggregatieafbeelding 1](../12-exercises/assets/advanced-aggregation-walkthrough-1.png)

## Te volgen stappen

**Haal de gegevens van het land op.**

![Geavanceerde samenvoegingsafbeelding 2](../12-exercises/assets/advanced-aggregation-walkthrough-2.png)

1. Creeer een nieuw scenario en noem het &quot;Geavanceerde samenvoeging.&quot;
1. Stel de triggermodule in op HTTP - Een aanvraagmodule maken.
1. Gebruik deze URL, https://restcountries.eu/rest/v2/ lang/es, die u een lijst van alle landen geeft waar Spaans wordt gesproken.
1. Laat de methode staan als Ophalen.
1. Klik op het selectievakje Reactie pareren.
1. Wijzig de naam van deze module &#39;Landen ophalen&#39;.
1. Klik eenmaal op Opslaan en Uitvoeren.

   **De output is één bundel, maar het komt in een serie met 24 inzamelingen, één voor elk Spaans sprekend land.**

   ![Geavanceerde samenvoeging van afbeelding 3](../12-exercises/assets/advanced-aggregation-walkthrough-3.png)

   **U moet subregio informatie voor elk van de landen verzamelen, zodat zult u een extra HTTP- verzoek moeten doen.**

1. Voeg een ander verzoek toe om subregioinformatie te krijgen. Het zal alleen het eerste land terugsturen, maar dat is nu OK. Voeg nog een HTTP Make een request module toe en gebruik de URL https://restcountries.eu/rest/v2/name/.
1. Als u de naam van het eerste land wilt ophalen, gaat u naar het deelvenster Toewijzing en klikt u op Gegevens. Vervolgens geeft u een naam op in de array. De [1] in het gegevensveld betekent dit dat het eerste item in de array wordt geretourneerd.

   + Klik op het nummer en wijzig de index indien nodig, maar in dit geval wilt u alleen het eerste item.

   ![Geavanceerde samenvoegingsafbeelding 4](../12-exercises/assets/advanced-aggregation-walkthrough-4.png)

1. Controleer het antwoord Parsen in het deelvenster Toewijzing en klik op OK.
1. Wijzig de naam &quot;Landgegevens ophalen&quot;.
1. Klik op Opslaan en voer vervolgens één keer uit.

   + De output is informatie voor één enkel land.

1. Om de andere landen te krijgen, moet je de array doorlopen. Voeg een iterator toe, die een lijst van dingen neemt en een bundel voor elk punt op de lijst uitvoert.

   **Voeg de iterator en aggregator toe.**

1. Klik met de rechtermuisknop tussen de HTTP-modules en voeg de Iterator Flow Control-module toe.
1. Selecteer in het veld Array de optie Gegevens in de module Landen ophalen.

   ![Geavanceerde samenvoegingsafbeelding 5](../12-exercises/assets/advanced-aggregation-walkthrough-5.png)

1. In de Get module van de Details van het Land, werk het gebied URL bij om het naamgebied van de iterator in plaats van van van de Get module van Landen te nemen.

   ![Geavanceerde samenvoegingsafbeelding 6](../12-exercises/assets/advanced-aggregation-walkthrough-6.png)

1. Voeg nu een numerieke aggregator toe na Get Country Details om de populaties te groeperen en samen te tellen.
1. De bronmodule is de iteratormodule.
1. De statistische functie is SUM.
1. De waarde is [gegevens:populatie] in de module Landdetails ophalen.
1. Klik op de optie Geavanceerde instellingen tonen onder aan en groep op [gegevens:subregio] in de module Landdetails ophalen.

   ![Geavanceerde samenvoegingsafbeelding 7](../12-exercises/assets/advanced-aggregation-walkthrough-7.png)

   **Voltooi de bewerking met een tekstaggregator om te verzamelen wat u binnen de numerieke aggregator hebt gegroepeerd.**

1. Voeg een tekstaggregator aan het eind toe.
1. De bronmodule is de numerieke aggregator.
1. In het tekstgebied invoegen: &quot;De totale populatie van [SLEUTEL] is [resultaat].&quot;

   ![Geavanceerde samenvoegingsafbeelding 8](../12-exercises/assets/advanced-aggregation-walkthrough-8.png)

1. Sla het bestand op en voer het één keer uit.

   + Controleer de uitvoer uit de uiteindelijke module.
