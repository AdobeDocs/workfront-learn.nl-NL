---
title: De standaardtekstmodus voor weergaven begrijpen
description: Leer welke tekstmodus is, welke camel is en welke standaardtekstmodus u kunt gebruiken in uw weergaven in Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 11367
exl-id: 156e5510-4a51-449f-9c8c-e16fdd8ea23d
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# De standaardtekstmodus voor weergaven begrijpen


>[!IMPORTANT]
>
>Vereisten:
>
>* Rapporteringselementen begrijpen
>* Rapportonderdelen begrijpen
>* Een basisweergave maken


>[!TIP]
>
>* Voor een beter begrip van de tekstmodus raden we u aan de opgenomen webinar-gebeurtenis te bekijken [Vraag het de Expert - Inleiding aan de Rapportering van de Wijze van de Tekst](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en), wat een uur lang is.
>* Als u nog meer wilt weten over de tekstmodus, raden we u aan de [Geavanceerde rapportage](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) zelfstudies, die samen 5,5 uur lang zijn.


In deze video leert u:

* Welke tekstmodus is ingesteld
* Wat kamelendoosje is
* De standaardtekstmodus &quot;insteekmodule en afspelen&quot; die u in uw weergaven kunt gebruiken

>[!VIDEO](https://video.tv.adobe.com/v/3410571/?quality=12)

## Taak - 4 ouderenmening

Creeer eerst een kolom voor de Naam van de Taak en de Naam van de Ouder, dan gebruik de volgende tekstwijze om de andere drie kolommen tot stand te brengen.

### Taak - Bovenliggend item van bovenliggende naam

```
displayname=Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:name
textmode=true
valuefield=parent:parent:name
valueformat=HTML
```

### Taak - Bovenliggend item van bovenliggende naam

```
displayname=Parent of Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:parent:name
textmode=true
valuefield=parent:parent:parent:name
valueformat=HTML
```

### Taak - Bovenliggend item van bovenliggende entiteit van bovenliggende naam

```
displayname=Parent of Parent of Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:parent:parent:name
textmode=true
valuefield=parent:parent:parent:parent:name
valueformat=HTML
```

![Een schermafbeelding die de weergave van de vier bovenliggende items weergeeft](assets/4-parents-view.png)

## Gebruiker - Herhalingen die lijsten in gebruikersmeningen tonen

### Gebruiker - Alle taakrollen

```
displayname=All job roles
listdelimiter=<p>
listmethod=nested(userRoles).lists
textmode=true
type=iterate
valuefield=role:name
valueformat=HTML
```

### Gebruiker - Alle taakrollen tonen primair

```
displayname=All Job Roles showing primary
listdelimiter=<p> 
listmethod=nested(userRoles).lists 
textmode=true
type=iterate 
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("** ",{role}.{name}," **"),{role}.{name})
valueformat=HTML
```

### Gebruiker - Alle teams

```
displayname=All teams
listdelimiter=<p>
listmethod=nested(teams).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

>[!NOTE]
>
>Er is een gebied van het Team toegankelijk door UI dat alle teams toont, komma&#39;s gescheiden, maar het gebruiken van de tekstwijze hierboven zal elk team op een afzonderlijke lijn tonen.


### Gebruiker - Alle groepen

```
displayname=All groups
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valuefield=group:name
valueformat=HTML
```

### Gebruiker - Alle groepen die homegroep tonen

```
displayname=All groups showing home group
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valueexpression=IF({user}.{homeGroupID}={group}.{ID},CONCAT("** ",{group}.{name}," **"),{group}.{name})
valueformat=HTML
```


### Gebruiker - Directe rapporten

```
displayname=Direct reports
listdelimiter=<p>
listmethod=nested(directReports).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

### Gebruiker - Toekomstige PTO

```
displayname=Future PTO
listdelimiter=<br>
listmethod=nested(reservedTimes).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=IF({startDate}>$$TODAY,CONCAT({startDate}," - ",{endDate}),"")
valueformat=HTML
width=150
```

![Een schermafbeelding die de weergave Gebruikerslijsten weergeeft](assets/user-lists-view-large.png)

## Taak - hoe te om taaktaken te tonen en aan status te werken

```
displayname=Assignments and Status
listdelimiter=<br>
listmethod=nested(assignments).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT({assignedTo}.{name},IF(ISBLANK({assignedTo}.{name}),"",IF({status}="AA"," - Requested",IF({status}="AD"," - Working"," - Done"))))
valueformat=HTML
width=150
```

![Een schermafbeelding met de toewijzingen en de statusweergave](assets/assignments-and-status-view.png)


## Taak - hoe te om rol en toewijzing op veelvoudige taaktaken te tonen

### Taak - Rol + uren

```
displayname=Role+hours
listdelimiter=<li>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT({role}.{name}," (",round({workRequired}/60,2),")")
valueformat=HTML
```

### Taak - Toewijzing + percentage toewijzing

```
displayname=Assignment+percent
valueexpression=CONCAT({assignedTo}.{name}," (",{assignmentPercent},")")
listdelimiter=<li>
listmethod=nested(assignments).lists
valueformat=HTML
textmode=true
type=iterate
```

![Een schermafbeelding met de weergave Toewijzingen en Rollen](assets/assignments-roles-and-percent-view.png)

## Taak - Voorgangers en opvolgers voor meerdere projecten

### Taakfilter (optioneel)

**Toon me alle taken die minstens één dwars-projectvoorganger hebben**

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### Taak - toon voorgangersnamen en projectvoorganger binnen is

```
displayname=Predecessor names
listdelimiter=<br>
listmethod=nested(predecessors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT("TASK = ",{predecessor}.{name}," >> PROJECT = ",{predecessor}.{project}.{name})
valueformat=HTML
width=150
```

### Taak - toon de namen van de opvolger en projectopvolger binnen

```
displayname=Successor names
listdelimiter=<br>
listmethod=nested(successors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT("TASK = ",{successor}.{name}," >> PROJECT = ",{successor}.{project}.{name})
valueformat=HTML
width=150
```

### Taak - Verwachte voltooiingsdatum van voorgangers weergeven

```
displayname=Predecessor projected completion dates
valueformat=atDate
listdelimiter=
textmode=true
width=90
stretch=0
valuefield=predecessor:projectedCompletionDate
type=iterate
listmethod=nested(predecessors).lists
shortview=false
```

### Taak - de vooruitgangsstatus van predecessors tonen

```
displayname=Predecessor progress status
listdelimiter=<br>
listmethod=nested(predecessors).lists
shortview=false
stretch=0
textmode=true
type=iterate
valueexpression=IF({predecessor}.{progressStatus}="OT","On Time",IF({predecessor}.{progressStatus}="LT","Late",IF({predecessor}.{progressStatus}="BH","Behind","At Risk")))
valueformat=HTML
width=90
```

### Taak - toon percent volledig van het cross-project voorganger- project

```
displayname=Predecessor project percent complete
listdelimiter=<br>
listmethod=nested(predecessors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=IF({isCP}=true,CONCAT({predecessor}.{project}.{percentComplete},"%"),"")
valueformat=HTML
width=150
```

![Een schermafbeelding die de voordecessors en de opvolgers van het Cross-project weergeeft](assets/cross-project-predecessors-and-successors.png)


## Taak - Herhaling die alle toegewezen personen toont en wie elk toewees

```
displayname=All assignees and requesters
listdelimiter=<p>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT("Assigned To: ",{assignedTo}.{name},"; Requested By: ",{assignedBy}.{name})
valueformat=HTML
```

![Een schermafbeelding waarin alle toegewezen personen worden weergegeven en aan wie elke persoon is toegewezen](assets/all-assignees-and-requesters.png)

## Taak/project - Herhaling die alle douaneformulieren op een project of een taak toont

```
displayname=All Forms Assigned
listdelimiter=<p>
listmethod=nested(objectCategories).lists
textmode=true
type=iterate
valuefield=category:name
valueformat=HTML
```

![Een schermafbeelding met alle aangepaste formulieren op een project](assets/all-custom-forms-on-a-project.png)


## Project - Herhaling die alle primaire contacten voor oplosbare middelen in projectweergave toont

```
displayname=Requestor
listdelimiter=<br>
listmethod=nested(resolvables).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=owner:name
valueformat=HTML
width=150
```

![Een het schermbeeld dat primaire contacten voor oplosbare voorwerpen toont](assets/primary-contacts-for-resolvables.png)

## Project - Herhaling die alle leden van het projectteam toont

```
displayname=Project Team Members
listdelimiter=<br>
listmethod=nested(projectUsers).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
```

![Een het schermbeeld dat alle leden van het projectteam toont](assets/all-project-team-members.png)

## Project - herhaling met vermelding van de entryDate voor alle oplosbare problemen voor een project

```
displayname=Resolvables entry date
linkedname=direct
listdelimiter=<br>
listmethod=nested(project.resolvables).lists
listsort=string(description)
querysort=description
section=0
textmode=true
type=iterate
valuefield=entryDate
valueformat=HTML
```

![Een schermafbeelding met de entryDate van alle oplosbare problemen voor een project](assets/resolvables-entry-date.png)

## Project - Toon de huisgroep van de oorspronkelijke projectaanvrager

```
displayname=Requestor home group
linkedname=direct
namekey=name
querysort=convertedOpTaskOriginator:homeGroup:name
textmode=true
valuefield=convertedOpTaskOriginator:homeGroup:name
valueformat=HTML
```

![Een het schermbeeld die de groep van het projectaanvrager van het huis toont](assets/requestor-home-group.png)

## Project - toon als het project een verzoekrij is

```
querysort=queueDef:isPublic
valueformat=val
description=0 (None), 1 (Public), 2 (Private), 3 (Company), 4 (Group)
linkedname=direct
textmode=true
enumtype=PROJ
valuefield=queueDef:isPublic
namekey=status
type=enum
enumclass=com.attask.common.constants.ProjectStatusEnum
displayname=Public Selection
```

![Een het schermbeeld dat toont als het project een verzoekrij is](assets/project-is-a-request-queue.png)

## Probleem - herhaling met alle leden van het projectteam voor het oplossen van problemen

```
displayname=Resolve Project: Team Members
listdelimiter=<br>
listmethod=nested(resolveProject.projectUsers).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
width=150
```

![Een het schermbeeld dat alle leden van het oplossingsprojectteam toont](assets/all-resolve-project-team-members.png)

## Probleem - herhaling met alle teams van de primaire contactpersoon van de uitgave

```
displayname=Requestor Teams
listdelimiter=<br>
listmethod=nested(owner.teams).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=name
valueformat=HTML
width=150
```

![Een schermafbeelding met alle primaire contactteams](assets/all-primary-contact-teams.png)

## Document - herhaling van map in een documentrapport

```
displayname=Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=name
valueformat=HTML
```

![Een schermafbeelding met de map in een documentrapport](assets/folder-in-a-document-report.png)

## Document - herhaling met bovenliggende map in een documentrapport

```
displayname=Parent Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=parent:name
valueformat=HTML
```

![Een schermafbeelding met bovenliggende map in een documentrapport](assets/parent-folder-in-a-document-report.png)

## Document - Datum goedkeuring document

```
displayname=Document Approval Dates
valueformat=HTML
listdelimiter=<br>
linkedname=direct
textmode=true
listsort=string(description)
valuefield=approvalDate
type=iterate
listmethod=nested(approvals).lists
shortview=false
section=0
```

![Een schermafbeelding met de weergave Datum documentgoedkeuring](assets/document-approval-dates.png)

## Goedkeuringen proefdrukken

### Goedkeuring proef - Naam van project tonen

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

### Goedkeuring proefdrukken - Taaknaam tonen

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

![Een schermafbeelding met het project en de taak van een proefdrukgoedkeuring](assets/proof-approval-project-and-task.png)
