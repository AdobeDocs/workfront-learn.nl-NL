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
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Geavanceerde samenvoegingsanalyse

Bel een webservice om details over meerdere landen te retourneren en de totale bevolking van alle landen, gegroepeerd per subregio, te identificeren.

![ een beeld van het scenario van de Fusie ](assets/iteration-and-aggregation-3.png)

## Geavanceerde samenvoegingsanalyse

Workfront raadt u aan om de video met een doorlichting te bekijken voordat u probeert de oefening opnieuw te maken in uw eigen omgeving.

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12&learn=on&enablevpops)

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

Creeer een nieuw scenario aan som alle uren het programma geopende taken in projecten in de marketing portefeuille. Vervolgens verzendt u een e-mail met de tekst &quot;Uw projectteam {Projectnaam} heeft zich {samengevat uren} van het totaal van de {geplande uren} geplande uren aangemeld, waarmee u zich op {percentage} van het plan bevindt.&quot;

**Uitdaging:** zie of kunt u het zelfde ding maar voor uren doen dat slechts dit jaar wordt geregistreerd.

## Meer informatie? We raden het volgende aan:

[ de documentatie van de Fusie van Workfront ](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=nl-NL)
