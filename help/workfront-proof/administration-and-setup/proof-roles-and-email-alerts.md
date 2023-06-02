---
title: Rollen en e-mailwaarschuwingen controleren
description: Leer hoe u de juiste proefdrukrollen en e-mailwaarschuwingen inschakelt, zodat proefontvangers toegang hebben tot proefdrukken en inzicht krijgen in het werk dat wordt uitgevoerd in [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: proof-roles-and-email-alerts.png
kt: 10177
exl-id: 15bfb18a-5392-4a91-a6a2-223f7ac30dc5
source-git-commit: 65bd26fefb280d12ec44a4923f6d96ac8d88d6fb
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Rollen en e-mailwaarschuwingen controleren

Dankzij de proefdrukrollen en e-mailwaarschuwingen kunt u de proefdrukworkflow verbeteren en ervoor zorgen dat ontvangers de juiste toegang hebben tot proefdrukken en inzicht hebben in het werk dat wordt uitgevoerd.

Laten we eens kijken naar een aantal basistevetoepassingen:

* **Proefrol —** Hiermee definieert u wat een gebruiker kan doen met een proefdruk (bijv. opmerking, markering, goedkeuring, enz.).
* **E-mailwaarschuwing —** E-mails die naar mensen worden verzonden in de proefwerkstroom wanneer er activiteit is op de proefdruk.

![Een afbeelding van de [!UICONTROL New Proof] met [!UICONTROL Proof role] en [!UICONTROL Email alerts] gemarkeerde kolommen.](assets/proof-roles-and-email-alerts.png)

Uw beheerder van het proefdruksysteem kan standaardproefdrukrollen en e-mailalarm voor de proefdrukgebruikers van uw organisatie plaatsen. Deze informatie kan bovendien worden ingebouwd in proefwerkstroomsjablonen (ook wel geautomatiseerde werkstroomsjablonen genoemd).

Het kan echter voorkomen dat u deze gegevens handmatig moet instellen tijdens het uploaden van een proefdruk.

[!DNL Workfront] geeft deze algemene aanbevelingen wanneer het toewijzen van proefdrukrollen aan proefontvangers:

* **Revisor en fiatteur —** Deze gebruikers kunnen zowel opmerkingen maken over bewijzen als een beslissing nemen (zoals goedgekeurd of afgewezen) op een bewijs. Gebruik deze proefdrukrol voor de belangrijkste interne en externe belanghebbenden in het evaluatieproces.
* **Recensent —** Sommige mensen in uw proefwerkstroom hoeven alleen opmerkingen te maken. Deze rol is ideaal voor hen. De revisorrol kan ook worden toegewezen aan [!DNL Workfront] gebruikers die proofs hoofdzakelijk uploaden of dienen als proef eigenaar maar anders geen deel van het proefdrukproces uitmaken.
* **Alleen-lezen —** Ideaal voor ontvangers die alleen de bewijzen hoeven te zien. [!UICONTROL Read Only] geeft toegang tot de weergave en staat geen opmerkingen toe.

[!DNL Workfront] biedt de volgende algemene aanbevelingen wanneer u e-mailwaarschuwingen toewijst aan proefontvangers:

* **Definitief besluit —** Dit stuurt een e-mail wanneer de laatste persoon een beslissing neemt over het bewijs. Wijs dit toe aan de persoon die de proefdrukwerkstroom controleert. Dit kan een proefdrukmanager, eigenaar van proefdrukken, maker van proefdrukken, projectmanager of andere [!DNL Workfront] gebruiker. [!DNL Workfront] Deze waarschuwing wordt aanbevolen wanneer een basisworkflow wordt gebruikt, zodat de persoon die het bewijs controleert weet dat alle beslissingen zijn genomen.
* **Besluiten —** Hierdoor worden waarschuwingen verzonden, aangezien elke belanghebbende een besluit neemt over de bewijskracht. Deze optie is het beste als u een geautomatiseerde workflow gebruikt, met verschillende beslissingen. Wijs dit toe aan de persoon die de proefdrukworkflow controleert. Dit kan een proefdrukmanager, eigenaar van proefdrukken, maker van proefdrukken, projectmanager of andere [!DNL Workfront] gebruiker.
* **Uitgeschakeld —** Gebruik deze optie voor gebruikers die een proefdruk maken van gasten om het aantal e-mails dat ze over de proefdruk ontvangen, te beperken. Ontvangers krijgen nog steeds een melding over nieuwe proefdrukken, nieuwe versies en late proefdrukken, plus [!DNL Workfront] gebruikers ontvangen directe berichten die in een proefdrukcommentaar zijn gemaakt met @username en gastontvangers met @e-mailadres.

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
