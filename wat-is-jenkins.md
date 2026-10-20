Jenkins is een open-source automatiseringsserver voor CI/CD waarmee je software automatisch kunt bouwen, testen en uitrollen.

Jenkins wordt veel gebruikt binnen DevOps-omgevingen om softwarewijzigingen gecontroleerd van broncode naar productie te brengen.

Belangrijkste functies:

- Continuous Integration (CI): Code automatisch bouwen en testen na wijzigingen in Git.
- Continuous Delivery/Deployment (CD): Software automatisch voorbereiden en uitrollen.
- Pipelines: Build-, test- en deploymentprocessen definiëren als code.
- Pluginarchitectuur: Integratie met Git, Docker, Maven, Kubernetes en andere tools.
- Distributed Builds: Taken verdelen over meerdere buildagents.
- Automatisering: Pipelines starten via Git-webhooks, schema's of handmatig.

### Belangrijke onderdelen

| Onderdeel          | Functie                                    |
| ------------------ | ------------------------------------------ |
| Jenkins Controller | Centrale server die pipelines beheert      |
| Agent              | Systeem waarop build- en testtaken draaien |
| Pipeline           | Geautomatiseerde reeks stappen             |
| Jenkinsfile        | Bestand waarin de pipeline als code staat  |
| Stage              | Logische fase, bijvoorbeeld Build of Test  |
| Plugin             | Uitbreiding voor externe tools en systemen |

### Veelgebruikte pipeline

```
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'npm ci && npm run build'
            }
        }

        stage('Test') {
            steps {
                sh 'npm test'
            }
        }
    }
}
```
