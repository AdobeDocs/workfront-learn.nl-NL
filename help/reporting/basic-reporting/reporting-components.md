---
title: Rapportonderdelen verkennen in Workfront
description: Workfront-rapportagecomponenten verfijnen de gegevensvisualisatie met op objecten gebaseerde filters, dynamische weergaven, gestructureerde groeperingen en jokertekenfunctionaliteit voor op maat gemaakte inzichten.
activity: use
feature: Reports and Dashboards
thumbnail: 335146.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8850
last-substantial-update: 2025-04-28T00:00:00Z
exl-id: e9f9ba24-540f-49e1-ac52-740df489317b
doc-type: video
source-git-commit: 66bab1a0b2316a31cb99916220500303e49797ad
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# Rapportonderdelen verkennen in Workfront

In de video wordt uitgelegd wat het concept is van het rapporteren van componenten in Workfront. Deze zijn essentieel voor het maken van filters, weergaven en groepen. De belangrijkste componenten zijn:

* **Type van Objecten:** specificeert het voorwerp van Workfront dat, zoals een project, een taak, of een uuringang wordt behandeld. &#x200B; Filters, weergaven en groepen zijn specifiek voor het objecttype. &#x200B;
* **Gebied Source en de Naam van het Gebied:** de gebiedsbron is het punt in Workfront waar de informatie in bijlage is, en de gebiedsnaam is het specifieke stuk van informatie (bijvoorbeeld, &quot;beschrijving&quot;voor een project). &#x200B;
* **Gebied van de Waarde:** vertegenwoordigt de inhoud van een gebied, zoals &quot;laag,&quot;&quot;normaal,&quot;hoog,&quot;of &quot;dringend&quot;voor het prioritaire gebied. &#x200B;
* **Kwalifier van de Filter:** bepaalt welke waarden om in een rapport te omvatten of uit te sluiten, zoals het tonen van taken met een prioriteit van &quot;hoog.&quot;&#x200B;


>[!VIDEO](https://video.tv.adobe.com/v/3447027/?captions=dut&quality=12&learn=on&enablevpops=0)

## Toetsen

* **Meldend Componenten:** Workfront die componenten melden omvat objecten type, gebiedsbron, gebiedsnaam, filterkwaliteiten, en waardegebied, die essentieel zijn voor het creëren van filters, meningen, en groeperingen. &#x200B;
* **Specificiteit van het Type van Objecten:** de Filters, de meningen, en de groeperingen zijn gebonden aan specifieke objecten types, zoals projecten, taken, of uuringangen, die ervoor zorgen dat de rapporten aan de relevante gegevens worden aangepast. &#x200B;
* **Regels van de Filter:** de filters gebruiken gebiedsbron, gebiedsnaam, kwalificfiers, en waarden om criteria te bepalen. &#x200B; Bijvoorbeeld, toont de filter &quot;Mijn Projecten&quot;slechts huidige projecten waar de het programma geopende gebruiker deel van het projectteam uitmaakt. &#x200B;
* **Mening en Groepen:** de vertoningenbron en de naamincombinaties van het gebied van meningen in kolommen (b.v., &quot;eigenaarnaam&quot;), terwijl de groeperingen gegevens organiseren die op specifieke criteria (b.v., &quot;bedrijfsnaam&quot;) worden gebaseerd. &#x200B;
* **Wildcard Gebruik:** De Kaders in filters staan dynamische aanpassing, zoals het identificeren van het programma geopende gebruikers binnen een projectteam toe, die verpersoonlijking in het melden verbeteren. &#x200B;

## Snelle verwijzing naar componenten rapporteren

![&#x200B; een beeld van het scherm om een filter &#x200B;](assets/reporting-components-1.png) tot stand te brengen

**A - de bron van het Gebied**

De opties voor de veldbron zijn afhankelijk van het geselecteerde objecttype. Vaak is de veldbron het item in Workfront waartoe een bepaalde informatie (ook bekend als de veldnaam) behoort. Soms is de veldbron hetzelfde als het objecttype.
De veldbron bepaalt welke veldnamen beschikbaar zijn.

Voorbeelden: [!UICONTROL Project] , [!UICONTROL Task] , [!UICONTROL Issue] , [!UICONTROL Assigned To]

**B - de naam van het Gebied**

Veldnamen zijn stukken informatie die beschikbaar zijn over wat u als veldbron hebt geselecteerd.

Dit kunnen Workfront-velden zijn die u hebt ingevuld, velden van een aangepast formulier of gegevens die Workfront automatisch vastlegt.

Met veldnamen worden de opties voor het waardeveld bepaald.

Voorbeelden: [!UICONTROL Progress Status], [!UICONTROL Description], [!UICONTROL Planned Completion Date], Aangepaste formuliervelden

**C - de kwalificeertekens van de Filter**

Met filteraanduidingen kunt u de mogelijke resultaten beperken die onder de geselecteerde veldbron en veldnaam kunnen worden weergegeven.

Hiermee geeft u op hoe de veldbron en veldnaam betrekking hebben op het waardeveld.

Voorbeelden: gelijk, Bevat, null, kleiner dan

**D - Waarde**

De waarde is de informatie die is ingevoerd in het veld dat is opgegeven met de veldnaam.

Waardeopties worden bepaald door de bron en veldnaam van het veld.

Jokertekens voor gebruikers en datums kunnen worden gebruikt in de waarde en vrije-formuliertekst.

Voorbeelden: Nieuw, Huidig, $$TODAYbw, Beschrijving

>[!TIP]
>
>Voor hulp die specifieke gebiedsnamen in Workfront begrijpen, kijk in de [&#x200B; Verklarende woordenlijst van de terminologie van Adobe Workfront &#x200B;](https://experienceleague.adobe.com/docs/workfront/using/basics/workfront-terminology-glossary.html?lang=nl-NL).

