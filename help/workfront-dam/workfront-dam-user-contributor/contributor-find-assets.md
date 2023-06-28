---
title: Middelen zoeken en ordenen in [!UICONTROL Workfront DAM]
description: Leer hoe u naar elementen kunt zoeken, in mappen kunt zoeken, zoekresultaten kunt stroomlijnen, metagegevens en trefwoorden kunt gebruiken als zoekfilters en meer in [!UICONTROL Workfront DAM].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# Medewerker: zoeken, middelen

In deze video leert u hoe u:

* Middelen zoeken
* Zoeken in mappen
* Zoekresultaten stroomlijnen
* Metagegevens en trefwoorden gebruiken als zoekfilters
* Mapdetails weergeven
* Metagegevens en trefwoorden van elementen weergeven en bijwerken

>[!VIDEO](https://video.tv.adobe.com/v/335253/?quality=12&learn=on)

## Basiszoekcriteria

In een standaardzoekopdracht wordt gekeken naar bestandsnamen, metagegevensvelden, trefwoorden en inhoud van elementen (afhankelijk van het type element). De map bevat geen mapnaam.

De meeste zoekresultaten komen exact overeen. Een uitzondering op deze regel &quot;exacte overeenkomst&quot; is wanneer de [!UICONTROL Workfront DAM] doorzoekt het filename gebied. [!UICONTROL Workfront DAM] retourneert niet alleen exacte overeenkomende bestandsnamen, maar retourneert slechts gedeeltelijke overeenkomende bestandsnamen.

## Gebruikersoperatoren tijdens het zoeken

Hoewel de basiszoekfuncties vaak de benodigde middelen vinden, moet u soms extra zoekparameters gebruiken.

### Gedeeltelijke overeenkomsten

Als u een gedeeltelijke overeenkomst wilt zoeken, voegt u een sterretje toe aan de zoekterm. De asterisk mag alleen aan het einde van een woord worden gebruikt.

### AND, operator

Als u resultaten wilt zoeken die meerdere zoektermen bevatten, voert u AND tussen de woorden in. De woorden staan in willekeurige volgorde. Wanneer u in alle velden zoekt, zijn beide woorden mogelijk niet in hetzelfde veld aanwezig. Parijs EN toren zullen bijvoorbeeld middelen vinden die beide woorden in een van de velden hebben.

### OR, operator

Gebruik de operator OR om te zoeken naar elementen die een van de zoektermen bevatten. Parijs OF Boog vindt bijvoorbeeld elementen met een van de woorden, maar niet noodzakelijkerwijs beide.

### Woorden

Als u een exacte woordgroep wilt zoeken, gebruikt u dubbele aanhalingstekens om de woorden. Alle woorden worden op volgorde gevonden. Met &quot;Eiffeltoren&quot; vindt u deze woorden bijvoorbeeld in de exacte volgorde.

### Negatieve operator

Als u een woord wilt uitsluiten van de zoekresultaten, plaatst u een minteken (-) vóór het woord. Zorg ervoor dat er geen ruimte is tussen het minteken en het woord. Als u bijvoorbeeld elementen wilt uitsluiten die het woord &#39;toren&#39; in de metagegevens hebben, kunt u uw zoekopdracht instellen als Parijs-toren.

### operator voor leeg veld

Als u elementen wilt zoeken die geen informatie bevatten in een specifiek metagegevensveld, voert u het veld dat u wilt zoeken in deze indeling in: ?[xxxxx]. Als u bijvoorbeeld elementen wilt zoeken waaraan geen trefwoorden zijn toegewezen, voert u in?[trefwoord] in het zoekveld.
