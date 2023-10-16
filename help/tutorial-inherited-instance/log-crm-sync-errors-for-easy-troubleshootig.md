---
title: Logga CRM-synkroniseringsfel för enkel felsökning
description: Lär dig hur du använder en logg med CRM Sync-fel för att undersöka CRM-synkroniseringsproblem och få det att fungera smidigt.
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-13875
thumbnail: KT-13875.jpeg
hide: false
source-git-commit: 4dc6aeed353fdd8bac960603af22b060ae2d7f00
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---


# Logga CRM-synkroniseringsfel för enkel felsökning

Som Marketo Engage-administratör bör kontrollen av om instansen är synkroniserad med CRM vara en viktig del av din [daglig rutin](https://nation.marketo.com/t5/champion-program-blogs/my-marketo-morning-routine-tips-for-driving-marketing-operation/ba-p/247508){target="_blank"}. While the [Notifications section](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/notification-types.html){target="_blank"} (finns i det övre högra hörnet av ditt Marketo Engage-gränssnitt) där du börjar hitta och undersöka vanliga synkroniseringsproblem, det finns ett proffstips som kan hjälpa dig att hantera instansens hälsa på ett organiserat sätt.  Adobe Marketo Champion(2022), Amy Goldfine, rekommenderar administratörsanvändare att föra en logg över CRM Sync-fel för att underlätta felsökning.

![Skärmbild på fliken Synkroniseringsfel](/help/tutorial-inherited-instance/_assets/Marketo_Engage_Admin_Salesforce_Sync_Errors_Tab.png)

## Varför registrera CRM-synkroniseringsfel?

Genom att logga CRM-synkroniseringsfelen kan Marketo Engage-administratörer granska problem och trender med CRM-administratörerna för att åtgärda grundorsaken. Följ stegen nedan för att dokumentera dina CRM-synkroniseringsproblem för din instans.

## Spara en logg över CRM-synkroniseringsfel

Innan du börjar ladda ned [Loggmall för synkroniseringsfel i CRM](/help/tutorial-inherited-instance/_assets/downloads/Adobe-Marketo-Engage_CRM-Sync-Error-Log-Template.xlsx).

**Steg 1:** Gå till *[!UICONTROL Admin]section* i Marketo Engage. Under *[!UICONTROL Integration]*, klicka *[!DNL Salesforce]*, *[!DNL Microsoft Dynamics]*, eller *[!DNL Veeva]*, beroende på vilket [!DNL CRM] du använder *[!UICONTROL Sync Errors]* -fliken.

**Steg 2:** Du kan [exportera poster med fel som [!DNL CSV] genom [!UICONTROL Filter] panel](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.html#filter-sync-errors){target="_blank"}. Om du bara har några timmar på dig kan du kopiera och klistra in direkt från *[!UICONTROL Sync Errors]* tabben är vägen dit.

**Steg 3:** Observera datumet då felet inträffade.

**Steg 4:** Ange antalet personposter som påverkas av felet. (Ibland genererar CRM endast ett fel för en person. Ibland finns det många som har samma fel på en gång.)

**Steg 5:** Observera e-postadressen till en person som påverkas av felet. Detta gör det enkelt för dig att referera till och diskutera felen med CRM-administratören.

**Steg 6:** Klistra in länkar till personposten i [!DNL Marketo Engage] och [!UICONTROL CRM Lead/Contact] uppgifter om den personen.

**Steg 7:** Klistra in den faktiska texten för felet i den sista kolumnen.

## Vad händer nu?

**Identifiera felkoder:** Om du vill veta mer om felkoderna kan du slå upp beskrivningarna i utvecklardokumentationen [Svarsnivåtabellen för felkoder](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes){target="_blank"} och hitta de vanliga stegen för att åtgärda felen.

## Författare

**Amy Goldfine**\
Adobe Marketo Champion(2022)
*Senior Manager, Marketing Operations, Iterable*

![Amy Goldfine](/help/tutorial-inherited-instance/_assets/authors/Customer_Author_Amy_Goldfine.png){width="25%"}

**Amy Chiu**
*Adobe &amp; Retention Marketing Manager på Adobe*

![Amy Chiu](/help/tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width="25%"}

