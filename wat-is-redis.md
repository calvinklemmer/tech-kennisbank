Redis (Remote Dictionary Server) is een snelle in-memory datastore waarmee gegevens voornamelijk in het werkgeheugen (RAM) worden opgeslagen en opgevraagd.

Redis wordt veel gebruikt voor caching, sessiebeheer en snelle gegevensuitwisseling tussen applicaties.

### Belangrijkste functies

- Caching: Veelgebruikte gegevens tijdelijk opslaan.
- Session Storage: Gebruikerssessies centraal beheren.
- Key-Value Storage: Gegevens opslaan met unieke sleutels.
- Pub/Sub: Berichten uitwisselen tussen applicaties zonder duurzame opslag of gegarandeerde aflevering.
- TTL (Time To Live): Gegevens automatisch laten verlopen.
- Persistence: Gegevens afhankelijk van de configuratie opslaan op schijf, bijvoorbeeld via RDB-snapshots of AOF.
- Replication: Gegevens repliceren naar andere Redis-instanties.

### Belangrijke onderdelen

| Onderdeel    | Functie                           |
| ------------ | --------------------------------- |
| Redis Server | Beheert de gegevensopslag         |
| redis-cli    | Commandlineclient                 |
| Key          | Unieke naam van een gegeven       |
| Value        | Opgeslagen waarde                 |
| TTL          | Geldigheidsduur van gegevens      |
| Pub/Sub      | Berichten publiceren en ontvangen |

### Voorbeeld

```
# Verbinden met Redis
redis-cli

# Waarde opslaan
SET gebruiker:1001 "Jan"

# Waarde opvragen
GET gebruiker:1001

# Waarde 60 seconden bewaren
SET sessie:abc123 "actief" EX 60

# Resterende geldigheidsduur bekijken
TTL sessie:abc123
```

### Verschil met PostgreSQL

| Redis                              | PostgreSQL                                          |
| ---------------------------------- | --------------------------------------------------- |
| Primair in-memory datastore        | Relationele database                                |
| Gericht op zeer snelle toegang     | Gericht op gestructureerde, duurzame gegevensopslag |
| Veelgebruikt voor caching          | Veelgebruikt als primaire applicatiedatabase        |
| Ondersteunt optionele persistentie | Ondersteunt duurzame transacties                    |

### In een DevOps-omgeving

Redis kan worden ingezet voor:

- Caching van API-responses.
- Centraal sessiebeheer.
- Tijdelijke opslag van gegevens.
- Rate limiting.
- Berichtenuitwisseling tussen applicaties.

Kort gezegd: Redis is een snelle datastore die vooral wordt gebruikt voor caching, sessies en tijdelijke gegevens, waardoor applicaties minder vaak een reguliere database hoeven te raadplegen.
