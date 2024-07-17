---
title: Meerdere factureringssnelheden begrijpen
description: Leer hoe u systeemfactureringssnelheden in een project overschrijft.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-multiple-billing-rates.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10048
exl-id: bda562b9-f8da-49c9-bea7-0440fdc4c24c
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# Meerdere factureringssnelheden begrijpen

Binnen [!DNL Workfront], heeft een projectmanager de capaciteit om systeemfactureringstarieven binnen een specifiek project met voeten te treden. Eerder, toen het nieuwe factureringstarief op het project werd toegepast, beïnvloedde het niet alleen toekomstige uren maar reeds het programma geopende uren.

Met de nieuwe mogelijkheid voor meerdere factureringssnelheden van [!DNL Workfront] kan de projectbeheerder bepalen welke periode een factureringsfrequentie moet worden toegepast. Op deze manier kan de projectbeheerder bepalen wanneer een tarief is overeengekomen of gewijzigd.

## De factureringssnelheid wijzigen

1. Ga naar de landingspagina van het project. Selecteer **[!UICONTROL Billing Rates]** in het linkerdeelvenster.

   ![ Een afbeelding van het selecteren [!UICONTROL Billing Rates] in [!DNL Workfront]](assets/project-finances-1.png)

1. Klik op de knop **[!UICONTROL Add Billing Rate]** op het tabblad **[!UICONTROL Billing Rates]** . Selecteer **[!UICONTROL New Billing Rate]** in de vervolgkeuzelijst.

   ![ Een afbeelding van het selecteren [!UICONTROL New Billing Rate] in [!DNL Workfront]](assets/project-finances-2.png)

1. Het dialoogvenster [!UICONTROL New Billing Rate] wordt weergegeven. Selecteer in het vervolgkeuzemenu **[!UICONTROL Job Role]** de taakrol waarop de nieuwe factureringsfrequentie wordt toegepast.

   ![ Een beeld van het selecteren van baanrollen in een nieuwe het facturerings tarief in [!DNL Workfront]](assets/project-finances-3.png)

1. Nadat de taakrol is geselecteerd, worden het veld [!UICONTROL Default Billing Rate] en het veld [!UICONTROL Billing Rate 1] weergegeven. Voer de nieuwe factureringssnelheid in het veld [!UICONTROL Billing Rate 1] in. Als die factureringssnelheid van toepassing is op het hele project (afgelopen, heden en volgende uren die zijn geregistreerd), klikt u op de knop **[!UICONTROL Save]** .

   ![ Een beeld van het bewaren van een nieuw het factureringstarief dat op het volledige project in [!DNL Workfront]](assets/project-finances-5.png) van toepassing is

1. Klik op de knop **[!UICONTROL Add Rate]** als de nieuwe factureringsfrequentie slechts gedurende een bepaalde periode van toepassing is. De velden [!UICONTROL Billing Rate 1 End Date] en [!UICONTROL Billing Rate 2] worden weergegeven. Voer de einddatum in voor [!UICONTROL Billing Rate 1] . U kunt geen Begindatum voor [!UICONTROL Billing Rate 1] invoeren omdat het systeem ervan uitgaat dat het project aan het begin is gestart.

   ![ een beeld van het creëren van een nieuw factureringstarief dat op een bepaalde periode van toepassing is, die bij het begin van het project in [!DNL Workfront]](assets/project-finances-6.png) beginnen

1. Indien dit niet het geval is:

   * Voer de standaardfactureringssnelheid voor [!UICONTROL Billing Rate 1] in.
   * Selecteer de einddatum voor [!UICONTROL Billing Rate 1] ([!UICONTROL Default Billing Rate]).
   * De begindatum voor [!UICONTROL Billing Rate 2] wordt automatisch ingesteld op de dag nadat [!UICONTROL Billing Rate 1] eindigt.
   * Voer de gewenste factureringssnelheid in de sectie [!UICONTROL Billing Rate 2] in.
   * Klik op de knop **[!UICONTROL Add Rate]** als u factuursnelheden wilt toevoegen.
   * Klik op **[!UICONTROL Save]** als u klaar bent.
   * Alle factureringssnelheden worden weergegeven op het tabblad [!UICONTROL Billing Rates] van het project.

   ![ een beeld van het creëren van nieuwe het factureringspercentages die op de verschillende tijdsperioden in [!DNL Workfront]](assets/project-finances-7.png) van toepassing zijn
