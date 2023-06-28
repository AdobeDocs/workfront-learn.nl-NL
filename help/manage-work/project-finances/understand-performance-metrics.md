---
title: Prestatiewaarden begrijpen
description: Leer hoe u de prestatiemetriek kunt gebruiken - de [!UICONTROL Performance Index Method] ([!UICONTROL PIM]) en de [!UICONTROL Estimate at Completion] ([!UICONTROL EAC]).
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
source-wordcount: '360'
ht-degree: 0%

---

# Prestatiewaarden begrijpen

Twee prestatiesmetriek die door projectmanagers worden gebruikt omvatten [!UICONTROL Performance Index Method] ([!UICONTROL PIM]) en de [!UICONTROL Estimate at Completion] ([!UICONTROL EAC]). Systeembrede standaardinstellingen kunnen worden ingesteld in [!DNL Workfront] en geldt voor nieuwe projecten. [!UICONTROL PIM] kan vervolgens worden gewijzigd voor afzonderlijke projecten.

**[!UICONTROL PIM]**

De instellingen voor de [!UICONTROL PIM] bepalen hoe [!DNL Workfront] berekent andere metriek van projectprestaties zoals [!UICONTROL Cost Performance Index] ([!UICONTROL CPI]), [!UICONTROL Cost Schedule Performance Index] ([!UICONTROL CSI]), [!UICONTROL Schedule Performance Index] ([!UICONTROL SPI]), en [!UICONTROL Estimate at Completion] ([!UICONTROL EAC]).

Opties voor de [!UICONTROL PIM] zijn gebaseerd op uren en kosten.

* **Uur** — Workfront gebruikt de geplande uren voor de berekening van de CPI en de EAC van het project. De EAC van het project wordt weergegeven als een getal, in uren.
* **Op basis van kosten** — Workfront gebruikt de geplande loonkosten voor de berekening van de CPI en de EAC van het project. EAC wordt weergegeven als een valutawaarde. Wanneer u deze optie gebruikt, moet u ervoor zorgen dat taaktoewijzingen (gebruikers en/of functies) aan kostentarieven zijn gekoppeld.

**[!UICONTROL EAC]**

[!UICONTROL EAC] geeft de geraamde totale kosten van uw taak of project weer wanneer deze zijn voltooid. De opties worden berekend op een projectniveau en rollen omhoog van taken/subtaken.

* **Berekenen op projectniveau** — [!UICONTROL EAC] voor de moedertaak en het project worden bepaald aan de hand van de werkelijke uren/werkelijke loonkosten in [!UICONTROL EAC] formules. De berekening omvat de werkelijke uren/kosten en uitgaven die rechtstreeks aan de bovenliggende taak of het bovenliggende project zijn toegevoegd.
* R **opladen van taken/subtaken** — [!UICONTROL EAC] voor de oudertaak en het project worden bepaald door omhoog het [!UICONTROL EAC] voor elke onderliggende taak. Deze berekening sluit de werkelijke uren/kosten uit die rechtstreeks aan een bovenliggende taak of project worden toegevoegd.

De [!UICONTROL EAC] berekeningen worden vermeld in [Schatting berekenen bij voltooiing (EAC)](https://experienceleague.adobe.com/docs/workfront/using/manage-work/projects/project-finances/calculate-eac.html?lang=en).

**Prestatiewaarden: Instellingen**

In te stellen [!UICONTROL PIM] en [!UICONTROL EAC] systeemstandaardinstellingen:

1. Selecteren **[!UICONTROL Setup]** in het hoofdmenu.
1. Klikken **[!UICONTROL Project Preferences]** klikt u in het menu van het linkerdeelvenster op **[!UICONTROL Projects]**
1. In de [!UICONTROL Project Status] sectie, zoeken [!UICONTROL Performance Index Method]. Selecteer op uren of op kosten-gebaseerd.
1. Voor [!UICONTROL Estimate at Completion]selecteert u Berekenen op projectniveau of Naar boven rollen vanuit taken/subtaken.
1. Klikken **[!UICONTROL Save]** onder aan het venster.

![Een afbeelding van de [!UICONTROL Project Preferences] scherm](assets/setting-up-finances-1.png)

**Set [!UICONTROL PIM] betreffende individuele projecten**

1. Ga naar de landingspagina van een project.
1. Klikken **[!UICONTROL Project Details]** in het linkerdeelvenster.
1. Open de **[!UICONTROL Finance]** sectie.
1. Dubbelklik op de onderstaande tekst **[!UICONTROL Performance Index Method]** om het te bewerken.
1. Selecteer op uren of op kosten-gebaseerd.
1. Klikken **[!UICONTROL Save]** Wijzigingen die moeten worden voltooid.

![Een afbeelding van de [!UICONTROL Project Details] scherm](assets/setting-up-finances-2.png)

[!UICONTROL PIM] kan op een projectmalplaatje worden geplaatst, in [!UICONTROL Finance] van de sjabloondetails.
