---
title: Probleemproblemen maken en beheren
description: Leer hoe u bestandscontroles instelt en beheert.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10020
exl-id: a5a9280b-0d48-413d-92de-f6a949e6b210
source-git-commit: 5d385de5cdcee0d433304c09507ba6bb5b0a10e6
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Uitgiftesegmenten maken en beheren

## Inleiding tot het uitgeven van ernstmogelijkheden

Een strengheid kan worden gebruikt om aan te geven hoe ernstig een probleem is of hoe het het werk dat wordt uitgevoerd kan beïnvloeden.

![[!UICONTROL Severity] in het menu [!UICONTROL Issue Details] venster](assets/admin-fund-severity-issue-details.png)

De [!UICONTROL Severity] veld kan worden geopend in het [!UICONTROL Issue Details]. Het kan ook in kolommeningen op lijsten en in douanerapporten worden omvat.

[!DNL Workfront] heeft vijf standaardwaarden:

* [!UICONTROL Cosmetic]
* [!UICONTROL Causes Confusion]
* [!UICONTROL Bug with workaround]
* [!UICONTROL Bug with no workaround]
* [!UICONTROL Fatal error]

Systeembeheerders kunnen deze standaardbestandsnamen wijzigen of nieuwe bestandsnamen maken.

Ernsten zijn alleen beschikbaar voor problemen met [!DNL Workfront].

## Uitgiftesegmenten maken en beheren

Als systeembeheerder, kunt u nieuwe controles tot stand brengen, indien nodig, om het werkschema van de kwestie te voltooien.

![[!UICONTROL Severities] pagina in [!UICONTROL Setup]](assets/admin-fund-severity-section.png)

1. Klikken **[!UICONTROL Setup]** in de **[!UICONTROL Main Menu]**.
1. Breid uit **[!UICONTROL Project Preferences]** in het linkerdeelvenster van het menu.
1. Selecteren **[!UICONTROL Severities]**.
1. Klik op **[!UICONTROL Add a New Severity]**.
1. Geef de ernst een naam die overeenkomt met het beoogde gebruik.
1. De **[!UICONTROL Importance]** Het getal komt overeen met de ernst van het probleem. Het hoogste getal komt overeen met de hoogste ernst. De [!UICONTROL Importance] getal moet uniek zijn.
1. Selecteer een kleur voor uw prioriteit. Dit wordt gebruikt in grafiekrapporten en andere plaatsen in [!DNL Workfront].
1. Wijs een van de ernstopties aan als de optie **[!UICONTROL Default Severity]**. Dit wordt automatisch toegepast op alle nieuwe uitgaven in Workfront.
1. Voeg een beschrijving toe van de ernst, zoals de manier waarop het wordt gebruikt.
1. Klik buiten de velden om op te slaan.

![[!UICONTROL Severities] list](assets/admin-fund-severity-new.png)

### De ernst wijzigen

Als een ernst niet meer relevant wordt voor uw uitgifteworkflows, kunt u deze hernoemen, verbergen of verwijderen.

Indien een ernst niet langer nodig is, [!DNL Workfront] raadt u aan de ernst te verbergen (klik op de knop [!UICONTROL Hide] (naast het in het installatiegebied). Hierdoor wordt de optie voor de ernst van de uitgave verwijderd uit het keuzemenu, maar blijft de ernst van de historische gegevens behouden, zodat deze nog steeds beschikbaar zijn voor rapportagedoeleinden.

![[!UICONTROL Hide] kolom gemarkeerd op [!UICONTROL Severities] pagina in [!UICONTROL Setup]](assets/admin-fund-severity-hide.png)

[!DNL Workfront] raadt u aan **niet** een ernst verwijderen die is gebruikt bij eerdere problemen. Wanneer u een ernst verwijdert, wordt u gevraagd een andere ernst te vervangen. Dit kan historische gegevens veranderen en rapportering beïnvloeden.

![Scherpteindheid verwijderen](assets/admin-fund-severity-delete.png)

<!---
learn more URLs
Create and customize issue severities
Update issue severity
--->
