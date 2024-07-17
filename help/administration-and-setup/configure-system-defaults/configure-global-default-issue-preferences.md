---
title: Voorkeuren voor algemene standaardproblemen configureren
description: Leer hoe u voorkeuren voor uitgaven instelt voor omgezette uitgaven, werkelijke datums en toegang tot uitgaven.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---

# Algemene voorkeuren voor standaardproblemen configureren

Verschillende instellingen voor het gehele systeem stellen standaardinstellingen vast voor de manier waarop problemen zich in bepaalde omstandigheden in [!DNL Workfront] gedragen.

De beste praktijken moeten de globale gebreken zoals zij verlaten en projectmanagers toestaan om aanpassingen aan te brengen zij op het projectniveau of in projectmalplaatjes nodig hebben.

U kunt de algemene voorkeuren voor uitgaven aanpassen, maar u en uw [!DNL Workfront] -consultant kunt het beste bespreken welke instellingen nodig zijn voor de workflows, processen en rapportagebehoeften van uw organisatie. Uw consultant kan u ook helpen begrijpen wat er gebeurt als bepaalde instellingen worden gewijzigd.

Met de voorkeuren voor uitgaven kunnen systeembeheerders de opties bepalen wanneer uitgaven worden omgezet in taken of projecten, hoe feitelijke datums worden berekend en wie toegang krijgt tot het project wanneer er problemen worden toegewezen. Laten we eens kijken waar deze instellingen zich bevinden in [!DNL Workfront] .

## Voorkeuren voor geconverteerde uitgaven

Met deze instellingen bepaalt u wat er met een probleem gebeurt wanneer het wordt geconverteerd naar een taak of project in [!DNL Workfront] .

![[!UICONTROL Tasks & Issues] voorkeurenvenster met [!UICONTROL Issues] gemarkeerde sectie ](assets/admin-fund-issue-prefs-converting.png)

1. Klik op **[!UICONTROL Setup]** in de **[!UICONTROL Main Menu]** .
1. Vouw de sectie **[!UICONTROL Project Preferences]** in het linkermenu uit.
1. Selecteer **[!UICONTROL Tasks & Issues]** .
1. Blader naar de sectie **[!UICONTROL Issues]** .
1. Klik op de gewenste opties.
1. Sla op wanneer u klaar bent.

Bekijk de opties in deze sectie, zodat u de juiste opties voor uw organisatie kunt kiezen.

* **[!UICONTROL Automatically update Resolvable Issue status when the status of the Resolving Object Changes]**

  Met deze instelling kunt u de resolutie van de oorspronkelijke uitgave koppelen aan de resolutie van het nieuwe object (taak of project).

  Als deze instelling is ingeschakeld (ingeschakeld), kunt u aangepaste uitgavestatussen maken die dezelfde statussleutel hebben als een taak of projectstatus. Wanneer de taak of het project (het oplosbare object) op de aangepaste status is ingesteld, wordt de wijziging ook weergegeven bij de status van de uitgave.

  Wanneer deze optie is uitgeschakeld, wordt de status van het oplossende object automatisch ingesteld op de standaardstatus in plaats van op aangepaste status.

  Deze instelling heeft alleen effect als de optie &quot;[!UICONTROL Keep the original issue and tie its resolution to the task]&quot; is geselecteerd.

* **[!UICONTROL Keep the original issue and tie is resolution to the task/project]**

  Wanneer de uitgave wordt omgezet, vertelt dit [!DNL Workfront] om de originele kwesties te houden. De status van de uitgave verandert wanneer de status van de taak of het project wordt gewijzigd. Wanneer de taak of het project als voltooid is gemarkeerd, wordt het probleem gemarkeerd als opgelost.

  Als deze optie niet wordt gecontroleerd, wordt de originele kwestie geschrapt en slechts blijft de omgezette taak of het project.

  Deze instelling heeft invloed op de rapportage over problemen die oorspronkelijk zijn aangemeld bij een project of die worden gemeld via een [!DNL Workfront] aanvraagwachtrij.

* **[!UICONTROL Allow Primary Contact to have access to the task/project]**

  Dit geeft de persoon die de originele kwestie creeerde toegang tot de taak of het project dat tijdens de omzetting wordt gecreeerd. Ze kunnen het werk beoordelen, updates uitvoeren en op de hoogte blijven van de voortgang.

