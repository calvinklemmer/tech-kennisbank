ELK Stack (Elasticsearch, Logstash en Kibana) is een platform voor centraal logbeheer, zoeken, analyseren en visualiseren van gegevens.

ELK wordt veel gebruikt voor monitoring, troubleshooting en securityanalyse binnen IT- en DevOps-omgevingen.

Belangrijkste functies:

- Centralized Logging: Logbestanden van meerdere systemen centraal verzamelen.
- Search & Analytics: Grote hoeveelheden loggegevens snel doorzoeken en analyseren.
- Monitoring: Applicaties en infrastructuur bewaken.
- Dashboards: Loggegevens en statistieken grafisch weergeven.
- Alerting: Waarschuwingen genereren bij fouten of verdachte gebeurtenissen.
- Security Analysis: Onderzoeken van beveiligingsincidenten.

### Belangrijke onderdelen

| Onderdeel     | Functie                                                             |
| ------------- | ------------------------------------------------------------------- |
| Elasticsearch | Zoek- en analyse-engine voor het opslaan en doorzoeken van gegevens |
| Logstash      | Verzamelt, verwerkt en transformeert loggegevens                    |
| Kibana        | Webinterface voor zoeken, dashboards en visualisaties               |
| Beats         | Lichtgewicht agents voor het verzamelen van logs en metrics         |
| Elastic Agent | Centrale agent voor logs, metrics en securitygegevens               |

Met Beats of Elastic Agent wordt ook gesproken van de Elastic Stack.

### Hoe werkt ELK?

Applicaties / Servers / Kubernetes

Produceren loggegevens

Elastic Agent / Beats / Logstash

Verzamelen en verwerken logs

Elasticsearch

Slaat gegevens op en indexeert ze

Kibana

Zoeken, analyseren en visualiseren
