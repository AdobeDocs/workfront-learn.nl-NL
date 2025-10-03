---
title: Geavanceerde samenvoegingsanalyse
description: Leer hoe te om de Webdienst te roepen om details over veelvoudige landen terug te keren en bevolking te identificeren, gegroepeerd door subregio, allen in  [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9040
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---

# Geavanceerde samenvoegingsanalyse

Bel een webservice om details over meerdere landen te retourneren en de totale bevolking van alle landen, gegroepeerd per subregio, te identificeren.

![&#x200B; een beeld van het scenario van de Fusie &#x200B;](assets/iteration-and-aggregation-3.png)

## Geavanceerde samenvoegingsanalyse

Workfront raadt u aan om de video met een doorlichting te bekijken voordat u probeert de oefening opnieuw te maken in uw eigen omgeving.

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12&learn=on&enablevpops=1)

## URL&#39;s uitvoeren

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`



## Versterking van het aggregatiebeginsel

Wanneer een module meerdere bundels uitvoert, voert elke module daarna elke bundel uit.

Om dit te verhinderen, voeg een aggregator na een module toe die potentieel veelvoudige bundels produceert.

U zult een schaduw rond om het even welk segment in uw scenario van a **begin-iterator** aan **eind-aggregator** zien. Zo kunt u deze segmenten gemakkelijk herkennen in uw Workfront Fusion-scenario.

## Uw beurt

>[!NOTE]
>
>Praktische oefeningen en uitdagingen zijn optioneel en zijn niet nodig om Fusion-training te voltooien.

Deze oefening bouwt op wat u in de analyse leerde, maar de oplossing wordt niet verstrekt.

Creeer een nieuw scenario aan som alle uren het programma geopende taken in projecten in de marketing portefeuille. Vervolgens verzendt u een e-mail met de tekst &quot;Uw {Project Name} projectteam heeft zich {summed hours} van de totale {planned hours} geplande uren aangemeld, waarmee u zich op {percentage} van het abonnement plaatst.&quot;

**Uitdaging:** zie of kunt u het zelfde ding maar voor uren doen dat slechts dit jaar wordt geregistreerd.

## Meer informatie? We raden het volgende aan:

[&#x200B; de documentatie van de Fusie van Workfront &#x200B;](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
