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
kt: 10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
source-git-commit: adf12d7846d2a1b4c32513a3955c080905044576
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# Begrijp het logboek van de systeemcontrole

Het logboek van de systeemcontrole is de beste manier van de systeembeheerder om een oog op te houden wat binnen gebeurt [!DNL Workfront]. Beschouw het logboek als de bron van de waarheid voor wie wat heeft veranderd en wanneer.

Open het auditlogboek door naar de [!UICONTROL Preferences] in de [!UICONTROL Setup] gebied. Standaard worden gegevens van de laatste zeven dagen weergegeven. Wijzig de filtercriteria om gegevens van verschillende datumbereiken weer te geven.

Wanneer een gebruiker bepaalde handelingen uitvoert, [!UICONTROL Workfront] registreert hen in [!UICONTROL Audit Logs] van de [!UICONTROL Setup] gebied.

![[!UICONTROL Log Type] vervolgkeuzemenu op het tabblad [!UICONTROL Audit Logs] pagina in [!UICONTROL Setup]](assets/admin-fund-audit-log-1.png)

Elke geregistreerde of geregistreerde actie toont:

* De datum en het tijdstip van de wijziging
* Het logtype
* De naam van de gebruiker die de handeling heeft voltooid
* Het object
* Alle details die aan de actie zijn gekoppeld
* Het IP-adres

![[!UICONTROL Audit Log] list](assets/admin-fund-audit-log-2.JPG)

## Het controlelogboek exporteren

Door de gegevens van het auditlogboek te exporteren, kunnen systeembeheerders de informatie delen met interne/externe accountants of beveiligingsspecialisten. Sommige organisaties vereisen dat bepaalde stammen worden bewaard om te voldoen aan de cyberbeveiligingsvoorschriften. Anderen hebben de informatie die in een veiligheidssysteem wordt ingevoerd voor analyse nodig.

Auditlogboeken kunnen worden geëxporteerd in een CSV-bestand (een bestand met komma&#39;s als scheidingsteken) dat kan worden geopend in een spreadsheettoepassing of normale teksteditor. Het exporteren is beperkt tot 50.000 rijen tegelijk. Gebruik de filters om de lijst te verkleinen als het totaal groter is dan 50.000.

![[!UICONTROL Export] aan [!UICONTROL Audit Logs] page](assets/admin-fund-audit-log-3.png)

<!---
learn more URLs
Audit logs
Managing audit logs
--->
