JWT (JSON Web Token) is een gestandaardiseerd formaat voor het uitwisselen van informatie tussen systemen, bijvoorbeeld over de identiteit en toegangsrechten van een gebruiker.

JWT wordt veel gebruikt bij OAuth 2.0 en OpenID Connect (OIDC).

### Belangrijkste kenmerken

- Claims: Bevat gegevens zoals gebruikers-ID, rollen en geldigheidsduur.
- Ondertekening of versleuteling: Een ondertekende JWT maakt controle van herkomst en integriteit mogelijk; een versleutelde JWT beschermt de inhoud tegen inzage.
- Compact: Geschikt voor HTTP-verzoeken.
- Stateless: Kan worden gevalideerd zonder telkens een database te raadplegen.
- Tijdgebonden: Claims zoals `exp` bepalen wanneer een token verloopt.

### Opbouw van een JWT

Een ondertekende JWT bestaat doorgaans uit drie Base64URL-gecodeerde onderdelen:

```
HEADER.PAYLOAD.SIGNATURE
```

| Onderdeel | Functie                                             |
| --------- | --------------------------------------------------- |
| Header    | Beschrijft het token en het ondertekeningsalgoritme |
| Payload   | Bevat claims over gebruiker en token                |
| Signature | Maakt verificatie van de handtekening mogelijk      |

### JWT en tokens

Een JWT is een tokenformaat, geen authenticatieprotocol.

- ID-token: Bevat informatie over de authenticatie van een gebruiker en is bedoeld voor de OIDC-client.
- Access token: Geeft een client toegang tot beveiligde resources. Een access token hoeft niet in JWT-formaat te zijn.
- Validatie: Controleer bij ondertekende JWT's onder andere de handtekening, uitgever, doelgroep en geldigheidsduur.

Een JWT kan ondertekend (JWS) of versleuteld (JWE) zijn.

### Beveiliging

Een standaard ondertekende JWT is niet versleuteld. De payload kan worden gelezen door iedereen die het token bezit. Sla er daarom geen gevoelige informatie in op.

Kort gezegd: JWT is een compact tokenformaat waarmee systemen informatie over identiteit en toegangsrechten betrouwbaar kunnen uitwisselen.
