Terraform is een Infrastructure as Code (IaC)-tool van HashiCorp waarmee je infrastructuur geautomatiseerd kunt aanmaken, configureren en beheren.

Terraform gebruikt de declaratieve configuratietaal HCL (HashiCorp Configuration Language).

Belangrijkste functies:

- Infrastructure as Code: Infrastructuur definiëren in configuratiebestanden.
- Automatisering: Servers, netwerken en cloudresources aanmaken en beheren.
- Declaratief beheer: Beschrijven wat de gewenste infrastructuur moet zijn.
- State Management: Bijhouden welke resources Terraform beheert.
- Multi-provider: Ondersteuning voor onder andere Azure, AWS, Kubernetes en VMware.
- Versiebeheer: Infrastructuurconfiguraties beheren via Git.

### Belangrijke onderdelen

| Onderdeel          | Functie                                       |
| ------------------ | --------------------------------------------- |
| `.tf`              | Terraform-configuratiebestand                 |
| Provider           | Koppeling met een platform of API             |
| Resource           | Infrastructuuronderdeel dat Terraform beheert |
| Module             | Herbruikbare verzameling configuraties        |
| State (`.tfstate`) | Vastgelegde toestand van beheerde resources   |
| HCL                | Configuratietaal van Terraform                |

### Veelgebruikte commando's

```
terraform init
terraform validate
terraform plan
terraform apply
terraform destroy
```

### Beveiliging van Terraform State

Het Terraform state-bestand kan gevoelige gegevens bevatten, ook wanneer deze in de uitvoer als sensitive zijn gemarkeerd.

Bewaar state daarom bij voorkeur in een beveiligde remote backend met toegangscontrole, versleuteling en waar nodig state locking. Sla state-bestanden met geheimen niet op in Git.

### Verschil met Helm en Argo CD

| Tool      | Functie                                            |
| --------- | -------------------------------------------------- |
| Terraform | Infrastructuur en resources declaratief beheren    |
| Helm      | Kubernetes-applicaties configureren en installeren |
| Argo CD   | Kubernetes-deployments synchroniseren met Git      |

Kort gezegd: Terraform automatiseert het beheer van infrastructuur via code, zodat omgevingen reproduceerbaar, controleerbaar en consistent kunnen worden ingericht.
