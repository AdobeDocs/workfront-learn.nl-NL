---
title: Webhooks wandelen
description: Leer hoe u een webhaak gebruikt om een app te maken om te bepalen of een klant oud genoeg is om alcohol te kopen, allemaal in [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9051
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Webhooks wandelen

## Overzicht

Dit scenario leidt tot een gemakwinkel app zodat kunnen zij gemakkelijk bepalen al dan niet een klant oud genoeg is om alcohol te kopen. De kassier hoeft alleen de naam en geboortedatum van de klant EN een geverifieerde clienttoken te posten naar een opgegeven URL. Zodra ingegaan, zal dat ons scenario teweegbrengen om de aangewezen reactie te berekenen en het aan de aanvrager terug te keren.

![Een beeld gebruikend de schakelaarmodule](assets/beyond-basic-modules-5.png)

## Webhooks wandelen

Workfront raadt u aan om de video met een doorlichting te bekijken voordat u probeert de oefening opnieuw te maken in uw eigen omgeving.

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12)

>[!TIP]
>
>Voor geleidelijke instructies bij de voltooiing van de analyse, ga naar [Webhooks wandelen](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/webhooks.html?lang=en) oefening.

## Postman instellen

Als u de doorlichting wilt volgen, moet u de gratis Postman-toepassing downloaden. Volg de onderstaande stappen om naar het rechtergebied van Postman te navigeren voor de oefening.

1. Maak een werkruimte en open deze.
1. Klik op het tabblad Nieuw en maak een nieuwe verzameling met de naam Drinking Age.
1. Klik nogmaals op het tabblad Nieuw en maak een nieuwe aanvraag voor een GET met de naam GET verjaardatum.
1. Wijzig de aanvraagactie van GET naar POST.
1. Ga naar het subtabgebied Body onder het veld URL POST.
1. Kies formuliergegevens onder het subtabblad Autorisatie.
1. Maak drie toetsen voor Naam, Verjaardatum en ClientToken.

![Een beeld gebruikend de schakelaarmodule](assets/beyond-basic-modules-6.png)

## Uw beurt

>[!NOTE]
>
>Praktische oefeningen en uitdagingen zijn optioneel en zijn niet nodig om Fusion-training te voltooien.

Deze oefening bouwt op wat u in de analyse leerde, maar de oplossing wordt niet verstrekt.

Maak een Workfront-webhaak die wacht op nieuwe updates die worden gemaakt en registreer vervolgens de datum, de naam van de persoon die de update heeft uitgevoerd en wat in de update staat. Stuur uzelf een e-mail met deze gegevens.

**Tip**: Met de Workfront Watch Events-triggermodule kunt u uw webhaak maken. Ook in Workfront-updates worden notities genoemd.

**Uitdaging**: Kunt u de URL vinden en toevoegen waarvoor de update is gemaakt, zodat u deze eenvoudig kunt openen?


## Meer informatie? We raden het volgende aan:

[Workfront Fusion-documentatie](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
