---
title: Voorkeuren voor algemene standaardproblemen configureren
description: Leer hoe u voorkeuren voor uitgaven instelt voor omgezette uitgaven, werkelijke datums en toegang tot uitgaven.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: 3ded3fe9d8b97b1c11cb382f8088930842399c98
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---

# Algemene voorkeuren voor standaardproblemen configureren

Verschillende instellingen voor het hele systeem stellen standaardwaarden vast voor de manier waarop problemen zich in bepaalde omstandigheden gedragen [!DNL Workfront].

De beste praktijken moeten de globale gebreken zoals zij verlaten en projectmanagers toestaan om aanpassingen aan te brengen zij op het projectniveau of in projectmalplaatjes nodig hebben.

U kunt de algemene voorkeuren voor uitgaven aanpassen, maar u en uw [!DNL Workfront] consultant bespreekt welke instellingen nodig zijn voor de workflows, processen en rapportagebehoeften van uw organisatie. Uw consultant kan u ook helpen begrijpen wat er gebeurt als bepaalde instellingen worden gewijzigd.

Met de voorkeuren voor uitgaven kunnen systeembeheerders de opties bepalen wanneer uitgaven worden omgezet in taken of projecten, hoe feitelijke datums worden berekend en wie toegang krijgt tot het project wanneer er problemen worden toegewezen. Laten we eens kijken waar deze instellingen zich bevinden [!DNL Workfront].

## Voorkeuren voor geconverteerde uitgaven

Met deze instellingen bepaalt u wat er met een probleem gebeurt wanneer het wordt omgezet in een taak of een project in [!DNL Workfront].

![[!UICONTROL Tasks & Issues] voorkeurenvenster met [!UICONTROL Issues] sectie gemarkeerd](assets/admin-fund-issue-prefs-converting.png)

1. Klikken **[!UICONTROL Setup]** in de **[!UICONTROL Main Menu]**.
1. Breid uit **[!UICONTROL Project Preferences]** in het linkerdeelvenster van het menu.
1. Selecteren **[!UICONTROL Tasks & Issues]**.
1. Naar de **[!UICONTROL Issues]** sectie.
1. Klik op de gewenste opties.
1. Sla op wanneer u klaar bent.

Bekijk de opties in deze sectie, zodat u de juiste opties voor uw organisatie kunt kiezen.

* **[!UICONTROL Automatically update Resolvable Issue status when the status of the Resolving Object Changes]**

   Met deze instelling kunt u de resolutie van de oorspronkelijke uitgave correleren met de resolutie van het nieuwe object (taak of project).

   Als deze instelling is ingeschakeld (ingeschakeld), kunt u aangepaste uitgavestatussen maken die dezelfde statussleutel hebben als een taak of projectstatus. Wanneer de taak of het project (het oplosbare object) op de aangepaste status is ingesteld, wordt de wijziging ook weergegeven bij de status van de uitgave.

   Wanneer deze optie is uitgeschakeld, wordt de status van het oplossende object automatisch ingesteld op de standaardstatus in plaats van op aangepaste status.

   Deze instelling heeft alleen effect als &quot;[!UICONTROL Keep the original issue and tie its resolution to the task]&quot; moet zijn geselecteerd.

* **[!UICONTROL Keep the original issue and tie is resolution to the task/project]**

   Wanneer de uitgave wordt omgezet, vertelt dit [!DNL Workfront] om de originele uitgaven te behouden. De status van de uitgave verandert wanneer de status van de taak of het project wordt gewijzigd. Wanneer de taak of het project als voltooid is gemarkeerd, wordt het probleem gemarkeerd als opgelost.

   Als deze optie niet wordt gecontroleerd, wordt de originele kwestie geschrapt en slechts blijft de omgezette taak of het project.

   Dit het plaatsen beïnvloedt het melden van kwesties oorspronkelijk die op een project worden geregistreerd of die door een [!DNL Workfront] aanvraagwachtrij.

* **[!UICONTROL Allow Primary Contact to have access to the task/project]**

   Dit geeft de persoon die de originele kwestie creeerde toegang tot de taak of het project dat tijdens de omzetting wordt gecreeerd. Ze kunnen het werk beoordelen, updates uitvoeren en op de hoogte blijven van de voortgang.

