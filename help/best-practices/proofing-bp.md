---
title: Best practices - Proofing
description: Ontdek de aanbevelingen met best practices van Adobe Workfront-experts over het instellen, beheren en gebruiken van proefdrukken in Workfront.
feature: Workfront Proof
role: Admin, Leader, User
level: Beginner
jira: KT-10920
exl-id: 394485ee-bb8f-4248-86a9-4c86174dd37f
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# Best practices - Proofing

## Wat is een &quot;beste praktijk&quot; van Adobe Workfront?

De beste praktijken zijn richtsnoeren die een efficiënte, efficiënte manier van handelen vertegenwoordigen; gemakkelijk door u en de gebruikers bij uw bedrijf worden aangenomen; en kan met succes over uw organisatie worden herhaald.

Houd er bij het beoordelen van deze aanbevelingen rekening mee dat sommige Workfront-best practices universeel zijn, terwijl andere specifieker voor het onderwerp kunnen zijn. Gebruik deze aanbevolen procedures als een raamwerk voor hulp bij het instellen en gebruiken van Workfront-systemen.

## Navigeren door deze pagina

Wanneer u door deze pagina bladert, vindt u eerst een lijst op hoog niveau met alle aanbevolen werkwijzen voor het onderwerp. Zo kunt u de aanbevelingen bekijken zonder in de details van &quot;waarom&quot; te duiken.

&quot;Waarom zijn deze beste praktijken?&quot; in de lijst op hoog niveau vindt u meer details over een aantal van de aanbevolen procedures en waarom deze worden beschouwd als een proces, gereedschap, enzovoort. U kunt het beste eerst een Workfront-exemplaar implementeren.

</br>
</br>

## Proofing in Workfront best practices

* Neem de tijd om testwerkstroomsjablonen te maken.

* Schakel de instelling E-mailbericht verzenden vanuit Workfront uit wanneer er een opmerking wordt gemaakt over een proefdruk in de Workfront-instellingen.

* Gebruik alleen-lezen of Revisor voor de instelling Rollen voor niet-ontvangers die een proefdruk van een document openen in Workfront.

* Pas de instellingen voor de back-endproefdrukken aan, zodat gebruikers deadlines kunnen zien in een kloknotatie van 12 uur.

* Stel een standaardproefdeadline in als onderdeel van de systeeminstellingen.

* Verberg de optie Niet relevante proefdrukbeslissing.

* Wijzig de volgorde van de opties voor de proefdrukbeslissing niet in de proefdrukinstellingen.

* Standaardwaarden voor gebruikers instellen voor proefdrukrollen en e-mailwaarschuwingen.

* Stel de proefdrukrol van de maker in op Revisor.

* Gebruik niet de proefdrukrol fiatteur.

* Vermijd de waarschuwingsoptie E-mailbericht dat alle activiteiten moet worden gecontroleerd.

</br>
</br>

## Waarom zijn deze beste praktijken?

**Beste praktijken**

Neem de tijd om testwerkstroomsjablonen te maken.

**Hieronder wordt beschreven waarom**

Met sjablonen kunt u niet alleen het maken en toewijzen van proefdrukken versnellen en stroomlijnen, maar ook consistente workflows voor proefdrukken voor vergelijkbare typen elementen. Zij zorgen er ook voor dat aan elke ontvanger van het bewijs de juiste bewijsrol en e-mailalarm wordt toegewezen, en dat een termijn is vastgesteld.

</br>
</br>

**Beste praktijken**

Schakel de instelling E-mailbericht verzenden vanuit Workfront uit wanneer er een opmerking wordt gemaakt over een proefdruk in de Workfront-instellingen.



**Hieronder wordt beschreven waarom**

Als deze instelling is ingeschakeld (standaard ingeschakeld), kunnen gebruikers meerdere e-mailmeldingen ontvangen voor elke opmerking op een proefdruk. Dit is een van de proefdrukfuncties en een van Workfront zelf. Deze dubbele meldingen leiden tot verstoring en verwarring van e-mailmeldingen en tot een volledig e-mailpostvak. Hierdoor kunnen gebruikers proofmeldingen die ze ontvangen, negeren. Dat zou op zijn beurt kunnen betekenen dat er geen termijnen worden gesteld.



**Opmerking**: Deze instelling vindt u in het Workfront Main Menu > Setup > Email > Review and Approval.

</br>
</br>

**Beste praktijken**

Gebruik alleen-lezen of Revisor voor de instelling Rollen voor niet-ontvangers die een proefdruk van een document openen in Workfront.



**Hieronder wordt beschreven waarom**

Voor alle andere opties voor deze instelling moet een proefdrukbeslissing worden genomen. Hierdoor kan de proefdrukworkflow worden verwijderd. Over het algemeen geldt dat mensen die niet aan de proefdrukworkflow worden toegevoegd, alleen de proefdrukproef moeten bekijken of opmerkingen moeten maken, de proefdrukproef niet moeten goedkeuren. De opties Alleen-lezen of Reviewer zijn dus de beste keuze.



**Opmerking**: Deze instelling vindt u in Workfront Main Menu > Setup > Review and Approval.

</br>
</br>

**Beste praktijken**

Pas de instellingen voor de back-endproefdrukken aan, zodat gebruikers deadlines kunnen zien in een kloknotatie van 12 uur.



**Hieronder wordt beschreven waarom**

