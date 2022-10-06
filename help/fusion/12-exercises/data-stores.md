---
title: Gegevensopslag
description: Leer hoe u bedrijfsnamen synchroniseert tussen twee systemen. (Dit moet tussen 60 en 160 tekens lang zijn, maar mag niet langer zijn dan 59 tekens)
feature: Workfront Fusion
role: User
level: Beginner
kt: 11055
thumbnail: KT11055.png
source-git-commit: c348222464180e994e7b414d1b84e07f58b6b2ae
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---


# Gegevensopslag

Leer hoe u bedrijfsnamen synchroniseert tussen twee systemen.

## Overzicht van oefening

Dit is het eerste deel van een eenrichtingssynchronisatie van bedrijven in Workfront en een ander systeem. Momenteel wordt alleen gesynchroniseerd tussen een Fusion-gegevensopslag en Workfront. Een tabel in een gegevensopslagruimte houdt de Workfront-id (WFID) en de bedrijfs-id in het CSV-bestand (CID) bij voor elk bedrijf. Dit maakt een tweerichtingssynchronisatie mogelijk op een bepaald moment in de toekomst.

![Gegevens slaan afbeelding 1 op](../12-exercises/assets/data-stores-walkthrough-1.png)

## Te volgen stappen

**Download het bestand van Workfront.**

1. Selecteer &quot;_Companies.csv&quot; in de map Workfront &quot;Fusion Exercise Files&quot; en klik op Documentdetails.
1. Kopieer het eerste id-nummer van het URL-adres.
1. In Fusion maakt u een nieuw scenario met de naam &quot;Gegevensopslag gebruiken voor het synchroniseren van gegevens&quot;.
1. Selecteer voor de triggermodule de module Workfront Download Document.
1. Stel uw Workfront-verbinding in en neem de document-id op die u van de Workfront-URL hebt gekopieerd.
1. Geef deze module de naam &quot;Get companies file&quot;.
1. Voeg nu een Parse CSV-module toe.
1. Typ 2 voor het veld Aantal kolommen.
1. Wijs Gegevens van de het documentmodule van de Download op het Csv- gebied toe.
1. Noem deze module &quot;Parse companies file.&quot;
1. Sla uw scenario op en klik eenmaal op Uitvoeren.

   **Maak een gegevensopslag en een gegevensstructuur.**

1. Voeg een de recordmodule van het Onderzoek van de gegevensopslag toe.
1. Maak een nieuwe gegevensopslagruimte met de naam &quot;Bedrijfssync&quot;.
1. Maak in de gegevensopslag een gegevensstructuur met de naam &quot;Company sync (struc)&quot;.
1. Maak vier velden.

   + CID - De bedrijfs-id in het CSV-bestand
   + Bedrijfsnaam
   + WFID - De Workfront-bedrijfsnaam
   + Aanmaakdatum - Zorg dat het gegevenstype datum is

   ![Afbeelding 2 wordt opgeslagen](../12-exercises/assets/data-stores-walkthrough-2.png)

1. Klik op Opslaan in de gegevensstructuur, stel de grootte van de gegevensopslag in op 1 en sla de gegevensopslag op.
1. Als u doorgaat in de module Data Store, stelt u een filter in waarbij de CID gelijk is aan de id van het bedrijf in de module Parse CSV (Kolom 1).
1. Klik op Geavanceerde instellingen tonen en selecteer de optie om door te gaan met de uitvoering van het scenario of de route, zelfs als deze module zonder resultaten retourneert.

   ![Afbeelding 3 wordt opgeslagen](../12-exercises/assets/data-stores-walkthrough-3.png)

1. Wijzig de naam van deze module &quot;Overeenkomende bedrijven&quot;.
1. Voeg een Workfront-zoekrecordmodule toe.
1. Kies Bedrijf als recordtype.
1. Zoekcriteria zijn de bedrijfsnaam in Workfront en zijn gelijk aan de bedrijfsnaam in het CSV-bestand.
1. Selecteer voor uitvoer de bedrijfsnaam en de id.

   ![Gegevensopslag afbeelding 4](../12-exercises/assets/data-stores-walkthrough-4.png)

