---
title: Inleiding tot universele aansluitingen
description: Vergroot uw begrip van het werken met REST universele schakelaars en het werken met de teruggekeerde gegevens.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11042
thumbnail: KT11042.png
exl-id: eb442c3e-26f3-44b7-9937-ed4eeba39fb1
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---

# Inleiding tot universele aansluitingen

Vergroot uw begrip van het werken met REST universele schakelaars en het werken met de teruggekeerde gegevens.

## Overzicht van oefening

Gebruikend een karakter Pokemon in een spreadsheet, roep de Pijn API door een schakelaar van HTTP om meer informatie over dat karakter te verzamelen en te posten.

![Inleiding tot universele connectors Afbeelding 1](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-1.png)

## Te volgen stappen

**Download het CSV-bestand van Workfront.**

1. Selecteer &quot;_Fusion2020_Shipping Manifest.csv&quot; in de map Workfront &quot;Fusion Exercise Files&quot; en klik op Documentdetails.
1. Kopieer het eerste id-nummer van het URL-adres.
1. Maak een nieuw scenario in Workfront Fusion. Noem het &quot;Gebruikend universele schakelaars.&quot;
1. Start met de module Download Document vanuit de Workfront-toepassing.
1. Stel uw Workfront-verbinding in en neem de document-id op die u van de Workfront-URL hebt gekopieerd.
1. Wijzig de naam van deze module &quot;Verzendmanifest downloaden&quot;.

   ![Inleiding tot universele connectors Afbeelding 9](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-9.png)

   **Analyseer de verschepende manifestgegevens.**

1. Voeg een andere module toe en selecteer CSV parseren.
1. CSV-bestand parseren voor 11 kolommen. Controleer CSV bevat kopballen doos. Kies het komma delimiterType, en zet Gegevens van de module van het Document van de Download op het CSV gebied.

   ![Inleiding tot universele connectors Image 2](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-2.png)

1. Wijzig de naam van deze module &quot;Parse Shipping manifest&quot;.
1. Sla het scenario op en klik eenmaal op Uitvoeren, zodat u de gegevens uit het CSV-bestand in de volgende stappen kunt zien.

   **Haal de Pokemon-gegevens op met de universele aansluiting.**

1. Voeg een HTTP Make een Request module toe.
1. Gebruik in het veld URL `https://pokeapi.co/api/v2/pokemon/[Character]`, waarbij [Teken] wordt in kaart gebracht aan Kolom 3 van de Parse CSV module.
1. Schakel het selectievakje Reactie pareren in.
1. Selecteer Geavanceerde instellingen tonen en schakel het selectievakje naast &quot;Alle frames als fouten evalueren&quot; in.
1. Klik op OK en wijzig de naam van de module &quot;Info over pokemon ophalen&quot;.

   **Uw toewijzingspaneel moet er als volgt uitzien:**

   ![Inleiding tot universele connectors Image 3](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-3.png)

   **In dit gedeelte van de oefening, wilt u slechts rij 1 in het Csv- dossier verwerken.**

1. Voeg een filter toe vóór de module Get Pokemon Info. Geef deze de naam &quot;Alleen rij 1&quot;.
1. Stel de voorwaarde zodanig in dat alleen id nummer 1 wordt doorgegeven. Id nummer 1 staat in rij 1 en ID-veld bevindt zich in kolom 1 in het CSV-bestand.

   ![Inleiding tot universele connectors Afbeelding 4](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-4.png)

1. Sla het scenario op.
1. Klik op Eenmaal uitvoeren en bekijk het foutbericht dat u ontvangt in HTTP Make a request module.

   >[!IMPORTANT]
   >
   >In het veld URL van invoergegevens wordt de naam van het teken met hoofdletters weergegeven. Dit werkt niet voor het maken van die API-aanroep omdat tekennamen in kleine letters moeten worden geschreven.

   ![Inleiding tot universele connectors Image 5](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-5.png)

1. Gebruik het toewijzingspaneel in het veld HTTP een aanvraag-URL maken om het [Teken] veld alle kleine letters met de **lager** functie.

   ![Inleiding tot universele aansluitingen Afbeelding 6](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-6.png)

   **Wijs informatie terug van API gebruikend de Reeks veelvoudige variabelen module.**

1. Voeg de module Meerdere variabelen instellen toe na Info van menu ophalen. Kaartnaam, hoogte, gewicht en mogelijkheden.
1. Aangezien het veld Abilities een array is, moet u niet vergeten de kaartfunctie te gebruiken om toegang te krijgen tot de naam van elke mogelijkheid in de array.

   ![Inleiding tot universele connectors Afbeelding 7](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-7.png)

   **Voer het scenario zonder het filter uit om een andere fout te ontdekken.**

1. Als u alle rijen in het CSV-bestand wilt verwerken, verwijdert u het filter Alleen rij 1:

   + Klik op het filterpictogram om dit te bewerken.
   + Verwijder het filterlabel.
   + Verwijder de voorwaarde.
   + Klik op OK.

1. Sla het scenario op en klik eenmaal op Uitvoeren.
1. Er treedt een fout op in de module Get Pokemon Info. Er is een superheld-teken doorgegeven aan de Pokemon-API.

   >[!NOTE]
   >
   >In de analyse van Routers, zult u zien hoe te om deze fout op te lossen door een afzonderlijke weg tot stand te brengen om superhelden te verwerken.

   ![Inleiding tot universele connectors Afbeelding 8](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-8.png)
