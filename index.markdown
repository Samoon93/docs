---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
# Introduktion til BeboerTavlens API
BeboerTavlen er et kommunikationssystem, der 

Datamodellen for BeboerTavlen kan illusteres med figuren \ref{fig:datamodel}.

|![\label{fig:datamodel}](/assets/kompontenter.drawio.png)|
|:--:| 
| *Figur: Datamodel* |

## Krav til brug af API'et
BeboerTavlen kræver at der udstilles en adgangsnøgle til en bruger, der er registreret i BeboerTavlens system. 

Adgangsnøglen følger med i mailen, der er sendt ud som email ved tegnelsen af en abonnementspakke.

API'et kan tilgås via OpenAPI specifikationen med linket `https://test.api.beboertavlen.dk/swagger/index.html` i test miljøet eller `https://api.beboertavlen.dk/swagger/index.html` i produktions miljøet.

## OpenAPI Specifikation
BeboerTavlens API er kompatibel med OpenAPI 3.0 specifikationen. Der er knyttet Swagger, der kan fortolke API forespørgslerne direkte fra linksne specificeret under sektionen \label{sek:krav}, hvor man kan teste API'et på en nem og hurtig måde på browseren.

Når man vil teste en metode i API'et, så trykker man på *Try it out* og angiver adgangsnøglen, og så trykker man på *Send*. Det er så muligt at se responsen på metode kaldet. 

