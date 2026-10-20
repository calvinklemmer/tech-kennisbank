CI/CD (Continuous Integration / Continuous Delivery of Deployment) is een DevOps-methodiek waarmee je het bouwen, testen en uitrollen van software automatiseert.

CI/CD wordt veel gebruikt om softwarewijzigingen sneller, consistenter en betrouwbaarder naar productie te brengen.

Belangrijkste functies:

- Continuous Integration (CI): Codewijzigingen automatisch integreren, bouwen en testen.
- Continuous Delivery: Software automatisch bouwen, testen en gereedmaken voor uitrol. De productie-uitrol kan een handmatige goedkeuring vereisen.
- Continuous Deployment: Wijzigingen die alle geautomatiseerde controles doorstaan automatisch naar productie uitrollen, zonder handmatige goedkeuringsstap.
- Automated Testing: Unit-, integratie- en securitytests uitvoeren.
- Artifact Management: Gebouwde software en containerimages opslaan.
- Rollback: Terugkeren naar een eerdere versie bij problemen.

### Belangrijke onderdelen

| Onderdeel      | Functie                                                   |
| -------------- | --------------------------------------------------------- |
| Pipeline       | Geautomatiseerde reeks build-, test- en deploymentstappen |
| Runner / Agent | Systeem dat pipelinejobs uitvoert                         |
| Build          | Broncode omzetten naar uitvoerbare software               |
| Artifact       | Resultaat van een build, bijvoorbeeld een JAR             |
| Registry       | Opslag van containerimages, bijvoorbeeld Harbor           |
| Deployment     | Nieuwe softwareversie uitrollen                           |

### Voorbeelden van CI/CD-tools

- GitLab CI/CD
- GitHub Actions
- Jenkins
- Azure DevOps
- Argo CD (GitOps-deployment)
