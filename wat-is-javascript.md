JavaScript (JS) is een programmeertaal waarmee interactieve websites, webapplicaties en serversoftware worden ontwikkeld.

JavaScript wordt rechtstreeks uitgevoerd door webbrowsers en kan via Node.js ook buiten de browser draaien.

TypeScript (TS) is een uitbreiding van JavaScript, ontwikkeld door Microsoft, die onder andere statische typecontrole toevoegt. TypeScript wordt doorgaans vóór uitvoering omgezet naar JavaScript. Sommige moderne runtimes ondersteunen ook rechtstreeks een deel van de TypeScript-syntax.

### Belangrijkste kenmerken van JavaScript

- Dynamisch getypeerd: Variabelen hebben geen vast gedeclareerd type.
- Browserondersteuning: Werkt rechtstreeks in moderne webbrowsers.
- Interactiviteit: Verwerkt gebruikersacties en wijzigt webpagina's.
- Asynchroon: Ondersteunt onder andere Promises en `async/await`.
- Node.js: Maakt server-side JavaScript mogelijk.

### Belangrijkste kenmerken van TypeScript

- Static Typing: Controleert typen tijdens ontwikkeling en compilatie.
- Type Safety: Helpt typefouten vroegtijdig te detecteren.
- Interfaces: Beschrijft de structuur van objecten.
- JavaScript Compatibility: Geldige JavaScript-code is in principe ook geldige TypeScript-code.
- Transpilation: Zet TypeScript om naar uitvoerbare JavaScript.
- Tooling: Biedt uitgebreide ondersteuning voor autocomplete en refactoring.

### Verschil tussen JavaScript en TypeScript

| JavaScript                                       | TypeScript                                        |
| ------------------------------------------------ | ------------------------------------------------- |
| Programmeertaal                                  | Uitbreiding van JavaScript                        |
| Dynamische typering                              | Optionele statische typering                      |
| Direct uitvoerbaar in browsers                   | Wordt doorgaans omgezet naar JavaScript           |
| Typefouten vaak pas tijdens uitvoering zichtbaar | Veel typefouten al tijdens ontwikkeling zichtbaar |
| Geschikt voor kleine en grote projecten          | Vooral nuttig bij grotere, complexere projecten   |
| Bestanden met `.js`                              | Bestanden met `.ts` en `.tsx`                     |

### Voorbeeld JavaScript

```
function begroet(naam) {
    return "Hallo " + naam;
}

begroet(123); // Wordt toegestaan
```

JavaScript accepteert hier een getal, ook al verwacht de functie conceptueel een naam.

### Voorbeeld TypeScript

```
function begroet(naam: string): string {
    return "Hallo " + naam;
}

begroet(123); // TypeScript geeft een typefout
```

TypeScript detecteert dat een getal wordt doorgegeven terwijl een string wordt verwacht.

### Samengevat

JavaScript is de programmeertaal die browsers uitvoeren.

TypeScript bouwt daarop voort met typecontrole, waardoor code beter onderhoudbaar wordt en veel programmeerfouten eerder worden ontdekt.

Kort gezegd: TypeScript is JavaScript met extra controles tijdens de ontwikkeling. Uiteindelijk wordt TypeScript omgezet naar JavaScript om uitgevoerd te kunnen worden.
