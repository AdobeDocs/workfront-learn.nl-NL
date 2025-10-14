---
title: Geavanceerde samenvoeging
description: Roep een webservice aan om details over meerdere landen te retourneren en om de bevolking te identificeren, gegroepeerd per subregio.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11048
thumbnail: KT11048.png
recommendations: noDisplay,catalog
exl-id: 5364befa-491d-4b75-b1f0-10244f70ad7c
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Geavanceerde samenvoeging

Begrijp hoe te om groeperingen te gebruiken wanneer het groeperen.

## Overzicht van oefening

Bel een webservice om details over meerdere landen te retourneren en de totale bevolking van alle landen, gegroepeerd per subregio, te identificeren.

![&#x200B; Geavanceerde Beeld van de Samenvoeging 1 &#x200B;](../12-exercises/assets/advanced-aggregation-walkthrough-1.png)

## Te volgen stappen

**krijgt landdetails.**

![&#x200B; Geavanceerde Beeld van de Samenvoeging 2 &#x200B;](../12-exercises/assets/advanced-aggregation-walkthrough-2.png)

1. Creeer een nieuw scenario en noem het &quot;Geavanceerde samenvoeging.&quot;
1. Stel de triggermodule in op HTTP - Een aanvraagmodule maken.
1. Gebruik deze URL, `https://restcountries.com/v2/lang/es` , die u een lijst van alle landen geeft waar Spaans wordt gesproken.
1. Laat de methode staan als Ophalen.
1. Klik op het selectievakje Reactie pareren.
1. Wijzig de naam van deze module &#39;Landen ophalen&#39;.
1. Klik eenmaal op Opslaan en Uitvoeren.

   **de output is één enkele bundel, maar het komt in een serie met 24 inzamelingen, voor elk Spaans sprekend land.**

   ![&#x200B; Geavanceerde Beeld 3 van de Samenvoeging &#x200B;](../12-exercises/assets/advanced-aggregation-walkthrough-3.png)

   **u moet subregion informatie voor elk van de landen verzamelen, zodat zult u een extra verzoek van HTTP moeten maken.**

1. Voeg een ander verzoek toe om subregioinformatie te krijgen. Het zal alleen het eerste land terugsturen, maar dat is nu OK. Voeg nog een HTTP Make een request module toe en gebruik de URL `https://restcountries.com/v2/name/{country name}` .
1. Als u de naam van het eerste land wilt ophalen, gaat u naar het deelvenster Toewijzing en klikt u op Gegevens. Vervolgens geeft u een naam op in de array. [ 1 ] op het gegevensgebied betekent het het eerste punt in de serie zal terugkeren.

   + Klik op het nummer en wijzig de index indien nodig, maar in dit geval wilt u alleen het eerste item.

![&#x200B; Geavanceerde Beeld 4 van de Samenvoeging &#x200B;](../12-exercises/assets/advanced-aggregation-walkthrough-4.png)

1. Controleer het antwoord Parsen in het deelvenster Toewijzing en klik op OK.
1. Wijzig de naam &quot;Landgegevens ophalen&quot;.
1. Klik op Opslaan en vervolgens eenmaal uitvoeren.

   + De output is informatie voor één enkel land.

1. Om de andere landen te krijgen, moet je de array doorlopen. Voeg een iterator toe, die een lijst van dingen neemt en een bundel voor elk punt op de lijst uitvoert.

   **voeg iterator en aggregator toe.**

1. Klik met de rechtermuisknop tussen de HTTP-modules en voeg de Iterator Flow Control-module toe.
1. Selecteer in het veld Array de optie Gegevens in de module Landen ophalen.

   ![&#x200B; Geavanceerde Beeld van de Samenvoeging 5 &#x200B;](../12-exercises/assets/advanced-aggregation-walkthrough-5.png)

1. In de Get module van de Details van het Land, werk het gebied URL bij om het naamgebied van de iterator in plaats van van van de Get module van Landen te nemen.

   ![&#x200B; Geavanceerde Beeld 6 van de Samenvoeging &#x200B;](../12-exercises/assets/advanced-aggregation-walkthrough-6.png)

1. Voeg nu een numerieke aggregator toe na Get Country Details om de populaties te groeperen en samen te tellen.
1. De bronmodule is de iteratormodule.
1. De statistische functie is SUM.
1. De waarde is [ gegevens:populatie ] van de Get module van de Details van het Land.
1. Klik de Show geavanceerde montagesoptie bij de bodem en de groep door [ gegevens:subregion ] van de Get module van de Details van het Land.

   ![&#x200B; Geavanceerde Beeld 7 van de Samenvoeging &#x200B;](../12-exercises/assets/advanced-aggregation-walkthrough-7.png)

   **beëindigt met een tekstaggregator om samen te voegen wat u binnen de numerieke aggregator groepeerde.**

1. Voeg een tekstaggregator aan het eind toe.
1. De bronmodule is de numerieke aggregator.
1. In het gebied van de Tekst, neem &quot;de totale bevolking van [ SLEUTEL ] op is [ resultaat ].&quot;

   ![&#x200B; Geavanceerde Beeld 8 van de Samenvoeging &#x200B;](../12-exercises/assets/advanced-aggregation-walkthrough-8.png)

1. Sla het bestand op en voer het uit.

   + Controleer de uitvoer uit de uiteindelijke module.
