---
layout: default
title: Arrangement
parent: API Docs
permalink: /api-docs/arrangement
---
# Introduktion til Arrangementer
Et arrangement kendertegner en begivenhed, som kan holdes i en boligafdeling. Datamodellen består af oplysninger som  titlen på begivenheden, antal deltagere, pris og mv. Der er desuden også et URL til dokument-opslaget, som kan hentes i form af PDF. Den udtømmende datamodel kan læses på [OpenAPI specifikationen](https://tst-beboertavlen.azurewebsites.net/swagger/index.html).

Det er muligt at hente oplysninger om, tilføje, opdatere eller slette et arrangement.

## Hent i en afdeling alle arrangementer
Et GET kald på `https://tst-beboertavlen.azurewebsites.net/api/v1/Apartment/department/2`, hvor nummer `2` indikere afdelingsid'et, hvilket i dette tilfælde er 'Ahorn Allé 2 3.mf, 4100 Ringsted' , vil resultere i responsen

``` 
{
      "id": "ce3d8677-6713-418f-8751-bb01d16e8b19",
      "title": "DAB Bestyrelsen",
      "totalAllowedAttendees": 1,
      "documentViewCount": 0,
      "attendees": null,
      "startTime": "2022-05-25T14:26:24",
      "endTime": "2022-05-26T14:26:25",
      "price": 23,
      "statusId": 1007,
      "status": "Sendt",
      "statusStyle": null,
      "departmentId": 2,
      "documentUrl": null,
      "department": "Søndre Parkvej",
      "createBy": "Samoon Ghazi",
      "createdByRole": null,
      "publishDate": "2022-05-24T14:26:33",
      "createDate": "2022-05-22T14:26:12.0133333",
      "listOfArrangementGroup": []
    },
    {
      "id": "8dee45ad-3694-47e4-a980-ac8a734c6d22",
      "title": "DAB Bestyrelsen",
      "totalAllowedAttendees": 1,
      "documentViewCount": 0,
      "attendees": null,
      "startTime": "2022-05-20T08:00:50",
      "endTime": "2022-05-20T09:00:52",
      "price": 250,
      "statusId": 1007,
      "status": "Sendt",
      "statusStyle": null,
      "departmentId": 2,
      "documentUrl": null,
      "department": "Søndre Parkvej",
      "createBy": "Samoon Ghazi",
      "createdByRole": null,
      "publishDate": "2022-05-25T14:22:54",
      "createDate": "2022-05-22T14:22:42.8566667",
      "listOfArrangementGroup": []
    },
    ..
``` 