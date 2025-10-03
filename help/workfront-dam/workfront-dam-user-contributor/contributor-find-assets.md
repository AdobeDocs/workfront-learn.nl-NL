---
title: Begrijp het vinden van activa als contribuant
description: Leer hoe u naar elementen kunt zoeken, in mappen kunt zoeken, zoekresultaten kunt stroomlijnen, metagegevens en trefwoorden kunt gebruiken als zoekfilters in [!UICONTROL Workfront DAM] .
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# Begrijp het vinden van activa als contribuant

In deze video leert u hoe u:

* Middelen zoeken
* Zoeken in mappen
* Zoekresultaten stroomlijnen
* Metagegevens en trefwoorden gebruiken als zoekfilters
* Mapdetails weergeven
* Metagegevens en trefwoorden van elementen weergeven en bijwerken

>[!VIDEO](https://video.tv.adobe.com/v/335253/?quality=12&learn=on&enablevpops=1)

## Basiszoekcriteria

In een standaardzoekopdracht wordt gekeken naar bestandsnamen, metagegevensvelden, trefwoorden en inhoud van elementen (afhankelijk van het type element). De map bevat geen mapnaam.

De meeste zoekresultaten komen exact overeen. Een uitzondering op deze regel &quot;exact overeenkomend&quot; is wanneer de [!UICONTROL Workfront DAM] in het veld filename zoekt. [!UICONTROL Workfront DAM] retourneert gedeeltelijke overeenkomende bestandsnamen in plaats van alleen exacte overeenkomende bestandsnamen.

## Gebruikersoperatoren tijdens het zoeken

Hoewel de basiszoekfuncties vaak de benodigde middelen vinden, moet u soms extra zoekparameters gebruiken.

### Gedeeltelijke overeenkomsten

Als u een gedeeltelijke overeenkomst wilt zoeken, voegt u een sterretje toe aan de zoekterm. De asterisk mag alleen aan het einde van een woord worden gebruikt.

### AND, operator

Als u resultaten wilt zoeken die meerdere zoektermen bevatten, voert u AND tussen de woorden in. De woorden kunnen in om het even welke orde worden gevonden. Wanneer u in alle velden zoekt, zijn beide woorden mogelijk niet in hetzelfde veld aanwezig. Parijs EN toren zullen bijvoorbeeld middelen vinden die beide woorden in een van de velden hebben.

### OR, operator

Gebruik de operator OR om te zoeken naar elementen die een van de zoektermen bevatten. Parijs OF Boog vindt bijvoorbeeld elementen met een van de woorden, maar niet noodzakelijkerwijs beide.

### Woorden

Als u een exacte woordgroep wilt zoeken, gebruikt u dubbele aanhalingstekens om de woorden. Alle woorden worden samen en op volgorde gevonden. Met &quot;Eiffeltoren&quot; vindt u deze woorden bijvoorbeeld in de exacte volgorde.

### Negatieve operator

Als u een woord wilt uitsluiten van de zoekresultaten, plaatst u een minteken (-) vóór het woord. Zorg ervoor dat er geen ruimte is tussen het minteken en het woord. Als u bijvoorbeeld elementen wilt uitsluiten die het woord &#39;toren&#39; in de metagegevens hebben, kunt u uw zoekopdracht instellen als Parijs-toren.

### operator voor leeg veld

Als u elementen wilt zoeken die geen informatie bevatten in een specifiek metagegevensveld, voert u het veld dat u wilt zoeken in de volgende indeling in: ?[ xxxxx ]. Bijvoorbeeld, als u activa wilt vinden die geen toegewezen sleutelwoorden hebben, ga binnen?[ sleutelwoord ] op het onderzoeksgebied.
