GitOps is een DevOps-beheermethodiek waarbij Git fungeert als centrale bron (Single Source of Truth) voor de gewenste configuratie van infrastructuur en applicaties.

GitOps gebruikt declaratieve configuraties en automatische synchronisatie om systemen consistent te beheren.

Belangrijkste functies:

- Declarative Configuration: Gewenste systeemconfiguraties vastleggen als code.
- Version Control: Wijzigingen beheren en traceren via Git.
- Automated Deployment: Configuratiewijzigingen automatisch toepassen.
- Drift Detection: Verschillen tussen gewenste en actuele configuraties detecteren.
- Self-Healing: Configuratieafwijkingen automatisch herstellen wanneer de GitOps-controller hiervoor is ingesteld.
- Auditability: Wijzigingen en goedkeuringen inzichtelijk maken.

### Belangrijke onderdelen

| Onderdeel                    | Functie                                          |
| ---------------------------- | ------------------------------------------------ |
| Git Repository               | Centrale opslag van gewenste configuraties       |
| Declarative Configuration    | Beschrijft hoe de omgeving eruit moet zien       |
| GitOps Controller            | Synchroniseert de omgeving met Git               |
| Reconciliation               | Vergelijkt en corrigeert configuratieverschillen |
| Pull Request / Merge Request | Gecontroleerd wijzigingen doorvoeren             |
| Argo CD / Flux               | Tools die GitOps implementeren                   |

### Hoe werkt GitOps?

1\. Configuratiewijziging in Git

Bijvoorbeeld een nieuwe containerimageversie

2\. Review en Merge

Wijziging wordt gecontroleerd en goedgekeurd

3\. GitOps Controller (Argo CD)

Detecteert de gewijzigde gewenste configuratie

4\. Kubernetes

Wordt gesynchroniseerd met de configuratie in Git

### Verschil met CI/CD

| CI/CD                                     | GitOps                                                |
| ----------------------------------------- | ----------------------------------------------------- |
| Automatiseert bouwen, testen en uitrollen | Beheert gewenste configuratie via Git                 |
| Kan deployments actief uitvoeren (push)   | Controller synchroniseert doorgaans vanuit Git (pull) |
| Bijvoorbeeld Jenkins                      | Bijvoorbeeld Argo CD                                  |

Kort gezegd: GitOps gebruikt Git als bron voor de gewenste systeemtoestand en zorgt ervoor dat infrastructuur en applicaties automatisch met die configuratie worden gesynchroniseerd.
