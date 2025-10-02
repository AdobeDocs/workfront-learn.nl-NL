---
title: Basistekstmodus voor groepen begrijpen
description: Leer over tekstwijze, camel geval, en één of andere basistekstwijze die u in uw rapportgroepen in Workfront kunt gebruiken.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2025-08-12T00:00:00Z
jira: KT-11369
exl-id: 5f45c64f-a22b-4983-91fd-9a1939f99fb1
doc-type: video
source-git-commit: 1fafcafb173ceb4115612e1c33ca36564c7a6c3d
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# Basistekstmodus voor groepen begrijpen

>[!PREREQUISITES]
>
>* [&#x200B; Begrijp rapporteringselementen &#x200B;](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=en)
>* [&#x200B; Begrijp het melden componenten &#x200B;](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=en)
>* [&#x200B; creeer een basisgroepering &#x200B;](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/create-a-basic-grouping.html?lang=en)


>[!TIP]
>
>* Om een diepgaander inzicht in tekstwijze te verkrijgen adviseren wij het letten op de geregistreerde webinar gebeurtenis [&#x200B; vragen de Deskundige - Inleiding aan de Wijze van de Tekst die &#x200B;](https://experienceleague.adobe.com/en/docs/events/classics/reporting-and-dashboards/introduction-to-text-mode-reporting) meldt, die één uur in lengte is.
>* Om nog meer over tekstwijze te leren adviseren wij het letten op [&#x200B; Geavanceerde het melden &#x200B;](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) leerprogramma&#39;s, die samen vijf en een half uur in lengte zijn.
>* Klik hier voor toegang [[!UICONTROL API Explorer] &#x200B;](https://developer.adobe.com/workfront/api-explorer/)

In deze video leert u:

* Welke tekstmodus is ingesteld
* Wat kamelendoosje is
* Sommige _blokken van de tekstwijze_ u kunt in uw rapportgroeperingen gebruiken

>[!VIDEO](https://video.tv.adobe.com/v/3410641/?quality=12&learn=on)

## De activiteiten van de &quot;Begrijpen basistekstwijze voor groeperingen&quot;

### Taak - 4 ouders groeperen

In de volgende tekstmodus worden taken gegroepeerd op maximaal vier niveaus van bovenliggende items en blijven bovenliggende items die niet bestaan leeg.

```
textmode=true
group.0.name=Parents
group.0.valueexpression=CONCAT({parent}.{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{name}),"",", "),IF(ISBLANK({parent}.{name}),"No parent",{parent}.{name}))
group.0.linkedname=parent
group.0.namekeyargkey.0=parent
group.0.namekeyargkey.1=name
group.0.valueformat=string
```

![&#x200B; het schermbeeld dat van A projecttaken toont die door 4 ouders &#x200B;](assets/4-parents-grouping.png) worden gegroepeerd


### Taak - Percentage volledige groepering

In de volgende tekstmodus worden taken gegroepeerd op basis van het percentage dat is voltooid. Taken worden gegroepeerd in een van de volgende categorieën:

* 0%
* 1% tot 25%
* 26% tot 50%
* 51% tot 75%
* 76% tot 99%
* 100%

```
group.0.linkedname=direct
group.0.namekey=percentComplete
group.0.valueexpression=IF({percentComplete}<1,"0%",IF({percentComplete}<26,"1% to 25%",IF({percentComplete}<51,"26% to 50%",IF({percentComplete}<76,"51% to 75%",IF({percentComplete}<100,"76% to 99%",IF({percentComplete}=100,"100","***"))))))
group.0.valueformat=doubleAsString
textmode=true
```

![&#x200B; het schermbeeld dat van A projecttaken toont die door percent volledig &#x200B;](assets/percent-complete-grouping.png) worden gegroepeerd

### Taak - statusEquatesWith, dan status

In de volgende tekstmodus worden taken gegroepeerd op statusEquatesWith en vervolgens op status.

```
group.0.enumclass=com.attask.common.constants.TaskStatusEnum
group.0.enumtype=TASK
group.0.linkedname=direct
group.0.name=State
group.0.type=enum
group.0.valuefield=statusEquatesWith
group.0.valueformat=val
group.1.enumclass=com.attask.common.constants.TaskStatusEnum
group.1.enumtype=TASK
group.1.linkedname=direct
group.1.namekey=status
group.1.type=enum
group.1.valuefield=status
group.1.valueformat=val
textmode=true
```

![&#x200B; het schermbeeld dat van A projecttaken toont die door statusEquatesWith &#x200B;](assets/status-equates-with.png) worden gegroepeerd


### Goedkeuring proef - groep per projectnaam

```
group.0.valueformat=HTML
group.0.valuefield=documentVersion:document:project:name
group.0.displayname=Project Name
```

![&#x200B; het schermbeeld dat van A goedkeuringen van het Bewijs toont die door projectnaam &#x200B;](assets/proof-approvals-grouped-by-project-name.png) worden gegroepeerd


### Goedkeuring proefdrukken - Groeperen op documentnaam

```
group.0.displayname=Document Name
group.0.valuefield=documentVersion:document:name
group.0.valueformat=HTML
```

![&#x200B; het schermbeeld dat van A goedkeuringen van het Bewijs toont die door projectnaam &#x200B;](assets/proof-approvals-grouped-by-doc-name.png) worden gegroepeerd

