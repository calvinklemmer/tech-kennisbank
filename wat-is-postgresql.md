PostgreSQL (ook wel Postgres) is een open-source relationeel databasebeheersysteem (RDBMS) waarmee je gestructureerde gegevens kunt opslaan, beheren en opvragen.

PostgreSQL wordt veel gebruikt voor webapplicaties, enterprise-software en cloudomgevingen.

Belangrijkste functies:

- Relationele opslag: Gegevens opslaan in tabellen met onderlinge relaties.
- SQL: Gegevens opvragen en wijzigen met Structured Query Language.
- ACID-transacties: Betrouwbare en consistente gegevensverwerking.
- Indexering: Zoekopdrachten en databaseprestaties optimaliseren.
- Replication: Databasegegevens repliceren voor hoge beschikbaarheid.
- Backup & Recovery: Back-ups maken en gegevens herstellen.
- Security: Authenticatie, rollen en toegangsrechten beheren.

### Belangrijke onderdelen

| Onderdeel         | Functie                                  |
| ----------------- | ---------------------------------------- |
| PostgreSQL Server | Database-engine                          |
| Database          | Logische verzameling gegevens            |
| Table             | Opslag van gegevens in rijen en kolommen |
| Schema            | Logische indeling van databaseobjecten   |
| SQL               | Taal voor databasebewerkingen            |
| psql              | Commandlineclient voor PostgreSQL        |
| pg_dump           | Tool voor databaseback-ups               |

### Veelgebruikte commando's

```
# Verbinden met een database
psql -h localhost -U appuser -d appdb

# Databases tonen
\l

# Tabellen tonen
\dt

# Verbinding afsluiten
\q
```

### Verschil met andere technologieën

| Technologie   | Primaire functie               |
| ------------- | ------------------------------ |
| PostgreSQL    | Relationele database           |
| Redis         | In-memory datastore en caching |
| Elasticsearch | Zoek- en analyse-engine        |

Kort gezegd: PostgreSQL is een betrouwbaar relationeel databasesysteem voor het persistent opslaan, beheren en opvragen van gegevens.
