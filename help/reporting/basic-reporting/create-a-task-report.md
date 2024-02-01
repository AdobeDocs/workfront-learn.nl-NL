---
title: Een taakrapport maken
description: Leer hoe u een taakrapport maakt met een complex filter en de rapporten vindt die u maakt in Workfront. Activiteit - maak een notitierapport met aanwijzingen.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335154.png
jira: KT-8859
exl-id: 90bad2e8-9cd2-4ae7-973b-eeab9d615bef
doc-type: video
source-git-commit: 2134c921e39a549808bb11235b32e25903f77df4
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 3%

---

# Een taakrapport maken

In deze video leert u:

* Hoe te om een taakrapport met een complex filter te creëren
* Hoe te de rapporten vinden u creeert

>[!VIDEO](https://video.tv.adobe.com/v/335154/?quality=12&learn=on)

## Activiteit 1: Een notitierapport maken met aanwijzingen

Maak een notitierapport dat u kunt gebruiken om te zoeken naar gebruikersnotities (opmerkingen of updates) of systeemnotities op basis van de inhoud van de notitie, de auteur, de ingangsdatum, de projectnaam of het type audit. Geef het rapport &quot;Note Search&quot; een naam.

Wanneer het gebruiken van de herinnering van de Tekst van de Nota, zal dit rapport binnen updateverbindingen zoeken om het even welke snel te halen die aan de criteria voldoen die in de herinneringen worden gespecificeerd. Wanneer u het rapport in werking stelt, te hoeven u niet om elke herinnering in te vullen, enkel degenen u om geeft. De lege waarden worden automatisch genegeerd.

De weergave moet kolommen bevatten voor:

* Notititie
* Tekst controleren
* Invoerdatum
* Eigenaar: Naam
* Type controle
* Taaknaam
* Naam van uitgave

Laat het filtertabblad leeg.

Groep op projectnaam.

Neem vragen op voor het volgende:

* Tekst controleren
* Notititie
* Naam eigenaar
* Invoerdatum
* Projectnaam
* Type controle

## Antwoord op activiteit 1

1. Selecteren **[!UICONTROL Reports]** van de **[!UICONTROL Main Menu]**.
1. Klik op de knop **[!UICONTROL New Report]** en selecteert u **[!UICONTROL Note]**.
1. In **[!UICONTROL Columns (View)]** Stel uw kolommen zo in dat deze bevatten:

   ![Een afbeelding van het scherm om kolommen met notitierapporten te maken](assets/note-report-columns.png)

   * [!UICONTROL Note] > [!UICONTROL Note Text]
   * [!UICONTROL Note] > [!UICONTROL Audit Text]
   * [!UICONTROL Note] > [!UICONTROL Entry Date]
   * [!UICONTROL Owner] > [!UICONTROL Name]
   * [!UICONTROL Note] > [!UICONTROL Audit Type]
   * [!UICONTROL Task] > [!UICONTROL Name]
   * [!UICONTROL Issue] > [!UICONTROL Name]

1. Selecteer de **[!UICONTROL Entry Date]** en wijzigt u de **[!UICONTROL Sort to Descending]**.
1. In de **[!UICONTROL Groupings]** tab, stel het rapport in op groeperen op [!UICONTROL Project] > [!UICONTROL Name].

   ![Een afbeelding van het scherm om groepen met notitierapporten te maken](assets/note-report-groupings.png)

1. Verlaten [!UICONTROL Filters] leeg.
1. Openen **[!UICONTROL Report Settings]** en noem het rapport &quot;Notitie zoeken&quot;.
1. In de [!UICONTROL Description] veld, zet iets als &quot;Zoeken naar systeem- of gebruikersnotities op basis van het geselecteerde type controle en andere aanwijzingen. De nota&#39;s van het systeem verschijnen in de kolom van de Tekst van de Controle en de nota&#39;s van de Gebruiker verschijnen in de kolom van de Tekst van de Nota.&quot;

   ![Een afbeelding van het scherm om instellingen voor notitierapporten te maken](assets/note-report-report-options.png)

1. Selecteren **[!UICONTROL Details Tab]** zodat het toont wanneer het rapport laadt.
1. Plaats het rapport om 200 punten te tonen wanneer het rapport op een dashboard wordt omvat.
1. Klikken **[!UICONTROL Report Prompts]** en toevoegen:

   ![Een afbeelding van het scherm om herinneringen voor notitierapporten te maken](assets/note-report-report-prompts.png)

   * [!UICONTROL Note] > [!UICONTROL Audit Text]
   * [!UICONTROL Note] > [!UICONTROL Note Text]
   * [!UICONTROL Owner] > [!UICONTROL Name]
   * [!UICONTROL Note] > [!UICONTROL Entry Date]
   * [!UICONTROL Project] > [!UICONTROL Name]
   * [!UICONTROL Note] > [!UICONTROL Audit Type]

1. Schakel het selectievakje in voor **[!UICONTROL Show Prompts in Dashboards]**.
1. Sla uw rapport op en sluit het.

## Activiteit 2: Een feedbackrapport voor een beheerder maken

Dit is een uitgifterapport waarin alle problemen worden weergegeven uit een wachtrij voor feedbackverzoeken die voor systeembeheerders is gemaakt. U kunt zien hoe u deze aanvraagwachtrij kunt maken in het dialoogvenster **Een wachtrij voor feedback van systeembeheerders maken** zelfstudie.

Dit rapport gebruikt ook een aangepast formulier. Als u wilt leren hoe u een aangepast formulier maakt, raadpleegt u de [Een aangepast formulier maken en delen](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/custom-data/custom-forms/custom-forms-creating-and-sharing-a-custom-form.html) zelfstudie.

Dit aangepaste formulier moet als volgt worden gemaakt:

Naam: feedback van beheerproces

1. Procestype (vervolgkeuzelijst)
   * toegangsniveaus
   * goedkeuringsproces (alleen algemeen)
   * e-mailberichten
   * lay-outsjabloon
   * mijlpad
   * projectsjabloon
   * herinneringsmeldingen
   * aanvraagwachtrij
1. Procesnaam (tekstveld met één regel)
1. Proceskwaliteit (vervolgkeuzelijst)
   * 1 - totaal nutteloos
   * 2 - niet erg nuttig
   * 3 - goed, maar beter
   * 4 - uitstekend
1. Probleem of goed nieuws (alineatekstveld)

Een speciaal rapport maken met de naam **Feedbackrapport van het team van Admin**.

De weergave moet de volgende kolommen hebben:

* Issue: Name
* Primaire contactpersoon: Naam
* Probleem: procestype
* Probleem: procesnaam
* Probleem: proceskwaliteit
* Probleem: probleem of goed nieuws
* Uitgifte: Datum van binnenkomst
* Uitgave: Leeftijd
* Probleem: toewijzingen
* Uitgave: status

Groeperen op procestype.

Filter op identiteitskaart van het project van de verzoekrij waar terugkoppelt kwesties verblijven.


![Een schermopname van het feedbackrapport van het Admin-team](assets/create-a-system-admin-feedback-request-queue.png)



## Antwoord op activiteit 2

1. Selecteren **[!UICONTROL Reports]** van de **[!UICONTROL Main Menu]**.
1. Klik op de knop **[!UICONTROL New Report]** en selecteert u **[!UICONTROL Issue]**.
1. In **[!UICONTROL Columns (View)]** Stel uw kolommen zo in dat deze bevatten:

   ![Een beeld van het scherm om de kolommen van het uitgifterapport tot stand te brengen](assets/task-report-activity-2-1.png)

   * [!UICONTROL Issue] > [!UICONTROL Name]
   * [!UICONTROL Primary Contact] > [!UICONTROL Name] Opmerking: dit wordt weergegeven met &quot;Eigenaar:Naam&quot; als kolomlabel. U kunt dit wijzigen in &quot;Gerapporteerd door&quot; door op Geavanceerde opties te klikken en &quot;Gerapporteerd door&quot; te typen in het dialoogvenster **Aangepast kolomlabel** veld.
   * [!UICONTROL Issue] > [!UICONTROL Process type]
   * [!UICONTROL Issue] > [!UICONTROL Process name]
   * [!UICONTROL Issue] > [!UICONTROL Process grade]
   * [!UICONTROL Issue] > [!UICONTROL Problem or good news]
   * [!UICONTROL Issue] > [!UICONTROL Entry date]
   * [!UICONTROL Issue] > [!UICONTROL Age]
   * [!UICONTROL Issue] > [!UICONTROL Assignments]
   * [!UICONTROL Issue] > [!UICONTROL Status]

1. Selecteer de **[!UICONTROL Entry Date]** en wijzigt u de **[!UICONTROL Sort to Descending]**.
1. In de **[!UICONTROL Groupings]** tab, stel het rapport in op groeperen op **[!UICONTROL Issue]>[!UICONTROL Process type]**.

   ![Een afbeelding van het scherm om groepen met uitgifterapporten te maken](assets/task-report-activity-2-2.png)

1. In de **[!UICONTROL Filters]** tabblad, voegt u een filter toe voor de **[!UICONTROL Issue]>[!UICONTROL Project ID]** om het project van de verzoekrij gelijk te maken waar terugkoppelt kwesties verblijven.

   ![Een afbeelding van het scherm om rapportfilters voor problemen te maken](assets/task-report-activity-2-3.png)

1. Sla uw rapport op en sluit het.
