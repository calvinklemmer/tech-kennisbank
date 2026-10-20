OpenID Connect (OIDC) is een open standaard voor authenticatie, gebouwd boven op OAuth 2.0.

OIDC maakt het mogelijk dat gebruikers veilig inloggen bij applicaties via een centrale Identity Provider (IdP), zoals Microsoft Entra ID of Google.

Belangrijkste functies:

- Authenticatie: Vaststellen wie een gebruiker is.
- Single Sign-On (SSO): Eén keer inloggen bij meerdere applicaties.
- Identity Federation: Authenticatie via externe Identity Providers.
- ID Token: Een JWT met informatie over de authenticatie en identiteit van de gebruiker; ID-tokens kunnen ondertekend en eventueel versleuteld zijn.
- Access Token: Token waarmee een applicatie toegang kan krijgen tot beveiligde API's.
- Standardisatie: Gestandaardiseerde communicatie tussen applicaties en Identity Providers.

### Belangrijke onderdelen

| Onderdeel               | Functie                                                     |
| ----------------------- | ----------------------------------------------------------- |
| Identity Provider (IdP) | Authenticeert de gebruiker           |
| Client / Relying Party  | Applicatie die OIDC gebruikt                                |
| ID Token                | Bevat identiteits- en authenticatieclaims                   |
| Access Token            | Geeft toegang tot beveiligde resources                      |
| Refresh Token           | Kan worden gebruikt om nieuwe tokens aan te vragen          |
| Authorization Code Flow | Veelgebruikte veilige authenticatieflow, doorgaans met PKCE |

### Hoe werkt OIDC?

1\. Gebruiker opent applicatie

Bijvoorbeeld een selfserviceportaal

2\. Redirect naar Identity Provider

De Identity Provider verzorgt de authenticatie

3\. Gebruiker logt in

Eventueel met MFA of externe IdP

4\. Authorization Code

Applicatie ontvangt een tijdelijke code

5\. Tokens en toegang

Applicatie wisselt de code in, valideert het ID Token en start de sessie

### ID-token versus access token

- ID-token: Is bedoeld voor de client om informatie over de authenticatie te controleren.
- Access token: Is bedoeld om beveiligde API's of andere resources aan te roepen.

Een API hoort niet uitsluitend op basis van een ID-token toegang te verlenen.

Kort gezegd: OAuth 2.0 regelt gedelegeerde toegang tot resources; OIDC voegt daar gestandaardiseerde gebruikersauthenticatie aan toe.
