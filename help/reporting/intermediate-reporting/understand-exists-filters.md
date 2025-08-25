---
title: BESTAANDE filters begrijpen
description: Leer wat een filter EXISTS is, wat het voor u kan doen, en hoe u één van kras kunt bouwen. Zie ook veel nuttige voorbeelden van EXISTS-filters.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Intermediate
jira: KT-1880
last-substantial-update: 2025-08-25T00:00:00Z
doc-type: video
source-git-commit: 7be0b8cce9cba04927d6704d0009b482bbcf4b41
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 0%

---

# BESTAANDE filters begrijpen

BESTAANDE filters zijn geavanceerd, de filters van de tekstwijze, die ons toestaan om rond de 2 lijst/gebied sprongbeperking in een standaard rapportbouwer te werken. Of ze kunnen worden gebruikt om objecten in het systeem te identificeren waarvoor geen specifieke relatievoorwaarde bestaat via NOTEXISTS.

In deze video leert u hoe u een EXISTS-filter kunt maken om &quot;Goedkeuring proef voor huidige projecten&quot; te zien in een rapport met proefdrukgoedkeuringen.

Voor een meer diepgaande analyse op hoe BESTAAT de functie, gelieve [ te zien de complexe filters van de Wijze van de Tekst gebruikend EXISTS verklaringen ](https://experienceleague.adobe.com/nl/docs/workfront/using/reporting/reports/text-mode/create-complex-text-mode-filters-using-exists-statements) documentatie creëren.

>[!VIDEO](https://video.tv.adobe.com/v/3471181/?quality=12&learn=on&enablevpops)

## Voorbeelden van bestaande filters

### Projectrapport bestaat

Dit gebruikt de taak als het verbinden voorwerp, door projectID te vergelijken die op het taakniveau wordt gevonden en het aan het gebied van identiteitskaart van het projectniveau aan te passen. Hierdoor kunnen de toewijzingsgebruikers op de taak worden vergeleken met een jokerteken $$USER.ID. Dit resulteert in het terugkeren van slechts projecten waar de het bekijken gebruiker aan wordt toegewezen
taak, ongeacht of zij de primaire ontvanger zijn of niet.

```
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:assignmentsUsersMM:ID=$$USER.ID
EXISTS:A:assignmentsUsersMM:ID_Mod=in
EXISTS:A:projectID=FIELD:ID
```


Dit gebruikt de kwestie (optask) als het verbinden voorwerp, door projectID ook te vergelijken die op het (optask) niveau wordt gevonden en dat aan het gebied van identiteitskaart van het projectniveau aan te passen. Dit controleert dan om te zien of hebben om het even welke kwesties (optasks) een ingangsdatum binnen de gespecificeerde spanwijdte. In dit geval zou elk project worden teruggegeven dat
had geen kwestie (optask) het programma geopend in een het rollen voorbije 30 dagen, toe te schrijven aan NOTEXISTS.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=OPTASK
EXISTS:A:entryDate=$$TODAY
EXISTS:A:entryDate_Mod=between
EXISTS:A:entryDate_Range=$$TODAY-30d
EXISTS:A:projectID=FIELD:ID
```

### Sjabloonrapport bestaat

Dit filter zal alle malplaatjes tonen die niet zijn gebruikt om of een project tot stand te brengen of aan een project in het afgelopen jaar in bijlage zijn geweest. Één voorbehoud is dat om te weten te komen of een malplaatje als gehechtheid werd gebruikt, het afhankelijk is van dat malplaatje dat taken in het heeft.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:entryDate=$$TODAY-1y
EXISTS:A:entryDate_Mod=gte
EXISTS:A:templateTask:templateID=FIELD:ID
EXISTS:B:$$EXISTSMOD=NOTEXISTS
EXISTS:B:$$OBJCODE=PROJ
EXISTS:B:entryDate=$$TODAY-1y
EXISTS:B:entryDate_Mod=gte
EXISTS:B:templateID=FIELD:ID
```

### Taakrapport bestaat

Dit gebruikt de lijst van de Gebruiker als het verbinden voorwerp, verbindend door de taken taskID en de taken identiteitskaart Dit controleert dan de teaminzameling van IDs aan gebruikersTeam IDs, die de taak terugkeren als om het even welke wijzers op het zelfde team zoals de het bekijken gebruiker zijn.

```
EXISTS:1:$$OBJCODE=USER
EXISTS:1:teams:ID=$$USER.teamIDs
EXISTS:1:userAssignments:taskID=FIELD:ID
```

### Gebruikersrapport bestaat

Hiermee worden alle gebruikers geretourneerd die de afgelopen 3 weken geen update hebben geplaatst. Dit gebruikt het notitieobject om de tussenruimte te overbruggen en vergelijkt de ownerID met een gebruikers-id. Vervolgens wordt die gebruiker geretourneerd als geen enkele notitie die eigendom is van deze gebruiker een ingangsdatum heeft van meer dan drie weken geleden.

```
EXISTS:A:$$OBJCODE=NOTE
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:ownerID=FIELD:ID
EXISTS:A:entryDate=$$TODAY-3w
EXISTS:A:entryDate_Mod=gt
```

Hiermee worden alle gebruikers geretourneerd die zich de afgelopen week niet hebben aangemeld. Dit gebruikt een uiterst gelijkaardige methode aan het bovenstaande voorbeeld, maar in plaats daarvan gebruikt de informatie van de uureigenaar en de ingangsdatum van het uur om te baseren wat de gebruikers het terugkeert.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=HOUR
EXISTS:A:entryDate=$$TODAY-1w
EXISTS:A:entryDate_Mod=gte
EXISTS:A:ownerID=FIELD:ID
```

In een gebruikersrapport, toon een lijst van gebruikers die het lusje van de Mensen van een project aanpast.

```
EXISTS:1:$$OBJCODE=PRTU
EXISTS:1:projectID=<projectID>
EXISTS:1:userID=FIELD:ID
```

### Rapport voor categorie (aangepast formulier) bestaat

Deze tekst zal u een lijst van alle projectvormen geven die helemaal niet aan een project zijn gebruikt. Dit moet worden gebruikt in combinatie met het objecttype van het formulier waarop we ons richten. Dus in dit geval is PROJ de focus, dus moeten we de callouts opnemen in de regels objTypes. Dit kan worden gebruikt
voor andere objecttypen door de aan objectcode gerelateerde onderdelen te wijzigen. Hiermee controleert u de verzameling projecten in bijgevoegde formulieren, de weergegeven formulieren en retourneert u als er geen overeenkomst is.

```
EXISTS:A:$$OBJCODE=PROJ
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:objectCategories:categoryID=FIELD:ID
objTypes=PROJ
objTypes_Mod=in
```

### Parameterrapport (aangepast veld) bestaat

Hiermee wordt een aangepast veld geretourneerd dat momenteel niet is gekoppeld aan een aangepast formulier in het systeem.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```

### Rapport bestaat

Dit zal om het even welk rapport terugkeren gebruikend een specifieke waarde in zijn filters.

```
EXISTS:1:$$OBJCODE=UIFT
EXISTS:1:ID=FIELD:filterID
EXISTS:1:preference:value=<value here>
EXISTS:1:preference:value_Mod=cicontains
```

Dit retourneert elk rapport dat aan een dashboard is gekoppeld.

```
EXISTS:A:$$OBJCODE=PRTBSC
EXISTS:A:internalSectionID=FIELD:ID
EXISTS:A:portalTab:ID_Mod=notblank
```

### Bewijs van goedkeuring bestaat

Dit zou alleen proefgoedkeuringen teruggeven voor projecten met de huidige status. Dit gebruikt het voorwerp van het Document om de hiaat van proefgoedkeuring aan project te overbruggen door currentVersionID aan documentVersionID te controleren, van daar springen wij aan de projectstatus.

```
EXISTS:1:$$OBJCODE=DOCU
EXISTS:1:currentVersionID=FIELD:documentVersionID
EXISTS:1:project:status=CUR
EXISTS:1:project:status_Mod=in
```
