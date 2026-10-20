npm (Node Package Manager) is de standaard package manager voor Node.js waarmee je JavaScript- en TypeScript-packages installeert, beheert en bijwerkt.

npm wordt doorgaans samen met Node.js geïnstalleerd.

Belangrijkste functies:

- Dependency management: Automatisch installeren en beheren van libraries en frameworks.
- Package installation: Packages zoals Angular, React en Storybook installeren.
- Scripts uitvoeren: Build-, test- en ontwikkelcommando's starten.
- Versiebeheer: Packageversies beheren via `package.json` en `package-lock.json`.
- Security auditing: Bekende kwetsbaarheden in dependencies controleren met `npm audit`.
- Package publishing: Eigen packages publiceren naar de npm-registry.

### Veelgebruikte commando's

| Commando                | Functie                                                         |
| ----------------------- | --------------------------------------------------------------- |
| `npm install`           | Installeert projectdependencies                                 |
| `npm ci`                | Installeert dependencies reproduceerbaar vanuit het lockbestand |
| `npm install <package>` | Installeert een package                                         |
| `npm run build`         | Voert het buildscript uit                                       |
| `npm run dev`           | Start de ontwikkelomgeving, indien geconfigureerd               |
| `npm audit`             | Controleert op bekende kwetsbaarheden                           |
| `npm update`            | Werkt dependencies bij binnen toegestane versies                |

### Belangrijke bestanden

- `package.json`: Definieert dependencies, scripts en projectinformatie.
- `package-lock.json`: Legt de exacte dependencyversies vast.
- `node_modules/`: Bevat de geïnstalleerde packages.

### Verschil met Maven

| npm                     | Maven             |
| ----------------------- | ----------------- |
| JavaScript / TypeScript | Voornamelijk Java |
| `package.json`          | `pom.xml`         |
| npm-registry            | Maven Central     |
| `npm run build`         | `mvn package`     |

Kort gezegd: npm is voor JavaScript/TypeScript ongeveer wat Maven voor Java is: een tool om dependencies te beheren en buildprocessen uit te voeren.
