---
title: Basismodus voor filters begrijpen
description: Leer welke tekstmodus is, welke camel is en welke standaardtekstmodus u kunt gebruiken in uw rapportfilters in Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2025-07-30T00:00:00Z
jira: KT-9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
source-git-commit: 721f246178c0a1dc396b9fe8db53a90e26246775
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# Basismodus voor filters begrijpen

>[!PREREQUISITES]
>
>* [ Begrijp rapporteringselementen ](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=nl-NL)
>* [ Begrijp het melden componenten ](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=nl-NL)
>* [ creeer een basisfilter ](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-filters.html?lang=nl-NL)


>[!TIP]
>
>* Om een diepgaander inzicht in tekstwijze te verkrijgen adviseren wij het letten op de geregistreerde webinar gebeurtenis [ vragen de Deskundige - Inleiding aan de Wijze van de Tekst die ](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en) meldt, die één uur in lengte is.
>* Om nog meer over tekstwijze te leren adviseren wij het letten op [ Geavanceerde het melden ](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=nl-NL) leerprogramma&#39;s, die samen vijf en een half uur in lengte zijn.
>* Klik hier voor toegang [[!UICONTROL API Explorer] ](https://developer.adobe.com/workfront/api-explorer/)


In deze video leert u:

* Welke tekstmodus is ingesteld
* Wat kamelendoosje is
* Een standaardtekstmodus voor &quot;plug-and-play&quot; die u in rapportfilters kunt gebruiken

>[!VIDEO](https://video.tv.adobe.com/v/3470328/?quality=12&learn=on&captions=dut)

## De activiteiten van &quot;Understanding basic text mode for filters&quot;


### Taak - Filter taken uit waar ik &quot;Gereed met mijn deel&quot; heb gemarkeerd

In de volgende tekstmodus worden taken uitgesloten waarvoor een gebruiker heeft aangegeven dat deze is uitgevoerd met Mijn onderdeel. U hoeft alleen maar een taakfilter te maken, filterregels toe te voegen en vervolgens over te schakelen naar de tekstmodus en de code hieronder te plakken na elke tekstmodus die u in het filter ziet.


>[!WARNING]
>
> Dit is niet bedoeld voor gebruik in kalenderfilters.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

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

>[!WARNING]
> 
> Dit is niet bedoeld voor gebruik in kalenderfilters.

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


### Opmerking - toon me alle opmerkingen waarin ik ben gelabeld

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
