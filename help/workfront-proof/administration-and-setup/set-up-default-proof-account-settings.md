---
title: Standaardinstellingen proefdrukaccount instellen
description: Leer hoe u standaardaccountinstellingen instelt die algemeen gelden voor alle proefdrukken en proefdrukken van gebruikers.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: set-up-proof-actual-default-settings.png
jira: KT-10236
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: 6eda8bcd-ab0f-4e02-9080-64b6051b327f
source-git-commit: 30748311c14fb8aa6b10c03a74e83f46bdb5dfbf
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 0%

---

# Standaardinstellingen proefdrukaccount instellen

Stel standaardaccountinstellingen in die wereldwijd van toepassing zijn op alle proefdrukken en proefdrukken van gebruikers: land, taal en tijdzone. Als u gebruikers in meerdere tijdzones of landen hebt, kunt u deze instellingen indien nodig aanpassen in het gebruikersprofiel van elk individu.

![&#x200B; venster van de montages van de Rekening voor het proef &#x200B;](assets/proof-system-setups-default-account-settings.png)

1. Selecteer **[!UICONTROL Proofing]** in [!DNL Workfront's] [!UICONTROL Main Menu] .
1. Selecteer **[!UICONTROL Account Settings]** in de bovenste navigatiebalk.
1. Selecteer de tab **[!UICONTROL Details]** .
1. Ga naar [!UICONTROL Country] en selecteer **[!UICONTROL Edit]** . Kies het land waarin het merendeel van uw proefgebruikers zich bevindt als uw standaardinstelling.
1. Selecteer **[!UICONTROL Save]** voor die instelling.
1. Ga naar het veld [!UICONTROL Default language] en selecteer **[!UICONTROL Edit]** . Kies de taal die het merendeel van de proefdrukgebruikers als standaardtaal zal gebruiken.
1. Selecteer **[!UICONTROL Save]** voor die instelling.
1. Ga naar het veld [!UICONTROL Time zone default] en selecteer **[!UICONTROL Edit]** . Kies de tijdzone waarin het merendeel van de proefdrukgebruikers zich standaard bevindt. Dit wordt de tijdzone die wordt herkend door proefwerkstromen die handmatig worden ingesteld. Het zal ook op de malplaatjes van het proefdrukwerkschema van toepassing zijn, maar elk malplaatje kan een tijdstreekreeks hebben.
1. Selecteer **[!UICONTROL Save]** voor die instelling.

## Aanbevolen procedures


| Beste praktijken | Daarom: |
|---|---|
| Pas de instellingen voor de back-endproefdrukken aan, zodat gebruikers deadlines kunnen zien in een kloknotatie van 12 uur. | Selecteer F j, Y, gi:een optie in de proefdrukmontages voor gebruikers die proefdrukdeadlines/tijden in een formaat AM/PM willen zien. Voor gebieden die een klok van 12 uur gebruiken, helpt dit met tijdhelderheid. <br> <br> Nota: Deze het plaatsen wordt gevonden door naar het Hoofdmenu van Workfront te gaan > het Beproeven > de Montages van de Rekening > Gebruikers > en het het formaatgebied van de Datum voor elke gebruiker uit te geven. |
| Stel een standaardproefdeadline in als onderdeel van de systeeminstellingen. | Wanneer een standaardproefdeadline is ingesteld (de uploaddatum + x aantal werkdagen) en de maker van de proefdruk vergeet een deadline toe te voegen, past Workfront deze deadline automatisch toe op elke geüploade proefdruk. <br> <br> Nota: Deze het plaatsen wordt gevonden door naar het Hoofdmenu van Workfront > het Proefdrukken > de Montages van de Rekening > Montages > de Gebreken van het Bewijs > Deadline (+ werkdagen) gebied te gaan. |
| Verberg de optie Niet relevante proefdrukbeslissing. | Deze beslissingsoptie veroorzaakt vaak verwarring onder fiatteurs, aangezien organisaties vaak niet bepalen wanneer de Niet relevante optie zou moeten worden gebruikt. De optie Niet relevant geeft in het algemeen aan dat het bewijs niet relevant is voor de bewijsverkrijger en dat het niet nodig is een goedgekeurde of afgewezen beslissing te nemen. Door Niet relevant te selecteren, staat dit het proefdrukwerkschema toe om verder te gaan.<br> <br> de Niet Relevante optie is niet nodig in de meeste proefdrukwerkschema&#39;s.<br> <br> Nota: Deze het plaatsen wordt gevonden door naar het Hoofdmenu van Workfront te gaan > het Proefdrukken > de Montages van de Rekening > Besluiten. |
| Wijzig de volgorde van de opties voor de proefdrukbeslissing niet in de proefdrukinstellingen. | Elke bewijsbeslissingsinstelling heeft een specifieke waarde/gewicht die, indien opnieuw geordend, verwarring kan veroorzaken in de proefconfiguraties. De beslissingsvolgorde en de waarde/het gewicht worden gebruikt als activeringstriggers voor de proeffase en bij rapportage.<br> <br> Nota: Deze het plaatsen wordt gevonden door naar het Hoofdmenu van Workfront te gaan > het Proefdrukken > de Montages van de Rekening > Besluiten. |
| Standaardwaarden voor gebruikers instellen voor proefdrukrollen en e-mailwaarschuwingen. | Deze montages bevolken automatisch wanneer het toewijzen van een proefwerkschema, het proces versnelt, en bijdragend aan consistentie over proefwerkschema&#39;s.<br> <br> Nota: De standaardinstellingen van de gebruiker worden gevonden door naar het Hoofdmenu van Workfront te gaan > het Beproeven > de Montages van de Rekening > Gebruikers > en de gebruiker te selecteren om gebreken voor te plaatsen. |
