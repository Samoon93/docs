---
layout: default
title: Lejlighed
parent: API Docs
permalink: /api-docs/lejlighed
---
# Introduktion til Lejligheder
En afdeling kendertegner en boligafdeling, hvor modellen indeholder oplysninger om adresse, by, boligselskab, tekniske kontaktperson og mv. Den udtømmende datamodel kan læses på [OpenAPI specifikationen](https://tst-beboertavlen.azurewebsites.net/swagger/index.html).

Det er muligt at hente oplysninger om, tilføje, opdatere eller slette en lejlighed i en afdeling. 

## Hent i en afdeling alle lejligheder
Et GET kald på `https://tst-beboertavlen.azurewebsites.net/api/v1/Apartment/department/2`, hvor nummer `2` indikere afdelingsid'et, hvilket i dette tilfælde er 'SønderParkvej, 4100 Ringsted', vil resultere i responsen.

``` 
{      
    {
      "id": 1002,
      "floor": 0,
      "room": null,
      "fullName": "Ahorn Allé 2 3.mf, 4100 Ringsted",
      "status": "web-resident-disabled",
      "userId": "a1e69276-1680-4d73-911a-281bd393832b",
      "email": "Jala.Nezami@beboertavlen.dk",
      "userName": "Jala.Nezami@beboertavlen.dk",
      "ascent": 0,
      "createBy": null,
      "createDate": "0001-01-01T00:00:00",
      "changedDate": "0001-01-01T00:00:00",
      "aparmentSortId": 0,
      "isDisabled": false
    },
    {
      "id": 1002,
      "floor": 0,
      "room": null,
      "fullName": "Ahorn Allé 2 3.mf, 4100 Ringsted",
      "status": "web-resident-disabled",
      "userId": "e542880f-ff22-4de2-8be1-3e27c6bb37ed",
      "email": "Sabawon.Ghazi@Beboertavlen.dk",
      "userName": "Sabawon.Ghazi@Beboertavlen.dk",
      "ascent": 0,
      "createBy": null,
      "createDate": "0001-01-01T00:00:00",
      "changedDate": "0001-01-01T00:00:00",
      "aparmentSortId": 0,
      "isDisabled": false
    },
    ..
}
``` 
<!--
TODO: FEJL!
## Hent oplysninger om en specifik lejlighed i en afdeling
# Et GET kald på `https://tst-beboertavlen.azurewebsites.net/api/v1/Apartment/department/1002`, hvor nummer `1002` indikere afdelingsid'et, hvilket i dette tilfælde er 'Ahorn Allé 2 3.mf, 4100 Ringsted' , vil resultere i responsen
-->
