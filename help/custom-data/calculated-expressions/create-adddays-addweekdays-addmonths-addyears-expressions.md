---
title: ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS-expressies maken
description: Leer hoe te om de uitdrukkingen ADD op een berekend gebied in Adobe te gebruiken en tot stand te brengen  [!DNL Workfront].
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335175.png
jira: KT-8912
exl-id: f194fbc8-99b3-4fed-9fc5-a2f5fa4593d2
doc-type: video
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS-expressies maken

In deze video leert u:

* Wat de expressies ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR berekenen
* Een ADDWEEKDAYS-gegevensexpressie maken in een berekend veld

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12&learn=on)

## Aanvullende voorbeelden

Hieronder vindt u een aantal extra ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR-expressies die Adobe Workfront-klanten hebben gemaakt.

**had moeten gedaan door** zijn

De klant wilde weten wanneer de taak zou moeten voltooid zijn gebaseerd op de Ware Datum van het Begin en de Geplande Duur. De voorspelde Voltooiingsdatum werkt in dit geval niet omdat deze kan worden verplaatst als de taak te laat is. De geplande Voltooiingsdatum helpt niet als er vertragingen optreden in eerdere taken.

De gecreëerde uitdrukking was ADDDAYS ({actualStartDate}, {durationMinutes}/480)

De tijd in het gebied van de Duur wordt opgeslagen in notulen. In deze expressie kan het veld Duur dus niet zelfstandig zijn als de tijd in dagen moet worden weerspiegeld. Daartoe moet de duur worden gedeeld door 480 minuten (480 minuten = 8 uur = 1 dag).

Daarom bevat de tweede waardegroef (Duur/480).


**de voltooiingsdatum van de Factuur**

In dit voorbeeld wordt niet alleen de ADDDAYS-expressie gebruikt, maar ook een aangepast veld dat eerder in het aangepaste formulier is gemaakt en opgeslagen.

De klant legt de datum vast waarop een factuur is verzonden via een aangepast datumveld met de naam &quot;Invoice Submission Date&quot;.

Zodra de factuur is verzonden, moet deze binnen 30 dagen worden ingevuld en ingediend. Om die voltooiing en het indienen van datum automatisch te produceren, wordt een berekend gebied ADDDAYS gebruikt samen met het de douaneveld van de Datum van de Verzending van de factuur. De expressie ziet er als volgt uit:

ADDDAYS({DE:Invoice-verzenddatum},30)
