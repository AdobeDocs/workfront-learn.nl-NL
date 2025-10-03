---
title: Een algemeen goedkeuringsproces en een goedkeuringsproces voor één gebruik maken
description: Leer hoe u een globaal goedkeuringsproces en een goedkeuringsproces voor één gebruik kunt maken voor een project, taak of uitgave.
activity: use
feature: Approvals
thumbnail: 335225.jpeg
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-8962
hide: true
doc-type: video
exl-id: e80dd36f-7aab-4cf1-873c-92dba684c13c
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# Een algemeen goedkeuringsproces en een goedkeuringsproces voor één gebruik maken

De processen van de goedkeuring op projecten, taken, en kwesties staan een projectmanager toe om deskundige bevestiging te krijgen dat het werk onmiddellijk is gedaan alvorens vooruit te gaan. De projectmanager kan een goedkeuringsproces voor elke situatie (dit wordt genoemd geworden enig-gebruik goedkeuringsproces) tot stand brengen of van een lijst van misschien vele goedkeuringsprocessen kiezen die eerder zijn gecreeerd om aan gemeenschappelijke behoeften (deze zijn genoemd als globaal, of bestaand, goedkeuringsprocessen) te voldoen.

Wanneer de objectstatus verandert in een status die is opgegeven in het goedkeuringsproces, wordt de fiatteur op verschillende manieren op de hoogte gesteld van het beoordelen van het werk en het goedkeuren of afwijzen ervan. Aangezien het hele project kan worden gepauzeerd in afwachting van een goedkeuring, moeten de fiatteurs er van tevoren van op de hoogte zijn dat zij om goedkeuring kunnen worden verzocht. Indien een fiatteur om welke reden dan ook buiten het kantoor is, mogen zij hun goedkeuringen delegeren aan een gekwalificeerde plaatsvervanger. Zie [ de taken, kwesties, en goedkeuringen van de Afgevaardigde ](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md) voor details.

In deze video leert u hoe u een algemeen goedkeuringsproces en een goedkeuringsproces voor één gebruik kunt maken voor een project, taak of uitgave.

>[!VIDEO](https://video.tv.adobe.com/v/335225/?quality=12&learn=on&enablevpops=1)

>[!TIP]
>
>U kunt één enkel proces van de gebruiksgoedkeuring voor een project of een taak aan een projectmalplaatje toevoegen.

>[!NOTE]
>
>U kunt één enkele gebruiksgoedkeuring voor projecten en kwesties op de zelfde manier plaatsen zoals die voor taken in de video wordt beschreven.

## Hoe te om automatische emissievergunningen in een verzoekrij toe te passen

Als u automatische goedkeuringen voor uitgaven wilt instellen in een aanvraagwachtrij, kunnen deze alleen worden uitgevoerd via een algemeen goedkeuringsproces voor uitgaven en worden deze toegepast in een [!UICONTROL Queue topic] .

Selecteer bij het maken of bewerken van een [!UICONTROL Queue topic] het algemene goedkeuringsproces in het veld **[!UICONTROL Default Approval]** .

![ Beeld dat hoe te om een standaardgoedkeuringsproces in een rijonderwerp te selecteren ](assets/automatic-issue-approval-1.png)

Mogelijk moet u het goedkeuringsproces voor uitgaven bewerken om ervoor te zorgen dat **[!UICONTROL Previous status]** niet is ingesteld op het moment dat de goedkeuring wordt geweigerd. De reden hiervoor is dat de vorige status **[!UICONTROL New]** is. Dit is ook de status die het goedkeuringsproces activeert. Het is dus de status waarop deze wordt ingesteld wanneer deze wordt goedgekeurd. Om verwarring te voorkomen wanneer de goedkeuring van het probleem wordt afgewezen, is het beter om de status in te stellen op een soort **[!UICONTROL Won't Resolve]** of een aangepaste status die voor dit doel is gemaakt.

![ Beeld dat het veranderen van de status toont te gebruiken wanneer de kwestie wordt verworpen ](assets/automatic-issue-approval-2.png)


## Aanbevolen zelfstudies over dit onderwerp

* [Taken, problemen en goedkeuringen delegeren](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [Groepsspecifieke goedkeuringsprocedures begrijpen](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [Een aanvraagstroom maken](/help/manage-work/request-queues/create-a-request-flow.md)

