Harbor is een open-source container registry waarmee je containerimages en andere OCI-artifacts centraal kunt opslaan, beheren en beveiligen.

Harbor wordt veel gebruikt in enterprise- en Kubernetes-omgevingen als alternatief voor publieke registries zoals Docker Hub.

Belangrijkste functies:

- Imageopslag: Docker- en OCI-containerimages centraal opslaan.
- Security scanning: Containerimages controleren op bekende kwetsbaarheden. Een scan garandeert niet dat een image volledig veilig is.
- Role-Based Access Control (RBAC): Toegangsrechten beheren voor gebruikers en projecten.
- Image signing: Digitale handtekeningen gebruiken om de herkomst en integriteit van artifacts te verifiëren.
- Replication: Images synchroniseren tussen registries.
- OCI-artifacts: Naast containerimages ook Helm Charts opslaan.

### Belangrijke onderdelen

| Onderdeel     | Functie                                      |
| ------------- | -------------------------------------------- |
| Registry      | Opslag van containerimages                   |
| Project       | Logische groepering van repositories         |
| Repository    | Verzameling imageversies                     |
| Tag           | Leesbare aanduiding van een imageversie      |
| Artifact      | Opgeslagen image of ander OCI-object         |
| Robot Account | Serviceaccount voor geautomatiseerde toegang |

### Veelgebruikte commando's

```
# Aanmelden bij Harbor
docker login harbor.example.nl

# Image taggen
docker tag myapp:latest harbor.example.nl/demo/myapp:v1

# Image uploaden
docker push harbor.example.nl/demo/myapp:v1

# Image downloaden
docker pull harbor.example.nl/demo/myapp:v1
```

Kort gezegd: Harbor slaat containerimages en andere OCI-artifacts centraal op en maakt ze beschikbaar voor deployments.
