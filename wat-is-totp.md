TOTP (Time-based One-Time Password) is een methode voor tweefactorauthenticatie (2FA/MFA) waarbij een tijdelijke, eenmalige toegangscode wordt gegenereerd op basis van de huidige tijd en een gedeelde geheime sleutel.

TOTP wordt veel gebruikt als extra beveiligingslaag bij het aanmelden op applicaties.

Belangrijkste kenmerken:

- Eenmalige codes: Iedere code is slechts kort geldig, meestal 30 seconden per tijdsinterval. De verifier moet hergebruik van een al geaccepteerde code voorkomen.
- Time-based: Codes veranderen automatisch op basis van de tijd.
- Shared Secret: Server en authenticator-app gebruiken dezelfde geheime sleutel.
- Offline: De authenticator-app heeft geen internetverbinding nodig.
- MFA: Wordt vaak gebruikt als tweede factor naast een wachtwoord.
- RFC 6238: De standaard waarin TOTP is vastgelegd.

### Belangrijke onderdelen

| Onderdeel         | Functie                                            |
| ----------------- | -------------------------------------------------- |
| Shared Secret     | Geheime sleutel die server en authenticator delen  |
| Authenticator App | Genereert tijdelijke toegangscodes                 |
| Time Step         | Tijdsinterval, meestal 30 seconden                 |
| HMAC              | Cryptografisch algoritme voor codegeneratie        |
| QR-code           | Wordt gebruikt om de authenticator te configureren |
| OTP               | Eenmalig wachtwoord, doorgaans zes cijfers         |

### Hoe werkt TOTP?

```
Gebruiker                  Applicatie
    |                         |
    |---- Gebruikersnaam ----->|
    |---- Wachtwoord --------->|
    |                         |
    |<--- TOTP-code gevraagd --|
    |                         |
    |  Authenticator-app       |
    |  genereert code          |
    |                         |
    |---- TOTP-code ---------->|
    |                         |
    |    Code controleren      |
    |                         |
    |<--- Toegang verleend ----|
```

### Authenticator-apps

Voorbeelden van apps die TOTP-codes kunnen genereren zijn Google Authenticator, Microsoft Authenticator en FreeOTP.

Bij het instellen wordt doorgaans een gedeelde geheime sleutel via een QR-code aan de authenticator-app toegevoegd.

### Verschil tussen HOTP en TOTP

| HOTP                                       | TOTP                                         |
| ------------------------------------------ | -------------------------------------------- |
| HMAC-based One-Time Password               | Time-based One-Time Password                 |
| Gebaseerd op een teller                    | Gebaseerd op de huidige tijd                 |
| Code verandert bij een nieuwe tellerwaarde | Code verandert automatisch per tijdsinterval |
| RFC 4226                                   | RFC 6238                                     |

Let op: TOTP biedt extra beveiliging, maar is niet volledig phishingbestendig. Voor phishingbestendige MFA zijn FIDO2/WebAuthn-passkeys of beveiligingssleutels doorgaans geschikter.

Kort gezegd: TOTP genereert tijdelijke beveiligingscodes waarmee gebruikers hun identiteit extra kunnen bevestigen bij het aanmelden op applicaties.