1. Klik op OK en wijzig de naam van deze module in Overeenkomende bedrijven.

   **Maak verschillende paden op basis van het feit of het bedrijf in Workfront of in de gegevensopslag bestaat.**

   **Verpletterend weg 1 - creeer een bedrijf.**

1. Voeg een routermodule aan het recht van de de archiefmodule van het Onderzoek van Workfront toe.
1. Voeg een Workfront-module Record maken toe aan het bovenste pad.
1. Stel het recordtype in op Bedrijf.
1. Selecteer Naam in velden die u wilt toewijzen. Wijs het naamgebied aan de output van de ParseCSV module (Kolom 2) toe.
1. Wijzig de naam van deze module &quot;Bedrijf maken&quot;.

   ![Afbeelding 5 wordt opgeslagen](../12-exercises/assets/data-stores-walkthrough-5.png)

1. Voeg een filter na de router toe om een bedrijf slechts tot stand te brengen als het niet reeds in Workfront is. Geef het de naam &quot;Niet in Workfront.&quot;
1. Stel de voorwaarde in op de id in de module Workfront Search en bestaat niet.

   ![Gegevensopslag afbeelding 6](../12-exercises/assets/data-stores-walkthrough-6.png)

   **De gegevensopslag in het volgende pad bijwerken.**

1. Voeg een module met variabelen instellen toe aan het einde van het bovenste pad.
1. Stel de naam van de variabele in op &quot;Workfront-id&quot;.
1. Stel de waarde Variabele in op de id in de module Bedrijf maken.
1. Wijzig de naam van deze module &quot;Workfront-id instellen&quot;.

   **Verpletterend weg 2 - werk de gegevensopslag bij.**

1. Creeer een filter op verpletterende weg 2. Geef deze de naam &#39;Niet in de gegevensopslag&#39;.

1. Plaats de Voorwaarde aan de Sleutel van de de opslagmodule van Gegevens en bestaat niet.

   ![Afbeelding 7 opslaan in gegevens](../12-exercises/assets/data-stores-walkthrough-7.png)

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

   ![Afbeelding 8 wordt opgeslagen](../12-exercises/assets/data-stores-walkthrough-8.png)

1. Klik op OK en wijzig de naam van deze module &quot;Bedrijfsitem maken&quot;.

   **Het verpletteren van weg 3-Synchroniseer de gegevensopslag tussen systemen.**

1. Begin door een filter op het verpletteren van weg 3 te creëren. Geef het de naam &quot;Bedrijf bestaat, niet in gegevensopslag.&quot;
1. Plaats de Voorwaarde aan de Sleutel van de de verslagenmodule van het Onderzoek van de opslag van Gegevens en bestaat niet.
1. Klik op de knop Toevoegen EN regel en wijs aan dat de bedrijfsnaam van het CSV-bestand (Kolom 2) gelijk is aan de naam van het bedrijf dat in de zoekmodule van Workfront wordt gevonden.

   ![Afbeelding 9 wordt opgeslagen](../12-exercises/assets/data-stores-walkthrough-9.png)

1. Voeg nu een andere toe/vervang een verslagmodule door te klonen aan het eind van het verpletteren van weg 2.
1. Sleep de gekloonde module in plaats aan het eind van het verpletteren van weg 3. Verwijder de lege module die er was.
1. Klik op de gekloonde module. Alle velden moeten hetzelfde blijven, behalve het veld WFID. Wijs het van de Vergelijkende module van het Onderzoek van Bedrijven toe.

   ![Gegevens slaan afbeelding 10 op](../12-exercises/assets/data-stores-walkthrough-10.png)

1. Klik op OK en wijzig de naam van deze module &quot;Bedrijfsitem maken&quot;.
