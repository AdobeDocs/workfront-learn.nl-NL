---
title: Basismodus voor filters begrijpen
description: Leer welke tekstmodus is, welke camel-case is en welke standaardtekstmodus u kunt gebruiken in uw rapportfilters in [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
source-git-commit: 21fb81fcb4b1468059e571a87e201fa48fb64ff7
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Basismodus voor filters begrijpen

>[!IMPORTANT]
>
>Vereisten:
>
>* Rapporteringselementen begrijpen
>* Rapportonderdelen begrijpen
>* Een basisfilter maken


In deze video leert u:

* Welke tekstmodus is ingesteld
* Wat kamelendoosje is
* Een standaardtekstmodus voor &quot;plug-and-play&quot; die u in rapportfilters kunt gebruiken

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12)

In de volgende tekstmodus worden taken uitgesloten waarvoor een gebruiker heeft aangegeven dat deze is uitgevoerd met Mijn onderdeel. U hoeft alleen maar een taakfilter te maken, filterregels toe te voegen en vervolgens over te schakelen naar de tekstmodus en de code hieronder te plakken na elke tekstmodus die u in het filter ziet.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## Extra filters voor de plug-in- en afspeelmodus

### Taak - toon me alle taken die mijn goedkeuring wachten

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

### Taak - Toon me alle taken die ik heb goedgekeurd

Maak een taakrapport met de gewenste filters en ga vervolgens naar het tabblad Filter en klik op Overschakelen naar tekstmodus. Voeg deze code toe aan wat er al is:

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

### Taak - toon me alle taken die minstens één dwars-projectvoorganger hebben

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### Taak - Toon me alle taken die ik aan anderen heb toegewezen

Maak een taakrapport met de gewenste filters en ga vervolgens naar het tabblad Filter en klik op Overschakelen naar tekstmodus. Voeg deze code toe aan wat er al is:

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Dit zal u alle taken tonen waar de het programma geopende gebruiker minstens één van de huidige toegewezen. Als de toegewezen personen door meerdere personen zijn toegewezen, wordt alleen de naam van de eerste persoon die iemand heeft toegewezen, weergegeven als &quot;Gevraagd door&quot; op de bestemmingspagina.

### Taak - toon me alle taken die - in afwachting van Goedkeuring volledig zijn

```
status=CPL:A
status_Mod=in
```


### Uitgeven - Geef me alle voltooide problemen weer - in afwachting van goedkeuring

```
status=CPL:A
status_Mod=in
```


### Project - Toon me alle projecten die volledig zijn - in afwachting van Goedkeuring

```
status=CPL:A
status_Mod=in
```


### Opmerking - Alle opmerkingen weergeven waarin ik ben gelabeld

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


### Rapport Parameter/aangepast veld - Aangepaste velden weergeven die niet zijn gekoppeld aan een aangepast formulier (zeer nuttig bij opschonen)

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
