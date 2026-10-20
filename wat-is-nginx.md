NGINX (uitgesproken als engine-x) is een open-source webserver, reverse proxy en load balancer waarmee je HTTP(S)-verkeer kunt verwerken en doorsturen.

NGINX bestaat nog steeds en wordt veel gebruikt binnen Linux-, DevOps- en Kubernetes-omgevingen.

Belangrijkste functies:

- Webserver: Websites en statische bestanden aanbieden.
- Reverse Proxy: Verzoeken doorsturen naar backendapplicaties.
- Load Balancing: Verkeer verdelen over meerdere servers.
- TLS Termination: HTTPS-verbindingen afhandelen.
- Caching: Veelgebruikte content tijdelijk opslaan.
- Ingress Controller: Kubernetes Ingress-regels uitvoeren via een NGINX-gebaseerde controller.

### Belangrijke onderdelen

| Onderdeel      | Functie                                   |
| -------------- | ----------------------------------------- |
| NGINX Server   | Verwerkt HTTP(S)-verzoeken                |
| nginx.conf     | Hoofdconfiguratiebestand                  |
| Server Block   | Configuratie voor een hostname of website |
| Location Block | Routeringsregels voor URL-paden           |
| Upstream       | Groep backendservers                      |
| Proxy Pass     | Stuurt verzoeken door naar een backend    |

### Voorbeeld reverse proxy

```
server {
    listen 443 ssl;
    server_name app.example.nl;

    ssl_certificate /etc/nginx/cert.pem;
    ssl_certificate_key /etc/nginx/key.pem;

    location / {
        proxy_pass http://backend:8080;
        proxy_set_header Host $host;
        proxy_set_header X-Forwarded-Proto $scheme;
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
    }
}
```

Dit is een vereenvoudigd voorbeeld; voor productie zijn aanvullende beveiligingsinstellingen en een correcte configuratie van vertrouwde proxyheaders nodig.

### NGINX versus Kubernetes Ingress

| NGINX                              | Kubernetes Ingress             |
| ---------------------------------- | ------------------------------ |
| Webserver en reverse-proxysoftware | Kubernetes API-resource        |
| Configureerbaar via `nginx.conf`   | Configureerbaar via YAML       |
| Werkt zelfstandig of in Kubernetes | Vereist een Ingress Controller |

Let op: De communitycontroller ingress-nginx is een afzonderlijk project van NGINX zelf. Het onderhoud daarvan is in maart 2026 beëindigd. NGINX als webserver en reverse proxy blijft bestaan.

Kort gezegd: NGINX is een webserver en reverse proxy die HTTP(S)-verkeer verwerkt en doorstuurt naar backendapplicaties.
