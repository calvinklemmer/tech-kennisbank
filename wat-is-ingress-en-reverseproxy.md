Ingress en Reverse Proxy zijn technologieën waarmee inkomend netwerkverkeer naar de juiste applicaties en services wordt doorgestuurd.

Een Reverse Proxy ontvangt verzoeken namens backendservers. Ingress is een Kubernetes-resource waarmee je HTTP(S)-routering naar services configureert, uitgevoerd door een Ingress Controller.

Belangrijkste functies:

- Routing: Verkeer doorsturen op basis van hostnames en URL-paden.
- Load Balancing: Verkeer verdelen over meerdere backendservers.
- TLS Termination: HTTPS-verbindingen afhandelen.
- Security: Toegangsregels en beveiligingsmaatregelen toepassen.
- Centralized Access: Meerdere applicaties via één toegangspunt bereikbaar maken.

### Belangrijke onderdelen

| Onderdeel          | Functie                                          |
| ------------------ | ------------------------------------------------ |
| Reverse Proxy      | Stuurt clientverzoeken door naar backendservers  |
| Ingress            | Kubernetes-resource met HTTP(S)-routeringsregels |
| Ingress Controller | Implementeert de Ingress-regels                  |
| NGINX / Traefik    | Software die als reverse proxy kan functioneren  |
| Load Balancer      | Verdeelt netwerkverkeer                          |
| TLS Termination    | Ontsleutelt inkomend HTTPS-verkeer               |

### Hoe werkt het?

Gebruiker / Browser

HTTPS-verzoek naar app.example.nl

Ingress Controller / Reverse Proxy

TLS-terminatie en routering

Kubernetes Service

Stabiel toegangspunt voor applicatie-Pods

Applicatie-Pod

Verwerkt het HTTP-verzoek

Kort gezegd: Een reverse proxy stuurt inkomend verkeer naar de juiste backend; Kubernetes Ingress definieert de routeringsregels die een Ingress Controller uitvoert.
