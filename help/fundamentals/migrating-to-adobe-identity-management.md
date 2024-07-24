---
title: Migrering till Adobe Identity Management
description: Beskrivning kommer snart.
role: User
level: Beginner
hide: true
hidefromtoc: true
feature: Marketing
exl-id: 8368a148-c0c8-462f-b166-9efc412c4a0f
source-git-commit: f6ae52b43770789c24237f0bc664d33541469a50
workflow-type: tm+mt
source-wordcount: '1089'
ht-degree: 0%

---

# Migrering till Adobe Identity Management

Adobe förbättrar hur du hanterar Adobe Marketo Engage prenumerationer och användare. Vi ökar produktiviteten för dig och din organisation genom att migrera dina Marketo Engage-prenumerationer och användare till Adobe Admin Console.

Med den här självstudiekursen kan du navigera i migreringen så att du kan hantera Adobe Marketo Engage tillsammans med andra Adobe-konton och produkter för dina användare på en central plats. Migreringen är nödvändig och påverkar inte ditt marknadsföringsarbetsflöde, innehåll, integreringar eller resurser.

## Checklista före migrering för Marketo Engage-administratörer {#pre-migration-checklist-for-marketo-engage-administrators}

För att din organisation ska kunna migrera Adobe Marketo Engage till Adobe Admin Console rekommenderar vi att du följer checklistan nedan för att hantera kommande ändringar.

### 1. Identifiera systemadministratörerna och diskutera vilka åtgärder de kan behöva vidta {#identify-your-system-administrators}

* Om du är osäker på vilka systemadministratörer som finns i din organisation kontaktar du ditt Adobe-kontoteam eller kontaktar Adobe Support `marketocares@marketo.com`.

* Bekräfta den Adobe Admin Console (eller Adobe Org) till vilken dina Marketo Engage-prenumerationer ska migreras.  Marketo Engage prenumerationer måste användas i samma organisation som Dynamic Chat, ett verktyg för automatisering av konversationer som är integrerat med Marketo Engage.
  `TBD LINK TO https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console#subscription-migration-complete`

