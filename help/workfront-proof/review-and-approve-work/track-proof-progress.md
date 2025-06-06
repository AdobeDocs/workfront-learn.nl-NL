---
title: Voortgang proefdruk bijhouden
description: Leer hoe u [!UICONTROL SOCD] -indicatoren, voortgangsbewijzen en rapporten kunt gebruiken om de voortgang van een proefdruk in  [!DNL &#x200B; Workfront] bij te houden.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
jira: KT-10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: 8ad86921177da189503211635116146e886dbd17
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 0%

---

# Voortgang proefdruk bijhouden

Als projectmanager, bewijsmanager, of andere belanghebbende bij het overzicht en goedkeuringsproces, zult u de vooruitgang van uw proefdrukken willen volgen. U kunt dit met [!DNL Workfront's] ingebouwde **indicatoren van de proefvooruitgang** op de [!UICONTROL Documents] pagina doen of door douanerapporten te schrijven.

Als u de voortgang van de proefdrukken in [!DNL Workfront] wilt weergeven, moet u een licentie voor Overzicht, Werkprogramma of Revisie hebben en een proefdrukgebruiker zijn. Als u niet zeker bent dat uw [!DNL Workfront] profiel aan deze vereisten voldoet, controleer met de het proefdrukken systeembeheerder bij uw organisatie.

## Voortgang proefdrukken bijhouden met [!UICONTROL SOCD] -indicatoren en proefdrukstatus

Bekijk op een hoog niveau hoe de proefdruk het overzichts- en goedkeuringsproces doorloopt met de pictogrammen [!UICONTROL SOCD] in de lijst [!UICONTROL Documents] . Deze pictogrammen geven aan welke specifieke maatregelen op het bewijs zijn genomen.

![ een beeld van de [!UICONTROL Documents] lijst in een [!DNL &#x200B; Workfront] project met de [!UICONTROL SOCD] benadrukte pictogrammen.](assets/manage-proofs-socd.png)

De pictogrammen geven het werk aan dat op een bewijs is verricht vanaf het moment dat u het bewijs naar de ontvangers verzendt tot het moment dat zij een beslissing nemen over het bewijs.

* **S —** De proef is verzonden naar ontvangers.
* **O —** De proef is geopend.
* **C —** Commentaren zijn gemaakt op de proef.
* **D —** een besluit is genomen over het bewijs (goedgekeurd, verworpen, enz.).

De kleuren geven aan of de handeling voltooid is of niet.

* **Wit —** de stap is nog niet gebeurd.
* **Groen —** de stap is voltooid.
* **Oranje —** De proefdeadline is binnen 24 uur en de stap is niet gebeurd.
* **Rood —** de proefdeadline is overgegaan en de stap is niet gebeurd.

De lus [!UICONTROL SOCD] in de [!UICONTROL Documents] -lijst, in het overzichtsvenster of in [!UICONTROL Document Details] is een overzicht op hoog niveau van de voortgang van de proefdruk. [!DNL Workfront] configureert deze op basis van de ontvanger die de &quot;meest achterop&quot; in het proefdrukproces is.

Bijvoorbeeld, als er drie recensenten/fiatteurs zijn en slechts twee van hen de proef hebben bekeken en commentaren gemaakt, dan zullen de [!UICONTROL SOCD] pictogrammen tonen het bewijs is verzonden ([!UICONTROL S]) en geopend ([!UICONTROL O]) maar niet dat de commentaren zijn gemaakt ([!UICONTROL C]).

**Zodra een definitief besluit** (b.v., goedgekeurd of verworpen) op een bewijs wordt gemaakt, kunnen alle indicatoren SOCD groen voor gebruikers in dat stadium lijken, zelfs als individuele acties (zoals het openen van de proef of het maken van commentaren) niet werden uitgevoerd. Dit is een systeembreed gedrag dat is ontworpen om de voltooiing van het gehele werkgebied te weerspiegelen, niet de individuele betrokkenheid.

**voorafgaand aan een besluit dat** wordt geregistreerd, wijst elke indicator SOCD op daadwerkelijke gebruikersactiviteit (b.v., wit als geen actie werd genomen, groen als de actie werd voltooid). Na de beslissing gaat het systeem ervan uit dat de workflow is voltooid en worden alle indicatoren dienovereenkomstig bijgewerkt.

Als u wilt weten hoe elke afzonderlijke proefdrukontvanger het doet, opent u de proefdrukworkflow. De algemene voortgang van de proefdrukken bevindt zich boven in het venster. Elk werkgebied heeft een eigen voortgangsindicator in de grijze balk.  En naast elke gebruiker is de vooruitgang van dat individu.

![ een beeld van de [!UICONTROL Proofing Workflow] sectie van een document.](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## Proefstatus

De status van het bewijs is gebaseerd op de status van de proefontvangers van het werkgebied. De algemene proefdrukstatus is zichtbaar op de pagina [!UICONTROL Documents] , rechts van de indicatoren [!UICONTROL SOCD] , zodat u gemakkelijk kunt zien of u een beslissing hebt over de proefdruk.

![ een beeld van de [!UICONTROL Documents] lijst in een [!DNL &#x200B; Workfront] project met de algemene benadrukte proefdrukstatus.](assets/manage-proofs-overall-status.png)

Deze proefdrukstatus geeft de algemene status van de proefdruk aan. Als twee ontvangers de proefdruk bijvoorbeeld hebben goedgekeurd, wordt de status van de afzonderlijke ontvangers weergegeven [!UICONTROL Approved] . Nochtans, heeft de derde ontvanger nog geen besluit genomen, zodat is de status van die persoon [!UICONTROL Pending]. Daarom wordt de algemene status weergegeven als [!UICONTROL Pending] .

Als de douanestatus voor uw organisatie werd gevormd, zullen die statussen worden gebruikt. Anders ziet u de standaardopties voor de status:

* [!UICONTROL Pending]
* [!UICONTROL Approved]
* [!UICONTROL Approved with Changes]
* [!UICONTROL Changes required]
* [!UICONTROL Not relevant]

Open het het proefdrukken werkschemavenster om een proefdrukstatus voor ontvangers te zien toegewezen de [!UICONTROL Reviewer & Approver] of [!UICONTROL Approver] proefdrukrollen.

## Rapporten in [!DNL Workfront]

U kunt de rapportmogelijkheden van [!DNL Workfront's] ook gebruiken om proeven te volgen aangezien zij door het overzicht en goedkeuringsproces bewegen.

Met een proefdrukgoedkeuringsrapport kunt u de openstaande goedkeuringen volgen om ervoor te zorgen dat de termijnen worden nageleefd.

![ een beeld van een rapport van de proefgoedkeuring in [!DNL &#x200B; Workfront].](assets/proof-approval-report.png)

Met een documentversierapport kunt u proefversies beheren en bijhouden.

![ een beeld van een rapport van de documentversie in [!DNL &#x200B; Workfront].](assets/document-version-report.png)

We raden u aan om samen met uw [!DNL Workfront] -consultant rapporten te maken die voldoen aan de vereisten van uw organisatie. Sommige rapporten moeten vertrouwd zijn met de rapportage in de tekstmodus van [!DNL Workfront's] .

## Uw beurt

Bespreek met uw team of testsysteembeheerder welke rapportage u in Workfront gebruikt om te controleren of workflows probleemloos werken.

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
