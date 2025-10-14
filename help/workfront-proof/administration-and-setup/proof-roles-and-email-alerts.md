---
title: Rollen en e-mailwaarschuwingen controleren
description: Leer hoe te om juiste proefdrukrollen en e-mailalarm toe te laten zodat hebben de proefontvangers toegang tot proef en zicht in het werk dat in  [!DNL &#x200B; Workfront] wordt gedaan.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: proof-roles-and-email-alerts.png
jira: KT-10177
exl-id: 15bfb18a-5392-4a91-a6a2-223f7ac30dc5
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Rollen en e-mailwaarschuwingen controleren

Dankzij de proefdrukrollen en e-mailwaarschuwingen kunt u de proefdrukworkflow verbeteren en ervoor zorgen dat ontvangers de juiste toegang hebben tot proefdrukken en inzicht hebben in het werk dat wordt uitgevoerd.

Laten we eens kijken naar een aantal basistevetoepassingen:

* **rol van het Bewijs -** bepaalt wat een gebruiker met een proef (b.v., commentaar, prijsverhoging, keurt goed, enz.) kan doen.
* **e-mailalarm —** E-mails die naar mensen in het proefdrukwerkschema worden verzonden wanneer er activiteit op de proef is.

![&#x200B; een beeld van het [!UICONTROL New Proof] venster met de [!UICONTROL Proof role] en [!UICONTROL Email alerts] benadrukte kolommen.](assets/proof-roles-and-email-alerts.png)

Uw beheerder van het proefdruksysteem kan standaardproefdrukrollen en e-mailalarm voor de proefdrukgebruikers van uw organisatie plaatsen. Deze informatie kan bovendien worden ingebouwd in proefwerkstroomsjablonen (ook wel geautomatiseerde werkstroomsjablonen genoemd).

Het kan echter voorkomen dat u deze gegevens handmatig moet instellen tijdens het uploaden van een proefdruk.

[!DNL Workfront] biedt de volgende algemene aanbevelingen wanneer u proefdrukrollen toewijst aan proefontvangers:

* **Recensent &amp; fiatteur -** Deze gebruikers kunnen zowel commentaren op proef maken als een besluit (zoals goedgekeurd of verworpen) op een bewijs nemen. Gebruik deze proefdrukrol voor de belangrijkste interne en externe belanghebbenden in het evaluatieproces.
* **Recensent —** Sommige mensen in uw proefwerkschema moeten slechts commentaren maken, is deze rol ideaal voor hen. De revisorrol kan ook worden toegewezen aan [!DNL Workfront] -gebruikers die in eerste instantie proefdrukken uploaden of als eigenaar van een proefdruk fungeren, maar die anders geen deel uitmaken van het proefdrukproces.
* **las slechts —** Ideaal voor ontvangers die slechts de proef hoeven te zien. [!UICONTROL Read Only] geeft toegang tot de weergave en staat geen opmerkingen toe.

[!DNL Workfront] biedt de volgende algemene aanbevelingen wanneer u e-mailwaarschuwingen toewijst aan proefontvangers:

* **Definitief besluit —** dit verzendt een e-mail wanneer de laatste persoon een besluit over het bewijs neemt. Wijs dit toe aan de persoon die de proefdrukwerkstroom controleert. Dit kan een proefdrukmanager, eigenaar van proefdrukken, maker van proefdrukken, projectmanager of andere [!DNL Workfront] gebruiker zijn. [!DNL Workfront] raadt deze waarschuwing aan als u een standaardworkflow gebruikt, zodat de persoon die de proefdruk controleert weet dat alle beslissingen zijn genomen.
* **Besluiten —** dit verzendt alarm aangezien elke het proefdrukken werkschemabelanghebbende een besluit over de proef neemt. Deze optie is het beste als u een geautomatiseerde workflow gebruikt, met verschillende beslissingen. Wijs dit toe aan de persoon die de proefdrukworkflow controleert. Dit kan een proefdrukmanager, eigenaar van proefdrukken, maker van proefdrukken, projectmanager of andere [!DNL Workfront] gebruiker zijn.
* **Gehandicapten —** Gebruik dit voor gastproefproefgebruikers om het aantal e-mails te beperken zij over de proef ontvangen. Ontvangers krijgen nog steeds een melding over nieuwe proefdrukken, nieuwe versies en recente proefdrukken, plus [!DNL Workfront] -gebruikers ontvangen directe berichten die in een proefdrukopmerking zijn gemaakt met @username en gastontvangers met @e-mailadres.

## Uw beurt

1. Meld u aan bij Workfront en maak gebruikers die proefdrukken maken die u nog niet hebt gemaakt. Stel het profiel voor proefdrukmachtigingen in de gebruikersinstellingen in op basis van de rol die de persoon in proefdrukwerkstromen zal spelen.
1. Voor gebruikers die al zijn gemaakt, bewerkt u de instellingen om zo nodig het profiel voor proefdrukmachtigingen aan te passen.
1. Open het gebied met instellingen voor proefdrukken en ga naar het tabblad Gebruikers. Controleer de persoonlijke instellingen voor uw gebruikers: taal, tijdzone, datumnotatie, standaardproefdrukrol en standaard-e-mailwaarschuwing. Dit is belangrijk als deze gebruikers zijn gemaakt voordat de standaardwaarden van het algemene systeem zijn ingesteld.

<!--
Download the proof role and email alert guides to have on hand as you start uploading proofs and assigning proof recipients.
-->

<!--
## Learn more
* Notifications for proof comments and decisions
-->

<!--
## Guides
* Proof roles
* Email alerts
-->
