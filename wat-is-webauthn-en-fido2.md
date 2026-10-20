WebAuthn (Web Authentication) en FIDO2 zijn standaarden voor veilige, phishingbestendige authenticatie, zowel zonder wachtwoord als in combinatie met andere authenticatiefactoren.

Ze maken gebruik van public-keycryptografie en worden toegepast bij passkeys, biometrische authenticatie en fysieke beveiligingssleutels.

### Belangrijkste kenmerken

- Passwordless: Ondersteunt aanmelden zonder wachtwoord, maar kan ook als extra authenticatiefactor worden gebruikt.
- Phishing Resistant: Inloggegevens zijn cryptografisch gekoppeld aan de juiste website.
- Public/Private Keys: Authenticatie via een sleutelpaar.
- Biometrie: Ondersteuning voor vingerafdruk- en gezichtsherkenning.
- Security Keys: Ondersteuning voor fysieke beveiligingssleutels, zoals YubiKeys.
- MFA: Kan sterke multifactorauthenticatie bieden.

### Verschil tussen WebAuthn en FIDO2

| Onderdeel    | Functie                                              |
| ------------ | ---------------------------------------------------- |
| FIDO2        | Overkoepelende authenticatiestandaard                |
| WebAuthn     | Browser-API voor authenticatie met publieke sleutels |
| CTAP2        | Protocol tussen apparaat en authenticator            |
| Passkey      | Gebruikersvriendelijke FIDO-authenticatiecredential  |
| Security Key | Fysiek apparaat voor authenticatie                   |

### Hoe werkt het?

1. Bij registratie wordt een cryptografisch sleutelpaar aangemaakt.
2. De publieke sleutel wordt opgeslagen bij de applicatie.
3. De privésleutel blijft onder controle van de authenticator; sommige passkeys kunnen veilig tussen apparaten worden gesynchroniseerd.
4. Bij het aanmelden ondertekent de authenticator een unieke uitdaging (challenge).
5. De applicatie controleert de handtekening met de publieke sleutel.

### Biometrie en privésleutels

Bij WebAuthn blijft de privésleutel bij de authenticator.

Biometrische gegevens, zoals een vingerafdruk of gezichtsscan, worden normaal gesproken lokaal gebruikt om de authenticator te ontgrendelen. Ze worden niet als authenticatiebewijs naar de website gestuurd.

### Verschil met TOTP

| TOTP                                     | WebAuthn / FIDO2                     |
| ---------------------------------------- | ------------------------------------ |
| Tijdelijke cijfercode                    | Cryptografische authenticatie        |
| Code kan worden onderschept via phishing | Phishingbestendig door domeinbinding |
| Authenticator-app                        | Passkey of beveiligingssleutel       |
| Code handmatig invoeren                  | Vaak biometrie, pincode of aanraking |

Kort gezegd: WebAuthn en FIDO2 maken veilige, phishingbestendige authenticatie mogelijk met passkeys of beveiligingssleutels en vormen een sterk alternatief voor wachtwoorden en TOTP.
