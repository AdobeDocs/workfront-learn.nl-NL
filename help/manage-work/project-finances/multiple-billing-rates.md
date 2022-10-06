---
title: Meerdere factureringssnelheden begrijpen
description: Binnen Workfront kan een projectmanager de factureringssnelheden van het systeem binnen een specifiek project overschrijven.
feature: Work Management
thumbnail: understand-multiple-billing-rates.png
type: Tutorial
role: User
level: Intermediate
kt: 10048
exl-id: bda562b9-f8da-49c9-bea7-0440fdc4c24c
source-git-commit: d0c842ad8bf6f52161f003a62237fbcd35d23176
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# Meerdere factureringssnelheden begrijpen

Within [!DNL Workfront], heeft een projectmanager de capaciteit om systeemfactureringstarieven binnen een specifiek project met voeten te treden. Eerder, toen het nieuwe factureringstarief op het project werd toegepast, beïnvloedde het niet alleen toekomstige uren maar reeds het programma geopende uren.

Met [!DNL Workfront]De nieuwe capaciteit van de meervoudige factureringssnelheid van de projectmanager kan bepalen welke periode een factureringstarief moet worden toegepast. Op deze manier kan de projectbeheerder bepalen wanneer een tarief is overeengekomen of gewijzigd.

## De factureringssnelheid wijzigen

1. Ga naar de landingspagina van het project. Selecteren **[!UICONTROL Billing Rates]** in het linkerdeelvenster.

   ![Een afbeelding van het selecteren [!UICONTROL Billing Rates] in [!DNL Workfront]](assets/project-finances-1.png)

1. Van de **[!UICONTROL Billing Rates]** klikt u op de knop **[!UICONTROL Add Billing Rate]** knop. Selecteren **[!UICONTROL New Billing Rate]** in de vervolgkeuzelijst.

   ![Een afbeelding van het selecteren [!UICONTROL New Billing Rate] in [!DNL Workfront]](assets/project-finances-2.png)

1. De [!UICONTROL New Billing Rate] wordt weergegeven. Van de **[!UICONTROL Job Role]** selecteert u in het vervolgkeuzemenu de taakrol waarop de nieuwe factureringsfrequentie wordt toegepast.

   ![Een afbeelding van het selecteren van taakrollen in een nieuwe factureringssnelheid in [!DNL Workfront]](assets/project-finances-3.png)

1. Als de taakrol is geselecteerd, wordt de [!UICONTROL Default Billing Rate] en de [!UICONTROL Billing Rate 1] wordt weergegeven. Voer de nieuwe factureringssnelheid in het dialoogvenster [!UICONTROL Billing Rate 1] veld. Als die factureringssnelheid van toepassing is op het hele project (verleden, heden en volgende uren die zijn geregistreerd), klikt u op de knop **[!UICONTROL Save]** knop.

   ![Een afbeelding van het opslaan van een nieuwe factureringssnelheid die van toepassing is op het gehele project in [!DNL Workfront]](assets/project-finances-5.png)

1. Als het nieuwe factureringstarief slechts voor een bepaalde periode van toepassing is, klik **[!UICONTROL Add Rate]** knop. De [!UICONTROL Billing Rate 1 End Date] en de [!UICONTROL Billing Rate 2] worden weergegeven. Voer de einddatum in voor [!UICONTROL Billing Rate 1]. U kunt geen begindatum invoeren voor [!UICONTROL Billing Rate 1] omdat het systeem ervan uitgaat dat het aan het begin van het project is gestart.

   ![Een afbeelding van het maken van een nieuwe factureringssnelheid die van toepassing is op een bepaalde periode, te beginnen bij het begin van het project in [!DNL Workfront]](assets/project-finances-6.png)

1. Indien dit niet het geval is:

   * Voer de standaardfactureringssnelheid in voor [!UICONTROL Billing Rate 1].
   * Selecteer de einddatum voor [!UICONTROL Billing Rate 1] ([!UICONTROL Default Billing Rate]).
   * De begindatum voor [!UICONTROL Billing Rate 2] wordt automatisch ingesteld op de volgende dag [!UICONTROL Billing Rate 1] eindigt.
   * Voer de gewenste factureringssnelheid in het dialoogvenster [!UICONTROL Billing Rate 2] sectie.
   * Ga door met het toevoegen van factuursnelheden, indien nodig, door op de knop **[!UICONTROL Add Rate]** knop.
   * Klik wanneer gereed **[!UICONTROL Save]**.
   * Alle factureringssnelheden worden weergegeven in het dialoogvenster [!UICONTROL Billing Rates] op het project.
   ![Een afbeelding van het maken van nieuwe factureringssnelheden die van toepassing zijn op de verschillende tijdsperioden in [!DNL Workfront]](assets/project-finances-7.png)
