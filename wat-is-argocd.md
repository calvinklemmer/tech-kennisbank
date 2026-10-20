Argo CD is een open-source GitOps-tool voor Kubernetes waarmee applicaties automatisch worden uitgerold en gesynchroniseerd op basis van configuraties in Git.

Argo CD controleert of de daadwerkelijke Kubernetes-omgeving overeenkomt met de gewenste configuratie in Git.

Belangrijkste functies:

- GitOps: Git fungeert als centrale bron voor de gewenste configuratie (Single Source of Truth).
- Continuous Delivery: Applicaties automatisch of handmatig uitrollen.
- Automatische synchronisatie: Verschillen tussen Git en Kubernetes detecteren en, indien ingeschakeld, automatisch synchroniseren.
- Drift Detection: Ongewenste configuratieafwijkingen signaleren.
- Rollback: Terugkeren naar een eerdere gewenste configuratie, doorgaans door een eerdere Git-versie opnieuw toe te passen.
- Webinterface: Applicaties, deployments en synchronisatiestatus bekijken.

### Belangrijke onderdelen

| Onderdeel              | Functie                                            |
| ---------------------- | -------------------------------------------------- |
| Git Repository         | Bevat de gewenste Kubernetes-configuratie          |
| Application            | Definieert welke configuratie waar wordt uitgerold |
| Application Controller | Vergelijkt gewenste en actuele toestand            |
| Repo Server            | Verwerkt Git-, Helm- en Kustomize-configuraties    |
| Sync                   | Past Kubernetes-resources aan                      |
| Health Status          | Toont de gezondheid van applicaties                |

### Verschil met Helm en Rancher

| Tool    | Functie                                            |
| ------- | -------------------------------------------------- |
| Helm    | Kubernetes-applicaties configureren en verpakken   |
| Argo CD | GitOps-deployments en synchronisatie automatiseren |
| Rancher | Kubernetes-clusters centraal beheren               |

Kort gezegd: Argo CD zorgt ervoor dat Kubernetes-applicaties overeenkomen met de configuratie in Git en automatiseert daarmee het deploymentproces volgens het GitOps-principe.
