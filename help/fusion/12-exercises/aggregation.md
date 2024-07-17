---
title: Samenvoeging
description: Leer meerdere bundels informatie samen te voegen tot één waarde.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11047
thumbnail: KT11047.png
recommendations: noDisplay,noCatalog
exl-id: 4626b623-8b05-41be-9cfc-917e28222855
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Samenvoeging

Leer meerdere bundels informatie samen te voegen tot één waarde.

## Overzicht van oefening

Gebruikend het &quot;Inleiding aan herhaling&quot;scenario u in de laatste oefening bouwde, de geplande uren op elke het werk taak in het project samenvoegen en een e-mail naar zich met die informatie verzenden.

![ Beeld van de Samenvoeging 1 ](../12-exercises/assets/aggregation-walkthrough-1.png)

## Te volgen stappen

**voeg een filter toe en SUM de geplande uren.**

1. Kloon het &quot;Inleiding aan herhaling&quot;scenario u in de vorige oefening creeerde, en noem het &quot;Inleiding aan samenvoeging.&quot;
1. Voeg een filter tussen de Gelezen module van Taken van het Project en de Telling toe # van takenmodule. Geef het filter de naam &quot;Alleen werktaken&quot;.
1. Plaats de voorwaarde aan Aantal van Kinderen [ Numerieke Exploitant: Gelijk aan ] 0.

   ![ Beeld van de Samenvoeging 2 ](../12-exercises/assets/aggregation-walkthrough-2.png)

1. Voeg na de module Willekeurige wiskunde een module Numerieke aggregator toe.
1. Plaats de bronmodule om de Taken van het Project te lezen.
1. Stel de functie Samenvoegen in op SUM.
1. Plaats de Waarde aan het gebied van het Werk van de Gelezen module van de Taken van het Project.
1. Wijzig de naam van deze module &quot;SUM van alle uren van het taakplan&quot;.

   ![ Beeld 3 van de Samenvoeging ](../12-exercises/assets/aggregation-walkthrough-3.png)

   **neem nota van de schaduw die toont dat de samenvoeging de herhaling beëindigt.**

   ![ Beeld van de Samenvoeging 4 ](../12-exercises/assets/aggregation-walkthrough-4.png)

   **verzend een e-mail met samengevoegde uren.**

1. Voeg een module Een e-mailbericht verzenden vanuit de e-mailtoepassing toe, na de numerieke aggregator.
1. Stuur de e-mail naar uzelf.
1. Onderwerpregel is &quot;Projectdetails&quot;.
1. Op het gebied van de Inhoud, zet &quot;Er is een project genoemd [ projectnaam ] dat een totaal aantal [ resultaat ] geplande uren heeft.&quot; &quot;[ projectnaam ]&quot;wordt genomen van Gelezen een module van het Verslag en &quot;[ resultaat ]&quot;wordt genomen van de samenvoegersmodule.

   ![ Beeld van de Samenvoeging 5 ](../12-exercises/assets/aggregation-walkthrough-5.png)

1. Sla het bestand op en voer het uit. Zoek de e-mail in uw Postvak IN.

Binnen de iteratie zijn de afzonderlijke bundels toegankelijk. Maar buiten de iteratie, in Send een e-mailmodule, kunnen slechts de samengevoegde gebieden worden betreden.
