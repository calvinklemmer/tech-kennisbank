SAML (Security Assertion Markup Language) is een open standaard voor authenticatie en Single Sign-On (SSO) tussen verschillende systemen.

SAML gebruikt XML om authenticatiegegevens veilig uit te wisselen tussen een Identity Provider (IdP) en een Service Provider (SP).

Belangrijkste functies:

- Single Sign-On (SSO): Eén keer inloggen bij meerdere applicaties.
- Identity Federation: Authenticatie tussen verschillende organisaties en systemen.
- XML Assertions: Uitwisselen van ondertekende authenticatie- en identiteitsgegevens.
- Trust Relationships: Vertrouwensrelaties op basis van metadata en certificaten.
- Digitale handtekeningen: Controle van authenticiteit en integriteit van SAML-berichten.

### Belangrijke onderdelen

| Onderdeel               | Functie                                                 |
| ----------------------- | ------------------------------------------------------- |
| Identity Provider (IdP) | Authenticeert de gebruiker                              |
| Service Provider (SP)   | Applicatie die de gebruiker toegang geeft               |
| SAML Assertion          | XML-document met authenticatie- en identiteitsgegevens  |
| SAML Response           | Bericht met de SAML Assertion                           |
| Metadata XML            | Beschrijft endpoints, certificaten en configuratie      |
| X.509-certificaat       | Wordt gebruikt om digitale handtekeningen te verifiëren |

### Hoe werkt SAML?

1\. Gebruiker opent applicatie

De Service Provider (SP)

2\. Redirect naar Identity Provider

Via een SAML AuthnRequest

3\. Gebruiker logt in

Bij de gekozen Identity Provider

4\. SAML Response

De IdP verstuurt een ondertekende assertion naar de SP

5\. Validatie en toegang

De SP valideert de response en start de gebruikerssessie

### Beveiliging en validatie

Een Service Provider moet onder andere controleren:

- Of de handtekening geldig is en afkomstig is van een vertrouwde partij.
- Of de assertion voor de juiste Service Provider bedoeld is.
- Of de geldigheidsperiode klopt.
- Of de response aansluit bij het verwachte authenticatieverzoek, waar van toepassing.

### SAML versus OIDC

| SAML                        | OIDC                                |
| --------------------------- | ----------------------------------- |
| XML-gebaseerd               | JSON/JWT-gebaseerd                  |
| Vooral enterprise-SSO       | Moderne web- en mobiele applicaties |
| SAML Assertions             | ID Tokens                           |
| Veelgebruikt bij federaties | Gebouwd boven op OAuth 2.0          |

Kort gezegd: SAML is een gestandaardiseerd protocol waarmee applicaties op basis van vertrouwde, ondertekende XML-berichten gebruikers kunnen authenticeren via een externe Identity Provider.
