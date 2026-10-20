Helm is een open-source package manager voor Kubernetes waarmee je applicaties eenvoudiger kunt installeren, configureren, upgraden en beheren.

Helm gebruikt zogenaamde Helm Charts om Kubernetes-resources te definiëren.

Belangrijkste functies:

- Package management: Kubernetes-applicaties als herbruikbare pakketten beheren.
- Templating: Kubernetes YAML-bestanden dynamisch genereren.
- Configuratiebeheer: Omgevingsspecifieke instellingen via `values.yaml`.
- Release management: Applicaties installeren, upgraden en terugdraaien.
- Herbruikbaarheid: Dezelfde Helm Chart gebruiken voor development, test en productie.

### Belangrijke onderdelen

| Onderdeel       | Functie                                |
| --------------- | -------------------------------------- |
| Chart.yaml      | Metadata van de Helm Chart             |
| values.yaml     | Standaardconfiguratie                  |
| templates/      | Kubernetes YAML-templates              |
| Release         | Geïnstalleerde instantie van een Chart |
| Helm Repository | Opslaglocatie voor Charts              |

### Veelgebruikte commando's

```
helm list -A
helm install myapp ./chart
helm upgrade myapp ./chart
helm rollback myapp 1
helm uninstall myapp
```

Kort gezegd: Kubernetes beheert de containers; Helm vereenvoudigt het installeren, configureren en updaten van applicaties binnen Kubernetes.
