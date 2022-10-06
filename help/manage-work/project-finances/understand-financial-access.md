---
title: Begrijp financiële toegang
description: Met financiële toegangsrechten kunnen beheerders bepalen wie de financiële informatie die in Workfront wordt bijgehouden, kan bekijken en bewerken.
feature: Work Management
thumbnail: understand-financial-access.png
type: Tutorial
role: User
level: Intermediate
kt: 10067
exl-id: 1c3d724a-8ff0-466f-9416-cff3da59c8ea
source-git-commit: d0c842ad8bf6f52161f003a62237fbcd35d23176
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Begrijp financiële toegang

Als uw organisatie financiële gegevens vastlegt met [!DNL Workfront], als systeembeheerder, is het uw verantwoordelijkheid om te beschermen en te beheren wie toegang heeft om die informatie te bekijken en uit te geven.

Er zijn twee dingen nodig voor een gebruiker om financiële informatie te bekijken of te bewerken:

1. Toegangsrechten moeten worden ingeschakeld in de [!UICONTROL Access Level].
2. Toestemming om deze toegangsrechten te gebruiken moet per object worden verleend.

Een gebruiker kan bijvoorbeeld rechten krijgen om financiële gegevens in zijn toegangsniveau te bekijken, maar hij kan alleen financiële gegevens bekijken over een taak die met hem wordt gedeeld en hij kan financieel worden bekeken in het delen van die taak.

Het is dus mogelijk voor een gebruiker met [!UICONTROL Access Level] het recht om financiële gegevens te bekijken zodat financiële gegevens op bepaalde objecten kunnen worden bekeken en niet op andere, afhankelijk van de individuele opties voor delen van die objecten. Geen enkele gebruiker kan echter financiële gegevens over een object bekijken, tenzij hij het recht heeft dat hem in zijn [!UICONTROL Access Level].

## [!UICONTROL Access Level] instellingen

Algehele toegang tot financiële gegevens wordt eerst verleend door [!DNL Workfront] licentietype.

**[!UICONTROL Plan]licenties kunnen:**

* Factureringsrecords beheren
* Rol- en kostenfacturering beheren en bekijken
* Facturering van gebruikers beheren en de kosten bekijken
* Kosten beheren
* Financiën weergeven en bewerken

**[!UICONTROL Work]licenties kunnen:**

* Kosten beheren
* Financiën weergeven

**[!UICONTROL Review]licenties kunnen:**

* Financiën weergeven

**Machtigingen kunnen worden gewijzigd door de [!UICONTROL Access Level]. De drie opties voor toegang tot financiële gegevens zijn:**

* [!UICONTROL No Access] — De gebruiker kan geen financiële informatie zien.
* [!UICONTROL View] — De gebruiker kan de informatie controleren en delen.
* [!UICONTROL Edit] — De gebruiker kan de gegevens maken, bewerken, verwijderen en delen. (Alleen beschikbaar voor een licentie voor abonnementen.)

![Een afbeelding waarin de algemene opties voor financiële gegevens worden weergegeven op een toegangsniveau](assets/setting-up-finances-8.png)

Houd er rekening mee dat de [!UICONTROL View] en [!UICONTROL Edit] opties hebben aanvullende instellingen voor een [!UICONTROL Plan] licentie. Klik op de versnelling op de knop [!UICONTROL View] knop voor deze opties:

**[!UICONTROL View]**

* Rollen en kosten weergeven
* Facturering van gebruikers en kostentarieven weergeven

![Een afbeelding met opties in de weergave Financiële gegevens in een toegangsniveau](assets/setting-up-finances-9.png)

**[!UICONTROL Edit]**

Deze twee opties zijn beschikbaar in het kader van de [!UICONTROL Edit] , samen met:

* Rollenfacturering en kostentarieven bewerken
* Facturering van gebruikers en kostentarieven bewerken

![Een afbeelding met opties voor het bewerken van financiële gegevens in een toegangsniveau](assets/setting-up-finances-10.png)

>[!NOTE]
>
>Een gebruiker met toegang om uitgaven toe te voegen kan ook de uitgaven bekijken die zij, evenals uitgaven toevoegen door hun directe rapporten toevoegen.
