---
title: Beheer van bedrijfsmiddelen als contribuant begrijpen
description: Leer hoe u elementen beheert in [!UICONTROL Workfront DAM] om uw workflow te verbeteren.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8996
exl-id: a09d0b0e-2631-414e-87e6-385ddbeb5cd2
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Beheer van bedrijfsmiddelen als contribuant begrijpen

In deze video leert u hoe u:

* Het menu Bewerken gebruiken op een element
* Een vervaldatum instellen
* Meldingen weergeven
* Instellingen voor individuele meldingen opgeven
* Een elementversie uploaden
* Nieuwe map maken
* Een sjabloon voor metagegevens toepassen op een map
* Mapmachtigingen instellen

>[!VIDEO](https://video.tv.adobe.com/v/335256/?quality=12&learn=on&enablevpops=1)

## Hoe werken elementversies?

Een deel van uw werkschema kan het beheren van veelvoudige versies-of ronden, proefdrukken, herhalingen, wat u hen-van activa ook roepen. U kunt alle versies beheren via [!UICONTROL Workfront DAM] .

Het systeem maakt automatische versiebeheer van elementen mogelijk wanneer een bestand met dezelfde naam als een bestaand bestand naar dezelfde map wordt geüpload. Neem contact op met de systeembeheerder om te zien of deze functionaliteit is ingeschakeld.

Als de automatische versiecontrole wordt aangezet, zal een activa slechts versie als het in de omslag wordt geladen die het originele element houdt. Beide elementen moeten dezelfde bestandsnaam hebben. Als het element in een andere map wordt geladen, wordt het element als een nieuw bestand ingevoerd.
Als versiebeheer niet is ingeschakeld, wordt een bestand met dezelfde naam als een bestaand bestand geüpload als een nieuw bestand, ongeacht de map waarin het bestand is geplaatst. Dit kan ertoe leiden dat twee elementen met dezelfde naam in dezelfde map staan.

U kunt ook handmatig versies van een bepaald element uploaden. Klik op het bewerkingspictogram op het element en selecteer vervolgens **[!UICONTROL Upload new version]** .

Als u middelen publiceert met versies naar Brand Connect, ziet de gebruiker van Brand Connect alleen de nieuwste versie van het middel.

## Status en vervaldatum van map en middelen

Statussen zijn een andere manier om de toegang tot mappen en elementen in [!UICONTROL Workfront DAM] te beheren. Statussen kunnen worden gebruikt om bepaalde elementen of mappen te verbergen voor [!UICONTROL Brand Connect] -gebruikers of om een middel of map te verlopen zodat alleen de systeembeheerder deze kan openen.

* **[!UICONTROL Active]** - Wordt gebruikt voor elementen en mappen. Assets en mappen met de status [!UICONTROL Active] zijn zichtbaar voor alle gebruikers met machtigingen en kunnen worden gepubliceerd naar [!UICONTROL Brand Connect] . [!UICONTROL Active] wordt aangegeven met een groene stip op een element of map.
* **[!UICONTROL Inactive]** - Wordt gebruikt voor elementen en mappen. Assets en mappen met de status [!UICONTROL Inactive] zijn zichtbaar voor [!UICONTROL Workfront DAM] -gebruikers, maar niet in [!UICONTROL Brand Connect] . [!UICONTROL Inactive] wordt aangegeven met een rode stip op een element of map.
* **[!UICONTROL Unexpired]** - Wordt alleen gebruikt voor elementen. Dit is de standaardstatus van alle elementen. Niet-verlopen elementen die ook [!UICONTROL Active] zijn, zijn zichtbaar in de [!UICONTROL Brand Connect] .
* **[!UICONTROL Expired]** - Wordt alleen gebruikt voor elementen. Assets met de status [!UICONTROL Expired] kan alleen door de systeembeheerder worden gedownload. Verlopen elementen zijn zichtbaar/niet zichtbaar in de [!UICONTROL Brand Connect] , afhankelijk van systeemconfiguraties.
