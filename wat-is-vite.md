Vite (uitgesproken als viet, Frans voor 'snel') is een moderne, open-source frontend-buildtool en developmentserver voor JavaScript- en TypeScript-projecten.

Vite wordt onder andere gebruikt bij React, Vue en Svelte. Ook Angular gebruikt Vite-technologie in zijn moderne ontwikkeltooling, maar beheert deze integratie doorgaans via de Angular CLI.

Belangrijkste functies:

- Developmentserver: Start een lokale webserver voor frontendontwikkeling.
- Hot Module Replacement (HMR): Verwerkt codewijzigingen direct in de browser zonder de volledige pagina opnieuw te laden.
- TypeScript-ondersteuning: Verwerkt TypeScript tijdens ontwikkeling en builds.
- Production builds: Bundelt en optimaliseert JavaScript, CSS en andere frontendbestanden.
- Snelle ontwikkeling: Gebruikt native ES Modules voor snelle opstarttijden.
- Pluginarchitectuur: Uitbreidbaar met plugins voor frameworks en andere functionaliteit.

### Veelgebruikte commando's

| Commando             | Functie                          |
| -------------------- | -------------------------------- |
| `npm run dev`        | Start de developmentserver       |
| `npm run build`      | Bouwt de productieversie         |
| `npm run preview`    | Bekijkt de productiebuild lokaal |
| `npx vite --version` | Toont de Vite-versie             |

De npm-scripts moeten wel in `package.json` zijn gedefinieerd.

### Belangrijke bestanden

| Bestand          | Functie                                           |
| ---------------- | ------------------------------------------------- |
| `vite.config.ts` | Configuratie van Vite                             |
| `package.json`   | Dependencies en npm-scripts                       |
| `tsconfig.json`  | TypeScript-configuratie                           |
| `index.html`     | HTML-entrypoint                                   |
| `dist/`          | Gebruikelijke outputdirectory van productiebuilds |

Kort gezegd: Vite versnelt het ontwikkelen en bouwen van moderne frontendapplicaties. TypeScript kan daarbij de programmeertaal zijn. Frameworks zoals React en Vue kunnen rechtstreeks met Vite werken; Angular gebruikt doorgaans de Angular CLI, die intern Vite-technologie kan inzetten.