* **[!UICONTROL Allow these settings to be changed during conversion]**

   Als deze optie is geselecteerd, betekent dit de standaardinstellingen voor &quot;[!UICONTROL Keep original issue]&quot; en &quot;[!UICONTROL Allow Primary Contact]&quot; kan worden gewijzigd door de gebruiker die de uitgave omzet. Schakel deze optie uit als u de standaardinstellingen ongewijzigd wilt laten.

<!---
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
--->

## Voorkeuren voor werkelijke datums

Er zijn meerdere typen datums die in de hele periode worden gebruikt [!DNL Workfront]. Werkelijke datums zijn een &#39;tijdstempel&#39; die [!DNL Workfront] wordt gegenereerd wanneer bepaalde statuswijzigingen optreden.

De [!UICONTROL Actual Start Date] tijdstempel wordt gemaakt wanneer de status van de uitgave verandert van Nieuw in een andere status. De [!UICONTROL Actual Completion Date] tijdstempel is het tijdstip waarop de status van de uitgave verandert in een status die aangeeft dat deze is gesloten.

Houd er rekening mee dat deze voorkeur de werkelijke datuminstellingen voor zowel taken als uitgaven bepaalt.

![[!UICONTROL Tasks & Issues] voorkeurenvenster met [!UICONTROL Actual Dates] sectie gemarkeerd](assets/admin-fund-issue-prefs-actual-dates.png)

1. Klikken **[!UICONTROL Setup]** in de **[!UICONTROL Main Menu]**.
1. Breid uit **[!UICONTROL Project Preferences]** in het linkerdeelvenster van het menu.
1. Selecteren **[!UICONTROL Tasks & Issues]**.
1. Naar de **[!UICONTROL Actual Dates]** sectie.
1. Selecteer de gewenste optie voor de **[!UICONTROL Actual Start Date]** — [!UICONTROL Now] (de huidige datum en tijd) of [!UICONTROL The Planned Start Date] (de [!UICONTROL Actual Start Date] komt overeen met de begindatum die is ingesteld in de uitgiftegegevens).
1. Selecteer nu de optie voor de **[!UICONTROL Actual Completion Date]** — [!UICONTROL Now] (de huidige datum en tijd) of [!UICONTROL The Planned Completion Date] (de [!UICONTROL Actual Start Date] komt overeen met de datum die is ingesteld in de uitgiftegegevens).
1. Sla op wanneer u klaar bent.


<!---
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
--->

## Toegang tot problemen

De [!UICONTROL Access] Met instellingen voor uitgaven bepaalt u welke toegang een gebruiker krijgt wanneer een uitgave in Workfront wordt toegewezen. Deze montages controleren toegang tot de kwestie zelf, naast toegang tot het project de kwestie wordt geassocieerd met.

Voordat u deze instellingen wijzigt, moet u eventuele workflows of processen met uw [!DNL Workfront] consultants en uw interne bestuursteam.

![[!UICONTROL Tasks & Issues] voorkeurenvenster met [!UICONTROL When someone is assigned to an ISSUE] sectie gemarkeerd](assets/admin-fund-issue-prefs-access-1.png)

1. Klikken **[!UICONTROL Setup]** in de **[!UICONTROL Main Menu]**.
1. Breid uit **[!UICONTROL Project Preferences]** in het linkerdeelvenster van het menu.
1. Selecteren **[!UICONTROL Tasks & Issues]**.
1. Naar de **[!UICONTROL Access]** en zoek naar de &quot;[!UICONTROL When someone is assigned to an ISSUE]&quot;.
1. Stel de gedeelde toegang voor de uitgave zelf in — [!UICONTROL View], [!UICONTROL Contribute], of [!UICONTROL Manage]. [!DNL Workfront] Het is raadzaam de geavanceerde opties ongewijzigd te laten.
1. Schakel het selectievakje in als de persoon aan wie de uitgave is toegewezen ook toegang tot het project moet hebben
1. Selecteer vervolgens de gedeelde toegang voor het project — [!UICONTROL View], [!UICONTROL Contribute], of [!UICONTROL Manage]. Terwijl u de [!UICONTROL Advanced Options], houdt u rekening met de workflows en toegangsbehoeften van uw organisatie.
1. Sla op wanneer u klaar bent.

![[!UICONTROL Access] venster weergeven [!UICONTROL Contribute] opties](assets/admin-fund-issue-prefs-access-2.png)

<!---
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
--->
