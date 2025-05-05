---
title: Marketo How to API Video - How to set the Access token in a variable
description: Lär dig hur du konfigurerar Postman-programmet och hur du använder variabler för att spara data i variabeln i återanvändbarhetssyfte.
feature: REST API
role: Admin, Developer
level: Experienced
doc-type: Technical Video
duration: 772
last-substantial-update: 2024-08-06T00:00:00Z
jira: KT-15548
exl-id: 4da86ed6-1072-4e0e-a648-16587badaeb3
source-git-commit: 3243c3047efa1bcb92581a58aafe17689ff945fd
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%

---

# API-hjälp - Ange åtkomsttoken i en variabel

Lär dig hur du konfigurerar Postman-programmet och använder variabler för att spara data i variabeln i återanvändbarhetssyfte. Du får också lära dig hur du gör ditt första Marketo Engage REST API-anrop för att hämta åtkomsttoken.

>[!PREREQUISITES]
>
>Innan du startar videon skapar du ett användarnamn för endast API med en AOI-roll och skapar en Launchpad-tjänst. Följ stegen i artiklarna nedan:
>
>* [Skapa endast en API-användarroll](https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user-role){target="_blank"}
>
>* [Skapa endast en API-användare](https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user){target="_blank"}
>
>* [Skapa en anpassad tjänst för användning med REST API](https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api){target="_blank"}

**Referenser som används i den här videon:**

* Marketo-autentiseringsslutpunkt: `{{{}base_url{}}}/identity/oauth/token?grant_type=client_credentials&client_id={{{}client_id{}}}&client_secret={{{}client_secret{}}}`

* JS-skript som hämtar access_token från svarstexten (platser under fliken Skript:):

```
var jsonData = pm.response.json();
pm.environment.set("access_token", jsonData.access_token);
```

* [Marketo Engage-dokumentation för utvecklare](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/rest/authentication){target="_blank"}

>[!VIDEO](https://video.tv.adobe.com/v/3453987/?learn=on&captions=swe)