* Läs mer om hur du kommunicerar med systemadministratörer i avsnittet [Exempel på e-post](#announce-the-migration-timeline).

### 2. Bekanta dig med förändringarna och effekterna av migreringen till Adobe Identity {#familiarize-yourself-with-the-changes}

I videon nedan visar produktledningsteamet på Marketo Engage hur du går igenom migreringsresan och vad du kan förvänta dig.

>[!VIDEO](https://video.tv.adobe.com/v/3430920t3/?quality=12&learn=on){trancript=true}

Mer hjälp om det här avsnittet för Marketo Engage-administratörer finns i följande hjälpartiklar:

* [Checklista för användarinställningar](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/user-setup){target="_blank"}

* [Adobe Identity Management - översikt](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}

* [Om Marketo-prenumeration och användarmigrering till Adobe Admin Console](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console){target="_blank"}

* [Migrerar till Adobe-identitet med migreringskonsolen](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity){target="_blank"}

* [Förstå hur du använder Adobe Admin Console](https://helpx.adobe.com/se/enterprise/using/admin-console.html){target="_blank"}

### 3. Tidslinjen för migrering och förberedelser som behövs för era interna team {#announce-the-migration-timeline}

* Markera migreringsdatumet på Marketo Engage-administratörernas och användarnas kalendrar när de har schemalagts.

Du kan ändra migreringsdatumet i **Admin** > **Migreringskonsol** > **Före migrering** för att bättre anpassa dig till den interna tidslinjen. Läs mer om omplanering och begränsningarna med [att ändra migreringsdatumet](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity#pre-migration){target="_blank"}.

* Skicka ett e-postmeddelande för att kommunicera med systemadministratörerna.

Nedan visas ett exempelmeddelande som du kan skicka till systemadministratörerna. Vanligtvis hanterar IT-avdelningen alla licenser för Adobe.

`---------------------------------------------------`

**Ämne: Support krävs - migrering av Marketo Engage-prenumerationer till Adobe Admin Console**

Hej `[IT Administrator/NAME]`!

Vår Marketo Engage-prenumeration migreras snart till Adobe Identity Management System. [Marknadsföringsgruppen] behöver din hjälp för att slutföra några nödvändiga steg innan användarmigreringen börjar, för att minimera påverkan för Marketo Engage-användare

`1.` Bekräfta om organisationen redan hanterar andra Adobe-produkter i Adobe Admin Console(er) och om Marketo Engage ska migreras till samma konsol.

* Observera att Marketo Engage prenumerationer måste befinna sig i samma organisation som Dynamic Chat, ett verktyg för automatisering av konversationer som är integrerat med Marketo Engage.

* Om du har frågor eller funderingar kring Admin Console som Marketo Engage ska läggas till i kontaktar du supportteamet på `marketocares@marketo.com` och inkluderar oss i ditt meddelande.

`2.` Leta efter ett e-postmeddelande från Adobe med ämnesraden&quot;Åtgärd krävs för att hantera användaråtkomst till Adobe Marketo Engage `[Package Tier]`&quot;. Det här e-postmeddelandet skickades efter att licenser för Marketo Engage har etablerats på Admin Console. Det är bara systemadministratörer som får det här e-postmeddelandet. Var vänlig informera oss omedelbart när du får den.

* Adobe kan be dig, som är systemadministratör för Admin Console, att automatiskt migrera användare till vår organisations befintliga konsol. I e-postmeddelandet med ämnesraden&quot;Åtgärd krävs för att hantera användaråtkomst till Adobe Marketo Engage `[Package Tier]`&quot; klickar du på knappen&quot;Kom igång&quot; för att gå till sidan för godkännande.

`3.` **Valfritt:** Konfigurera enkel inloggning (SSO) på Adobe Admin Console.

* För att hjälpa våra användare att logga in med enkel inloggning på deras Adobe-identitet framåt, ber vi dig att hjälpa till med konfigurationen av enkel inloggning på Adobe Admin Console innan användarmigrering sker.
Vi uppskattar ditt samarbete under den här övergången. Meddela mig när du har slutfört dessa steg så att jag kan fortsätta med användarmigreringen med Marketo Engage.
Med vänlig hälsning

`[Your Name]`

`---------------------------------------------------`

* Skicka ett e-postmeddelande till Marketo Engage-användare.

Nedan visas ett exempel på ett e-postmeddelande som du kan använda för att meddela kommande migrering till Marketo Engage-användare som inte har administratörsbehörighet.

`---------------------------------------------------`

**Ämne: Viktig uppdatering - Migrering av Marketo Engage-prenumerationer till Adobe Admin Console**

Bästa Marketo Engage-användare!

Vi har ett viktigt meddelande om vår Marketo Engage-instans och hur du kommer att logga in. Adobe flyttar abonnemang och användare på Marketo Engage till Adobe Admin Console för att göra det möjligt för sina kunder att centralisera all produktadministration på ett och samma ställe. Detta påverkar inte arbetsflöden, innehåll, integreringar eller resurser för marknadsföring.

Nyckelinformation:

* Migreringsdatum: [Ange schemalagt datum - hitta det i Marketo Engage under **Admin** > **Migreringskonsol** > **Före migrering**]

* Tidsinställning: Migreringen börjar vid midnatt lokal tid för vår prenumeration.

* Inverkan: Ingen förlust av produktåtkomst sker under migreringen av användaren. Om du är inloggad när ditt konto migreras kommer du att loggas ut och uppmanas att logga in igen inom några minuter med hjälp av Adobe-identitet efter migreringen.

* Fördelar: Autentisera Marketo Engage och andra Adobe-produkter genom att använda en enda Adobe-identitet, antingen en Adobe ID-identitet eller en enkel inloggning (Adobe Federated ID).

Vad du behöver göra:

`1.` Förbered: Du måste ha e-postverifiering för att kunna migrera till en Adobe-identitet.

i. Du har fått ett e-postmeddelande med en länk (gäller i 3 dagar). Om länken har upphört att gälla kan du skicka bekräftelsemeddelandet igen genom att gå till **Admin** > **Mitt konto** > **Kontoinställningar** och klicka på **Skicka verifiering igen**.
ii. En aktiv användarsession krävs för att e-postverifieringen ska lyckas. Logga först in på din Marketo Engage-prenumeration med din identitetsleverantörs-URL (IdP).

`2.` Inbyggt: När ditt användarkonto har migrerats får du ett e-postmeddelande från Adobe om ändringarna av inloggningsmetoden.

i. Acceptera den nya inbjudan genom att klicka på knappen Acceptera inbjudan och logga in med Adobe-identitet.
ii. Logga in med en befintlig Adobe ID på inloggningssidan för Adobe.

`3.` Kontakta: Om du har några frågor eller behöver hjälp efter att ditt konto har migrerats eller om ditt konto inte har migrerats och du inte längre har åtkomst till Marketo Engage, kan du kontakta Marketo Engage migreringsteamet på [din interna e-postadress/telefon].

Vi uppskattar ditt samarbete under den här övergången. Tack för din förståelse och ditt engagemang för att skydda våra system.

Bästa,

[Ditt namn]

`---------------------------------------------------`