Selecteer F j, Y, gi:een optie in de proefdrukmontages voor gebruikers die proefdrukdeadlines/tijden in een formaat AM/PM willen zien. Voor gebieden die een klok van 12 uur gebruiken, helpt dit met tijdhelderheid.



**Opmerking**: U vindt deze instelling door naar het hoofdmenu van Workfront > Proofing > Accountinstellingen > Gebruikers > te gaan en het veld Datumnotatie voor elke gebruiker te bewerken.

</br>
</br>

**Beste praktijken**

Stel een standaardproefdeadline in als onderdeel van de systeeminstellingen.



**Hieronder wordt beschreven waarom**

Wanneer een standaardproefdeadline is ingesteld (de uploaddatum + x aantal werkdagen) en de maker van de proefdruk vergeet een deadline toe te voegen, past Workfront deze deadline automatisch toe op elke geüploade proefdruk.



**Opmerking**: U vindt deze instelling door naar het veld Workfront Main Menu > Proofing > Account Settings > Settings > Proof Defaults > Deadline (+ werkdagen) te gaan.

</br>
</br>


**Beste praktijken**

Verberg de optie Niet relevante proefdrukbeslissing.



**Hieronder wordt beschreven waarom**

Deze beslissingsoptie veroorzaakt vaak verwarring onder fiatteurs, aangezien organisaties vaak niet bepalen wanneer de Niet relevante optie zou moeten worden gebruikt. De optie Niet relevant geeft in het algemeen aan dat het bewijs niet relevant is voor de bewijsverkrijger en dat het niet nodig is een goedgekeurde of afgewezen beslissing te nemen. Als u Niet relevant selecteert, kan de proefdrukworkflow worden voortgezet.


De optie Niet relevant is niet nodig in de meeste proefwerkstromen.

**Opmerking**: U vindt deze instelling door naar het hoofdmenu van Workfront > Proofing > Accountinstellingen > Besluiten te gaan.

</br>
</br>

**Beste praktijken**

Wijzig de volgorde van de opties voor de proefdrukbeslissing niet in de proefdrukinstellingen.



**Hieronder wordt beschreven waarom**

Elke bewijsbeslissingsinstelling heeft een specifieke waarde/gewicht die, indien opnieuw geordend, verwarring kan veroorzaken in de proefconfiguraties. De beslissingsvolgorde en de waarde/het gewicht worden gebruikt als activeringsmechanisme voor de proeffase en bij de rapportage.



**Opmerking**: U vindt deze instelling door naar het hoofdmenu van Workfront > Proofing > Accountinstellingen > Besluiten te gaan.

</br>
</br>

**Beste praktijken**

Standaardwaarden voor gebruikers instellen voor proefdrukrollen en e-mailwaarschuwingen.



**Hieronder wordt beschreven waarom**

Deze instellingen worden automatisch ingevuld wanneer u een proefwerkstroom toewijst, het proces versnelt en bijdraagt aan consistentie in proefwerkstromen.



**Opmerking**: Standaardinstellingen voor gebruikers worden gevonden door naar het hoofdmenu van Workfront > Proofing > Accountinstellingen > Gebruikers > te gaan en de gebruiker te selecteren waarvoor u standaardwaarden wilt instellen.

</br>
</br>

**Beste praktijken**

Stel de proefdrukrol van de maker in op Revisor.



**Hieronder wordt beschreven waarom**

Met de proefdrukrol van Revisor kan de maker van de proefdruk opmerkingen maken en opmerkingen van anderen openen. Meestal hoeft de maker van het bewijs geen beslissing te nemen over een bewijs dat hij heeft geüpload. Voor de rollen fiatteur, Reviewer en fiatteur, Auteur of Moderator proof moet een beslissing worden genomen. Als de maker van het bewijs een van deze bewijsrollen krijgt toegewezen maar nooit een besluit neemt, kan dit negatieve gevolgen hebben voor de bewijstermijnen.

</br>
</br>

**Beste praktijken**

Gebruik niet de proefdrukrol fiatteur.



**Hieronder wordt beschreven waarom**

Met de proefdrukrol fiatteur kan de gebruiker geen opmerkingen maken over deze proefdruk. Dit kan ertoe leiden dat een gebruiker de proefdruk verwerpt zonder uitleg, omdat hij geen opmerkingen kan maken. Gebruik in plaats hiervan de proefdrukrol Reviewer en fiatteur, zodat de gebruiker feedback kan geven.

</br>
</br>

**Beste praktijken**

Vermijd de waarschuwingsoptie E-mailbericht dat alle activiteiten moet worden gecontroleerd.

**Hieronder wordt beschreven waarom**

Met deze optie wordt een e-mailmelding met een proefdruk verzonden wanneer er iets gebeurt met een proefdruk. Er wordt een opmerking toegevoegd, een antwoord wordt geplaatst, er wordt een beslissing genomen, enzovoort. De ontvanger ziet in wezen de bewijskracht.

Voor eigenaars en makers van bewijzen werkt de e-mailwaarschuwing voor beslissingen het beste voor werkstromen met meerdere etappes en het uiteindelijke besluit werkt het best voor werkstromen in één fase. In het algemeen kan iedereen anders worden ingesteld op Uitgeschakeld, tenzij hij of zij op de hoogte wil worden gesteld van anderen die opmerkingen maken of beslissingen nemen (in dat geval werkt een van de opties voor samenvattende e-mail het beste).
