---
title: Geavanceerde samenvoegingsanalyse
description: Leer hoe u een webservice kunt aanroepen om details over meerdere landen te retourneren en om de populatie, gegroepeerd per subregio, te identificeren in [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9040
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# Geavanceerde samenvoegingsanalyse

## Overzicht

Bel een webservice om details over meerdere landen te retourneren en de totale bevolking van alle landen, gegroepeerd per subregio, te identificeren.

![Een afbeelding van het Fusion-scenario](assets/iteration-and-aggregation-3.png)

## Geavanceerde samenvoegingsanalyse

Workfront raadt u aan om de video met een doorlichting te bekijken voordat u probeert de oefening opnieuw te maken in uw eigen omgeving.

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12&learn=on)

## URL&#39;s uitvoeren

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`

>[!TIP]
>
>Voor geleidelijke instructies bij de voltooiing van de analyse, ga naar [Geavanceerde samenvoegingsanalyse](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/advanced-aggregation.html?lang=en) oefening.

## Versterking van het aggregatiebeginsel

Wanneer een module meerdere bundels uitvoert, voert elke module daarna elke bundel uit.

Om dit te verhinderen, voeg een aggregator na een module toe die potentieel veelvoudige bundels produceert.

U zult een schaduw rond om het even welk segment in uw scenario van een zien **beginiterator** aan de **end-aggregator**. Zo kunt u deze segmenten gemakkelijk herkennen in uw Workfront Fusion-scenario.

## Uw beurt

>[!NOTE]
>
>Praktische oefeningen en uitdagingen zijn optioneel en zijn niet nodig om Fusion-training te voltooien.

Deze oefening bouwt op wat u in de analyse leerde, maar de oplossing wordt niet verstrekt.

Creeer een nieuw scenario aan som alle uren het programma geopende taken in projecten in de marketing portefeuille. Vervolgens verzendt u een e-mail met de tekst &quot;Uw projectteam {Projectnaam} heeft zich {samengevat uren} van het totaal van de {geplande uren} geplande uren aangemeld, waarmee u op {percentage} van het abonnement wordt gezet.&quot;

**Uitdaging:** Kijk of je hetzelfde kunt doen, maar alleen voor uren die dit jaar zijn geregistreerd.

## Meer informatie? We raden het volgende aan:

[Workfront Fusion-documentatie](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
