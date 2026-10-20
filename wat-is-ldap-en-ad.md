LDAP (Lightweight Directory Access Protocol) is een protocol waarmee applicaties gebruikers, groepen en andere gegevens in een directory kunnen opzoeken en beheren.

Active Directory (AD) is de directorydienst van Microsoft voor centraal gebruikers-, computer- en toegangsbeheer binnen organisaties.

### Belangrijkste functies

- Gebruikersbeheer: Accounts centraal beheren.
- Groepsbeheer: Gebruikers indelen in groepen.
- Authenticatie: Identiteiten controleren.
- Autorisatie: Toegangsrechten koppelen aan gebruikers en groepen.
- Directory Queries: Gebruikers en groepen opzoeken via LDAP.
- Single Sign-On (SSO): AD kan via Kerberos geïntegreerde aanmelding ondersteunen.

### Verschil tussen LDAP en AD

| LDAP                                                   | Active Directory                          |
| ------------------------------------------------------ | ----------------------------------------- |
| Protocol                                               | Directorydienst van Microsoft             |
| Beschrijft hoe directorygegevens worden benaderd       | Slaat gebruikers, groepen en computers op |
| Wordt door verschillende directorydiensten ondersteund | Ondersteunt onder andere LDAP en Kerberos |
| Geen zelfstandige gebruikersdatabase                   | Centrale gebruikers- en beheerdienst      |

### Voorbeeld van een directorykoppeling

Een applicatie kan via LDAP gebruikers en groepen opzoeken in een centrale directory.

Bijvoorbeeld:

1. Een gebruiker meldt zich aan.
2. De applicatie of authenticatiedienst controleert de identiteit via de directory.
3. Groepsinformatie kan worden gebruikt bij het bepalen van toegangsrechten.

LDAP is hierbij het communicatieprotocol; de directorydienst beheert de gegevens.

### Beveiliging

Gebruik bij voorkeur LDAPS of LDAP met StartTLS, zodat directoryverkeer versleuteld wordt.

Kort gezegd: LDAP is het protocol om directorygegevens te benaderen; Active Directory is een Microsoft-directorydienst die onder andere LDAP gebruikt. Applicaties kunnen via LDAP bestaande organisatieaccounts gebruiken.
