Grafana is een open-source observability- en visualisatieplatform waarmee je metrics, logs en traces uit verschillende databronnen kunt analyseren en weergeven in dashboards. De gegevens worden doorgaans opgeslagen in gekoppelde systemen, zoals Prometheus, Loki of Tempo.

Grafana wordt veel gebruikt binnen Kubernetes-, DevOps- en monitoringomgevingen.

Belangrijkste functies:

- Dashboards: Prestatiegegevens grafisch visualiseren.
- Monitoring: CPU-, geheugen-, netwerk- en applicatieprestaties inzichtelijk maken.
- Alerting: Waarschuwingen genereren bij afwijkingen.
- Multi-Data Source: Gegevens combineren uit onder andere Prometheus, Elasticsearch en Loki.
- Observability: Metrics, logs en traces gezamenlijk analyseren.
- Querying: Gegevens opvragen via querytalen zoals PromQL.

### Belangrijke onderdelen

| Onderdeel      | Functie                                          |
| -------------- | ------------------------------------------------ |
| Grafana Server | Webinterface voor dashboards en beheer           |
| Dashboard      | Verzameling visualisaties                        |
| Panel          | Individuele grafiek, tabel of meetwaarde         |
| Data Source    | Koppeling met bijvoorbeeld Prometheus            |
| Alert Rule     | Voorwaarde voor het genereren van waarschuwingen |
| Grafana Loki   | Systeem voor opslag en analyse van logs          |
| Grafana Tempo  | Backend voor distributed tracing                 |

### Verschil met Prometheus

| Prometheus                   | Grafana                             |
| ---------------------------- | ----------------------------------- |
| Verzamelt en bewaart metrics | Visualiseert en analyseert gegevens |
| Time Series Database         | Dashboard- en observabilityplatform |
| Gebruikt PromQL              | Ondersteunt meerdere databronnen    |
| Metrics en alertregels       | Dashboards en alerting              |

Kort gezegd: Prometheus verzamelt de meetgegevens en Grafana maakt deze inzichtelijk via dashboards, grafieken en waarschuwingen.
