---
title: Begrijp het Logboek van de Controle van het Systeem
description: Leer hoe te om het logboek van de systeemcontrole te gebruiken om te herzien wanneer de veranderingen werden aangebracht en wanneer aan punten.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner, Intermediate
thumbnail: 10040.jpeg
jira: KT-10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
source-git-commit: 4568e4e47b719e2dee35357d42674613112a9c43
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Begrijp het logboek van de systeemcontrole

Het systeemcontrolelogboek is de beste manier van de systeembeheerder om de ontwikkelingen in [!DNL Workfront] in de gaten te houden. Beschouw het logboek als de bron van de waarheid voor wie wat heeft veranderd en wanneer.

Open het auditlogboek door naar de sectie [!UICONTROL Preferences] in het [!UICONTROL Setup] -gebied te gaan. Standaard worden gegevens van de laatste zeven dagen weergegeven. Wijzig de filtercriteria om gegevens van verschillende datumbereiken weer te geven.

Wanneer een gebruiker bepaalde handelingen uitvoert, worden deze door [!UICONTROL Workfront] vastgelegd in de [!UICONTROL Audit Logs] -sectie van het [!UICONTROL Setup] -gebied.

![[!UICONTROL Log Type] vervolgkeuzelijst op de [!UICONTROL Audit Logs] pagina in [!UICONTROL Setup]](assets/admin-fund-audit-log-1.png)

Elke geregistreerde of geregistreerde actie toont:

* Datum en tijdstip van de wijziging
* Het logtype
* De naam van de gebruiker die de handeling heeft voltooid
* Het object
* Alle details die aan de actie zijn gekoppeld
* Het IP-adres

![[!UICONTROL Audit Log] list &#x200B;](assets/admin-fund-audit-log-2.JPG)

## Het controlelogboek exporteren

Door de gegevens van het auditlogboek te exporteren, kunnen systeembeheerders de informatie delen met interne/externe accountants of beveiligingsspecialisten. Sommige organisaties vereisen dat bepaalde stammen worden bewaard om te voldoen aan de cyberbeveiligingsvoorschriften. Anderen hebben de informatie die in een veiligheidssysteem wordt ingevoerd voor analyse nodig.

Auditlogboeken kunnen worden geëxporteerd in een CSV-bestand (een bestand met komma&#39;s als scheidingsteken) dat kan worden geopend in een spreadsheettoepassing of normale teksteditor. Het exporteren is beperkt tot 50.000 rijen tegelijk. Gebruik de filters om de lijst te verkleinen als het totaal groter is dan 50.000.

![[!UICONTROL Export] op [!UICONTROL Audit Logs] page &#x200B;](assets/admin-fund-audit-log-3.png)

<!--
learn more URLs
Audit logs
Managing audit logs
-->