* **[!UICONTROL Allow these settings to be changed during conversion]**

  Wanneer geselecteerd, betekent deze optie de standaardmontages voor &quot;[!UICONTROL Keep original issue]&quot;en &quot;[!UICONTROL Allow Primary Contact]&quot;kunnen worden veranderd door de gebruiker die de kwestie omzet. Schakel deze optie uit als u de standaardinstellingen ongewijzigd wilt laten.

<!---
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
--->

## Voorkeuren voor werkelijke datums

[!DNL Workfront] bevat meerdere typen datums. Werkelijke datums zijn een &#39;tijdstempel&#39; die [!DNL Workfront] genereert wanneer bepaalde statuswijzigingen optreden.

De tijdstempel van [!UICONTROL Actual Start Date] wordt gemaakt wanneer de status van de uitgave verandert van Nieuw in een andere status. De tijdstempel van [!UICONTROL Actual Completion Date] is wanneer de status van de uitgave verandert in een status die aangeeft dat deze is gesloten.

Houd er rekening mee dat deze voorkeur de werkelijke datuminstellingen voor zowel taken als uitgaven bepaalt.

![[!UICONTROL Tasks & Issues] voorkeurenvenster met [!UICONTROL Actual Dates] gemarkeerde sectie ](assets/admin-fund-issue-prefs-actual-dates.png)

1. Klik op **[!UICONTROL Setup]** in de **[!UICONTROL Main Menu]** .
1. Vouw de sectie **[!UICONTROL Project Preferences]** in het linkermenu uit.
1. Selecteer **[!UICONTROL Tasks & Issues]** .
1. Blader naar de sectie **[!UICONTROL Actual Dates]** .
1. Selecteer de gewenste optie voor **[!UICONTROL Actual Start Date]** — [!UICONTROL Now] (de huidige datum en tijd) of [!UICONTROL The Planned Start Date] (de [!UICONTROL Actual Start Date] komt overeen met de begindatum die is ingesteld in de uitgiftegegevens).
1. Selecteer nu de optie voor **[!UICONTROL Actual Completion Date]** — [!UICONTROL Now] (de huidige datum en tijd) of [!UICONTROL The Planned Completion Date] (de [!UICONTROL Actual Start Date] komt overeen met de datum die is ingesteld in de uitgiftegegevens).
1. Sla op wanneer u klaar bent.


<!---
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
--->

## Toegang tot problemen

De instellingen in [!UICONTROL Access] voor uitgaven bepalen welke toegang een gebruiker krijgt wanneer een uitgave aan hem of haar wordt toegewezen in Workfront. Deze montages controleren toegang tot de kwestie zelf, naast toegang tot het project de kwestie wordt geassocieerd met.

Voordat u deze instellingen wijzigt, moet u eventuele workflows of procesbehoeften bespreken met uw [!DNL Workfront] -consultants en uw interne governanceteam.

![[!UICONTROL Tasks & Issues] voorkeurenvenster met [!UICONTROL When someone is assigned to an ISSUE] gemarkeerde sectie ](assets/admin-fund-issue-prefs-access-1.png)

1. Klik op **[!UICONTROL Setup]** in de **[!UICONTROL Main Menu]** .
1. Vouw de sectie **[!UICONTROL Project Preferences]** in het linkermenu uit.
1. Selecteer **[!UICONTROL Tasks & Issues]** .
1. Blader naar de sectie **[!UICONTROL Access]** en zoek naar de optie &quot;[!UICONTROL When someone is assigned to an ISSUE]&quot;.
1. Stel de deeltoegang in voor de uitgave zelf — [!UICONTROL View], [!UICONTROL Contribute] of [!UICONTROL Manage] . [!DNL Workfront] raadt u aan de geavanceerde opties ongewijzigd te laten.
1. Schakel het selectievakje in als de persoon aan wie de uitgave is toegewezen ook toegang tot het project moet hebben
1. Selecteer vervolgens de gedeelde toegang voor het project — [!UICONTROL View], [!UICONTROL Contribute] of [!UICONTROL Manage] . Houd bij het instellen van de [!UICONTROL Advanced Options] rekening met de workflows en toegangsbehoeften van uw organisatie.
1. Sla op wanneer u klaar bent.

![[!UICONTROL Access] venster met [!UICONTROL Contribute] opties ](assets/admin-fund-issue-prefs-access-2.png)

<!---
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
--->
