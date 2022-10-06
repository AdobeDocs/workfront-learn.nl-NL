---
title: Aangepaste vragen maken
description: Leer wat een douaneherinnering is, hoe te om een douaneherinnering tot stand te brengen gebruikend tekstwijze en sommige voorbeelden die u in rapportering kunt gebruiken binnen [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
source-git-commit: 83c7379a5398c78cea31a4571b34fd5b64bce027
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# Aangepaste vragen maken

In deze video leert u:

* Wat een aangepaste prompt is
* Een aangepaste vraag maken met de tekstmodus
* Enkele voorbeelden die u in uw rapportage kunt gebruiken

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12)

## Activiteit: Aangepaste vragen maken

1. Creeer een douaneherinnering die de volgende projectstatussen in het snelle drop-down menu toont:
   * Planning
   * Huidig
   * Voltooid
   * Dead
1. Wijzig de herinnering om huidige projecten te tonen die deze maand worden verwacht.

## Antwoorden

1. Uw aangepaste aanwijzingen moeten er ongeveer als volgt uitzien en de volgende tekstmodus hebben:

   ![Een afbeelding van het scherm om een nieuw filter in de tekstmodus te maken](assets/cp-01.png)

   Zodra u sparen de douaneherinnering, zou het snelle drop-down menu als dit moeten kijken:

1. De tekstmodus in de aangepaste prompt moet er als volgt uitzien:

![Een afbeelding van het scherm om een nieuw filter in de tekstmodus te maken](assets/cp-02.png)

```
   status=CUR&plannedCompletionDate=$$TODAYbm&plannedCompletionDate_Mod=between&plannedCompletionDate_Range=$$TODAYem 
```

En het drop-down etiket voor actieve herinneringen zou moeten worden bijgewerkt om op de verandering in de code als dit te wijzen:

![Een afbeelding van het scherm om een nieuw filter in de tekstmodus te maken](assets/cp-02a.png)
