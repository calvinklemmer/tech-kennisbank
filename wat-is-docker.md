Docker is een open-source platform waarmee je applicaties kunt verpakken, distribueren en uitvoeren in containers.

Een container bevat de applicatie en de benodigde dependencies, zodat deze consistent kan draaien op verschillende systemen.

Belangrijkste functies:

- Containerisatie: Applicaties geïsoleerd uitvoeren.
- Portabiliteit: Containerimages consistent gebruiken op compatibele systemen en cloudplatformen. Linux-containers op Windows vereisen doorgaans een Linux-omgeving, bijvoorbeeld via WSL 2.
- Imagebeheer: Applicaties en dependencies verpakken in herbruikbare images.
- Reproduceerbaarheid: Consistente ontwikkel-, test- en productieomgevingen.
- Efficiëntie: Containers delen de kernel van het hostsysteem en zijn doorgaans lichter dan virtuele machines.

### Belangrijke onderdelen

| Onderdeel        | Functie                                                    |
| ---------------- | ---------------------------------------------------------- |
| Dockerfile       | Instructies voor het bouwen van een image                  |
| Docker image     | Verpakt bestandssysteem en configuratie van een applicatie |
| Docker container | Draaiende instantie van een image                          |
| Docker Compose   | Beheren van meerdere samenwerkende containers              |
| Docker Registry  | Opslag en distributie van images, bijvoorbeeld Harbor      |

### Veelgebruikte commando's

```
docker build -t myapp .
docker run -d --name myapp myapp
docker ps
docker logs myapp
docker stop myapp
```

Kort gezegd: Docker verpakt applicaties in containers, zodat ze voorspelbaar en consistent kunnen worden uitgerold en uitgevoerd.
