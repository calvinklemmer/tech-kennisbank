kind (Kubernetes IN Docker) is een open-source tool waarmee lokale Kubernetes-clusters worden aangemaakt met containers als Kubernetes-nodes. kind ondersteunt onder andere Docker en Podman als containerprovider.

kind wordt vooral gebruikt voor ontwikkeling, testen en CI/CD-pipelines, zonder dat een volledig Kubernetes-platform nodig is.

### Belangrijkste functies

- Local Kubernetes: Kubernetes-clusters lokaal draaien.
- Docker-based: Kubernetes-nodes uitvoeren als containers.
- Multi-node Clusters: Clusters met meerdere nodes simuleren.
- CI/CD Testing: Kubernetes-configuraties automatisch testen.
- Disposable Clusters: Testclusters eenvoudig aanmaken en verwijderen.
- Version Testing: Verschillende Kubernetes-versies testen.

### Belangrijke onderdelen

| Onderdeel        | Functie                                   |
| ---------------- | ----------------------------------------- |
| kind             | Tool voor het beheren van lokale clusters |
| Docker           | Draait de Kubernetes-nodes als containers |
| Control Plane    | Beheert het Kubernetes-cluster            |
| Worker Node      | Voert applicatieworkloads uit             |
| kubectl          | Beheert Kubernetes-resources              |
| kind-config.yaml | Optionele clusterconfiguratie             |

### Veelgebruikte commando's

```
# Cluster aanmaken
kind create cluster --name test

# Clusters tonen
kind get clusters

# Kubernetes-nodes bekijken
kubectl get nodes

# Cluster verwijderen
kind delete cluster --name test
```

### Verschil met een regulier Kubernetes-cluster

| kind                                     | Regulier Kubernetes                                  |
| ---------------------------------------- | ---------------------------------------------------- |
| Gericht op lokale ontwikkeling en testen | Gericht op test-, acceptatie- en productieomgevingen |
| Nodes draaien als Docker-containers      | Nodes draaien doorgaans op VM's of fysieke servers   |
| Snel aan te maken en te verwijderen      | Vereist meer infrastructuur en beheer                |
| Niet bedoeld als productieplatform       | Kan productieapplicaties hosten                      |

### In een DevOps-omgeving

kind kan worden gebruikt om:

- Helm Charts en Kubernetes-manifests te testen.
- Deployments lokaal te controleren.
- CI/CD-tests uit te voeren.
- Kubernetes-versies en configuraties te valideren.

Kort gezegd: kind maakt het mogelijk om snel een tijdelijk Kubernetes-cluster binnen Docker te starten, vooral voor lokale ontwikkeling en geautomatiseerde tests.
