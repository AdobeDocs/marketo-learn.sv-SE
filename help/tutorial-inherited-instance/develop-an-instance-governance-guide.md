---
title: Utveckla en instansstyrningsguide med dokumentation
description: Lär dig hur du skapar och underhåller dokumentation och ändringsloggar för din Marketo Engage-instans. Detta sparar inte bara tid för teamets kunskapsdelning utan förbättrar även hälsan och effektiviteten i instansen.
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-14103
thumbnail: KT-14103.jpeg
hide: false
source-git-commit: 4dc6aeed353fdd8bac960603af22b060ae2d7f00
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 0%

---


# Utveckla en instansstyrningsguide med dokumentation

När du går in i ett äldre [!DNL Marketo Engage] Det har till exempel ofta en utmaning att sakna aktuell funktionell och teknisk dokumentation. Som administratör är det ett viktigt ansvar att fastställa riktlinjer för att säkerställa korrekt instansstyrning som du inte kan missa. Det är en av de kritiska strategierna för att [öka effektiviteten när du arbetar i en etablerad Marketo Engage-instans](https://nation.marketo.com/t5/champion-program-blogs/3-tips-to-increase-your-efficiency-in-an-inherited-instance/ba-p/247582).

Den här stegvisa självstudiekursen som du kommer ifrån [!DNL Adobe Marketo Champion] (2018), Nick Hajdin, hjälper dig genom den här processen att skapa en översikt över instansinställningarna, dokumentera dina primära operativa program och underhålla en [!DNL changelog] att tillämpa en strikt styrningspolicy.

## Varför utveckla en instansstyrningsguide och dokumentation för din ärvda instans?

Detaljerad dokumentation och en [!DNL changelog] är avgörande för effektiv hantering och kunskapsöverföring inom [!DNL Marketo Engage] -instans. Genom att hålla reda på ändringar och beslut som du har fattat under instanskonfigurationen kan du:

1. Utbilda interna användare enklare på ett skalbart sätt.
2. Bygg effektivare i [!DNL Marketo Engage] på lång sikt.
3. Bibehåll hälsan och hygienen i din instans och gå vidare för att slippa lägga timmar på att gräva i e-post, [granskningsspår](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/audit-trail/audit-trail-overview.html)och [aktivitetslogg](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.html) för att få kontext.
4. Spara tid vid överföring [!DNL Marketo Engage] kunskap till en ny [!DNL Marketo Engage] om teamet har någon omsättning.

## [!DNL Marketo Engage] styrningsguide 101

En styrningsguide fungerar som en källa till sanning för instansens konfiguration och systemdesignkraven. Nyckelinformation som rekommenderas i det här dokumentet är:

* Program-/mappstrukturer
* Behörighet för användare och roll
* Kommunikationsbegränsningar
* Styrningsstandarder
* Intern användarutbildning innan de får åtkomst till plattformen

## Utveckla och underhålla en styrningsguide för [!DNL Marketo Engage] instance

### Steg 1: Identifiera din aktuella styrningsguide och dokumentation

* **Jag kan inte hitta någon dokumentation för min ärvda instans:** Om du nyligen har påbörjat en ny roll och inte kan hitta någon dokumentation för den ärvda instansen kan du **gå till steg 2** och komma igång med en nedladdningsbar mall som vi har tillhandahållit.
* **Jag har dokumentation till hands:** Grattis, det här är ett gott tecken! Se till att de är relevanta för att se när den senaste ändringen görs. Om det inte underhålls aktivt av dina teammedlemmar rekommenderar vi att du uppdaterar dem och informerar dina interna användare om hur de håller det uppdaterat.

### Steg 2: Identifiera elementen som ska inkluderas i [!DNL Marketo Engage] Dokumentation och [!DNL Changelogs]

Formatet varierar från en molnbaserad plattform till ett delat dokument. Du kan utforma det format som passar din organisations behov. [Här är en enkel dokumentations- och Exchange-Excel-mall](/help/tutorial-inherited-instance/_assets/downloads/Adobe_Marketo_Engage_Inherited_Instance_Documentation-Changlog.xlsx) som täcker de viktiga element som du kan komma igång med. Bland dessa finns:

* Dokumentation
   * Programmallsnamn
   * Kanal
   * Skapad den
   * Skapad av
   * Programmets syfte
   * Status
   * Länk till programmall
   * OBS
* Changelog
   * Programmallsnamn
   * Ändringsdatum
   * Uppdaterat av
   * Uppdateringssyfte
   * Upplevelse före ändring (inkludera länkar/skärmbilder)
   * Upplevelse efter ändring (inkludera länkar/skärmbilder)
   * URL till program

### Steg 3: Identifiera och dokumentera det aktuella läget för de primära operativa programmen

Börja med att identifiera de viktigaste operativa programmen med påverkan på prenumerationsnivå. Exempel är datahanteringskampanjer, leadlivscykel, poängsättning för leads, [!DNL CRM] Synka och leverera.

För varje identifierat operativt program dokumentera dess nuvarande status. Detta innehåller information om programmets syfte, konfiguration, associerade smarta kampanjer och integrering med andra verktyg (om tillämpligt).

### Steg 4: Tvinga [!DNL Changelog] Underhåll

Nästa steg är att etablera en strikt styrningspolicy för [!DNL Marketo Engage] instans som anger &quot;[!DNL Changelog] underhåll.&quot; Denna policy säkerställer att alla uppdateringar som görs av de operativa programmen i hela instansen dokumenteras noggrant.

Undervisa teamet om vikten av dessa dokument och hur man får tillgång till och uppdaterar dem på rätt sätt. Det kan vara praktiskt att tilldela ansvarsområden för att underhålla ändringsloggen, så att ett fåtal utsedda medlemmar i Marketing Operation-teamet eller administratörer konsekvent registrerar ändringar och tillhandahåller signaturer.

### Steg 5: Centralisera dokumentation

Upprätta en central plats eller lagringsplats för lagring av all dokumentation som är relaterad till din [!DNL Marketo Engage] -instans. Det kan vara en delad enhet, en dedikerad mapp eller ett molnbaserat system.

### Steg 6: Regelbunden granskning och uppdatering

Schemalägg regelbundna granskningar av din dokumentation för att säkerställa att den är korrekt och aktuell. Den kan lätt förbises under upptagna tider. Ställ in påminnelser i din kalender proaktivt för att säkerställa att ditt team regelbundet uppdaterar för att återspegla ändringar eller optimeringar i de operativa programmen.

## Vad händer nu?

Kom igång genom att ladda ned den här [enkel mall](/help/tutorial-inherited-instance/_assets/downloads/Adobe_Marketo_Engage_Inherited_Instance_Documentation-Changlog.xlsx).

Följ stegen ovan för att utveckla din styrningsguide och dokumentation. När du arbetar med processen bör du tänka på följande regler:

**Uppdatera befintlig dokumentation:**
Det är viktigt att hålla dokumentationen uppdaterad. Om det inte har ändrats de senaste 3 åren sparar du tid på att granska din dokumentation medan du granskar instansen.

**Dela och utbilda:**
Dela din dokumentation och [!DNL changelog] tillsammans med relevanta teammedlemmar och informera dem om hur de uppdaterar dessa register.

**Periodisk granskning:** planera in tiden för att granska och underhålla dem under året så att de omfattar nya ändringar, optimeringar eller justeringar när de inträffar.

Genom att hålla omfattande och aktuell dokumentation för Marketo Engage sparar du tid och arbete på lång sikt och underlättar effektiv instanshantering.

### Författare

**Nick Hajdin**
[!DNL Adobe Marketo Champion] 2018
*[!DNL Digital Technology Senior Manager at Accenture]*

![Nick Hajdin](/help/tutorial-inherited-instance/_assets/authors/Customer_Author_Nicholas_Hajdin.png){width="30%"}

**Amy Chiu**
*Adobe &amp; Retention Marketing Manager, Adobe*

![Amy Chiu](/help/tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width=30%}
