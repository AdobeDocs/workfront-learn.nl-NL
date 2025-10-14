---
title: Gegevensstructuren
description: Gegevens van een bronbestand omzetten in een doelbestand. (Dit moet tussen 60 en 160 tekens lang zijn, maar mag niet langer zijn dan 58 tekens)
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11054
thumbnail: KT11054.png
recommendations: noDisplay,catalog
exl-id: 06a39a87-23f3-4d4a-995e-d32fb9c5f50d
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '1079'
ht-degree: 0%

---

# Gegevensstructuren

Gegevens van een bronbestand omzetten in een doelbestand.

## Overzicht van oefening

Open een CSV-bestand dat een lijst met tijdgegevens bevat. Deze tijdgegevens worden gedurende minuten vastgelegd door meerdere gebruikers. Het doel is deze informatie te nemen en een nieuwe CSV te produceren die de totale tijd, in uren toont, die door elke gebruiker, elke dag wordt geregistreerd.

![&#x200B; Beeld van de structuren van Gegevens 1 &#x200B;](../12-exercises/assets/data-structures-walkthrough-1.png)

![&#x200B; Beeld van de structuren van Gegevens 2 &#x200B;](../12-exercises/assets/data-structures-walkthrough-2.png)


In dit scenario opent u een bestand dat een lijst bevat met tijdgegevens voor gewerkte minuten, zoals de datum en tijd, het aantal minuten dat is ingevoerd en het e-mailadres van wie de gegevens heeft ingevoerd. Er zijn 100 inzendingen, waarvan sommige door dezelfde individuen zijn gemaakt en sommige op dezelfde dag als andere.

Als u een bestand wilt maken waarin de totale tijd, in uren, die elke dag door elk individu wordt gewerkt, wordt weergegeven, gaat u als volgt te werk:

1. Haal in de triggermodule een bestand op uit de Workfront-map. Download het bestand.
1. In de eerste module CSV, ontleed de gegevens van de tijdingang aan output één bundel voor elke tijdingang. Dit is een iterator.
1. De eerste module van Hulpmiddelen is een numerieke aggregator. Hiermee voegt u alle minuten samen en groepeert u de rijen per e-mailadres en vervolgens op datum. Het resultaat is het totaal aantal minuten dat elke dag per e-mailadres is gewerkt.
1. De tweede module van Hulpmiddelen is een Vastgestelde module van de Variabele. Gebruik deze optie om de minuten op te maken om deze met 60 decimalen te delen en om te afronden naar 2 decimalen.
1. Stel het uitvoerbestand in in de tweede CSV-module.
1. Upload het CSV-bestand in de uiteindelijke module naar Workfront.

## Te volgen stappen

**Download het dossier van Workfront.**

1. Selecteer &quot;_Fusion1.0JanTime.csv&quot; in de map Workfront &quot;Fusion Exercise Files&quot; en klik op Documentdetails.
1. Kopieer het eerste id-nummer van het URL-adres.
1. Maak een nieuw scenario. Geef deze de naam &#39;Gegevensstructuren maken en gebruiken&#39;.
1. Start met de module Download Document vanuit de Workfront-toepassing.
1. Stel uw Workfront-verbinding in en neem de document-id op die u van de Workfront-URL hebt gekopieerd.

   ![&#x200B; Beeld van de structuren van Gegevens 3 &#x200B;](../12-exercises/assets/data-structures-walkthrough-3.png)

   **ontleed de gegevens van de tijdingang.**

1. Voeg een andere module toe en selecteer CSV parseren.
1. CSV-bestand parseren voor 7 kolommen. Controleer CSV bevat kopballen doos. Kies het scheidingsteken voor komma&#39;s en plaats Gegevens in het CSV-veld.

   ![&#x200B; Beeld van de structuren van Gegevens 4 &#x200B;](../12-exercises/assets/data-structures-walkthrough-4.png)

1. Klik eenmaal op Uitvoeren om de uitvoer weer te geven.
1. Open de uitvoeringscontrole om de input en de output van de Parse CSV module te zien. Er is één bundel (een CSV-bestand) als invoer en meerdere bundels als uitvoer (één bundel voor elke rij in het CSV-bestand). Het moet er ongeveer als volgt uitzien:

   ![&#x200B; Beeld van de structuren van Gegevens 5 &#x200B;](../12-exercises/assets/data-structures-walkthrough-5.png)

   **daarna, zet de gegevens in de gewenste outputvorm, met samengevoegde tijdtotalen die in uren in plaats van notulen worden uitgedrukt.**

1. Voeg een module voor het gereedschap Numerieke aggregatie toe.
1. Selecteer de bronmodule, die de ParseCSV module is.
1. Selecteer SUM voor de statistische functie.
1. Het veld Waarde is kolom 7 van het CSV-bestand. Dit zijn de minuten die door elke gebruiker worden geregistreerd.
1. Als u de velden op groep wilt optellen, klikt u op Geavanceerde instellingen en stelt u Groeperen in op e-mail (kolom 4), datum (kolom 5).

   + Deze som wordt voor elke combinatie van het e-mailbericht en de datum berekend. Plaats een komma tussen kolom 4 en kolom 5. Dit wordt later als scheidingsteken gebruikt.

   **Uw toewijzingspaneel zou als dit moeten kijken:**

   ![&#x200B; Beeld van de structuren van Gegevens 6 &#x200B;](../12-exercises/assets/data-structures-walkthrough-6.png)

1. Klik eenmaal op Uitvoeren om de uitvoer van de aggregatie te controleren.

   **de outputbundels zouden als dit moeten kijken:**

   ![&#x200B; Beeld van de structuren van Gegevens 7 &#x200B;](../12-exercises/assets/data-structures-walkthrough-7.png)

   **zet nu de samengevoegde notulen in uren om.**

1. Voeg nog een gereedschapsmodule toe en selecteer Variabele instellen.
1. Geef de variabele &quot;Uren&quot; een naam.
1. Stel de waarde van de variabele in op formatNumber(result/60;2;.;,)

   **Uw toewijzingspaneel zou als dit moeten kijken:**

   ![&#x200B; Beeld van de structuren van Gegevens 8 &#x200B;](../12-exercises/assets/data-structures-walkthrough-8.png)

   **daarna, krijg de waarden opstelling voor het outputdossier. U wilt de userID en de datumwaarde die voor de groepen worden gebruikt. U wilt ook de uren die werden berekend.**

1. Voeg een andere module-CSV module toe gebruikend de aggregator creëren CSV (geavanceerd).
1. De bronmodule is Tools - Numerieke aggregator.
1. Klik op Toevoegen in het veld Gegevensstructuur en geef onze gegevensstructuur de naam &quot;Dagelijkse aangegeven tijd&quot;.
1. Klik op Item toevoegen om het eerste item te maken.
1. Geef het item de naam &quot;UserID&quot; en stel het type in op Text. Klik toevoegen.
1. Klik nogmaals op Item toevoegen om het tweede item te maken.
1. Geef het item de naam Datum, stel het type in op Datum en klik op Toevoegen.
1. Klik nog een keer op Item toevoegen.
1. Geef het item de naam &quot;Uren&quot;, stel het type in op Nummer en klik op Toevoegen.

   **Uw gegevensstructuur zou als dit moeten kijken:**

   ![&#x200B; Beeld 9 van de structuren van Gegevens &#x200B;](../12-exercises/assets/data-structures-walkthrough-9.png)

1. Klik op Opslaan om de gegevensstructuur Tijd geregistreerd voor dagelijkse som te voltooien.

   **nu u levert de waarden voor de drie gebieden u enkel creeerde. U zou die drie gebieden in het CSV toewijzingspaneel moeten zien.**

1. Klik in het veld Gebruikersnaam en kies GET op het tabblad Algemene functies. In de eerste parameter, zet SPLIT van de tekst en binaire functies tabel. De eerste parameter voor de functie SPLIT is het Sleutelgebied. Voeg een komma als scheidingsteken en 1 als index toe. Dit geeft aan dat u wilt dat de GET het eerste veld in de array Key ophaalt.
1. Kopieer deze expressie naar het veld Datum. Wijzig de index van 1 tot en met 2 in de tweede waarde in de array.
1. Voeg voor het veld Uren het veld Uren toe met het gereedschap Variabele instellen.

   **Uw Csv- kaartpaneel zou als dit moeten kijken:**

   ![&#x200B; Beeld van de structuren van Gegevens 10 &#x200B;](../12-exercises/assets/data-structures-walkthrough-10.png)

   **als u het scenario nu in werking stelt, zou u deze output moeten zien:**

   ![&#x200B; Beeld van de structuren van Gegevens 11 &#x200B;](../12-exercises/assets/data-structures-walkthrough-11.png)

   **nu, voeg een module toe om deze output te nemen en het als document aan een bestaand project in Workfront te uploaden.**

1. Open het project in Workfront en kopieer de project-id van URL.
1. Ga terug naar het scenario in Fusion en voeg een andere module-de module van het Document van de Upload van Workfront toe app.
1. Plak de project-id in het veld Verwante record-id.
1. Kies Project voor het Verwante type van Verslag.
1. Kies de optie Kaart voor het Source-bestand.
1. Gebruik voor de documentnaam de bestandsnaam die u hebt gedownload en voeg &quot;Bijgewerkt&quot; vóór de naam toe.
1. Voor de inhoud van het Dossier, gebruik de output van de Tekst van de Create CSV module.

   **Uw toewijzingspaneel zou als dit moeten kijken:**

   ![&#x200B; Beeld van de structuren van Gegevens 12 &#x200B;](../12-exercises/assets/data-structures-walkthrough-12.png)

1. Klik op OK en sla het scenario op.
1. Klik eenmaal op Uitvoeren om het scenario uit te voeren.

   **controleer de uitvoeringsinspecteur in de Upload module van het Document om het document te bevestigen werd geupload.**

   ![&#x200B; Beeld van de structuren van Gegevens 13 &#x200B;](../12-exercises/assets/data-structures-walkthrough-13.png)
