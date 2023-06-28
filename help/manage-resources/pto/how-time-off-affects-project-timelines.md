---
title: De tijd van de tonen beïnvloedt projectchronologie
description: Zie wat er met een projecttijdlijn gebeurt wanneer de tijd van het plaatsen aan en uit is.
feature: Resource Management
type: Tutorial
role: Leader, User
level: Intermediate, Experienced
activity: use
team: Technical Marketing
jira: KT-10180
exl-id: 0f79dd8d-b7ce-4ee9-b211-23c8ed5d497c
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# Hoe tijd van invloed is op projecttijdlijnen

Of de tijd van een toegewezen gebruiker van factoren in de projectchronologie afhangt van een project dat geroepen plaatst [!UICONTROL User Time Off]. Deze instelling bepaalt of de tijd voor de primaire taakontvanger de geplande datums voor die taak voor het project aanpast.

Laten we kijken wat er gebeurt met een projecttijdlijn wanneer alle instellingen zijn geselecteerd—C[!UICONTROL onsider user time off in task durations] of [!UICONTROL Ignore user time off in task durations].

![Gebruikerstijd instellen](assets/toapt_01.png)

## Overweeg de gebruikerstijd in taakduur

Dit is de standaardinstelling van Workfront.

In dit voorbeeld heeft de primaire ontvanger voor de taak dagen vrij gemarkeerd op hun persoonlijke kalender.

![persoonlijke kalender](assets/toapt_02.png)

De projectmanager wil deze persoon aan een taak toewijzen die data heeft gepland die de tijd van de gebruiker weg overlappen.

![projecttaak met datums](assets/toapt_03.png)

Wanneer deze gebruiker aan de taak wordt toegewezen, passen de geplande data automatisch aan. De geplande voltooiingsdatum van de taak is nu enkele dagen verlengd om rekening te houden met de tijd van de gebruiker. Het is belangrijk om op te merken dat deze wijziging van invloed kan zijn op de geplande data van andere taken in het project en mogelijk op de geplande afsluitdatum van het project.

![projecttaak op tijd](assets/toapt_04.png)

## [!UICONTROL Ignore user time off in task durations]

Met deze optie blijven de geplande data van de taak zoals oorspronkelijk gepland, ook al heeft de primaire ontvanger tijdens de duur van die taak geen tijd meer.

Het teamlid heeft dagen vrij gemarkeerd op zijn kalender.

![pto-kalender met duidelijke datums](assets/toapt_05.png)

De projectmanager wijst hen een taak toe die de tijd weg overlapt. Zodra de gebruiker wordt toegewezen, blijven de taak geplande data zoals oorspronkelijk gepland.

![projecttaakdatums aanpassen](assets/toapt_06.png)

Om ervoor te zorgen dat het werk op tijd wordt gedaan, zou het nuttig kunnen zijn om een andere persoon toe te wijzen die aan de taak kan werken terwijl de oorspronkelijke ontvanger uit het bureau is.

## Pas het plaatsen op het projectniveau aan

U wijzigt als volgt de instelling voor de tijd van de gebruiker bij een project:

* Open het project door op de naam ervan te klikken in Workfront.

* Selecteren [!UICONTROL Edit] in het menu met drie punten in de paginakoptekst, rechts van de projectnaam.

* Naar de [!UICONTROL Project Settings] en zoek de [!UICONTROL User Time Off] veld.

* Selecteer de optie die u op dit project wilt toepassen — [!UICONTROL Consider user time off in task durations] of I[!UICONTROL gnore user time off in task durations].

* Klik op de knop [!UICONTROL Save] in de rechterbovenhoek van het venster.

![Overweeg de gebruikerstijd in taakduur](assets/toapt_07.png)


**Opmerking**: Deze instelling is niet beschikbaar wanneer u [!UICONTROL Project Details] in het linkerdeelvenstermenu van de projectpagina.

Een globale instelling hiervoor bestaat in de projectvoorkeuren in het dialoogvenster [!UICONTROL Setup] -menu. Deze instelling wordt beheerd door uw systeembeheerder. Groepbeheerders kunnen deze instelling mogelijk aanpassen voor de groepen die ze beheren.

Workfront raadt u aan deze instelling in te stellen op de manier waarop u wilt dat de meeste projecten binnen uw organisatie tijd kunnen afhandelen.

Het plaatsen kan ook in projectmalplaatjes, door de malplaatjedetails worden gebouwd.
