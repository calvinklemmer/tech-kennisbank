Apache Maven is een open-source build- en dependencymanagementtool, voornamelijk voor Java-projecten.

Maven automatiseert het bouwen, testen en verpakken van applicaties.

Belangrijkste functies:

- Dependency management: Automatisch downloaden en beheren van Java-libraries.
- Build automation: Compileren, testen en verpakken van applicaties.
- Packaging: Genereren van `.jar`, `.war` en andere artifacts.
- Testing: Automatisch uitvoeren van unit-tests; integratietests kunnen via aanvullende pluginconfiguratie worden ingericht.
- Pluginbeheer: Uitbreidbaar met plugins voor bijvoorbeeld codeanalyse en deployment.
- CI/CD: Integratie met Jenkins, GitLab CI en GitHub Actions.

Configuratie: Maven gebruikt een `pom.xml`-bestand (Project Object Model) waarin dependencies, plugins en buildinstellingen staan.

Voorbeeld:

```
mvn clean package
```

Dit verwijdert eerdere buildresultaten, compileert de applicatie, voert standaard de unit-tests uit en genereert een artifact. Integratietests vereisen doorgaans aanvullende configuratie.

Kort gezegd: Maven automatiseert het bouwen, testen en verpakken van Java-projecten en beheert hun dependencies.
