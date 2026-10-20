Postman is een API-platform waarmee ontwikkelaars en beheerders API's kunnen ontwikkelen, testen, documenteren en beheren.

Postman wordt veel gebruikt voor het testen van REST API's en is vergelijkbaar met Bruno en Insomnia.

Belangrijkste functies:

- API Testing: HTTP-verzoeken uitvoeren met GET, POST, PUT, PATCH en DELETE.
- REST API: REST-endpoints testen en responses analyseren.
- Authentication: Ondersteuning voor onder andere Basic Auth, Bearer Tokens en OAuth 2.0.
- Collections: API-verzoeken organiseren in verzamelingen.
- Environment Variables: Variabelen gebruiken voor verschillende omgevingen.
- Automated Testing: Automatische controles uitvoeren op API-responses.
- API Documentation: API-documentatie genereren en delen.
- Collaboration: Samenwerken aan API's via gedeelde workspaces.

### Belangrijke onderdelen

| Onderdeel   | Functie                                                   |
| ----------- | --------------------------------------------------------- |
| Workspace   | Werkomgeving voor API-projecten                           |
| Collection  | Verzameling API-verzoeken                                 |
| Request     | HTTP-verzoek naar een API                                 |
| Response    | Antwoord van de API-server                                |
| Environment | Omgevingsspecifieke variabelen                            |
| Postman CLI | API-tests uitvoeren via de commandline                    |
| Newman      | Commandlinetool voor het uitvoeren van Postman-collecties |

### Voorbeeld API-verzoek

Met Postman kan bijvoorbeeld een REST API worden getest:

```
GET https://api.example.nl/v1/users
```

De API retourneert een HTTP-statuscode en doorgaans een JSON-response.

### Verschil met Bruno

| Postman                                | Bruno                                     |
| -------------------------------------- | ----------------------------------------- |
| Uitgebreid API-platform                | Lichtgewicht API-client                   |
| Gedeelde workspaces en cloudintegratie | Lokale opslag en Git-integratie           |
| Collecties in Postman-formaat          | Collecties in `.bru`-bestanden            |
| Uitgebreide samenwerkingsfuncties      | Gericht op lokaal en Git-gebaseerd werken |

Kort gezegd: Postman is een uitgebreid platform waarmee API's kunnen worden getest, gedocumenteerd en beheerd, inclusief ondersteuning voor authenticatie, automatisering en samenwerking.
