---
title: Details van proefdrukken begrijpen
description: Dig dieper in de details achter een proef in  [!DNL &#x200B; Workfront]  door het summiere paneel en [!UICONTROL Document Details] pagina.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: understand-proof-details.png
jira: KT-10110
exl-id: 196f9318-eced-4825-b0fd-8592b6cb3403
source-git-commit: cb72c429f0ef4cd9945282876aa49189dab1bd96
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# Details van proefdrukken begrijpen

## Details van proefdrukken weergeven

Als proefdrukmanager of eigenaar kunt u dieper in de details achter een proefdruk graven door het overzichtspaneel en de [!UICONTROL Document Details] pagina. Begin door uw proef in de [!UICONTROL Documents] sectie van een project, een taak, of een kwestie te vinden.

### Het deelvenster Samenvatting

Selecteer een proefdruk in de documentenlijst en klik vervolgens op het pictogram Samenvatting rechtsboven in het scherm.

![ een beeld van de [!UICONTROL Documents] sectie van een project met geselecteerde proef.](assets/document-summary-1.png)

Klik vervolgens op Overzicht om de overzichtssectie uit te vouwen.

![ een beeld van de [!UICONTROL Documents] sectie van een project met geselecteerde proef en het summiere paneel uitgevouwen. Zowel worden het pictogram van het samenvattingspaneel als het samenvattingsvenster gemarkeerd.](assets/document-summary-2.png)

Schuif vervolgens omlaag naar de sectie Proofing. Hier ziet u de eigenaar van de proefdrukken, de voortgang, het aantal opmerkingen, de status en de vervaldatum.

![ een beeld van de [!UICONTROL Documents] sectie van een project met geselecteerde proef en het summiere paneel uitgevouwen. Zowel worden het pictogram van het samenvattingspaneel als het samenvattingsvenster gemarkeerd.](assets/document-summary-3.png)

Nota: De [!UICONTROL Approvals] sectie in het summiere paneel is voor **document** goedkeuringen en **is niet** gebonden aan het de proefoverzicht en goedkeuringsproces. De twee processen zijn gescheiden in [!DNL Workfront] .

### [!UICONTROL Document Details]

Klik op [!UICONTROL Document Details] voor meer informatie over de proefdruk.

![ een beeld van de [!UICONTROL Documents] sectie van een project met geselecteerde proef en [!UICONTROL Document Details] benadrukt.](assets/document-summary-4.png)

Hiermee gaat u naar de pagina [!UICONTROL Document Details] en een aantal aanvullende opties in het linkerdeelvenster.

![ een beeld van de pagina van de proef in [!DNL &#x200B; Workfront].](assets/document-details.png)

Het is belangrijk om op te merken dat de mogelijkheid om informatie met betrekking tot het proefdrukproces te zien afhankelijk is van uw proefdruktoestemmingen in [!DNL Workfront].

Via de proefdrukpagina hebt u toegang tot de volgende secties via het menu van het linkerdeelvenster:

* **Updates —** Commentaren die in de proefdrukkijker worden gemaakt tonen hier, met een markering van de &quot;proefdrukcommentaar&quot;. U kunt ook opmerkingen maken over het bestand, net zoals u opmerkingen maakt over een taak of project (deze opmerkingen worden niet weergegeven in de proefdrukviewer).
* **goedkeurt —** Deze sectie is voor documentgoedkeuringen, niet het proefdrukken goedkeuringen. De twee typen goedkeuringen zijn afzonderlijke processen in [!DNL Workfront] en zijn niet aan elkaar gekoppeld. Als u proefdrukworkflows gebruikt voor revisies en goedkeuringen, gebruikt u deze sectie niet.
* **Alle Versies —** spoor en beheer de versiegeschiedenis van de proef. Het is misschien gemakkelijker om deze gegevens te openen in het overzichtsvenster in de [!UICONTROL Documents] -lijst.
* **Forms van de Douane -** de vormen van de Douane worden gebruikt op proeven om organisatie-specifieke informatie te vangen. Deze informatie kan samen met het bestand worden doorgegeven aan geïntegreerde documentopslagsystemen, zoals [!DNL Workfront] DAM of Adobe Experience Manager. Aangepaste formulieren worden ingesteld door uw systeembeheerder of groepsbeheerder van [!DNL Workfront] . Bespreek met uw team of uw beheerders of u aangepaste formulieren op proefdrukken wilt gebruiken.
* **het Proofing Workflow —** leidt of wijzigt het werkschema dat aan de proef wordt toegewezen. U kunt dit venster ook openen met de koppeling [!UICONTROL Proofing Workflow] op de proefdruk in de lijst [!UICONTROL Documents] .

Laten we eens nader naar twee van de secties kijken: [!UICONTROL Proofing Viewer Settings] en [!UICONTROL Proofing Activity] .

### [!UICONTROL Proofing Viewer Settings]

Met deze instellingen kunt u de toegang tot de proefdruk zelf beheren.

![ een beeld van [!UICONTROL Proofing Viewer Settings] van de pagina van de proef met de [!UICONTROL Proofing Viewer Settings] optie die in het linkerpaneelmenu wordt benadrukt.](assets/proofing-settings-on-details-page.png)

* **[!UICONTROL Require login. This proof cannot be shared with guest users]—** De proefdruk kan alleen worden gedeeld met personen met een [!DNL Workfront] -proeflicentie.
* **[!UICONTROL Require decisions to be electronically signed]—** Wanneer u een proefdruk deelt, is dit alleen mogelijk als de ontvanger over proefdrukmachtigingen beschikt in [!DNL Workfront] en als de ontvanger de proefdruk elektronisch ondertekent door zijn wachtwoord voor proefdrukken in te voeren wanneer hij of zij een proefdrukbeslissing neemt. (Opmerking: het proefdrukwachtwoord is anders dan het wachtwoord voor [!DNL Workfront] . Het wachtwoord voor proefdrukken is niet gemakkelijk toegankelijk, zodat de meeste ontvangers dit wachtwoord niet weten.) Adobe raadt u aan contact op te nemen met uw [!DNL Workfront] consultant voordat u deze functie gebruikt.
* **[!UICONTROL Lock proof when all required decisions are made]—** Dit sluit het bewijs aan om het even welke verdere commentaren, antwoorden, besluiten, etc., zodra elk besluit over het bewijs is genomen. Hierdoor wordt de hele proefversie vergrendeld, niet alleen een specifiek stadium van de proefdrukworkflow.
* **[!UICONTROL Allow downloading the original file]—** Ontvangers van een proef kunnen het originele bronbestand van de proef van de het proefdrukken kijker downloaden.
* **[!UICONTROL Allow sharing proof via public URL or embed code]—** Ontvangers van het bewijs kunnen een openbaar toegankelijke proefdruk met iedereen delen.
* **[!UICONTROL Allow subscribing to proof via public URL or embed code]—** Iedereen die de openbare URL heeft ontvangen, kan zich aan de proef toevoegen met zijn e-mailadres en naam (als het geen proefgebruikers is) of met zijn e-mailadres en wachtwoord voor proefdrukken (als het een proefdrukgebruiker is). (Opmerking: het proefdrukwachtwoord is niet hetzelfde als een [!DNL Workfront] -wachtwoord.)


### [!UICONTROL Proofing Activity]

Op deze pagina worden alle activiteiten bijgehouden die op de proefdruk zijn uitgevoerd, plus de e-mailberichten die met betrekking tot deze proefdruk zijn verzonden.

![ een beeld van de [!UICONTROL Proofing Activity] sectie van de pagina van de proef met de [!UICONTROL Proofing Activity] optie die in het linkerpaneelmenu wordt benadrukt.](assets/proofing-activity-in-details.png)

De sectie **[!UICONTROL Activity]** bevat tijdstempels voor opmerkingen en beslissingen, plus de persoon die deze heeft gemaakt. Ook wordt bijgehouden wanneer testwerkstroomfasen zijn gestart, wanneer een ontvanger voor het eerst een proefdruk heeft geopend en andere informatie die een bewijsleider of eigenaar wil weten. Deze details kunnen nuttig zijn wanneer u probeert om dingen te ontdekken zoals, waarom een het proefdrukken werkschemafase nooit uit, bijvoorbeeld werd geschopt.

De tijdstempels van de sectie **[!UICONTROL Messages]** wanneer e-mailwaarschuwingen en berichten zijn verzonden naar ontvangers, die ze hebben verzonden, en de inhoud van het bericht. Dit kan nuttig zijn wanneer het oplossen van problemen als iemand zegt zij geen e-mail over een bewijs hebben ontvangen. U kunt controleren of en wanneer een e-mailbericht is verzonden.

Adobe raadt de conceptmanager en de eigenaar van het bewijs aan de informatie in deze twee secties te kennen. Wanneer u deze informatie combineert met inzicht in de manier waarop u de voortgangsbalk van [!UICONTROL SOCD] kunt lezen, kunt u uw proefdrukken echt begrijpen en beheren, ongeacht waar ze zich in de proefdrukworkflow bevinden.

Als u klaar bent met werken in de sectie [!UICONTROL Document Details] , gebruikt u het pad van de broodkruimel om terug te keren naar de sectie [!UICONTROL Documents] van het project, de taak of geeft u de proefdruk op in de bijlage.

![ een beeld van het broodkruimelspoor in de kopbal.](assets/proof-breadcrumb.png)

<!--
#### Learn more
* [!UICONTROL Document details] overview
* Add a custom form to a document
* Request document approvals
* Summary for documents overview
* View activity on a proof within [!DNL Workfront]
-->
