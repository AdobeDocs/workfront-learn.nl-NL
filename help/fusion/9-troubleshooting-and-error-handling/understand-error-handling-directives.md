---
title: Richtlijnen voor foutafhandeling begrijpen
description: Meer informatie over de aanwijzingen van de fouthandler waarmee uitvoering kan worden voortgezet en over de instructies die de uitvoering stoppen, kunt u in [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: Jira ticket
exl-id: cb8d0880-73d2-4118-b800-a126f8509309
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---

# Richtlijnen voor foutafhandeling begrijpen

In deze video leert u:

* De drie instructies van de foutenmanager die uitvoering toestaan om verder te gaan
* De twee instructies van de foutenmanager die de uitvoering tegenhouden

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12)

## Richtlijnen — Het scenario gaat verder

### Hervatten

* Er wordt een vervangend uitvoerbestand opgegeven en geleverd aan de module die een fout aantreft.
* De volgende modules worden verwerkt.
* De status van de uitvoering van het scenario is gemarkeerd als &quot;succes.&quot;

![Een afbeelding van een instructie Hervatten](assets/troubleshooting-and-error-handling-2.png)

### Break

* De status van de uitvoering van het scenario wordt opgeslagen in de wachtrij met onvolledige uitvoeringen waar de fout handmatig kan worden opgelost. Er zijn echter enkele uitzonderingen die hier worden genoemd.
* De volgende modules worden niet verwerkt.
* Als er onverwerkte bundels zijn, gaat de uitvoering van het scenario normaal voort.
* De status van de uitvoering van het scenario wordt gemarkeerd als &quot;waarschuwing.&quot;

![Afbeelding van een instructie Break](assets/troubleshooting-and-error-handling-3.png)

### Negeren

* De fout wordt genegeerd en de verdere modules worden niet verwerkt.
* Als er onverwerkte bundels zijn, gaat de uitvoering van het scenario normaal voort.
* De status van de uitvoering van het scenario is gemarkeerd als &quot;succes.&quot;

![Een afbeelding van een instructie Negeren](assets/troubleshooting-and-error-handling-4.png)

## Richtlijnen — Scenario-stops

### Terugdraaien

* De uitvoering van het scenario wordt onmiddellijk gestopt en een terugdraaiingsfase is begonnen op alle modules in een poging om hen allen aan hun aanvankelijke staat terug te keren.
* De volgende modules worden niet verwerkt.
* Met uitzondering van een aantal fouttypen wordt het scenario gedeactiveerd na het aantal opeenvolgende fouten dat is opgegeven onder Scenario-instellingen.
* De status van de uitvoering van het scenario wordt gemarkeerd als &quot;fout.&quot;

>[!NOTE]
>
>Dit is het standaardgedrag als geen route van de foutenmanager aan de module in bijlage is en &quot;het Opslaan van Onvolledige Uitvoeringen&quot;het plaatsen onder de montages van het Scenario niet wordt gecontroleerd.

![Een afbeelding van een instructie Terugdraaien](assets/troubleshooting-and-error-handling-5.png)

### Vastleggen

* De fout wordt genegeerd en de verdere modules worden niet verwerkt.
* Als er onverwerkte bundels zijn, gaat de uitvoering van het scenario normaal voort.
* De status van de uitvoering van het scenario is gemarkeerd als &quot;succes.&quot;

![Afbeelding van een instructie Vastleggen](assets/troubleshooting-and-error-handling-6.png)
