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
source-git-commit: 0ff5accae867f07cc31ac2be7b0c12981412346e
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 1%

---

# Basisfilteractiviteiten maken

## Activiteit 1 - Alle projecten in de marketingportefeuille

In deze activiteit zult u een projectfilter creëren genoemd &quot;Alle projecten in de portefeuille van de Marketing&quot;in [!UICONTROL Legacy filter] ervaring. Dit zal u alle projecten in de portefeuille genoemd &quot;Portfolio van de Marketing&quot;ongeacht hun status tonen.

Hieronder vindt u stapsgewijze instructies.

### Antwoord op Activiteit 1

![Een afbeelding van het scherm om een nieuw filter te maken](assets/basic-filter-activity-1.png)

1. Ga naar de [!UICONTROL Projects] gebied van de [!UICONTROL Main Menu]. Dit toont u een lijst van projecten.
1. Klik op de knop **[!UICONTROL Filter]** en selecteert u [!UICONTROL Legacy Filters].
1. Selecteren **[!UICONTROL New Filter]**.
1. Geef het filter de naam &quot;Alle projecten in het marketingportfolio&quot;.
1. Klik op **[!UICONTROL Add Filter Rule]**.
1. In de [!UICONTROL Start typing field name] veld, typ &quot;[!UICONTROL portfolio name]&quot;. Selecteer vervolgens [!UICONTROL Name] onder de [!UICONTROL Portfolio] veldbron.
1. Laat de [!UICONTROL Equal] -operator zoals deze is.
1. Typ &quot;[!UICONTROL marketing]&quot; in de [!UICONTROL Start typing name] veld.
1. Selecteren [!UICONTROL Marketing Portfolio] er wordt aangenomen dat u een portfolio met die naam hebt waarop u wilt filteren. Als u niet gewoon de functie voor het vooruitgaan van tekst gebruikt om het gewenste portfolio te zoeken.
1. Klik op **[!UICONTROL Save Filter]**.

## Activiteit 2 - Projecten waarvan ik eigenaar ben en die deze maand aflopen

In deze video maakt u een projectfilter met de naam &quot;Projecten waarvan ik eigenaar ben en die deze maand worden gesloten&quot; in het dialoogvenster [!UICONTROL Legacy filter] ervaring. Als u veel projecten in de gaten houdt, kunt u met dit filter inzoomen op de projecten die binnenkort gesloten zullen worden.

Hieronder vindt u stapsgewijze instructies.

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12&learn=on)

### Antwoord op Activiteit 2

![Een afbeelding van het scherm om een nieuw filter te maken](assets/basic-filter-activity-updated-6-15-21.png)

1. Ga naar de [!UICONTROL Projects] gebied van de [!UICONTROL Main Menu]. Dit toont u een lijst van projecten.
1. Klik op de knop **[!UICONTROL Filter]** en selecteert u [!UICONTROL Legacy Filters].
1. Selecteren **[!UICONTROL New Filter]**.
1. Geef uw filter de naam &quot;Projecten waarvan ik eigenaar ben en die deze maand worden gesloten&quot;.
1. Klik op **[!UICONTROL Add Filter Rule]**.
1. In de [!UICONTROL Start typing field name] veld, typ &quot;owner&quot;. Selecteer vervolgens [!UICONTROL Owner ID] onder de [!UICONTROL Project] veldbron.
1. Laat de [!UICONTROL Equal] -operator zoals deze is.
1. Typ ‘$’ in het dialoogvenster [!UICONTROL Start typing name] veld.
1. Selecteren [!UICONTROL $$USER.ID]. Dit is de vervanging voor het programma geopende gebruiker.
1. Klikken [!UICONTROL Add Filter Rule] opnieuw.
1. In de [!UICONTROL Start typing field name] veld, begin met typen &quot;Is voltooid&quot;. Selecteer vervolgens [!UICONTROL Is Complete] onder het veld Project.
1. Laat de [!UICONTROL Equal] -operator zoals deze is.
1. Selecteer &quot;Onwaar&quot;.
1. Klikken [!UICONTROL Add Filter Rule] opnieuw.
1. In de [!UICONTROL Start typing field name] veldtype &quot;geplande&quot;, selecteer vervolgens [!UICONTROL Planned Completion Date] onder de [!UICONTROL Project] veldbron.
1. Wijzig de [!UICONTROL Equal] operator to [!UICONTROL This Month].
1. Klik op **[!UICONTROL Save Filter]**.
