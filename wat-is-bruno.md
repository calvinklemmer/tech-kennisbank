Bruno is een open-source API-client waarmee ontwikkelaars en beheerders HTTP-API's kunnen testen, debuggen en documenteren.

Bruno is een alternatief voor tools zoals Postman en Insomnia. Het onderscheidt zich doordat API-collecties lokaal worden opgeslagen als tekstbestanden die eenvoudig met Git kunnen worden beheerd.

Belangrijkste functies:

- API Testing: HTTP-verzoeken uitvoeren met GET, POST, PUT, PATCH en DELETE.
- REST API: REST-endpoints testen en responses bekijken.
- Authentication: Ondersteuning voor onder andere Basic Auth, Bearer Tokens en OAuth 2.0.
- Collections: API-verzoeken organiseren in verzamelingen.
- Environment Variables: Variabelen gebruiken voor verschillende omgevingen.
- Scripting & Tests: Automatische controles uitvoeren op API-responses.
- Git Integration: API-collecties versioneren via Git.

### Belangrijke onderdelen

| Onderdeel   | Functie                                          |
| ----------- | ------------------------------------------------ |
| Collection  | Verzameling API-verzoeken                        |
| Request     | HTTP-verzoek naar een API                        |
| Response    | Antwoord van de API-server                       |
| Environment | Omgevingsspecifieke variabelen                   |
| `.bru`      | Bestandsformaat voor Bruno-verzoeken             |
| Bruno CLI   | Collecties en tests uitvoeren via de commandline |

### Voorbeeld API-verzoek

Met Bruno kan bijvoorbeeld een REST API worden getest:

```
GET https://api.example.nl/v1/users
```

De API retourneert een HTTP-statuscode en doorgaans een JSON-response.

### Verschil met Postman

| Bruno                          | Postman                                     |
| ------------------------------ | ------------------------------------------- |
| Open-source API-client         | API-platform met desktop- en clouddiensten  |
| Lokale tekstbestanden (`.bru`) | Collecties doorgaans beheerd binnen Postman |
| Git-georiënteerde werkwijze    | Sterke focus op samenwerking via workspaces |
| Werkt zonder cloudaccount      | Biedt uitgebreide cloudintegratie           |

Kort gezegd: Bruno is een API-testtool waarmee HTTP-verzoeken kunnen worden uitgevoerd en gecontroleerd, waarbij API-collecties lokaal en via Git beheerd kunnen worden.
