HashiCorp Vault is een systeem voor het veilig opslaan, beheren en beschikbaar stellen van secrets zoals wachtwoorden, API-tokens, certificaten en encryptiesleutels.

Vault wordt veel gebruikt in DevOps-, cloud- en Kubernetes-omgevingen.

### Belangrijkste functies

- Secrets Management: Gevoelige gegevens centraal en versleuteld opslaan.
- Access Control: Toegang regelen via policies en authenticatiemethoden.
- Dynamic Secrets: Tijdelijke inloggegevens automatisch genereren.
- Secrets Rotation: Wachtwoorden en sleutels periodiek vervangen.
- PKI: Certificaten uitgeven en beheren.
- Audit Logging: Vastleggen wie welke secrets heeft benaderd.

### Belangrijke onderdelen

| Onderdeel             | Functie                                 |
| --------------------- | --------------------------------------- |
| Vault Server          | Beheert secrets en toegangscontrole     |
| Secrets Engine        | Slaat secrets op of genereert ze        |
| Authentication Method | Controleert de identiteit van clients   |
| Policy                | Bepaalt welke secrets toegankelijk zijn |
| Token                 | Geeft een client tijdelijk toegang      |
| KV Store              | Opslag voor sleutel-waardegegevens      |

### In een DevOps-omgeving

Vault kan worden gebruikt om:

- Databasewachtwoorden veilig beschikbaar te stellen.
- API-tokens buiten Git-repositories te houden.
- Applicaties in Kubernetes van secrets te voorzien.
- Tijdelijke databasecredentials te genereren.
- TLS-certificaten automatisch te beheren.

### Verschil met Kubernetes Secrets

| Kubernetes Secrets                       | HashiCorp Vault                              |
| ---------------------------------------- | -------------------------------------------- |
| Ingebouwde Kubernetes-functionaliteit    | Zelfstandig secretsmanagementsysteem         |
| Opslag binnen Kubernetes                 | Centrale opslag voor meerdere omgevingen     |
| Beperkte ingebouwde rotatiemogelijkheden | Uitgebreide rotatie en dynamische secrets    |
| Gericht op Kubernetes-workloads          | Ook geschikt voor VM's, applicaties en CI/CD |

Kubernetes Secrets bevatten doorgaans Base64-gecodeerde gegevens; Base64 is geen versleuteling. Versleuteling van Secrets in etcd vereist een geschikte encryptie-at-rest-configuratie.

Kort gezegd: HashiCorp Vault beheert gevoelige gegevens centraal en veilig, zodat applicaties en beheertools secrets kunnen gebruiken zonder deze in broncode of configuratiebestanden op te slaan.
