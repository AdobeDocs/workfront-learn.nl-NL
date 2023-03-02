---
title: Analyse van gegevenswinkels
description: Leer hoe u een gegevenswinkel kunt gebruiken om bedrijfsnamen te synchroniseren tussen een lijst met bedrijven en Workfront met [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9055
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Analyse van gegevenswinkels

## Overzicht

Hierbij gebruiken we een gegevensopslag om bedrijfsnamen te synchroniseren tussen een lijst met bedrijven en Workfront.

Dit maakt deel uit van een eenrichtingssynchronisatie van bedrijven in Workfront en een ander systeem. Momenteel wordt alleen synchronisatie uitgevoerd tussen een CSV-bestand en Workfront. Maar het zal ook een lijst in een gegevensopslag handhaven die spoor van Workfront identiteitskaart (WFID) en bedrijfsidentiteitskaart in het CSV dossier (CID) voor elk bedrijf zal houden. Op die manier kunnen we dit op een gegeven moment in de toekomst tot een tweerichtingssynchronisatie maken.

![Een afbeelding van een Fusion-scenario](assets/data-structures-and-data-stores-2.png)

## Analyse van gegevenswinkels

Workfront raadt u aan om de video met een doorlichting te bekijken voordat u probeert de oefening opnieuw te maken in uw eigen omgeving.

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12)

>[!TIP]
>
>Voor geleidelijke instructies bij de voltooiing van de analyse, ga naar [Analyse van gegevenswinkels](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/data-stores.html?lang=en) oefening.


## Slotopmerking

Nu u klaar bent met het leren over gegevensstructuren en gegevensopslagruimten, kunt u zich afvragen: &quot;Wanneer moet u deze gebruiken?&quot;

Gegevensstructuren worden meestal gebruikt voor het serieel ordenen of parseren van gegevensindelingen zoals JSON, XML, CSV en andere. Gegevensstructuren bieden u de mogelijkheid om de structuur van uw gegevens te beheren en zelfs gegevens te valideren. De gemeenschappelijkste reden u een gegevensstructuur gebruikt moet geldige gegevens tot stand brengen om naar API te verzenden die JSON of XML verwacht. In deze gevallen zult u de JSON- of XML-toepassing samen met de gegevensstructuur willen gebruiken om ervoor te zorgen dat de gegevens de juiste indeling hebben.

Gegevensopslagplaatsen zouden slechts moeten worden gebruikt om blijvende gegevens op te slaan die door meer dan één scenario uitvoering moeten worden betreden. U kunt bijvoorbeeld metagegevens opslaan over de laatste record die is verwerkt voor geavanceerd gebruik, waarvoor u nauwkeurige controle over de verwerking nodig hebt.

De opslag van gegevens wordt niet ontworpen om als gegevenspakhuis of logboekregistratie worden gebruikt. Gegevensopslag is niet toegankelijk buiten Workfront Fusion en de meeste interacties met gegevensopslag vinden plaats via een Workfront Fusion-scenario. Daarom is het niet mogelijk om een gegevensopslag te verbinden met een analytisch of rapporteringshulpmiddel dat voor gegevenspakhuis en registrerengebruikgevallen zou worden verwacht. De rol van Workfront Fusion in gebruiksgevallen zoals deze zou zijn om een systeem te bevolken aangewezen voor het organiseren van en het opslaan van gegevens (b.v. SQL, MariaDB).

## Meer informatie? We raden het volgende aan:

[Workfront Fusion-documentatie](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
