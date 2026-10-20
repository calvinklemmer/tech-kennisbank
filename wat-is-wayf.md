WAYF (Where Are You From) is een Identity Provider Discovery-mechanisme waarmee gebruikers kunnen kiezen via welke organisatie of Identity Provider (IdP) ze willen inloggen.

WAYF wordt veel gebruikt binnen federatieve authenticatieomgevingen, bijvoorbeeld bij SURFconext en OpenConext.

Belangrijkste functies:

- IdP-selectie: Gebruikers kiezen hun organisatie of Identity Provider.
- Federatieve authenticatie: Inloggen via de eigen organisatie.
- Single Sign-On (SSO): Toegang tot meerdere diensten via de eigen IdP.
- Discovery Service: Beschikbare Identity Providers zoeken en selecteren.
- Gebruiksgemak: Gebruikers hoeven niet te weten welke technische authenticatieprotocollen worden gebruikt.

### Hoe werkt WAYF?

1\. Gebruiker opent applicatie

Bijvoorbeeld een selfserviceportaal

2\. WAYF-scherm

Gebruiker kiest zijn organisatie

3\. Redirect naar gekozen IdP

Bijvoorbeeld de IdP van de eigen organisatie

4\. Authenticatie

Gebruiker logt in bij de eigen organisatie

5\. Terug naar applicatie

Na succesvolle authenticatie beoordeelt de applicatie of de gebruiker toegang krijgt

### Rol binnen federatieve authenticatie

WAYF verzorgt de selectie van de juiste Identity Provider, maar voert zelf geen gebruikersauthenticatie uit.

De daadwerkelijke authenticatie vindt plaats bij de gekozen Identity Provider.

Kort gezegd: WAYF is het keuzescherm waarmee gebruikers aangeven bij welke organisatie ze horen, zodat ze naar de juiste Identity Provider worden doorgestuurd om in te loggen.
