---
title: Gebeurtenismeldingen instellen
description: Leer hoe u kunt bepalen welke e-mail- en in-app-meldingen gebruikers ontvangen door gebeurtenismeldingen te beheren.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
thumbnail: 10093.jpeg
kt: 10093
exl-id: 6bd3a777-0ed8-4383-ad8e-f1238e334e78
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

<!---
this has the same content as the system administrator notification setup and mangement section of the email and inapp notificiations learning path
--->

<!---
add URL link in the note at the top of the LP
--->

# Gebeurtenismeldingen instellen

>[!NOTE]
>
>Vanwege een gefaseerde implementatie is de functionaliteit waarmee systeem- en groepsbeheerders gebeurtenismeldingen kunnen beheren, tijdelijk niet beschikbaar voor sommige [!DNL Workfront] klanten. Volg dit artikel voor updates met betrekking tot de release: Configuratie van gebeurtenismeldingen voor groepen ontgrendelen.

Systeembeheerders bepalen welke meldingen gebruikers moeten ontvangen via [!DNL Workfront].

![[!UICONTROL Email Notifications] in het [!UICONTROL Setup] gebied](assets/admin-fund-notifications-1.png)

De [!UICONTROL Event Notifications] lijst wordt gegroepeerd op type. Voor elke vermelde gebeurtenismelding worden vijf gegevens weergegeven:

* **[!UICONTROL Active]—** De [!UICONTROL Active] kunt u een melding in- of uitschakelen op systeemniveau.
* **[!UICONTROL Name]—** Dit is de naam van het bericht binnen [!DNL Workfront].
* **[!UICONTROL Description]—** De beschrijving geeft een korte uitleg van de maatregelen die zijn genomen om een aanmelding te doen ontstaan of die moeten worden genomen naar aanleiding van het ontvangen van de kennisgeving.
* **[!UICONTROL Email Subject]—** Wat wordt op de onderwerpregel aan de gebruiker weergegeven wanneer het e-mailbericht naar gebruikers wordt verzonden.
* **[!UICONTROL Group Access]—** Ontgrendel berichten zodat zij door groepsbeheerders kunnen worden beheerd.

## Meldingen inschakelen

Als u meldingen op algemeen systeemniveau wilt beheren, moet u ervoor zorgen dat op de zoekbalk [!UICONTROL System Event Notifications].

Schakel een specifiek bericht in om het beschikbaar te maken voor alle gebruikers door op de schakelknop te klikken, zodat het blauwe wordt weergegeven. Als het blauw verborgen is, is de melding uitgeschakeld.

![[!UICONTROL Active] kolom op [!UICONTROL Email Notifications] page](assets/admin-fund-notifications-2.png)

Zodra een gebeurtenisbericht wordt aangezet, worden de berichten verzonden onmiddellijk wanneer de gebeurtenis voorkomt.

## Groepsbeheerderscontrole toestaan

De beheerders van de groep kunnen toestemming, door systeembeheerders worden verleend, om de berichtlijst verder aan te passen die op hoe hun groepen en subgroups functioneren en wat hun werkschema&#39;s zijn.

![[!UICONTROL Group Access] kolom op [!UICONTROL Email Notifications] page](assets/ganotifications_01.png)

Om groepsbeheerders de mogelijkheid te geven om meldingen voor hun groepen en subgroepen te beheren, moeten de meldingen op systeemniveau worden ontgrendeld.

* Navigeer naar het tabblad Gebeurtenismeldingen op de pagina E-mailmeldingen.

* Zorg ervoor de onderzoeksbar meldt de Berichten van de Gebeurtenis van het Systeem.

* Ontgrendel één enkel bericht voor alle groepsbeheerders door de knevel in de kolom van de Toegang van de Groep te klikken zodat verschijnt het blauw.

* U kunt meerdere meldingen tegelijk ontgrendelen door het selectievakje links van elke melding in te schakelen en op het pictogram Ontgrendelen op de werkbalk boven de lijst te klikken.

![[!UICONTROL Group Access] kolom op [!UICONTROL Email Notifications] page](assets/ganotifications_02.png)

Vergrendel een ontgrendeld bericht door op de schakeloptie te klikken, zodat de grijstint wordt weergegeven. Meerdere meldingen vergrendelen door de selectievakjes in te schakelen en op het pictogram Ontgrendelen op de werkbalk te klikken.

![[!UICONTROL Group Access] kolom op [!UICONTROL Email Notifications] page](assets/ganotifications_03.png)

Ontgrendelde berichten worden weergegeven voor groepsbeheerders op hoofdniveau om te bepalen of dat bericht nodig is voor hun groepen en subgroepen. Subgroepen erven de berichtconfiguraties van hun hoogste oudergroep. ﻿


## Groepsmeldingen beheren

Zodra de systeembeheerder ontgrendelde meldingsopties heeft, kunnen de groepbeheerders de meldingen van een groep beheren vanaf de afzonderlijke pagina Groep door op Gebeurtenismeldingen in het menu van het linkerdeelvenster te klikken. Vervolgens kunt u meldingsopties activeren of deactiveren.

![[!UICONTROL Group Access] kolom op [!UICONTROL Email Notifications] page](assets/managegroupnotifications_01.png)

Systeembeheerders kunnen zo nodig de meldingen van een groep beheren via de pagina Meldingen door de groepsnaam in te voeren in de zoekbalk boven in het venster.

![[!UICONTROL Group Access] kolom op [!UICONTROL Email Notifications] page](assets/managegroupnotifications_02.png)

## Pro-tips

Sommige meldingen [!DNL Workfront] raadt u aan uw gebruikers ter beschikking te stellen.

Voor de meeste gebruikers:

* [!UICONTROL A predecessor of one of my tasks is completed]
* [!UICONTROL Someone includes me on a directed update]
* [!UICONTROL Someone comments on my work item]
* [!UICONTROL The due date changes on a task I’m assigned to]


Specifiek voor projectmanagers:

* [!UICONTROL A project I’m on becomes active]
* [!UICONTROL A project I own gets behind]
* [!UICONTROL An issue is added to a project I own]
* [!UICONTROL Milestone task is completed on a project I own]

<!---
learn more URLs
--->
