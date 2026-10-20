Prometheus is een open-source monitoring- en alertingplatform waarmee je prestatiegegevens (metrics) van applicaties, servers en infrastructuur verzamelt en analyseert.

Prometheus wordt veel gebruikt binnen Kubernetes- en DevOps-omgevingen.

Belangrijkste functies:

- Metrics Collection: Verzamelt prestatiegegevens zoals CPU-, geheugen- en netwerkgebruik.
- Time Series Database (TSDB): Slaat meetwaarden op met tijdstempels.
- Pull-based Monitoring: Haalt periodiek metrics op via HTTP-endpoints.
- PromQL: Querytaal voor het analyseren van metrics.
- Alerting: Evalueert alertregels op basis van metrics. Alertmanager kan de gegenereerde alerts vervolgens groeperen, routeren en als meldingen versturen.
- Service Discovery: Ontdekt automatisch te monitoren systemen, bijvoorbeeld binnen Kubernetes.

### Belangrijke onderdelen

| Onderdeel         | Functie                                         |
| ----------------- | ----------------------------------------------- |
| Prometheus Server | Verzamelt en bewaart metrics                    |
| Exporter          | Maakt metrics van systemen beschikbaar          |
| PromQL            | Querytaal voor metrics                          |
| Alertmanager      | Verwerkt en routeert waarschuwingen             |
| Pushgateway       | Ontvangt metrics van kortlopende batchprocessen |
| Grafana           | Externe tool voor dashboards en visualisaties   |

### Hoe werkt Prometheus?

Applicaties / Kubernetes / Exporters

Stellen metrics beschikbaar via HTTP

Prometheus

Verzamelt, bewaart en analyseert metrics

Grafana

Dashboards en visualisaties

Alertmanager

Waarschuwingen en notificaties

### Verschil met ELK en Dynatrace

| Platform   | Primaire toepassing        |
| ---------- | -------------------------- |
| Prometheus | Metrics en alerting        |
| ELK Stack  | Logs en loganalyse         |
| Dynatrace  | Brede observability en APM |
| Splunk     | Loganalyse en SIEM         |

Kort gezegd: Prometheus verzamelt en analyseert meetwaarden van systemen en applicaties, zodat je prestaties, beschikbaarheid en afwijkingen kunt monitoren.
