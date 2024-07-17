---
title: Tips en trucs - Filters, Weergaven en Groepen
description: Bekijk de aanbevelingen van Adobe Workfront-experts over het instellen, beheren en gebruiken van Workfront-filters, -weergaven en -groepen.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10911
exl-id: 845aa0b4-3fe9-4bc1-9dde-2f22c537e758
source-git-commit: 0ff5accae867f07cc31ac2be7b0c12981412346e
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 0%

---

# Tips en trucs - Filters, Weergaven en Groepen

## Wat is een &quot;beste praktijk&quot; van Adobe Workfront?

De beste praktijken zijn richtlijnen die een efficiënte, efficiënte actie vertegenwoordigen; gemakkelijk door u en de gebruikers bij uw bedrijf worden aangenomen; en kunnen met succes over uw organisatie worden herhaald.

Houd er bij het beoordelen van deze aanbevelingen rekening mee dat sommige Workfront-best practices universeel zijn, terwijl andere specifieker voor het onderwerp kunnen zijn. Gebruik deze aanbevolen procedures als een raamwerk voor hulp bij het instellen en gebruiken van Workfront-systemen.

## Navigeren door deze pagina

Wanneer u door deze pagina bladert, vindt u eerst een lijst op hoog niveau met alle aanbevolen werkwijzen voor het onderwerp. Zo kunt u de aanbevelingen bekijken zonder in de details van &quot;waarom&quot; te duiken.

&quot;Waarom zijn deze beste praktijken?&quot; in de lijst op hoog niveau vindt u meer details over een aantal van de aanbevolen procedures en waarom deze worden beschouwd als een proces, gereedschap, enzovoort. U kunt het beste eerst een Workfront-exemplaar implementeren.

</br>
</br>

## Aanbevolen werkwijzen voor filters, weergaven en groepen

* Knip het aantal aangepaste rapporten dat u maakt af door filters, weergaven en groepen in een objectlijst te gebruiken om de gegevens op te halen die u nodig hebt.

* Gebruik de lijstcontroles in lay-outmalplaatjes om onnodige filters, meningen, en groepen voor algemeen gebruikte voorwerpen (projecten, taken, programma&#39;s, enz.) te verbergen.

* Deel aangepaste filters, weergaven en groeperingen die relevant zijn voor de workflows en processen van uw organisatie via de lijstbesturingselementen voor lay-outsjablonen.

* Wanneer u filters maakt voor de projectstatus, taakstatus of uitgiftestatus, gebruikt u de instructie (object)>>Status is gelijk aan de naam van de veldbron/het veld met de optie Gelijk, in plaats van Project>>Bron/veldnaam van het statusveld.

</br>
</br>

## Waarom zijn deze beste praktijken?

**Beste praktijken**

Knip het aantal aangepaste rapporten dat u maakt af door filters, weergaven en groepen in een objectlijst te gebruiken om de gegevens op te halen die u nodig hebt.

**hier is waarom**

Het maken van eenmalige gebruiksrapporten voor elk gegevenssegment dat u wilt zien, is tijdrovend en werkt het Workfront-systeem in de war.

Voor instructies op hoe te om rapporten met herinneringen tot stand te brengen zien het hoofdstuk geëtiketteerd &quot;hoe te opstelling en gebruiksrapportherinneringen&quot;in [ begrijpt rapportmontages ](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/report-settings.html) video.

Voor instructies op hoe te om rapporten met douaneherinneringen tot stand te brengen zie [ douaneherinneringen ](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/custom-prompts.html) creëren.

</br>
</br>

**Beste praktijken**

Gebruik de lijstcontroles in lay-outmalplaatjes om onnodige filters, meningen, en groepen voor algemeen gebruikte voorwerpen (projecten, taken, programma&#39;s, enz.) te verbergen.

**hier is waarom**

Minder is meer. Het verbergen van filter, mening, en het groeperen van lijstopties die niet relevant voor de dagelijkse werkschema&#39;s van uw gebruikers zijn vernauwt de lijsten, wat het voor gebruikers gemakkelijker maakt om te vinden wat zij sneller nodig hebben.

Voor instructies op hoe te om filters, meningen, of groeperingen met lay-outmalplaatjes te verbergen zie [ rapportlijsten met lay-outmalplaatjes ](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/administration-and-setup/layout-templates/customize-reporting-lists-with-layout-templates.html) aanpassen.

</br>
</br>

**Beste praktijken**

Deel aangepaste filters, weergaven en groeperingen die relevant zijn voor de workflows en processen van uw organisatie via de lijstbesturingselementen voor lay-outsjablonen.

**hier is waarom**

Als u filters, meningen, en groeperingen hebt gecreeerd die informatie specifiek voor de dagelijkse processen van gebruikers tonen, is het gemakkelijk om deze door de lay-outmalplaatjes te delen. Dit verzekert iedereen toegewezen die lay-outmalplaatje filter, mening, en groeperingsopties relevant voor hun werkschema heeft.

Het aanpassen van de informatie die u voor uw gebruikers zichtbaar door de lay-outmalplaatjes wilt is ook een tijd-redder voor systeem en groepsbeheerders omdat zij niet elke filter, mening, of groeperingsoptie individueel zullen moeten delen.

Voor instructies op hoe te om filters, meningen, of groeperingen met lay-outmalplaatjes te delen zie [ rapporteringslijsten met lay-outmalplaatjes ](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/administration-and-setup/layout-templates/customize-reporting-lists-with-layout-templates.html) aanpassen.

</br>
</br>

**Beste praktijken**

Wanneer u filters maakt voor de projectstatus, taakstatus of uitgiftestatus, gebruikt u de instructie (object)>>Status is gelijk aan de naam van de veldbron/het veld met de optie Gelijk, in plaats van Project>>Bron/veldnaam van het statusveld.

**hier is waarom**

Door (object)>>Equates with te gebruiken, neemt u alle aangepaste statussen op die die specifieke status hebben toegewezen in het veld Equates with in de statusinstellingen. Terwijl u het filter instelt als (object)>>Status > Gelijk vereist dat u specifieke statuten voor het filter selecteert. Dit zou een onderhoudsuitdaging kunnen betekenen als u voor die nieuwe statussen in diverse filters rekenschap moet geven. Elk filter moet worden geopend en bijgewerkt met de nieuwe status.

Als u bijvoorbeeld alle huidige projecten wilt zien, kunt u het filter zo instellen dat Project > > Status > Gelijk > Huidige staat wordt gelezen. Maar als iemand een douanestatus genoemd Actief toevoegt en het aan Huidig vergelijkt, zal dat filter geen projecten met de Actieve status vinden. Als u echter Project>>Status is gelijk aan > Gelijk > Huidig, zoekt het filter objecten met de status Huidig of Actief omdat ze beide Huidig hebben in het veld Gelijk aan.
