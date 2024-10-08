---
title: Migrering till Adobe Identity Management
description: Den här självstudiekursen hjälper dig att navigera mellan prenumerationer och användare på Marketo Engage till Adobe Admin Console.
role: Admin
level: Intermediate, Experienced
recommendations: noDisplay, noCatalog
last-substantial-update: 2024-07-26T00:00:00Z
feature: Marketing
exl-id: 8368a148-c0c8-462f-b166-9efc412c4a0f
source-git-commit: 2172f08f9a6171ef3a25cf6250e2f53eab8195fe
workflow-type: tm+mt
source-wordcount: '1170'
ht-degree: 0%

---

# Migrering till Adobe Identity Management

Adobe förbättrar hur du hanterar Adobe Marketo Engage prenumerationer och användare. Vi ökar produktiviteten för er organisation genom att migrera era era Marketo Engage-prenumerationer och användare till Adobe Admin Console.

Den här självstudiekursen hjälper dig att navigera i migreringen så att du kan börja hantera Adobe Marketo Engage tillsammans med andra Adobe-konton och -produkter för dina användare på en central plats. Migreringen är nödvändig och påverkar inte ditt marknadsföringsarbetsflöde, innehåll, integreringar eller resurser.

## Checklista före migrering för Marketo Engage-administratörer {#pre-migration-checklist-for-marketo-engage-administrators}

För att din organisation ska kunna migrera Adobe Marketo Engage till Adobe Admin Console rekommenderar vi att du följer checklistan nedan för att hantera kommande ändringar.

### 1. Identifiera systemadministratörer och IT-team och diskutera åtgärder de kan behöva vidta {#identify-your-system-administrators}

* Om du är osäker på vilka systemadministratörer som finns i din organisation kontaktar du ditt Adobe-kontoteam eller kontaktar Adobe Support `marketocares@marketo.com`.

* Bekräfta den Adobe Admin Console (eller Adobe Org) till vilken dina Marketo Engage-prenumerationer ska migreras. Du har antagligen en Adobe Admin Console för [Dynamic Chat](/help/dynamic-chat/dynamic-chat-overview.md){target="_blank"}, ett verktyg för intern konversationsautomation i Marketo Engage. Prenumerationer på Marketo Engage måste distribueras i samma organisation som Dynamic Chat.

* Arbeta med IT-teamet för att tillåtslista alla Adobe-domäner som visas [ högst upp i den här artikeln](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/configure-protocols-for-marketo){target="_blank"} för att förhindra avbrott i åtkomsten till Marketo Engage efter migreringen till Adobe Identity.

