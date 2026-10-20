Ansible is een open-source IT-automatiserings- en configuratiemanagementtool waarmee je servers, applicaties en infrastructuur geautomatiseerd kunt configureren en beheren.

Ansible is grotendeels agentless: Linux-servers worden doorgaans via SSH beheerd en Windows-systemen via WinRM of PSRP.

Belangrijkste functies:

- Configuration Management: Servers automatisch en consistent configureren.
- Automation: Terugkerende beheertaken automatiseren.
- Application Deployment: Applicaties installeren en configureren.
- Orchestration: Meerdere beheertaken in de juiste volgorde uitvoeren.
- Idempotentie: Veel modules zorgen dat herhaald uitvoeren geen onnodige wijzigingen veroorzaakt.
- Infrastructure Management: Linux-, Windows- en netwerkapparatuur beheren.

### Belangrijke onderdelen

| Onderdeel     | Functie                                         |
| ------------- | ----------------------------------------------- |
| Control Node  | Systeem waarop Ansible wordt uitgevoerd         |
| Managed Node  | Systeem dat Ansible beheert                     |
| Inventory     | Overzicht van te beheren systemen               |
| Playbook      | YAML-bestand met automatiseringstaken           |
| Module        | Voert een specifieke beheertaak uit             |
| Role          | Herbruikbare verzameling taken en configuraties |
| Ansible Vault | Versleutelen van gevoelige configuratiegegevens |

### Veelgebruikte commando's

```
ansible all -m ping
ansible-playbook site.yml
ansible-playbook site.yml --check
ansible-inventory --list
```

### Verschil met Terraform

| Ansible                           | Terraform                              |
| --------------------------------- | -------------------------------------- |
| Configuratie en automatisering    | Infrastructuur provisioning            |
| YAML-playbooks                    | HCL-configuraties                      |
| Doorgaans agentless via SSH/WinRM | Werkt via provider-API's               |
| Vooral operationele configuratie  | Vooral gewenste infrastructuurtoestand |

Kort gezegd: Terraform maakt en beheert infrastructuur; Ansible configureert systemen en automatiseert beheertaken. Beide tools vullen elkaar aan binnen DevOps.
