---
title: OR-instructies maken in filters
description: Leer hoe u een OF verklaring gebruikt om Workfront te vertellen dat u of dit OF dat in uw rapport wilt zien.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
kt: 9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
source-git-commit: 65bd26fefb280d12ec44a4923f6d96ac8d88d6fb
workflow-type: tm+mt
source-wordcount: '915'
ht-degree: 0%

---

# OR-instructies maken in filters

Wanneer u een filter met veelvoudige lijnen van criteria bouwt, door gebrek plaatst Workfront EN tussen elke lijn. Dit betekent elk resultaat in de lijst wanneer u dit filter gebruikt voldoet aan alle filterregels.

In dit voorbeeld hebben we drie criteria, of regels, voor een projectfilter:

1. Het project moet een geplande einddatum hebben die in de huidige maand valt.
1. Het project moet in de portefeuille van de Marketing van Gebeurtenissen zijn.
1. Het project moet een actief project zijn, wat betekent dat het een status Actief moet hebben.

![Een afbeelding van het maken van een filter met AND-instructies in [!DNL Workfront]](assets/or-statement-1.png)

De projecten in de resultatenlijst voldoen aan alle drie de criteria, waardoor u de zoekresultaten kunt beperken zodat u precies de informatie kunt zien die u nodig hebt.

![Een afbeelding van een gefilterde lijst in [!DNL Workfront]](assets/or-statement-2.png)

Nochtans, kunnen er tijden zijn u de filterresultaten wilt om aan diverse criteria te voldoen, en dat is wanneer OF de verklaringen kunnen helpen. Met een OF verklaring, vertelt u het filter dat u dingen wilt zien die om het even welk van uw OF verklaringen in tegenstelling tot ALLE EN verklaringen aanpassen.

## OR-instructies gebruiken

OR-instructies vergroten of vergroten de hoeveelheid informatie die het filter zoekt omdat een item in de resultatenlijst alleen aan een van de filterregels moet voldoen, niet aan alle regels.

Kijk naar eenvoudig OF verklaring-projecten u de projectmanager (eigenaar) voor OF projecten bent die door u werden gecreeerd.

![Een afbeelding van het maken van een filter met OR-instructies in [!DNL Workfront]](assets/or-statement-3.png)

Nadat u beide filterregels hebt ingesteld, klikt u op EN tussen de twee en schakelt u deze over naar OR.

![Een afbeelding van het maken van een filter met OR-instructies in [!DNL Workfront]](assets/or-statement-4.png)

OR tussen de twee filterregels breidt uw onderzoekscriteria uit, die Workfront vertellen om projecten te vinden die één of andere van die opties-uw naam is op het gebied van de projecteigenaar of u bent de persoon die het project creeerde.

## Meerdere filterregels met OR-instructies

Nu bekijken een OF verklaring die veelvoudige filterregels op elke kant van OF bevat. Dit gebruikt de zelfde twee regels zoals voordien maar voegt regel-projecten ook toe moet een Huidige status hebben.

![Een afbeelding van het maken van een filter met OR-instructies in [!DNL Workfront]](assets/or-statement-5.png)

De filterregels zijn door Workfront &quot;gegroepeerd&quot; aan beide zijden van de OR (er is een grijs vak rondom de OR). Dit vertelt Workfront om de regels aan elke kant van OF samen in werking te stellen, die projecten vinden die aan beide criteria voldoen omdat zij met EN worden aangesloten.

In dit voorbeeld zoekt Workfront naar:

* Projecten die uw naam op het gebied van de projecteigenaar hebben die ook een status van Huidig hebben.
* **PLUS (OF)**
* Projecten die u hebt gemaakt en die ook de status Huidig hebben.

Het plaatsen van de &quot;projectstatus evenaart Huidige&quot;regel op elke kant van OF verzekert dat de regel samen met elk van de andere regels werkt. Deze algemene regel wordt soms de &quot;constante&quot; genoemd.

>[!NOTE]
>
>U bent niet beperkt tot één herhaalde filterregel op elke kant van OF. Afhankelijk van uw behoeften, kunt u veelvoudige hebben. Workfront raadt u aan deze herhaalde regels tot een minimum te beperken om ervoor te zorgen dat het filter de gewenste resultaten oplevert.

## Wat gebeurt er zonder de algemene filterregel?

Zonder de algemene filterregel(s) krijgt u mogelijk niet de verwachte zoekresultaten.

Bijvoorbeeld, als u de &quot;projectstatus de Huidige&quot;regel slechts aan één kant van OF plaatst, werkt het slechts met de andere filterregels in die sectie. In de onderstaande afbeelding ziet u dat de regel &quot;projectstatus is gelijk aan huidige&quot; alleen in de bovenste sectie voorkomt.

![Een afbeelding van het maken van een filter met OR-instructies in [!DNL Workfront]](assets/or-statement-6.png)

Dit betekent dat Workfront zal zoeken naar:

* Projecten die uw naam op het gebied van de projecteigenaar hebben en een status van Huidig hebben.
* **PLUS (OF)**
* Alle projecten die u hebt gemaakt.

Zoals u kunt zien, geeft deze filterinstelling u iets andere resultaten dan het filter met de herhaalde filterregel. Daarom is het belangrijk dat u ervoor zorgt dat het filter op de juiste manier is ingesteld, zodat u de gewenste resultaten krijgt en deze nodig hebt.

U kunt OR-instructies niet vaak gebruiken bij het maken van filters. Maar zo kunt u het aantal filters verminderen dat u moet maken. Zorg er gewoon voor dat uw filters niet te veel resultaten opleveren. Een lange lijst kan het vinden van de juiste informatie moeilijker maken voor gebruikers.

## OR filteractiviteit

U wilt onvolledige taken vinden die aan u worden toegewezen of die niet aan niemand worden toegewezen. U stelt een filter zo in dat het eronder lijkt. Geeft dit filter u de gewenste resultaten? Waarom of waarom niet?

![Een afbeelding van een onjuist gemaakte OR-instructie in [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### Antwoorden

Nr, zal dit filter niet de resultaten verstrekken u voor-taken hoopt die niet gebeëindigd zijn die of aan u of aan geen worden toegewezen-omdat de filterregel voor de taakstatus slechts aan één kant van OF is.

In plaats daarvan genereert dit filter een lijst met de volgende gegevens:

* Taken die aan u worden toegewezen die een status van Bezig of Nieuw hebben.
* **PLUS (OF)**
* Alle niet toegewezen taken, ongeacht de status.

Het filter moet er net zo uitzien als hieronder. Merk op dit filter de filterregel voor taakstatus op beide kanten van OF heeft.

![Een afbeelding van een correct gemaakte OR-instructie in [!DNL Workfront]](assets/or-statement-your-turn-2.png)
