---
title: Uitoefening van gegevensopslag
description: Leer hoe u bedrijfsnamen synchroniseert tussen twee systemen. (Dit moet tussen 60 en 160 tekens lang zijn, maar mag niet langer zijn dan 59 tekens)
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11055
thumbnail: KT11055.png
recommendations: noDisplay,catalog
exl-id: e4aa9a97-679a-4575-a2c6-b6ac304ce9c2
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Uitoefening van gegevensopslag

Leer hoe u bedrijfsnamen synchroniseert tussen twee systemen.

## Overzicht van oefening

Dit is het eerste deel van een eenrichtingssynchronisatie van bedrijven in Workfront en een ander systeem. Momenteel wordt alleen gesynchroniseerd tussen een Fusion-gegevensopslag en Workfront. Een tabel in een gegevensopslagruimte houdt de Workfront-id (WFID) en de bedrijfs-id in het CSV-bestand (CID) bij voor elk bedrijf. Dit maakt een tweerichtingssynchronisatie mogelijk op een bepaald moment in de toekomst.

![ Gegevens slaat Beeld 1 ](../12-exercises/assets/data-stores-walkthrough-1.png) op

## Te volgen stappen

**Download het dossier van Workfront.**

1. Selecteer &quot;_Companies.csv&quot; in de map Workfront &quot;Fusion Exercise Files&quot; en klik op Documentdetails.
1. Kopieer het eerste id-nummer van het URL-adres.
1. In Fusion maakt u een nieuw scenario met de naam &quot;Gegevensopslag gebruiken voor het synchroniseren van gegevens&quot;.
1. Selecteer voor de triggermodule de module Workfront Download Document.
1. Stel uw Workfront-verbinding in en neem de document-id op die u van de Workfront-URL hebt gekopieerd.
1. Geef deze module de naam &quot;Get companies file&quot;.
1. Voeg nu een Parse CSV-module toe.
1. Typ 2 voor het veld Aantal kolommen.
1. Wijs Gegevens van de het documentmodule van de Download op het CSV gebied toe.
1. Noem deze module &quot;Parse companies file.&quot;
1. Sla uw scenario op en klik eenmaal op Uitvoeren.

   **creeer een gegevensopslag en een gegevensstructuur.**

1. Voeg een de recordmodule van het Onderzoek van de gegevensopslag toe.
1. Maak een nieuwe gegevensopslagruimte met de naam &quot;Bedrijfssync&quot;.
1. Maak in de gegevensopslag een gegevensstructuur met de naam &quot;Company sync (struc)&quot;.
1. Maak vier velden.

   + CID - De bedrijfs-id in het CSV-bestand
   + Bedrijfsnaam
   + WFID - De Workfront-bedrijfsnaam
   + Aanmaakdatum - Zorg dat het gegevenstype datum is

   ![ Gegevens slaat Beeld 2 ](../12-exercises/assets/data-stores-walkthrough-2.png) op

1. Klik op Opslaan in de gegevensstructuur, stel de grootte van de gegevensopslag in op 1 en sla de gegevensopslag op.
1. Als u doorgaat in de module Data Store, stelt u een filter in waarbij de CID gelijk is aan de id van het bedrijf in de module Parse CSV (Kolom 1).
1. Klik op Geavanceerde instellingen tonen en selecteer de optie om door te gaan met de uitvoering van het scenario of de route, zelfs als deze module zonder resultaten retourneert.

   ![ Gegevens slaat Beeld 3 ](../12-exercises/assets/data-stores-walkthrough-3.png) op

1. Wijzig de naam van deze module &quot;Overeenkomende bedrijven&quot;.
1. Voeg een Workfront-zoekrecordmodule toe.
1. Kies Bedrijf als recordtype.
1. Zoekcriteria zijn de bedrijfsnaam in Workfront gelijk aan de bedrijfsnaam in het CSV-bestand.
1. Selecteer voor uitvoer de bedrijfsnaam en de id.

   ![ Gegevens slaat Beeld 4 ](../12-exercises/assets/data-stores-walkthrough-4.png) op

1. Klik op OK en wijzig de naam van deze module in Overeenkomende bedrijven.

   **creeer verschillende wegen die op worden gebaseerd of het bedrijf binnen Workfront of de gegevensopslag bestaat.**

   **Verpletterend weg 1 - creeer een bedrijf.**

