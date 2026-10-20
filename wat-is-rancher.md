Rancher is een open-source Kubernetes-managementplatform waarmee je meerdere Kubernetes-clusters centraal kunt beheren, configureren en monitoren.

Rancher biedt een webinterface voor Kubernetes-beheer en wordt ontwikkeld door SUSE.

Belangrijkste functies:

- Clusterbeheer: Meerdere Kubernetes-clusters centraal beheren.
- Webinterface: Kubernetes-resources beheren zonder uitsluitend `kubectl` te gebruiken.
- RBAC: Toegangsrechten beheren voor gebruikers en teams.
- Monitoring: Inzicht in de status en prestaties van clusters, nodes en Pods.
- Application management: Applicaties installeren en beheren via Helm Charts.
- Multi-clusterbeheer: Verschillende Kubernetes-omgevingen vanuit één platform beheren.

### Belangrijke onderdelen

| Onderdeel        | Functie                                |
| ---------------- | -------------------------------------- |
| Rancher Server   | Centrale beheeromgeving                |
| Cluster          | Kubernetes-omgeving                    |
| Project          | Groepering van Kubernetes-namespaces   |
| Workloads        | Applicaties, Deployments en Pods       |
| Cluster Explorer | Webinterface voor Kubernetes-resources |
| Apps             | Helm-gebaseerd applicatiebeheer        |

### Samenhang

Containerimage → Registry → Helm → Kubernetes

Rancher biedt een centrale beheerlaag voor Kubernetes-clusters.

Kort gezegd: Kubernetes voert de containers uit, Helm beheert de applicatiedeployments en Rancher biedt een centrale webinterface om Kubernetes-clusters en applicaties te beheren.
