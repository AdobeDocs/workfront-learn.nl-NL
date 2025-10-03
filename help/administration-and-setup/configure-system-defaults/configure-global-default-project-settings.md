---
title: Algemene standaardprojectinstellingen configureren
description: Leer hoe u een aangepaste status wijzigt, algemene projectvoorkeuren instelt en schema's maakt die algemene standaardinstellingen zijn.
feature: System Setup and Administration
role: Admin
level: Intermediate
activity: deploy
type: Tutorial
team: Technical Marketing
thumbnail: 335065.png
jira: KT-8753
exl-id: b961ba8c-9597-4ed4-a6d7-79689c8e290d
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# Algemene standaardprojectinstellingen configureren

<!--
21.4 updates have been made
-->

In deze video leert u hoe u:

* Een aangepaste status wijzigen
* Algemene projectvoorkeuren instellen
* Planningen maken en gebruiken

>[!VIDEO](https://video.tv.adobe.com/v/335065/?quality=12&learn=on&enablevpops=1)

## Globale en groepsproject-, taak- en uitgaven-instellingen

Wanneer u de [!UICONTROL Projects] montages in [!DNL Workfront] opent, zult u merken het &quot; [!UICONTROL System Project Preferences]&quot;in de onderzoeksbar bij de bovenkant van het venster zegt. Dit laat u weten deze montages iedereen in uw [!DNL Workfront] systeem beïnvloeden — het is een globale configuratie.

![[!UICONTROL Project Preferences] pagina in [!UICONTROL Setup]](assets/admin-fund-system-project-preferences-1.png)

Wanneer u de [!UICONTROL Tasks & Issues] -instellingen opent, ziet u iets gelijkaardigs.

![[!UICONTROL Task & Issue Preferences] in [!UICONTROL Setup]](assets/admin-fund-task-issue-preferences-2.png)

Het is echter mogelijk dat niet elke groep in [!DNL Workfront] hetzelfde project, dezelfde taak en dezelfde voorkeuren voor uitgaven nodig heeft. Bijvoorbeeld, wil de marketing groep de status van een nieuw project plant terwijl de groep van de projectmanager de status van het Verzoek verkiest.

Met [!DNL Workfront] kunnen groepsbeheerders bepaalde project-, taak- en uitgavevoorkeuren voor hun groepen aanpassen. Welke voorkeuren kunnen worden aangepast, wordt bepaald door de systeembeheerder van [!DNL Workfront] met behulp van de schakelopties voor vergrendelen en ontgrendelen.

Begin door naar het [!UICONTROL Setup] -gebied te navigeren:

1. Selecteer **[!UICONTROL Setup]** in de **[!UICONTROL Main Menu]** .
1. Vouw **[!UICONTROL Project Preferences]** in het linkermenu uit.
1. Selecteer **[!UICONTROL Projects]** of **[!UICONTROL Tasks & Issues]** , afhankelijk van de instellingen die u wilt wijzigen.

Vergrendel een voorkeur om te voorkomen dat groepsbeheerders die instelling voor hun groep aanpassen.

![ Vergrendeld voorkeursbericht ](assets/admin-fund-preferences-locked-3.png)

Ontgrendel de voorkeur om het voor groepsbeheerders ter beschikking te stellen om aan te passen.

![ Ontgrendeld voorkeursbericht ](assets/admin-fund-preferences-unlocked-4.png)

Sommige instellingen kunnen niet worden ontgrendeld en blijven algemene systeeminstellingen.

![ Vergrendeld voorkeursbericht ](assets/admin-fund-preferences-always-locked-5.png)

### Voorkeuren voor groepen en subgroepen instellen

Voor instellingen die door de systeembeheerder zijn ontgrendeld, kunnen de groepbeheerders aanpassingen aanbrengen voor de groep(en) die zij beheren en voor subgroepen die onder die groepen zijn genest. Bovendien kunnen groepsbeheerders bepalen welke instellingen hun subgroepbeheerders kunnen wijzigen.

1. Selecteer **[!UICONTROL Setup]** in de **[!UICONTROL Main Menu]** .
1. Klik op **[!DNL Groups]** in het linkermenu.
1. Klik op de naam van de groep of subgroep om deze te openen.
1. Selecteer **[!UICONTROL Project Preferences]** of **[!UICONTROL Tasks & Issues Preferences]** in het linkermenu.
1. Breng de benodigde wijzigingen aan voor elk van de ontgrendelde voorkeuren.
1. Selecteer **[!UICONTROL Save]**.

![[!UICONTROL Project Status] -sectie op [!UICONTROL Group] page ](assets/admin-fund-group-preferences.png)

Als uw organisatie geen groepsbeheerders gebruikt, kan de systeembeheerder de voorkeursinstellingen voor de verschillende groepen beheren.

<!--
learn more URLs and guides
Create or edit a group status 
Group administrators 
Configure system-wide project preferences 
Configure project preferences for a group 
Configure task and issue preferences for a group 
Create and modify a group’s schedule 
-->
