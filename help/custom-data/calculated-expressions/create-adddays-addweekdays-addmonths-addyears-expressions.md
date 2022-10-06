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
source-git-commit: 2b9a31b45ff94222a77c05292ee5b9d8229f5f0b
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---

# ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS-expressies maken

In deze video leert u:

* Wat de expressies ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR berekenen
* Een ADDWEEKDAYS-gegevensexpressie maken in een berekend veld

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12)

## Aanvullende voorbeelden

Hieronder vindt u een aantal extra ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR-expressies Adobe [!DNL Workfront] klanten hebben gemaakt.

**Moet zijn uitgevoerd door**

De klant wilde weten wanneer de taak zou moeten voltooid zijn gebaseerd op de Ware Datum van het Begin en de Geplande Duur. De geplande voltooiingsdatum werkt in dit geval niet omdat de taak kan worden verplaatst als de taak te laat is. De geplande uitvoeringsdatum helpt niet als er vertragingen optreden in eerdere taken.

De gemaakte expressie was ADDDAYS (werkelijke begindatum (duur/480))

De tijd in het gebied van de Duur wordt opgeslagen in notulen. In deze expressie kan het veld Duur niet zelfstandig zijn als de tijd in dagen moet worden weergegeven. Daartoe moet de duur worden gedeeld door 480 minuten (480 minuten = 8 uur = 1 dag).

Daarom bevat de tweede waardegroef (Duur/480).


**Datum van voltooiing van factuur**

Dit voorbeeld bevat een ander berekend veld, dat al is gemaakt en opgeslagen in het systeem, binnen de expressie.

De klant heeft de datum waarop de factuur is verzonden vastgelegd vastgelegd in een aangepast datumveld met de naam &quot;Invoice-verzenddatum&quot;, in het aangepaste formulier. Zodra de factuur is verzonden, hebben zij 30 dagen de tijd om de factuur in te vullen en in te dienen. Om die voltooiing en het indienen datum automatisch te veroorzaken, creeerden zij een berekend gebied gebruikend ADDDDAYS en het gebied van de Datum van de Verzending van de Rekening. De uitdrukking zag er als volgt uit:

ADDDAYS(Datum van factuurindiening,30)
