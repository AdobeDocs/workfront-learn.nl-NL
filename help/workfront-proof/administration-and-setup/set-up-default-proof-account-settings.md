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
last-substantial-update: 2024-01-23T00:00:00Z
exl-id: 6eda8bcd-ab0f-4e02-9080-64b6051b327f
source-git-commit: 731005176bc02e3a4d26d00373931fa7444afeea
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 0%

---

# Standaardinstellingen proefdrukaccount instellen

Stel standaardaccountinstellingen in die wereldwijd van toepassing zijn op alle proefdrukken en proefdrukken van gebruikers: land, taal en tijdzone. Als u gebruikers in meerdere tijdzones of landen hebt, kunt u deze instellingen indien nodig aanpassen in het gebruikersprofiel van elk individu.

![Venster met accountinstellingen voor proefdrukken](assets/proof-system-setups-default-account-settings.png)

1. Selecteren **[!UICONTROL Proofing]** van [!DNL Workfront's] [!UICONTROL Main Menu].
1. Selecteren **[!UICONTROL Account Settings]** in de bovenste navigatiebalk.
1. Selecteer de **[!UICONTROL Details]** tab.
1. Ga naar [!UICONTROL Country] veld en selecteer **[!UICONTROL Edit]**. Kies het land waarin het merendeel van uw proefgebruikers zich bevindt als uw standaardinstelling.
1. Selecteren **[!UICONTROL Save]** voor die instelling.
1. Ga naar de [!UICONTROL Default language] veld en selecteer **[!UICONTROL Edit]**. Kies de taal die het merendeel van de proefdrukgebruikers als standaardtaal zal gebruiken.
1. Selecteren **[!UICONTROL Save]** voor die instelling.
1. Ga naar de [!UICONTROL Time zone default] veld en selecteer **[!UICONTROL Edit]**. Kies de tijdzone waarin het merendeel van de proefdrukgebruikers zich standaard bevindt. Dit wordt de tijdzone die wordt herkend door proefwerkstromen die handmatig worden ingesteld. Het zal ook op de malplaatjes van het proefdrukwerkschema van toepassing zijn, maar elk malplaatje kan een tijdstreekreeks hebben.
1. Selecteren **[!UICONTROL Save]** voor die instelling.

## Aanbevolen procedures


| Beste praktijken | Daarom: |
|---|---|
| Pas de instellingen voor de back-endproefdrukken aan, zodat gebruikers deadlines kunnen zien in een kloknotatie van 12 uur. | Selecteer F j, Y, gi:een optie in de proefdrukmontages voor gebruikers die proefdrukdeadlines/tijden in een formaat AM/PM willen zien. Voor gebieden die een klok van 12 uur gebruiken, helpt dit met tijdhelderheid. <br> <br>Opmerking: deze instelling vindt u in het hoofdmenu van Workfront > Proofing > Accountinstellingen > Gebruikers > en in het datumnotatieveld voor elke gebruiker. |
| Stel een standaardproefdeadline in als onderdeel van de systeeminstellingen. | Wanneer een standaardproefdeadline is ingesteld (de uploaddatum + x aantal werkdagen) en de maker van de proefdruk vergeet een deadline toe te voegen, past Workfront deze deadline automatisch toe op elke geüploade proefdruk. <br> <br>Opmerking: deze instelling vindt u in het hoofdmenu van Workfront > Proofing > Accountinstellingen > Instellingen > Standaardinstellingen proef > Deadline (+ werkdagen). |
| Verberg de optie Niet relevante proefdrukbeslissing. | Deze beslissingsoptie veroorzaakt vaak verwarring onder fiatteurs, aangezien organisaties vaak niet bepalen wanneer de Niet relevante optie zou moeten worden gebruikt. De optie Niet relevant geeft in het algemeen aan dat het bewijs niet relevant is voor de bewijsverkrijger en dat het niet nodig is een goedgekeurde of afgewezen beslissing te nemen. Als u Niet relevant selecteert, kan de proefdrukworkflow worden voortgezet.<br> <br>De optie Niet relevant is niet nodig in de meeste proefwerkstromen.<br> <br>Opmerking: deze instelling vindt u in het hoofdmenu van Workfront > Proofing > Accountinstellingen > Besluiten. |
| Wijzig de volgorde van de opties voor de proefdrukbeslissing niet in de proefdrukinstellingen. | Elke bewijsbeslissingsinstelling heeft een specifieke waarde/gewicht die, indien opnieuw geordend, verwarring kan veroorzaken in de proefconfiguraties. De beslissingsvolgorde en de waarde/het gewicht worden gebruikt als activeringsmechanisme voor de proeffase en bij de rapportage.<br> <br>Opmerking: deze instelling vindt u in het hoofdmenu van Workfront > Proofing > Accountinstellingen > Besluiten. |
| Standaardwaarden voor gebruikers instellen voor proefdrukrollen en e-mailwaarschuwingen. | Deze instellingen worden automatisch ingevuld wanneer u een proefwerkstroom toewijst, het proces versnelt en bijdraagt aan consistentie in proefwerkstromen.<br> <br>Opmerking: de standaardinstellingen van de gebruiker vindt u in het hoofdmenu van Workfront > Proofing > Accountinstellingen > Gebruikers > en door de gebruiker te selecteren waarvoor u standaardwaarden wilt instellen. |
