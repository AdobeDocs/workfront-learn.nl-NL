---
title: Proefverslagen
description: Leer hoe u de rapportmogelijkheden kunt gebruiken om de voortgang van de proefdrukken te beheren.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: report-on-proofs.png
jira: KT-10233
exl-id: 9a1a9e16-61cc-4f95-977a-8870b7fd0dda
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 0%

---

# Proefverslagen

[!DNL Workfront]Dankzij de functies voor digitale proefdrukken kunt u projecten en gerelateerde workflows voor revisie op één locatie beheren — [!DNL Workfront]. Verkrijg waardevol inzicht in het het proefdrukken werk dat met rapporttypes, gebiedsbronnen, en gebiedsnamen wordt gedaan die overzicht en goedkeuringsinformatie tonen.

We raden u aan met uw [!DNL Workfront] consultant om rapporten te maken die voldoen aan de vereisten van uw organisatie. Sommige verslagen moeten bekend zijn met [!DNL Workfront]rapportage van de tekstmodus.

Begin met deze standaard standaardrapporten om uw teams te helpen proefdrukken te beheren die door een evaluatie- en goedkeuringsproces in [!DNL Workfront].

## [!UICONTROL Proof Approval]

Met dit rapporttype kunt u uitstaande proefdrukken bijhouden om ervoor te zorgen dat de termijnen worden nageleefd.

![Selecteren [!UICONTROL Proof Approval] van de [!UICONTROL New Report] vervolgkeuzemenu](assets/proof-system-setups-proof-approval-report.png)

De opties voor weergave en filter omvatten [!UICONTROL decision date], [!UICONTROL proof approval], [!UICONTROL approver stage], [!UICONTROL workflow template], en [!UICONTROL requester information]. Bij rapportage in de tekstmodus kunt u een groep maken die de lijst indeelt op documentnaam. Zie [Basistekstmodus voor groepen begrijpen](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-groupings.html?lang=en).

Wanneer het schrijven van de rapporten van de proefdrukgoedkeuring, zorg ervoor u informatie met betrekking tot de recentste versie van de proefdrukken krijgt. [!DNL Workfront] U wordt aangeraden deze veldbron en veldnaam op te nemen in het filter:

**[!UICONTROL Proof Approval]>>[!UICONTROL Is Current Document Version]**

![Tabblad Filters in rapportbuilder](assets/proof-system-setups-proof-approval-report-is-current-version.png)

Dit is nuttig wanneer u over proefdrukken rapporteert die veelvoudige versies hebben zodat maakt het rapport van slechts de huidige versie van elk bewijs een lijst die goedkeuring vereist. Hiermee worden de eerdere versies uitgefilterd die u niet meer hoeft te bewerken.

## [!UICONTROL Document Version]

Met dit rapporttype kunt u versies beheren en bijhouden in [!DNL Workfront].

![Selecteren [!UICONTROL Document Version] van de [!UICONTROL New Report] vervolgkeuzemenu](assets/proof-system-setups-document-version-report.png)

De opties van de mening omvatten informatie van [!UICONTROL document version], [!UICONTROL document], [!UICONTROL entered by], [!UICONTROL proof approval status], [!UICONTROL proof creator], en [!UICONTROL document provider].

Groepen kunnen worden uitgevoerd door [!UICONTROL document version], [!UICONTROL entered by], [!UICONTROL proof approval status]of gegevens over de eigenaar van het bewijs.

Inclusief filters [!UICONTROL document version], [!UICONTROL access level], [!UICONTROL document], [!UICONTROL entered by], [!UICONTROL proof approval status], [!UICONTROL proof creator]en documentprovidergegevens.

U kunt de naam van het proefdrukstadium tonen dat momenteel voor elk document op het rapport met deze kolom in een mening actief is:

**[!UICONTROL Document Versions]>>[!UICONTROL Active Proof Stages]**

![Tabblad Filters in rapportbuilder](assets/proof-system-setups-active-proof-stages.png)

Als momenteel geen werkgebied actief is, is de kolom leeg.

Deze veldbron >> veldnaam is ook als filter beschikbaar in een rapport.

Gebruik de [!UICONTROL Proof Creator] de veldbron om informatie over de gebruiker te melden die de proef creeerde. Kies de optie [!UICONTROL Name] veldbron voor het weergeven van de naam van de maker van de proef in een weergave.

**[!UICONTROL Proof Creator]>>[!UICONTROL Name]**

Deze veldbron >> keuzelijst is ook beschikbaar als filter.

![Tabblad Filters in rapportbuilder](assets/proof-system-setups-proof-creator-name.png)

<!--
Learn More Icon
Learn how to create reports in [!DNL Workfront] with the Report Creation class.
Access to proofing functionality
-->
