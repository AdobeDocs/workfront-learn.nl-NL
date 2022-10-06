---
title: Switch, functie
description: Leer hoe te om de schakelaarfunctionaliteit te gebruiken gebruikend de functie van de Schakelaar.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11051
thumbnail: KT1101.png
source-git-commit: f367e016498d5c1814cab79e19e6e9001db2851f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---


# Switch, functie

Leer hoe te om de schakelaarfunctionaliteit te gebruiken gebruikend de functie van de Schakelaar.

## Overzicht van oefening

Voor eenvoudige gegevensveranderingen, gebruik de functie van de Schakelaar om één waarde in een modulegebied om te zetten in een andere. In deze oefening, verander de twee-letterige sleutel in de daadwerkelijke naam voor de status van de projectvooruitgang om in een e-mail te verzenden.

![Schakelfunctie Afbeelding 1](../12-exercises/assets/switch-function-walkthrough-1.png)

## Te volgen stappen

1. Kloon het scenario genoemd &quot;het Delen van variabelen tussen het verpletteren van wegen.&quot;
1. Noem het nieuwe scenario &quot;het Delen variabelen tussen het verpletteren van wegen - Schakelaar.&quot;
1. Klik de trekkermodule en voeg de Status van de Voortgang aan de sectie van Output toe.
1. Voeg in de module Een e-mailbericht verzenden de Voortgangsstatus toe aan het veld Inhoud.

   + Als u enkel over de waarde die uit de module van het Onderzoek komt in kaart brengt, is er een twee-lettercode voor de vooruitgangsstatus.
   + Als u de code voor de volledige naam van elke mogelijke vorderingsstatus wilt &quot;wisselen&quot;, gebruikt u de functie &quot;switch&quot; op het tabblad Algemene functies.

1. De schakelaarfunctie gebruikt de waarde of de uitdrukking van de Status van de Voortgang als sleutel, dan keert de outputwaarde terug die op die sleutel wordt gebaseerd.

   + Een sleutelwaarde wordt bepaald in de eerste positie na de Status van de Voortgang (&quot;LT&quot;) met de overeenkomstige output die in de tweede positie wordt bepaald (&quot;Late&quot;).
   + De volgende sleutelwaarde wordt gedefinieerd in de derde positie, waarbij de corresponderende uitvoer wordt gedefinieerd in de vierde positie, enz., voor zoveel toetsen als gewenst.

      ![Schakelfunctie Afbeelding 2](../12-exercises/assets/switch-function-walkthrough-2.png)