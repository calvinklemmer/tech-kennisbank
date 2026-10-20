OpenConext is een open-source Identity Federation-platform waarmee gebruikers via hun eigen organisatie veilig kunnen inloggen bij applicaties en diensten van andere organisaties.

OpenConext wordt onder andere gebruikt als technologie achter federatieve authenticatieomgevingen zoals SURFconext.

Belangrijkste functies:

- Identity Federation: Verbindt Identity Providers (IdP's) met Service Providers (SP's).
- Single Sign-On (SSO): Inloggen bij meerdere diensten via de eigen organisatie.
- WAYF: Gebruikers laten kiezen via welke organisatie ze inloggen.
- SAML: Ondersteunt federatieve authenticatie via SAML 2.0.
- OIDC: Ondersteuning voor OpenID Connect via aanvullende componenten.
- Attribuutuitwisseling: Identiteitsgegevens gecontroleerd doorgeven aan applicaties.

### Belangrijke onderdelen

| Onderdeel               | Functie                                           |
| ----------------------- | ------------------------------------------------- |
| Identity Provider (IdP) | Authenticeert gebruikers                          |
| Service Provider (SP)   | Biedt applicaties en diensten aan                 |
| Service Provider Proxy  | Tussenlaag voor federatieve authenticatie         |
| WAYF / Discovery        | Selectie van de juiste Identity Provider          |
| EngineBlock             | Centrale component voor federatieve authenticatie |

### Voorbeeld van federatieve authenticatie

Een mogelijke authenticatieketen:

`Applicatie → Federatieplatform → WAYF → Identity Provider`

1. De gebruiker opent een aangesloten applicatie.
2. Via WAYF selecteert de gebruiker de eigen organisatie.
3. De Identity Provider van die organisatie authenticeert de gebruiker.
4. Het federatieplatform geeft de benodigde authenticatie- en identiteitsinformatie door aan de applicatie.

Kort gezegd: OpenConext verbindt organisaties en applicaties via federatieve authenticatie, zodat gebruikers met hun bestaande organisatieaccount toegang krijgen tot externe diensten.
