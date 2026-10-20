Kustomize is een open-source configuratietool waarmee Kubernetes YAML-bestanden kunnen worden aangepast en hergebruikt, zonder de oorspronkelijke configuratie te wijzigen.

Kustomize wordt veel gebruikt binnen Kubernetes-, DevOps- en GitOps-omgevingen en is geïntegreerd in `kubectl`.

### Belangrijkste functies

- Base & Overlays: Basisconfiguraties hergebruiken voor verschillende omgevingen.
- Declarative Configuration: Gewenste configuratie vastleggen in YAML.
- Patching: Specifieke instellingen aanpassen zonder bestanden te dupliceren.
- Environment Management: Verschillen tussen development, test en productie beheren.
- GitOps Integration: Configuraties beheren via Git en Argo CD.
- Native Kubernetes: Direct beschikbaar via `kubectl`.

### Belangrijke onderdelen

| Onderdeel          | Functie                                                   |
| ------------------ | --------------------------------------------------------- |
| Base               | Gemeenschappelijke Kubernetes-configuratie                |
| Overlay            | Omgevingsspecifieke aanpassingen                          |
| kustomization.yaml | Beschrijft welke resources en wijzigingen worden gebruikt |
| Patch              | Past specifieke configuratievelden aan                    |
| Resources          | Kubernetes-objecten zoals Deployments en Services         |

### Voorbeeld directorystructuur

```
kubernetes/
├── base/
│   ├── deployment.yaml
│   ├── service.yaml
│   └── kustomization.yaml
└── overlays/
    ├── dev/
    │   └── kustomization.yaml
    ├── test/
    │   └── kustomization.yaml
    └── prod/
        └── kustomization.yaml
```

### Veelgebruikte commando's

```
# Gegenereerde configuratie bekijken
kubectl kustomize overlays/dev

# Configuratie toepassen op Kubernetes
kubectl apply -k overlays/dev
```

### Verschil met Helm

| Kustomize                  | Helm                            |
| -------------------------- | ------------------------------- |
| Past bestaande YAML aan    | Genereert YAML vanuit templates |
| Gebruikt bases en overlays | Gebruikt charts en values       |
| Geen eigen template-engine | Ondersteunt Go-templates        |
| Geïntegreerd in kubectl    | Afzonderlijke CLI               |

Beide tools kunnen worden gebruikt met Argo CD.

Kort gezegd: Kustomize maakt het mogelijk om Kubernetes-configuraties centraal te beheren en per omgeving aan te passen, zonder YAML-bestanden onnodig te dupliceren.
