---
title: Webhooks doorlopen
description: Leer hoe te om een webhaak te gebruiken om een app te creëren om te bepalen al dan niet een klant oud genoeg is om alcohol te kopen, allen in  [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9051
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Webhooks doorlopen

Dit scenario leidt tot een gemakwinkel app zodat kunnen zij gemakkelijk bepalen al dan niet een klant oud genoeg is om alcohol te kopen. De kassier hoeft alleen de naam en geboortedatum van de klant EN een geverifieerde clienttoken te plaatsen in een URL die is opgegeven. Zodra ingegaan, zal dat ons scenario teweegbrengen om de aangewezen reactie te berekenen en het aan de aanvrager terug te keren.

![&#x200B; een beeld gebruikend de schakelaarmodule &#x200B;](assets/beyond-basic-modules-5.png)

## Webhooks doorlopen

Workfront raadt u aan om de video met een doorlichting te bekijken voordat u probeert de oefening opnieuw te maken in uw eigen omgeving.

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12&learn=on&enablevpops=1)


## Postman instellen

Als u de doorlichting wilt volgen, moet u de gratis Postman-toepassing downloaden. Volg de onderstaande stappen om naar het rechtergebied van Postman te navigeren voor de oefening.

1. Maak een werkruimte en open deze.
1. Klik op het tabblad Nieuw en maak een nieuwe verzameling met de naam Drinking Age.
1. Klik nogmaals op het tabblad Nieuw en maak een nieuwe GET-aanvraag met de naam GET verjaardatum.
1. Wijzig de aanvraagactie van GET in POST.
1. Ga naar het subtabblad Body onder het veld POST URL.
1. Kies formuliergegevens onder het subtabblad Autorisatie.
1. Maak drie toetsen voor Naam, Verjaardatum en ClientToken.

![&#x200B; een beeld gebruikend de schakelaarmodule &#x200B;](assets/beyond-basic-modules-6.png)

## Uw beurt

>[!NOTE]
>
>Praktische oefeningen en uitdagingen zijn optioneel en zijn niet nodig om Fusion-training te voltooien.

Deze oefening bouwt op wat u in de analyse leerde, maar de oplossing wordt niet verstrekt.

Maak een Workfront-webhaak die wacht op nieuwe updates die worden gemaakt en registreer vervolgens de datum, de naam van de persoon die de update heeft uitgevoerd en wat in de update staat. Stuur uzelf een e-mail met deze gegevens.

**Hint**: Gebruik de de trekkermodule van de Gebeurtenissen van het Horloge van Workfront om uw webhaak tot stand te brengen. Ook in Workfront-updates worden notities genoemd.

**Uitdaging**: Kan u URL vinden en toevoegen waar de update voor gemakkelijke toegang werd gemaakt?


## Meer informatie? We raden het volgende aan:

[&#x200B; de documentatie van de Fusie van Workfront &#x200B;](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
