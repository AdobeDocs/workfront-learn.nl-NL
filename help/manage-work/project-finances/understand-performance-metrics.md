---
title: Prestatiewaarden begrijpen
description: 'Leer hoe u de maatstaven voor de prestaties gebruikt: [!UICONTROL Performance Index Method] ([!UICONTROL PIM]) en [!UICONTROL Estimate at Completion] ([!UICONTROL EAC]).'
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10065
exl-id: 190c66f5-b412-48bd-8695-3bd7da088ccb
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---

# Prestatiewaarden begrijpen

Twee prestatiesmetriek die door projectmanagers worden gebruikt omvatten [!UICONTROL Performance Index Method] ([!UICONTROL PIM]) en [!UICONTROL Estimate at Completion] ([!UICONTROL EAC]). Standaardwaarden voor het hele systeem kunnen worden ingesteld in [!DNL Workfront] en worden toegepast op nieuwe projecten. [!UICONTROL PIM] kan vervolgens worden gewijzigd voor afzonderlijke projecten.

**[!UICONTROL PIM]**

De instellingen voor de [!UICONTROL PIM] bepalen hoe [!DNL Workfront] andere maatstaven voor projectprestaties berekent, zoals [!UICONTROL Cost Performance Index] ([!UICONTROL CPI]), [!UICONTROL Cost Schedule Performance Index] ([!UICONTROL CSI]), [!UICONTROL Schedule Performance Index] ([!UICONTROL SPI]) en [!UICONTROL Estimate at Completion] ([!UICONTROL EAC]).

De opties voor [!UICONTROL PIM] zijn gebaseerd op uren en kosten.

* **op uur-Gebaseerde** — Workfront gebruikt de geplande uren in het berekenen van CPI en EAC van het project. De EAC van het project wordt weergegeven als een getal, in uren.
* **Op kosten-gebaseerd** — Workfront gebruikt de geplande arbeidskosten in het berekenen van CPI en EAC van het project. EAC wordt weergegeven als een valutawaarde. Wanneer u deze optie gebruikt, moet u ervoor zorgen dat taaktoewijzingen (gebruikers en/of functies) aan kostentarieven zijn gekoppeld.

**[!UICONTROL EAC]**

[!UICONTROL EAC] geeft de geraamde totale kosten van uw taak of project weer wanneer deze zijn voltooid. De opties worden berekend op een projectniveau en rollen omhoog van taken/subtaken.

* **berekent op projectniveau** - [!UICONTROL EAC] voor de oudertaak en het project worden bepaald gebruikend de daadwerkelijke uren/daadwerkelijke arbeidskosten in [!UICONTROL EAC] formules. De berekening omvat de werkelijke uren/kosten en uitgaven die rechtstreeks aan de bovenliggende taak of het bovenliggende project zijn toegevoegd.
* R **omhoog vanaf taken/subtasks** - [!UICONTROL EAC] voor de oudertaak en het project worden bepaald door omhoog [!UICONTROL EAC] voor elke kindtaak toe te voegen. Deze berekening sluit de werkelijke uren/kosten uit die rechtstreeks aan een bovenliggende taak of project worden toegevoegd.

De [!UICONTROL EAC] berekeningen worden vermeld in [ Berekenen schatten bij Voltooiing (EAC) ](https://experienceleague.adobe.com/docs/workfront/using/manage-work/projects/project-finances/calculate-eac.html?lang=en).

**Metriek van Prestaties: Montages**

Als u de standaardinstellingen van [!UICONTROL PIM] en [!UICONTROL EAC] wilt instellen:

1. Selecteer **[!UICONTROL Setup]** in het hoofdmenu.
1. Klik op **[!UICONTROL Project Preferences]** in het menu van het linkerdeelvenster en klik vervolgens op **[!UICONTROL Projects]**
1. Ga naar [!UICONTROL Performance Index Method] in de sectie [!UICONTROL Project Status] . Selecteer op uren of op kosten-gebaseerd.
1. Selecteer voor [!UICONTROL Estimate at Completion] Berekenen op projectniveau of Naar boven rollen op basis van taken/subtaken.
1. Klik op **[!UICONTROL Save]** onder in het venster.

![ een beeld van het [!UICONTROL Project Preferences] scherm ](assets/setting-up-finances-1.png)

**Reeks [!UICONTROL PIM] op individuele projecten**

1. Ga naar de landingspagina van een project.
1. Klik op **[!UICONTROL Project Details]** in het linkerdeelvenster.
1. Open de sectie **[!UICONTROL Finance]** .
1. Dubbelklik op de onderstaande tekst **[!UICONTROL Performance Index Method]** om deze te bewerken.
1. Selecteer op uren of op kosten-gebaseerd.
1. Klik op **[!UICONTROL Save]** Wijzigingen om te voltooien.

![ een beeld van het [!UICONTROL Project Details] scherm ](assets/setting-up-finances-2.png)

[!UICONTROL PIM] kan op een projectmalplaatje, in [!UICONTROL Finance] sectie van de malplaatjedetails worden geplaatst.
