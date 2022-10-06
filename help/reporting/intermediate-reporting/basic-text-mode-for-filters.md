---
title: Basismodus voor filters begrijpen
description: Leer welke tekstmodus is, welke camel-case is en welke standaardtekstmodus u kunt gebruiken in uw rapportfilters in [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
source-git-commit: 83c7379a5398c78cea31a4571b34fd5b64bce027
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Basismodus voor filters begrijpen

In deze video leert u:

* Welke tekstmodus is ingesteld
* Wat kamelendoosje is
* Een standaardtekstmodus voor &quot;plug-and-play&quot; die u in rapportfilters kunt gebruiken

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12)

In de volgende tekstmodus worden taken uitgesloten waarvoor een gebruiker heeft aangegeven dat deze is uitgevoerd met Mijn onderdeel. U hoeft alleen maar een taakfilter te maken, filterregels toe te voegen en vervolgens over te schakelen naar de tekstmodus en de code hieronder te plakken na elke tekstmodus die u in het filter ziet.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## Activiteit: Vragen over de tekstmodus

1. Hoe zou u de camelcase voor het gebied met de naam &quot;ingegaan door identiteitskaart&quot;schrijven?
1. Maak in een Issue-rapport een filter om problemen weer te geven die zijn gemarkeerd als gesloten maar die nog moeten worden goedgekeurd.

## Antwoorden

1. Het hoofdlettergebruik voor de kameel voor het veld &quot;Door id ingevoerd&quot; moet als volgt worden geschreven:
1. De tekstwijze zou als dit in de filter van het voorwaardenrapport moeten kijken:

   ![Een afbeelding van het scherm om een nieuw filter in de tekstmodus te maken](assets/btm-answer.png)
