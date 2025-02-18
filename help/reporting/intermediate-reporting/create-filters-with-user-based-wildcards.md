---
title: Filters maken met jokertekens op basis van gebruiker
description: Leer hoe te om op gebruiker-gebaseerde vervangingen te gebruiken en hoe te om een filter te bouwen dat op de het programma geopende gebruiker wordt gebaseerd.
activity: use
feature: Reports and Dashboards
thumbnail: 336810.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9081
exl-id: 46c83acd-6e43-42aa-875f-ae24b09a7fee
doc-type: video
source-git-commit: 88c2161e897f23587ccc1d0e867b6f8961927a0f
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# Filters maken met jokertekens op basis van gebruiker

In deze video leert u hoe u:

* Begrijp waarom om vervangingen te gebruiken
* Een filter maken met een op gebruikers gebaseerd jokerteken

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12&learn=on)

>[!TIP]
>
>Gebruik de het gebiedsbron en naam van de Gebruikers van de Taak > van identiteitskaart wanneer het bouwen van filters die taak bekijken of taakinformatie uitgeven.  Bij deze optie wordt naar alle   gebruikers die zijn toegewezen aan de taak of uitgave, niet alleen de &quot;eigenaar&quot; of de primaire ontvanger.

>[!TIP]
>
>Gebruik de $$USER.ID (in plaats van uw naam) zelfs wanneer het bouwen van filters voor zich. Op deze manier, als iemand een filter ziet dat je gebruikt en zegt &quot;dat met mij delen&quot;, is het filter al ingesteld zodat elke persoon die het gebruikt zijn eigen informatie ziet.

>[!TIP]
>
>U moet altijd de Gelijke filterkwalificatie gebruiken wanneer het gebruiken van op gebruiker-gebaseerde vervangingen.


## Filters maken met op gebruikers gebaseerde jokertekenactiviteiten

[ klik hier ](/help/assets/create-filters-with-user-based-wildcards-activities.pdf) om een PDF van deze pagina te downloaden.

### Activiteit 1

Deze week heb je wat extra tijd, dus je wilt zien of er iemand in je team is die hulp kan gebruiken bij het toewijzen van taken. Maak een taakfilter om te zoeken naar taken die deze week moeten worden uitgevoerd en die nog niet zijn voltooid.

### Antwoord 1

Je bent geweldig om je teamgenoten te helpen! Als het filter is ingesteld zoals de onderstaande afbeelding, vindt u taken:

* Dat is nog niet voltooid (wat betekent dat ze geen [!UICONTROL Complete] status of status hebben die gelijk is aan [!UICONTROL Complete] );
* Dit zijn projecten met een [!UICONTROL Current] status (u wilt immers geen taken vinden voor projecten die nog niet zijn gestart);
* die aan iemand in uw huisteam worden toegewezen, zoals die door de teammontages van Workfront wordt bepaald;
* En die een voltooiingsdatum van enige tijd deze week hebben (deze regel gebruikte het vooraf gebouwde datumfilter om &quot;deze week&quot;te bepalen).

![ een beeld van het scherm om een taakfilter met een op gebruiker-gebaseerde vervanging ](assets/user-wildcard-exercise-answer.png) tot stand te brengen

Mogelijk moet u extra filters toevoegen als u de lijst een beetje meer wilt beperken. U kunt bijvoorbeeld een filterregel toevoegen die een specifiek programma of portfolio bekijkt waarvan uw team werkt.
