---
title: Routers doorlopen
description: Leer hoe te om een router te gebruiken om de bundels van Pokemon vs superheroes onderaan de correcte weg binnen over te gaan [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9013
exl-id: 6c111e5b-1c8f-43fd-9e2d-16599de2a337
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# Routers doorlopen

## Overzicht

Gebruik een router om de bundels van Pokemon versus van superhelden onderaan de correcte weg over te gaan, dan creeer een taak voor elk karakter.

![Een afbeelding van het Fusion-scenario](assets/universal-connectors-and-routing-2.png)

## Routers doorlopen

Workfront raadt u aan om de video met een doorlichting te bekijken voordat u probeert de oefening opnieuw te maken in uw eigen omgeving.

>[!VIDEO](https://video.tv.adobe.com/v/335272/?quality=12)

## URL&#39;s uitvoeren

* Superhero-API-website: `https://www.superheroapi.com/`
* Eerste URL voor oefening: `https://www.superheroapi.com/api/{access-token}/{character-id}/appearance`
* Tweede URL voor oefening: `https://www.superheroapi.com/api/{access-token}/{character-id}/powerstats`

Als u moeite hebt om uw eigen superheldtoken te openen, kunt u dit gedeelde token gebruiken: 10110256647253588. Houd rekening met het aantal keren dat u de superheld-API aanroept, zodat dit gedeelde token voor iedereen blijft werken.

>[!TIP]
>
>Voor geleidelijke instructies bij de voltooiing van de analyse, ga naar [Routers doorlopen](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/routers.html?lang=en) oefening.


## Items zoeken in het deelvenster Toewijzing

Met het veld Zoeken-items boven aan de deelvensters met toewijzingen kunt u snel velden in het deelvenster zoeken, zelfs als deze in arrays zijn genest. De zoekopdracht is niet hoofdlettergevoelig.

![Een afbeelding van het eerste deelvenster met zoekopdrachten](assets/universal-connectors-and-routing-3.png)

![Een afbeelding van het tweede deelvenster Zoeken](assets/universal-connectors-and-routing-4.png)

## Tips en trucs voor het werken met API&#39;s

Tot dit punt, hebt u met zeer eenvoudige API (de Interface van de Programmering van de Toepassing) gewerkt die geen extra authentificatie vereist om informatie nodig in het scenario te trekken. Hier volgen enkele tips voor het navigeren met API&#39;s en universele connectors.

## Stap 1: Het type API bepalen

Workfront en veel softwaresystemen zijn gebouwd met behulp van de REST-API (Representational State Transfer), het eenvoudigste en meest standaard type API dat momenteel wordt gebruikt. Er zijn echter een paar andere, zoals:

* SOAP (Simple Object Access Protocol) (Workfront&#39;s Proof API is gebaseerd op SOAP)
* FTP (File Transfer Protocol)
* SFTP (Secure File Transfer Protocol)
* Zoek op internet naar API-typen en trefwoorden voor meer informatie.

>[!NOTE]
>
>Wanneer u verbinding maakt met grotere platforms, zoals Salesforce, bieden verschillende onderdelen van die platforms verschillende API&#39;s. Zorg ervoor u juiste voor de dienst vindt u wilt verbinden met.

## Stap 2: Het type verificatie bepalen dat door de API wordt vereist

API-verificatie is een vorm van identificatie die wordt gebruikt om de toegang tot een service te regelen, bijvoorbeeld wanneer u verbinding probeert te maken via Workfront Fusion. Het helpt u aan een ander systeem bewijzen dat u gemachtigd bent om tot het systeem toegang te hebben. OAuth 2 is het gemeenschappelijkste type van authentificatie die vandaag wordt gebruikt. Meer informatie vindt u met een internetzoekopdracht over API-verificatie.

Verificatie kan het moeilijkste aspect zijn van het werken met een API. Een van de meest waardevolle functies van de universele connectors van Workfront Fusion is dat Workfront Fusion verificatie voor u kan afhandelen bij het gebruik van veelgebruikte verificatiemethoden zoals basisverificatie, zoals OAuth 2, API Key en andere. Zodra u een verbinding gebruikend de aangewezen module van de Fusie van Workfront voor uw authentificatiemethode (b.v. OAuth 2) creeert, zal de Fusion van Workfront voortdurend API sleutels en/of tokens produceren telkens als u uw scenario wilt in werking stellen.

Meer informatie over de verschillende verificatietypen die Workfront biedt in het artikel met uitgebreide verificatieoverzichten op Experience League.

## Stap 3: Lees de API-documentatie en zoek de benodigde eindpunten

Wanneer een API met een ander systeem in wisselwerking staat, worden de aanraakpunten van deze mededeling beschouwd als eindpunten. Een eindpunt is de plaats waar APIs verzoeken verzenden en waar het middel leeft.

Wanneer u met een API werkt via een universele aansluiting, moet u begrijpen welke eindpunten door de API worden ondersteund en welke gegevens voor elke aanvraag zijn vereist. API-documentatie moet de eindpunten van een API beschrijven en aangeven hoe algemene bewerkingen zoals maken, lezen, bijwerken of verwijderen moeten worden uitgevoerd. Het uitvoeren van deze aanroepen vereist enige oefening, met name als u nog nooit API-aanroepen hebt gemaakt of als u nog niet eerder met een nieuwe API hebt gewerkt.

Meer informatie over Workfront Fusion Universal Connectors en hoe u deze kunt instellen voor verbinding met de API&#39;s die u op het Experience League nodig hebt.

## Slotopmerking

U kunt de volledige lijst van onze vooraf gebouwde app schakelaars in Experience League controleren. Als u een nieuwe app-aansluiting wilt voorstellen aan het Workfront Fusion-productteam, dient u uw idee in bij Innovation Lab. Meer informatie over het innovatielaboratorium, en hoe u op ideeën kunt stemmen en kunt deelnemen aan de prioritering van het Leaderboard, als u dat nog niet eerder hebt gedaan. Als u reeds toegang tot het laboratorium van Innovatie hebt, login en leg uw ideeën voor.

## Uw beurt

>[!NOTE]
>
>Praktische oefeningen en uitdagingen zijn optioneel en zijn niet nodig om Fusion-training te voltooien.

Deze oefening bouwt op wat u in de analyse leerde, maar de oplossing wordt niet verstrekt.

Maak in de module Meerdere variabelen instellen voor Pokemon-tekens een variabele met de naam &quot;Status (niveau)&quot;. Wijs de naam van de Stats van Pokemon in deze variabele toe. Gebruik de mogelijkheid van de arraywaarde om de weergave van de array te wijzigen, zodat elke status een nieuwe regel is, zoals hieronder wordt weergegeven.

**Tip:** Er zijn slechts zes verschillende Pokemon stats met een vergelijkbaar niveau.

![Een afbeelding van statistische gegevens](assets/universal-connectors-and-routing-5.png)

**Uitdaging:** Zie of u de arrayformules kunt gebruiken om de Abilities ertoe te brengen om de zelfde manier te tonen zoals hierboven als verschillende rijen eerder dan een koord van waarden die door een komma worden gescheiden. De onderstaande schermafbeelding bevat een tip.

![Een afbeelding van een arraynaam](assets/universal-connectors-and-routing-6.png)

## Meer informatie? We raden het volgende aan:

[Workfront Fusion-documentatie](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
