---
title: Basisfilteractiviteiten maken
description: In deze activiteit zult u een projectfilter genoemd "Projecten creëren I Zelf die deze Maand sluiten."
activity: use
feature: Reports and Dashboards
thumbnail: 336807.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8856
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 1%

---

# Basisfilteractiviteiten maken

## Activiteit 1 - Alle projecten in de marketingportefeuille

In deze activiteit zult u een projectfilter genoemd &quot;Alle projecten in de portefeuille van de Marketing&quot;in de [!UICONTROL Legacy filter] ervaring creëren. Dit toont u alle projecten in de portefeuille genoemd &quot;Marketing Portfolio&quot;ongeacht hun status.

Hieronder vindt u stapsgewijze instructies.

### Antwoord op Activiteit 1

![ een beeld van het scherm om een nieuw filter ](assets/basic-filter-activity-1.png) tot stand te brengen

1. Navigeer naar het [!UICONTROL Projects] -gebied vanuit [!UICONTROL Main Menu] . Dit toont u een lijst van projecten.
1. Klik op het menu **[!UICONTROL Filter]** en selecteer [!UICONTROL Legacy Filters] .
1. Selecteer **[!UICONTROL New Filter]** .
1. Geef het filter de naam &quot;Alle projecten in het marketingportfolio&quot;.
1. Klik op **[!UICONTROL Add Filter Rule]**.
1. Typ &quot;[!UICONTROL portfolio name]&quot; in het veld [!UICONTROL Start typing field name] . Selecteer vervolgens [!UICONTROL Name] onder de veldbron van [!UICONTROL Portfolio] .
1. Laat de operator [!UICONTROL Equal] ongewijzigd.
1. Typ &quot;[!UICONTROL marketing]&quot; in het veld [!UICONTROL Start typing name] .
1. Selecteer [!UICONTROL Marketing Portfolio] ervan uitgaande dat u een portfolio met die naam hebt waarop u wilt filteren. Als u niet gewoon de functie voor het vooruitgaan van tekst gebruikt om het gewenste portfolio te zoeken.
1. Klik op **[!UICONTROL Save Filter]**.

## Activiteit 2 - Projecten waarvan ik eigenaar ben en die deze maand aflopen

In deze video maakt u een projectfilter met de naam &quot;Projecten waarvan ik eigenaar ben en die deze maand afsluiten&quot; in de [!UICONTROL Legacy filter] -ervaring. Als u veel projecten in de gaten houdt, kunt u met dit filter inzoomen op de projecten die binnenkort gesloten zullen worden.

Hieronder vindt u stapsgewijze instructies.

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12&learn=on&enablevpops)

### Antwoord op Activiteit 2

![ een beeld van het scherm om een nieuw filter ](assets/basic-filter-activity-updated-6-15-21.png) tot stand te brengen

1. Navigeer naar het [!UICONTROL Projects] -gebied vanuit [!UICONTROL Main Menu] . Dit toont u een lijst van projecten.
1. Klik op het menu **[!UICONTROL Filter]** en selecteer [!UICONTROL Legacy Filters] .
1. Selecteer **[!UICONTROL New Filter]** .
1. Geef uw filter de naam &quot;Projecten waarvan ik eigenaar ben en die deze maand worden gesloten&quot;.
1. Klik op **[!UICONTROL Add Filter Rule]**.
1. Typ in het veld [!UICONTROL Start typing field name] &quot;owner&quot;. Selecteer vervolgens [!UICONTROL Owner ID] onder de veldbron van [!UICONTROL Project] .
1. Laat de operator [!UICONTROL Equal] ongewijzigd.
1. Typ ‘$’ in het veld [!UICONTROL Start typing name] .
1. Selecteer [!UICONTROL $$USER.ID] . Dit is de vervanging voor het programma geopende gebruiker.
1. Klik nogmaals op [!UICONTROL Add Filter Rule] .
1. Typ &quot;Is voltooid&quot; in het veld [!UICONTROL Start typing field name] . Selecteer vervolgens [!UICONTROL Is Complete] onder de bron van het veld Project.
1. Laat de operator [!UICONTROL Equal] ongewijzigd.
1. Selecteer &quot;Onwaar&quot;.
1. Klik nogmaals op [!UICONTROL Add Filter Rule] .
1. Typ in het veld [!UICONTROL Start typing field name] het veldtype &quot;geplande&quot; en selecteer vervolgens [!UICONTROL Planned Completion Date] onder de veldbron [!UICONTROL Project] .
1. Wijzig de operator [!UICONTROL Equal] in [!UICONTROL This Month] .
1. Klik op **[!UICONTROL Save Filter]**.
