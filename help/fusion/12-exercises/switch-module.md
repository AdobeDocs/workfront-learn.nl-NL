---
title: Switch-module
description: Begrijp hoe te om de module van de Schakelaar te gebruiken wanneer u complexere of dynamische gegevenstransformaties moet uitvoeren.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11052
thumbnail: KT11052.png
exl-id: 1b810168-582d-4d7d-b061-d152af546bc8
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---

# Switch-module

Begrijp hoe te om de module van de Schakelaar te gebruiken wanneer u complexere of dynamische gegevenstransformaties moet uitvoeren.

## Overzicht van oefening

Zoek naar direct-mailprojecten in uw testaandrijving, dan verander de naam van elk project dat op een waarde wordt gebaseerd die op een douanegebied in bijlage aan het project wordt geselecteerd.

![Switch module Image 1](../12-exercises/assets/switch-module-walkthrough-1.png)

## Te volgen stappen

1. Creeer een nieuw scenario en noem het &quot;Gebruikend de module van de Schakelaar.&quot;
1. Gebruik de zoekmodule van Workfront voor de triggermodule.
1. Stel uw Workfront-verbinding in en stel het recordtype in op Project.
1. In de criteria van het Onderzoek, specificeer dat u slechts projecten wilt zien die een waarde op het de douaneveld van het Kanaal hebben.
1. Selecteer voor uitvoer de optie Id, Naam, Referentienummer en het aangepaste veld Kanaal.

   ![Switch module Image 2](../12-exercises/assets/switch-module-walkthrough-2.png)

1. Voeg de module van de Schakelaar van Hulpmiddelen toe.
1. Wijs voor het veld Invoer het aangepaste kanaalveld toe vanuit de module Zoeken.

   ![Switch module Image 3](../12-exercises/assets/switch-module-walkthrough-3.png)

1. Voeg vervolgens gevallen toe voor elke mogelijke waarde die afkomstig is uit het aangepaste veld Kanaal. De mogelijke waarde wordt weergegeven in het veld Patroon. U wilt dat het outputgebied een specifieke 3 lettercode omvat die door het aantal van de projectverwijzing wordt gevolgd, toen de projectnaam.

   **Uw toewijzingspaneel moet er als volgt uitzien:**

   ![Modusafbeelding 4 schakelen](../12-exercises/assets/switch-module-walkthrough-4.png)

1. U kunt zoveel extra gevallen toevoegen als u wilt. Let op het veld Anders onderaan. Dit wordt gebruikt als de invoerwaarde niet overeenkomt met een van de gevallen.

   **Werk de projectnaam in Workfront bij.**

   ![Afbeelding 5 van de module Switch](../12-exercises/assets/switch-module-walkthrough-5.png)

1. Voeg een Workfront Update Record module toe.
1. In het gebied van identiteitskaart, kaart aan identiteitskaart van de trekkermodule.
1. Stel het recordtype in op Project.
1. Selecteer het gebied van de Naam van de Uitgezochte Gebieden aan de sectie van de Kaart, en kaart het aan de output van de module van de Schakelaar.
1. Sla uw scenario op en voer het één keer uit. Bekijk de bijgewerkte projectnamen in uw testaandrijving.
