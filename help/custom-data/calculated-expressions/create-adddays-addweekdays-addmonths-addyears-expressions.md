---
title: ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS-expressies maken
description: Leer hoe u de ADD-expressies in een berekend veld in Adobe gebruikt en maakt [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335175.png
kt: 8912
exl-id: f194fbc8-99b3-4fed-9fc5-a2f5fa4593d2
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS-expressies maken

In deze video leert u:

* Wat de expressies ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR berekenen
* Een ADDWEEKDAYS-gegevensexpressie maken in een berekend veld

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12)

## Aanvullende voorbeelden

Hieronder vindt u een aantal extra ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR-expressies die Adobe Workfront-klanten hebben gemaakt.

**Moet zijn uitgevoerd door**

De klant wilde weten wanneer de taak zou moeten voltooid zijn gebaseerd op de Ware Datum van het Begin en de Geplande Duur. De geplande voltooiingsdatum werkt in dit geval niet omdat de taak kan worden verplaatst als de taak te laat is. De geplande uitvoeringsdatum helpt niet als er vertragingen optreden in eerdere taken.

De gemaakte expressie is ADDDAYS({actualStartDate},{durationMinutes}/480)

De tijd in het gebied van de Duur wordt opgeslagen in notulen. In deze expressie kan het veld Duur niet zelfstandig zijn als de tijd in dagen moet worden weergegeven. Daartoe moet de duur worden gedeeld door 480 minuten (480 minuten = 8 uur = 1 dag).

Daarom bevat de tweede waardegroef (Duur/480).


**Datum van voltooiing van factuur**

In dit voorbeeld wordt niet alleen de ADDDAYS-expressie gebruikt, maar ook een aangepast veld dat eerder in het aangepaste formulier is gemaakt en opgeslagen.

De klant legt de datum vast waarop een factuur is verzonden via een aangepast datumveld met de naam &quot;Invoice Submission Date&quot;.

Zodra de factuur is verzonden, moet deze binnen 30 dagen worden ingevuld en ingediend. Om die voltooiing en het indienen van datum automatisch te produceren, wordt een berekend gebied ADDDAYS gebruikt samen met het de douaneveld van de Datum van de Verzending van de factuur. De expressie ziet er als volgt uit:

ADDDAYS({DE:Invoice-verzenddatum},30)
