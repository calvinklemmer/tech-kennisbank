OAuth 2.0 (Open Authorization) is een open standaard voor gedelegeerde autorisatie, waarmee applicaties beperkte toegang kunnen krijgen tot beveiligde resources zonder dat gebruikers hun wachtwoord hoeven te delen.

OAuth 2.0 vormt ook de basis voor OpenID Connect (OIDC).

Belangrijkste functies:

- Gedelegeerde toegang: Applicaties toegang geven tot resources namens een gebruiker.
- Access Tokens: Tijdelijke toegangsbewijzen voor beveiligde API's.
- Scopes: Bepalen welke toegangsrechten een applicatie aanvraagt.
- Token Expiration: Toegang beperken door tokens een geldigheidsduur te geven.
- Refresh Tokens: Indien uitgegeven, nieuwe access tokens verkrijgen zonder dat de gebruiker doorgaans opnieuw hoeft in te loggen of toestemming te geven.
- Authorization Flows: Verschillende manieren om toegang te verkrijgen, bijvoorbeeld Authorization Code met PKCE.

### Belangrijke onderdelen

| Onderdeel            | Functie                                        |
| -------------------- | ---------------------------------------------- |
| Resource Owner       | Eigenaar van de beveiligde resources           |
| Client               | Applicatie die toegang aanvraagt               |
| Authorization Server | Geeft access tokens uit |
| Resource Server      | API die beveiligde resources aanbiedt          |
| Access Token         | Bewijs van verleende toegang                   |
| Scope                | Aanduiding van aangevraagde toegangsrechten    |

### Hoe werkt OAuth 2.0?

1. Een applicatie vraagt toestemming voor toegang tot bepaalde resources.
2. De gebruiker wordt doorgestuurd naar de Authorization Server.
3. Na autorisatie ontvangt de applicatie een authorization code.
4. De applicatie wisselt de code in voor een access token.
5. De applicatie gebruikt het token om de beveiligde API aan te roepen.

Dit beschrijft de gebruikelijke Authorization Code Flow.

### OAuth 2.0 versus OIDC

- OAuth 2.0: Regelt gedelegeerde toegang tot beveiligde resources.
- OIDC: Voegt gestandaardiseerde gebruikersauthenticatie toe.

Bij de Authorization Code Flow wordt doorgaans PKCE gebruikt. Hiermee wordt voorkomen dat een onderschepte authorization code eenvoudig door een andere partij kan worden ingewisseld.

Kort gezegd: OAuth 2.0 regelt welke applicatie toegang krijgt tot welke resources, zonder dat gebruikers hun wachtwoord aan die applicatie hoeven te geven.