* **Valfritt:** [Implementera enkel inloggning (SSO)](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console#subscription-migration-complete){target="_blank"} före användarmigrering.

* Lär dig hur du kommunicerar med systemadministratörer i avsnittet [Exempel på e-post](#announce-the-migration-timeline).

### 2. Bekanta dig med förändringarna och effekterna av migreringen till Adobe Identity {#familiarize-yourself-with-the-changes}

I videon nedan visar produktledningsteamet på Marketo Engage hur du går igenom migreringsresan och vad du kan förvänta dig.

>[!VIDEO](https://video.tv.adobe.com/v/3430920t3/?t=170/?quality=12&learn=on){transcript=true}

Mer hjälp om det här avsnittet för Marketo Engage-administratörer finns i följande hjälpartiklar:

* [Checklista för användarinställningar](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/user-setup){target="_blank"}

* [Adobe Identity Management - översikt](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}

* [Om Marketo-prenumeration och användarmigrering till Adobe Admin Console](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console){target="_blank"}

* [Migrerar till Adobe-identitet med migreringskonsolen](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity){target="_blank"}

* [Förstå hur du använder Adobe Admin Console](https://helpx.adobe.com/se/enterprise/using/admin-console.html){target="_blank"}

### 3. Tidslinjen för migrering och förberedelser som behövs för era interna team {#announce-the-migration-timeline}

* Markera migreringsdatumet på Marketo Engage-administratörernas och användarnas kalendrar när de har schemalagts.

   * Du kan ändra migreringsdatumet i **Admin** > **Migreringskonsol** > **Före migrering** så att det passar din interna tidslinje bättre. Läs mer om omplanering och begränsningarna med [att ändra migreringsdatumet](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity#pre-migration){target="_blank"}.

* **Skicka ett e-postmeddelande till systemadministratörerna**

Nedan visas ett exempelmeddelande som du kan skicka till systemadministratörerna. Vanligtvis hanterar IT-avdelningen alla licenser för Adobe.

`---------------------------------------------------`

**Ämne: Support krävs - migrering av Marketo Engage-prenumerationer till Adobe Admin Console**

Hej `[IT Administrator/NAME]`!

Vår Marketo Engage-prenumeration migreras snart till Adobe Identity Management System. `[Marketing Operation team]` behöver din hjälp för att slutföra några nödvändiga steg innan användarmigreringen börjar, för att minimera påverkan för Marketo Engage-användare.

`1.` Bekräfta om organisationen redan hanterar andra Adobe-produkter i Adobe Admin Console(er) och om Marketo Engage ska migreras till samma konsol.

* Marketo Engage prenumerationer måste finnas i samma organisation som Dynamic Chat, ett verktyg för automatisering av konversationer som är integrerat med Marketo Engage.

* Om du har frågor eller funderingar kring Admin Console kontaktar du Adobe Support på `marketocares@marketo.com` och CC oss.

`2.` Leta efter ett e-postmeddelande från Adobe med ämnesraden&quot;Åtgärd krävs för att hantera användaråtkomst till Adobe Marketo Engage `[Package Tier]`&quot;. Det här e-postmeddelandet skickades efter att licenser för Marketo Engage har etablerats på Admin Console. Det är bara systemadministratörer som får det här e-postmeddelandet. Var vänlig informera oss omedelbart när du får den.

* Adobe kan be dig, systemadministratören för Admin Console, att automatiskt migrera användare till vår organisations befintliga konsol. I e-postmeddelandet med ämnesraden&quot;Åtgärd krävs för att hantera användaråtkomst till Adobe Marketo Engage `[Package Tier]`&quot; klickar du på knappen&quot;Kom igång&quot; för att gå till sidan för godkännande.

`3.` Efter migreringen kommer Marketo Engage att gå från experience.adobe.com till Adobe Experience Cloud. Tillåtslista alla Adobe-domäner som visas [högst upp i den här artikeln](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/configure-protocols-for-marketo){target="_blank"} för att förhindra avbrott i åtkomsten till Marketo Engage.

`4.` **Valfritt:** Konfigurera enkel inloggning (SSO) på Adobe Admin Console.

* För att hjälpa våra användare som loggar in med enkel inloggning (SSO) på sin Adobe-identitet att gå framåt bör du hjälpa till med konfigurationen av enkel inloggning på Adobe Admin Console innan användarmigrering sker.

Vi uppskattar ditt samarbete under den här övergången. Meddela mig när du har slutfört de här stegen så att jag kan fortsätta med migreringen.

Med vänlig hälsning

`[Your Name]`

`---------------------------------------------------`

* **Skicka ett e-postmeddelande till Marketo Engage-användare**

Nedan visas ett exempel på ett e-postmeddelande som du kan använda för att meddela kommande migrering till Marketo Engage-användare som inte har administratörsbehörighet.

`---------------------------------------------------`

**Ämne: Viktig uppdatering - Migrering av Marketo Engage-prenumerationer till Adobe Admin Console**

Bästa Marketo Engage-användare!

Vi har ett viktigt meddelande om vår Marketo Engage-instans och hur du kommer att logga in. Adobe flyttar abonnemang och användare på Marketo Engage till Adobe Admin Console för att vi ska kunna centralisera all produktadministration på ett och samma ställe. Detta påverkar inte arbetsflöden, innehåll, integreringar eller resurser för marknadsföring.

**Nyckelinformation:**

* **Migreringsdatum**: `[Specify the scheduled date - please find this in Marketo Engage under Admin > Migration Console > Pre-migration]`

* **Timing**: Migreringen börjar vid midnatt lokal tid för vår prenumeration.

* **Effekt**: Ingen förlust av produktåtkomst uppstår under användarmigrering. Om du är inloggad när ditt konto migreras kommer du att loggas ut och uppmanas att logga in igen inom några minuter med hjälp av Adobe-identitet efter migreringen.

* **Fördelar**: Autentisera Marketo Engage och andra Adobe-produkter genom att använda en enda Adobe-identitet, antingen en Adobe ID-identitet eller ett Adobe-Federated ID (SSO).

**Vad du behöver göra:**

`1.` **Förbered**: Du måste ha e-postverifiering för att kunna migrera till en Adobe-identitet.

i. Du har fått ett e-postmeddelande med en länk (gäller i 3 dagar). Om länken har upphört att gälla kan du skicka bekräftelsemeddelandet igen från Marketo Engage genom att klicka på ikonen &quot;Min profil&quot; och sedan gå till **Mitt konto** > **Kontoinställningar** > **Skicka bekräftelsen igen**.

ii. En aktiv användarsession krävs för att e-postverifieringen ska lyckas. Logga först in på din Marketo Engage-prenumeration med din identitetsleverantörs-URL (IdP).

`2.` **Inbyggt**: När ditt användarkonto har migrerats får du ett e-postmeddelande från Adobe om ändringarna av inloggningsmetoden.

i. Acceptera den nya inbjudan genom att klicka på knappen Acceptera inbjudan och logga in med Adobe-identitet.

ii. Logga in med en befintlig Adobe ID på inloggningssidan för Adobe.

iii. Du måste först logga in på Marketo Engage-instansen för tidigare bokmärkta URL:er på den engage-xx.marketo.com domän du navigerar till.

`3.` **Kontakta**: Om du har frågor eller behöver hjälp efter att ditt konto har migrerats, eller om ditt konto inte har migrerats och du har förlorat åtkomsten till Marketo Engage, kan du kontakta migreringsteamet för Marketo Engage på `[your internal contact email/phone]`.

Vi uppskattar ditt samarbete under den här övergången. Tack för din förståelse och ditt engagemang för att skydda våra system.

Med vänlig hälsning

`[Your Name]`

`---------------------------------------------------`
