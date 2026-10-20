Alertmanager is een open-source alertmanagementsysteem dat onderdeel is van het Prometheus-ecosysteem. Het verwerkt waarschuwingen (alerts) die door Prometheus en andere compatibele systemen worden gegenereerd.

Alertmanager zorgt ervoor dat meldingen op de juiste manier bij de juiste personen of systemen terechtkomen.

Belangrijkste functies:

- Alert Routing: Waarschuwingen doorsturen naar de juiste ontvangers.
- Grouping: Gerelateerde waarschuwingen bundelen.
- Deduplication: Dubbele meldingen voorkomen.
- Silencing: Waarschuwingen tijdelijk onderdrukken, bijvoorbeeld tijdens onderhoud.
- Inhibition: Minder belangrijke waarschuwingen onderdrukken wanneer een gerelateerde, ernstigere storing actief is.
- Notifications: Meldingen versturen via e-mail, Slack, PagerDuty of webhooks.

### Belangrijke onderdelen

| Onderdeel      | Functie                                                   |
| -------------- | --------------------------------------------------------- |
| Prometheus     | Verzamelt metrics en genereert alerts op basis van regels |
| Alerting Rules | Definiëren wanneer een waarschuwing ontstaat              |
| Alertmanager   | Verwerkt en routeert waarschuwingen                       |
| Receiver       | Bestemming van een melding                                |
| Route          | Bepaalt welke receiver een alert ontvangt                 |
| Silence        | Onderdrukt geselecteerde alerts tijdelijk                 |
| Webhook        | Stuurt meldingen naar externe systemen                    |

### Hoe werkt Alertmanager?

```
Applicaties / Kubernetes / Servers
               |
               v
           Prometheus
        (metrics + regels)
               |
               v
          Alertmanager
     (groeperen en routeren)
               |
       +-------+-------+
       |       |       |
       v       v       v
     E-mail   Slack   Webhook
```

### Verschil met Prometheus en Grafana

| Technologie  | Primaire functie                             |
| ------------ | -------------------------------------------- |
| Prometheus   | Metrics verzamelen en alertregels evalueren  |
| Alertmanager | Alerts verwerken, groeperen en doorsturen    |
| Grafana      | Metrics visualiseren en dashboards aanbieden |

Kort gezegd: Alertmanager verwerkt waarschuwingen van Prometheus en zorgt ervoor dat relevante storingsmeldingen gecontroleerd en zonder onnodige duplicaten bij de juiste ontvangers terechtkomen.
