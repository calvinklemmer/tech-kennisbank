Kubernetes (K8s) is een open-source containerorkestratieplatform waarmee je containerapplicaties automatisch kunt uitrollen, beheren en schalen.

Kubernetes wordt veel gebruikt om Docker- en andere OCI-compatibele containerimages in productieomgevingen uit te voeren.

Belangrijkste functies:

- Containerorkestratie: Containers automatisch verdelen over servers.
- Self-healing: Uitgevallen containers herstarten of vervangen via Kubernetes-mechanismen en controllers, voor zover voldoende clusterresources beschikbaar zijn.
- Scaling: Applicaties horizontaal op- en afschalen.
- Load balancing: Netwerkverkeer verdelen over applicatie-instanties.
- Rolling updates: Nieuwe versies uitrollen met minimale onderbreking.
- Configuratiebeheer: ConfigMaps en Secrets beheren.

### Belangrijke onderdelen

| Onderdeel  | Functie                                                 |
| ---------- | ------------------------------------------------------- |
| Cluster    | Verzameling servers waarop Kubernetes draait            |
| Node       | Server (fysiek of virtueel) binnen het cluster          |
| Pod        | Kleinste deploybare eenheid, met één of meer containers |
| Deployment | Beheert gewenste aantallen Pods en updates              |
| Service    | Stabiel netwerkadres voor Pods                          |
| Ingress    | Regelt externe HTTP(S)-toegang tot Services             |
| Namespace  | Logische scheiding van resources                        |

### Veelgebruikte commando's

```
kubectl get nodes
kubectl get pods -A
kubectl get deployments -A
kubectl get services -A
kubectl logs <podnaam>
```

Kort gezegd: Docker verpakt en draait containers; Kubernetes beheert die containers op schaal, inclusief beschikbaarheid, netwerkverkeer en updates.