1. Voeg een routermodule aan het recht van de de archiefmodule van het Onderzoek van Workfront toe.
1. Voeg een Workfront-module Record maken toe aan het bovenste pad.
1. Stel het recordtype in op Bedrijf.
1. Selecteer Naam in velden die u wilt toewijzen. Wijs het naamgebied aan de output van de ParseCSV module (Kolom 2) toe.
1. Wijzig de naam van deze module &quot;Bedrijf maken&quot;.

   ![ Gegevens slaat Beeld 5 ](../12-exercises/assets/data-stores-walkthrough-5.png) op

1. Voeg een filter na de router toe om een bedrijf slechts tot stand te brengen als het niet reeds in Workfront is. Geef het de naam &quot;Niet in Workfront.&quot;
1. Stel de voorwaarde in op de id in de module Workfront Search en bestaat niet.

   ![ Gegevens slaat Beeld 6 ](../12-exercises/assets/data-stores-walkthrough-6.png) op

   **voorbereidingen om de gegevensopslag in de volgende weg bij te werken.**

1. Voeg een module met variabelen instellen toe aan het einde van het bovenste pad.
1. Stel de naam van de variabele in op &quot;Workfront-id&quot;.
1. Stel de waarde Variabele in op de id in de module Bedrijf maken.
1. Wijzig de naam van deze module &quot;Workfront-id instellen&quot;.

   **Verpletterend weg 2 - werk de gegevensopslag bij.**

1. Creeer een filter op het verpletteren van weg 2. Geef deze de naam &#39;Niet in de gegevensopslag&#39;.

1. Plaats de Voorwaarde aan de Sleutel van de de opslagmodule van Gegevens en bestaat niet.

   ![ Gegevens slaat Beeld 7 ](../12-exercises/assets/data-stores-walkthrough-7.png) op

1. De eerste module in dit pad is de module Get variable.
1. Stel de naam van de variabele in op &quot;Workfront-id&quot;.
1. Wijzig de naam van deze module &#39;Workfront-id ophalen&#39;.
1. Voeg een andere module toe uit de app Data store, voeg een record toe of vervang een record.
1. Kies Bedrijfssynchronisatie in het veld Gegevensopslag. Dit is de gegevensopslag die u eerder hebt gemaakt.
1. Laat het veld Sleutel leeg.
1. Wijs het CID gebied van Kolom 1 in de Parse CSV module toe.
1. Wijs het gebied van de bedrijfsnaam van Kolom 2 in de ParseCSV module toe.
1. Wijs het WFID-veld toe vanuit de module Workfront-id ophalen.
1. Gebruik voor het veld Gemaakt op-datum de functie formatDate van het tabblad Datum en tijd om de huidige datum op te maken als DD-MM-JJJJ.

   ![ Gegevens slaat Beeld 8 ](../12-exercises/assets/data-stores-walkthrough-8.png) op

1. Klik op OK en wijzig de naam van deze module &quot;Bedrijfsitem maken&quot;.

   **Verpletterend weg 3-Sync de gegevensopslag tussen systemen.**

1. Begin door een filter op het verpletteren van weg 3 te creëren. Geef het de naam &quot;Bedrijf bestaat, niet in gegevensopslag.&quot;
1. Plaats de Voorwaarde aan de Sleutel van de de verslagenmodule van het Onderzoek van de opslag van Gegevens en bestaat niet.
1. Klik op de knop Toevoegen EN regel en wijs aan dat de bedrijfsnaam van het CSV-bestand (Kolom 2) gelijk is aan de naam van het bedrijf dat in de zoekmodule van Workfront wordt gevonden.

   ![ Gegevens slaat Beeld 9 ](../12-exercises/assets/data-stores-walkthrough-9.png) op

1. Voeg nu een andere toe/vervang een verslagmodule door te klonen aan het eind van het verpletteren van weg 2.
1. Sleep de gekloonde module in plaats aan het eind van het verpletteren van weg 3. Verwijder de lege module die er was.
1. Klik op de gekloonde module. Alle velden moeten hetzelfde blijven, behalve het veld WFID. Wijs het van de Vergelijkende module van het Onderzoek van Bedrijven toe.

   ![ Gegevens slaat Beeld 10 ](../12-exercises/assets/data-stores-walkthrough-10.png) op

1. Klik op OK en wijzig de naam van deze module &quot;Bedrijfsitem maken&quot;.
