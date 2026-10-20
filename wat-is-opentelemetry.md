OpenTelemetry (OTel) is een open-source observability-framework waarmee je telemetrygegevens van applicaties en infrastructuur gestandaardiseerd kunt verzamelen, verwerken en exporteren.

OpenTelemetry is vendor-neutraal en wordt gebruikt binnen DevOps-, Kubernetes- en cloudomgevingen. Het biedt standaarden en hulpmiddelen voor telemetry, maar is zelf geen volledige monitoring- of opslagbackend.

Belangrijkste functies:

- Metrics: Prestatiegegevens zoals CPU-gebruik, responstijden en foutpercentages verzamelen.
- Logs: Applicatie- en systeemgebeurtenissen verzamelen.
- Traces: Verzoeken volgen door verschillende applicaties en services.
- Instrumentation: Applicaties voorzien van meetpunten, automatisch of handmatig.
- Context Propagation: Trace-informatie doorgeven tussen services.
- Vendor-neutraliteit: Telemetrygegevens exporteren naar verschillende monitoringplatforms.

### Belangrijke onderdelen

| Onderdeel         | Functie                                                |
| ----------------- | ------------------------------------------------------ |
| OpenTelemetry SDK | Genereert en verwerkt telemetrygegevens in applicaties |
| OTel Collector    | Ontvangt, verwerkt en exporteert telemetrygegevens     |
| OTLP              | Standaardprotocol voor telemetrygegevens               |
| Instrumentation   | Toevoegen van meetpunten aan applicaties               |
| Exporter          | Stuurt telemetrygegevens naar een backend              |
| Trace / Span      | Beschrijft een verzoek en afzonderlijke bewerkingen    |

### Hoe werkt OpenTelemetry?

Applicaties / Services / Kubernetes

Genereren metrics, logs en traces

OpenTelemetry Collector

Ontvangt, verwerkt en routeert telemetrygegevens

Monitoringplatform

Bijvoorbeeld Prometheus, Grafana Tempo of Dynatrace

### Verschil met Prometheus en Grafana

| Technologie   | Primaire functie                       |
| ------------- | -------------------------------------- |
| OpenTelemetry | Telemetry verzamelen en doorsturen     |
| Prometheus    | Metrics opslaan, bevragen en monitoren |
| Grafana       | Gegevens visualiseren en analyseren    |

Kort gezegd: OpenTelemetry standaardiseert het verzamelen en uitwisselen van metrics, logs en traces, onafhankelijk van het monitoringplatform dat deze gegevens uiteindelijk verwerkt.
