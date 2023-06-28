---
title: Voortgang proefdruk bijhouden
description: Leren gebruiken [!UICONTROL SOCD] indicatoren, de vooruitgang van het bewijs en verslagen om de vooruitgang van een bewijs in [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
jira: KT-10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# Voortgang proefdruk bijhouden

Als projectmanager, proefbeheerder of andere belanghebbende bij het beoordelings- en goedkeuringsproces wilt u de voortgang van uw proefdrukken bijhouden. U kunt dit doen met [!DNL Workfront’s] ingebouwd **voortgangsindicatoren** op de [!UICONTROL Documents] of door aangepaste rapporten te schrijven.

De voortgang van de proefdrukken weergeven in [!DNL Workfront], hebt u een licentie voor Overzicht, Werkprogramma of Revisie nodig en moet u een proefdrukgebruiker zijn. Als u twijfelt [!DNL Workfront] voldoet aan deze vereisten, raadpleegt u de systeembeheerder van het proefdruksysteem bij uw organisatie.

## Voortgang proefdruk bijhouden met [!UICONTROL SOCD] indicatoren en status van bewijs

Bekijk op hoog niveau hoe de proefdruk het beoordelings- en goedkeuringsproces doorloopt met het [!UICONTROL SOCD] pictogrammen in de [!UICONTROL Documents] lijst. Deze pictogrammen geven aan welke specifieke maatregelen op het bewijs zijn genomen.

![Een afbeelding van de [!UICONTROL Documents] lijst in een [!DNL  Workfront] met de [!UICONTROL SOCD] gemarkeerde pictogrammen.](assets/manage-proofs-socd.png)

De pictogrammen geven het werk aan dat op een bewijs is verricht vanaf het moment dat u het bewijs naar de ontvangers verzendt tot het moment dat zij een beslissing nemen over het bewijs.

* **S —** Het bewijs is naar de ontvangers verzonden.
* **O —** Het bewijs is geopend.
* **C —** Op het bewijs zijn opmerkingen gemaakt.
* **D —** Er is een besluit genomen over het bewijs (goedgekeurd, verworpen, enz.).

De kleuren geven aan of de handeling voltooid is of niet.

* **Wit —** De stap is nog niet uitgevoerd.
* **Groen —** De stap is voltooid.
* **Oranje —** De proefdrukdeadline is binnen 24 uur en de stap is niet uitgevoerd.
* **Rood —** De proefdrukdeadline is verstreken en de stap is niet uitgevoerd.

De [!UICONTROL SOCD] op de [!UICONTROL Documents] in het overzichtsvenster of in het dialoogvenster [!UICONTROL Document Details]is een overzicht op hoog niveau van de voortgang van het bewijs. [!DNL Workfront] configureert dit op basis van de ontvanger die de &quot;meest achterop&quot; in het proefdrukproces is.

Als er bijvoorbeeld drie revisoren/fiatteurs zijn en slechts twee van hen de bewijzen hebben bekeken en opmerkingen hebben gemaakt, dan [!UICONTROL SOCD] de pictogrammen geven aan dat het bewijs is verzonden ([!UICONTROL S]) en geopend ([!UICONTROL O]), maar er zijn geen opmerkingen gemaakt ([!UICONTROL C]).

Als u wilt weten hoe elke afzonderlijke proefdrukontvanger het doet, opent u de proefdrukworkflow. De algemene voortgang van de proefdrukken bevindt zich boven in het venster. Elk werkgebied heeft een eigen voortgangsindicator in de grijze balk.  En naast elke gebruiker is de voortgang van die persoon.

![Een afbeelding van de [!UICONTROL Proofing Workflow] van een document.](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## Proefstatus

De bewijsstatus is gebaseerd op de status van de proefontvangers van het werkgebied. De algemene proefdrukstatus is zichtbaar op het tabblad [!UICONTROL Documents] pagina, rechts van [!UICONTROL SOCD] indicatoren, zodat u gemakkelijk kunt zien of u een besluit over het bewijs hebt.

![Een afbeelding van de [!UICONTROL Documents] lijst in een [!DNL  Workfront] project met de algemene proefstatus gemarkeerd.](assets/manage-proofs-overall-status.png)

Deze proefdrukstatus geeft de algemene status van de proefdruk aan. Als twee ontvangers bijvoorbeeld het bewijs hebben goedgekeurd, wordt in hun individuele status het bewijs weergegeven [!UICONTROL Approved]. De derde ontvanger heeft echter nog geen beslissing genomen, zodat de status van de persoon [!UICONTROL Pending]. De algemene status wordt dan ook weergegeven als [!UICONTROL Pending].

Als de douanestatus voor uw organisatie werd gevormd, zullen die statussen worden gebruikt. Anders ziet u de volgende standaardstatusopties:

* [!UICONTROL Pending]
* [!UICONTROL Approved]
* [!UICONTROL Approved with Changes]
* [!UICONTROL Changes required]
* [!UICONTROL Not relevant]

Open het venster van de testwerkstroom om een proefdrukstatus te zien voor ontvangers aan wie de [!UICONTROL Reviewer & Approver] of [!UICONTROL Approver]proefrollen.

## Rapporten in [!DNL Workfront]

U kunt ook gebruikmaken van [!DNL Workfront’s] rapporteringsmogelijkheden om proefdrukken bij te houden terwijl ze het beoordelings- en goedkeuringsproces doorlopen.

Met een proefdrukgoedkeuringsrapport kunt u de openstaande goedkeuringen volgen om ervoor te zorgen dat de termijnen worden nageleefd.

![Afbeelding van een proefdrukgoedkeuringsrapport in [!DNL  Workfront].](assets/proof-approval-report.png)

Met een documentversierapport kunt u proefversies beheren en bijhouden.

![Een afbeelding van een documentversierapport in [!DNL  Workfront].](assets/document-version-report.png)

We raden u aan met uw [!DNL Workfront] adviseur om rapporten te creëren die aan de vereisten van uw organisatie voldoen. Sommige verslagen moeten bekend zijn met [!DNL Workfront’s] rapportage van de tekstmodus.

## Uw beurt

Bespreek met uw team of de systeembeheerder van het testsysteem welke rapportage u in Workfront gebruikt om te controleren of de workflows probleemloos werken.

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
