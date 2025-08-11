---
title: OR-instructies maken in filters
description: Met de flexibele filterlogica van Workfront kunnen gebruikers de rapportageweergaven verfijnen aan de hand van de standaard AND-regels, optionele OR-voorwaarden en georganiseerde filtergroepen voor complexe criteria.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
jira: KT-9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
last-substantial-update: 2025-08-11T00:00:00Z
doc-type: video
source-git-commit: b3cff8f86ceeb6e79e2b88ab335b2671aa25600a
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# OR-instructies maken in filters

In de video wordt uitgelegd hoe u filters met meerdere regels maakt en gebruikt in Workfront. &#x200B; Workfront gebruikt standaard &quot;AND&quot; tussen filterregels. Dit houdt in dat alle voorwaarden waar moeten zijn voor een item dat in de lijst wordt weergegeven.
U kunt ook de filterlogica wijzigen in &#39;&#39;OR&#39;&#39;, waarin items worden weergegeven die aan een van de voorwaarden voldoen.
De video demonstreert ook het maken van filters voor taken met behulp van filtergroepen. &#x200B; U kunt bijvoorbeeld twee groepen maken: een voor onvolledige taken die zijn toegewezen aan het creatieve team en die te laat zijn, en een voor onvolledige taken die zijn toegewezen aan het creatieve team en die niet zijn toegewezen. &#x200B; Binnen elke groep is de logica &quot;AND&quot; van toepassing, wat betekent dat aan alle voorwaarden in de groep moet worden voldaan. &#x200B; De logica &quot;OF&quot;tussen groepen verzekert taken die aan de voorwaarden van één van beide groep voldoen worden getoond.

>[!VIDEO](https://video.tv.adobe.com/v/3470699/?quality=12&learn=on&captions=dut)

## OR filteractiviteit

U wilt onvolledige taken vinden die aan u worden toegewezen of die niet aan niemand worden toegewezen. U stelt een filter zo in dat het eronder lijkt. Geeft dit filter u de gewenste resultaten? Waarom of waarom niet?

![ Een afbeelding van een onjuist gemaakte OR-instructie in [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### Antwoorden

Nr, zal dit filter niet de resultaten verstrekken u voor-taken hoopt die niet worden gebeëindigd die of aan u of aan geen worden toegewezen-omdat de filterregel voor de taakvolledigheid slechts aan één kant van OF is.

In plaats daarvan genereert dit filter een lijst met de volgende gegevens:

* Taken die aan u zijn toegewezen en die niet zijn voltooid.
* **PLUS (OF)**
* Alle niet toegewezen taken, ongeacht de status.

Het filter moet er net zo uitzien als hieronder. Merk op dit filter de filterregel voor taakvolledigheid op beide kanten van OR heeft.

![ Een beeld van behoorlijk gecreeerd OF verklaring in [!DNL Workfront]](assets/or-statement-your-turn-2.png)
