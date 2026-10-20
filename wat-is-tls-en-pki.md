TLS (Transport Layer Security) en PKI (Public Key Infrastructure) zijn technologieën voor het beveiligen van communicatie en het beheren van digitale identiteiten en certificaten.

TLS zorgt voor versleutelde communicatie, terwijl PKI het vertrouwen in digitale certificaten organiseert.

Belangrijkste functies:

- Encryptie: Beschermen van gegevens tijdens transport.
- Authenticatie: De identiteit van servers en eventueel clients verifiëren.
- Integriteit: Detecteren of gegevens onderweg zijn gewijzigd.
- Certificaatbeheer: Digitale certificaten uitgeven, vernieuwen en intrekken.
- Trust Management: Vertrouwensrelaties beheren via Certificate Authorities (CA's).
- mTLS: Wederzijdse authenticatie tussen client en server.

### Belangrijke onderdelen

| Onderdeel                  | Functie                                                 |
| -------------------------- | ------------------------------------------------------- |
| TLS                        | Protocol voor beveiligde communicatie                   |
| PKI                        | Infrastructuur voor certificaten en vertrouwensrelaties |
| X.509-certificaat          | Koppelt een identiteit aan een publieke sleutel         |
| Certificate Authority (CA) | Ondertekent en verstrekt certificaten                   |
| Private Key                | Geheime cryptografische sleutel                         |
| Public Key                 | Publieke cryptografische sleutel                        |
| Truststore                 | Bevat vertrouwde certificaten of CA's                   |
| Keystore                   | Bevat sleutels en certificaten                          |

### Hoe werkt TLS?

1. Een client maakt verbinding met een server via HTTPS.
2. De server presenteert zijn TLS-certificaat.
3. De client controleert het certificaat en de vertrouwensketen.
4. Client en server komen cryptografisch sessiesleutels overeen.
5. De communicatie verloopt versleuteld en met integriteitsbescherming.

### Verschil tussen TLS en PKI

| TLS                                     | PKI                                                |
| --------------------------------------- | -------------------------------------------------- |
| Beveiligt netwerkcommunicatie           | Beheert certificaten en vertrouwen                 |
| Gebruikt cryptografische sessiesleutels | Gebruikt certificaten en publieke/private sleutels |
| Bijvoorbeeld HTTPS                      | Bijvoorbeeld een interne CA                        |

Kort gezegd: TLS beveiligt de verbinding; PKI zorgt voor het certificaatbeheer en de vertrouwensbasis waarmee systemen elkaars identiteit kunnen controleren.
