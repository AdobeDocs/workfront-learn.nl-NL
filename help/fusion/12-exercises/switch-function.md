---
title: Overschakelen van functies
description: Leer hoe te om de schakelaarfunctionaliteit te gebruiken die de functie van de Schakelaar gebruikt.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11051
thumbnail: KT1101.png
recommendations: noDisplay,catalog
exl-id: 3142fae2-5210-4f63-9d2c-66dec58867fa
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---

# Overschakelen van functies

Leer hoe te om de schakelaarfunctionaliteit te gebruiken die de functie van de Schakelaar gebruikt.

## Overzicht van oefening

Voor eenvoudige gegevensveranderingen, gebruik de functie van de Schakelaar om één waarde in een modulegebied om te zetten in een andere. In deze oefening, verander de twee-letterige sleutel in de daadwerkelijke naam voor de status van de projectvooruitgang om in een e-mail te verzenden.

![&#x200B; functieBeeld 1 van de Schakelaar &#x200B;](../12-exercises/assets/switch-function-walkthrough-1.png)

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

     ![&#x200B; functieBeeld 2 van de Schakelaar &#x200B;](../12-exercises/assets/switch-function-walkthrough-2.png)
