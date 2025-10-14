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
jira: KT-10093
exl-id: 6bd3a777-0ed8-4383-ad8e-f1238e334e78
source-git-commit: 4568e4e47b719e2dee35357d42674613112a9c43
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

<!--
this has the same content as the system administrator notification setup and mangement section of the email and inapp notificiations learning path
-->

<!--
add URL link in the note at the top of the LP
-->

# Gebeurtenismeldingen instellen

>[!NOTE]
>
>Vanwege een gefaseerde implementatie is de functionaliteit waarmee systeem- en groepsbeheerders gebeurtenismeldingen kunnen beheren, tijdelijk niet beschikbaar voor sommige [!DNL Workfront] -klanten. Volg dit artikel voor updates met betrekking tot de release: ontgrendel de configuratie van gebeurtenismeldingen voor groepen.

Systeembeheerders bepalen welke meldingen gebruikers moeten ontvangen via [!DNL Workfront] .

![[!UICONTROL Email Notifications] in het [!UICONTROL Setup] gebied &#x200B;](assets/admin-fund-notifications-1.png)

De lijst [!UICONTROL Event Notifications] wordt gegroepeerd op type. Voor elke vermelde gebeurtenismelding worden vijf gegevens weergegeven:

* **[!UICONTROL Active]—** Met de kolom [!UICONTROL Active] kunt u een melding in- of uitschakelen op systeemniveau.
* **[!UICONTROL Name]—** Dit is de naam van de melding binnen [!DNL Workfront] .
* **[!UICONTROL Description]—** De beschrijving verstrekt een korte verklaring van welke actie plaatsvond om een bericht teweeg te brengen of in antwoord op het ontvangen van het bericht moet worden genomen.
* **[!UICONTROL Email Subject]—** Wat zal aan de gebruiker in de onderwerpregel worden getoond wanneer e-mail naar gebruikers wordt verzonden.
* **[!UICONTROL Group Access]—** Ontgrendel berichten zodat zij door groepsbeheerders kunnen worden beheerd.

## Meldingen inschakelen

Als u meldingen op algemeen systeemniveau wilt beheren, moet u ervoor zorgen dat op de zoekbalk staat [!UICONTROL System Event Notifications] .

Schakel een specifiek bericht in om het beschikbaar te maken voor alle gebruikers door op de schakelknop te klikken, zodat het blauwe wordt weergegeven. Als het blauw verborgen is, is de melding uitgeschakeld.

![[!UICONTROL Active] column on [!UICONTROL Email Notifications] page &#x200B;](assets/admin-fund-notifications-2.png)

Zodra een gebeurtenisbericht wordt aangezet, worden de berichten verzonden onmiddellijk wanneer de gebeurtenis voorkomt.

## Groepsbeheerderscontrole toestaan

De beheerders van de groep kunnen toestemming, door systeembeheerders worden verleend, om de berichtlijst verder aan te passen die op hoe hun groepen en subgroups functioneren en wat hun werkschema&#39;s zijn.

![[!UICONTROL Group Access] column on [!UICONTROL Email Notifications] page &#x200B;](assets/ganotifications_01.png)

Om groepsbeheerders de mogelijkheid te geven om meldingen voor hun groepen en subgroepen te beheren, moeten de meldingen op systeemniveau worden ontgrendeld.

* Navigeer naar het tabblad Gebeurtenismeldingen op de pagina E-mailmeldingen.

* Zorg ervoor de onderzoeksbar meldt de Berichten van de Gebeurtenis van het Systeem.

* Ontgrendel één enkel bericht voor alle groepsbeheerders door de knevel in de kolom van de Toegang van de Groep te klikken zodat verschijnt het blauw.

* U kunt meerdere meldingen tegelijk ontgrendelen door het selectievakje links van elke melding in te schakelen en op het pictogram Ontgrendelen op de werkbalk boven de lijst te klikken.

![[!UICONTROL Group Access] column on [!UICONTROL Email Notifications] page &#x200B;](assets/ganotifications_02.png)

Vergrendel een ontgrendeld bericht door op de schakeloptie te klikken, zodat de grijstint wordt weergegeven. Meerdere meldingen vergrendelen door de selectievakjes in te schakelen en op het pictogram Ontgrendelen op de werkbalk te klikken.

![[!UICONTROL Group Access] column on [!UICONTROL Email Notifications] page &#x200B;](assets/ganotifications_03.png)

Ontgrendelde berichten worden weergegeven voor groepsbeheerders op hoofdniveau om te bepalen of dat bericht nodig is voor hun groepen en subgroepen. Subgroepen erven de berichtconfiguraties van hun hoogste oudergroep. ﻿


## Groepsmeldingen beheren

Zodra de systeembeheerder ontgrendelde meldingsopties heeft, kunnen de groepbeheerders de meldingen van een groep beheren vanaf de afzonderlijke pagina Groep door op Gebeurtenismeldingen in het menu van het linkerdeelvenster te klikken. Vervolgens kunt u meldingsopties activeren of deactiveren.

![[!UICONTROL Group Access] column on [!UICONTROL Email Notifications] page &#x200B;](assets/managegroupnotifications_01.png)

Systeembeheerders kunnen zo nodig de meldingen van een groep beheren via de pagina Meldingen door de groepsnaam in te voeren in de zoekbalk boven in het venster.

![[!UICONTROL Group Access] column on [!UICONTROL Email Notifications] page &#x200B;](assets/managegroupnotifications_02.png)

## Pro-tips

Er zijn enkele meldingen die [!DNL Workfront] aanbeveelt om deze beschikbaar te maken voor uw gebruikers.

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

<!--
learn more URLs
-->
