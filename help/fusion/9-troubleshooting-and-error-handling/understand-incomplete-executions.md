---
title: Onvolledige uitvoeringen begrijpen
description: Leer welke onvolledige uitvoeringen zijn en hoe te om een fout te behandelen die in een onvolledige uitvoering in  [!DNL Adobe Workfront Fusion] resulteert.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9066
exl-id: 3b7bf669-4736-4ba5-bcec-0d3fe0b2ce74
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# Onvolledige uitvoeringen begrijpen

Onvolledige uitvoeringen kunnen worden opgeslagen in Workfront Fusion, waar ze later kunnen worden gecontroleerd en opgelost. Leer hoe u deze geweldige functie kunt gebruiken.

In deze video leert u:

* Onvolledige executies
* Hoe te om een fout te behandelen die in een onvolledige uitvoering resulteert

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12&learn=on&enablevpops)

## Fouten die leiden tot onvolledige uitvoeringen

Er zijn verschillende categorieën fouten die ertoe leiden dat onvolledige uitvoeringen worden opgeslagen.

Verschillende ontvangen fouttypen zijn afhankelijk van de API&#39;s waarmee u verbinding maakt. De fout kan een validatiefout zijn die het gevolg is van onvolledige of onjuiste gegevens, meestal als gevolg van een ontbrekend item dat wordt verwacht om alle gegevens in een module te kunnen verwerken. Of de fouten kunnen optreden als de eindbestemming niet beschikbaar is vanwege een tijdelijke of langdurige verbindingsfout (bijvoorbeeld tijdens verbinding met e-mail of externe FTP-server).

Als een fout op de eerste module in het scenario voorkomt, houdt de uitvoering onmiddellijk tegen en geen onvolledige uitvoering wordt opgeslagen.

Als een fout op een andere module voorkomt en er geen route van de foutenmanager in bijlage is, dan:

* Als het fouttype ConnectionError, RateLimitError, OutOfSpaceError of ModuleTimeoutError is, wordt een onvolledige uitvoeringsrecord met auto-retry opgeslagen.
* Als het fouttype DataError, InvalidConfigurationError, InvalidAccessTokenError, UnexpectedError, MaxFileSizeExceededError of MaxResultsExceededError is, wordt een onvolledige uitvoeringsrecord zonder auto-retry opgeslagen.
* Als het fouttype iets anders is dan hierboven, mislukt de uitvoering.

## Meer informatie? We raden het volgende aan:

[ de documentatie van de Fusie van Workfront ](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
