TypeScript is een open-source programmeertaal van Microsoft die JavaScript uitbreidt met statische typering (static typing).

TypeScript wordt veel gebruikt bij moderne frontendframeworks zoals Angular en React.

Belangrijkste kenmerken:

- Static typing: Variabelen, functies en objecten kunnen expliciete datatypes krijgen.
- Type checking: Typefouten worden tijdens de ontwikkeling en compilatie gedetecteerd.
- JavaScript-compatibel: Bestaande JavaScript-code kan grotendeels worden hergebruikt.
- Objectgeoriënteerd: Ondersteuning voor classes, interfaces en inheritance.
- Betere IDE-ondersteuning: Autocompletion, refactoring en foutdetectie.
- Transpilatie: TypeScript wordt omgezet naar JavaScript dat browsers en Node.js kunnen uitvoeren.

### Voorbeeld

JavaScript:

```
function begroeting(naam) {
    return "Hallo " + naam;
}
```

TypeScript:

```
function begroeting(naam: string): string {
    return "Hallo " + naam;
}
```

In TypeScript wordt gecontroleerd of `naam` een string is en of de functie een string teruggeeft.

### Belangrijke onderdelen

| Onderdeel       | Functie                                            |
| --------------- | -------------------------------------------------- |
| `.ts`           | TypeScript-broncode                                |
| `.tsx`          | TypeScript met JSX-syntax, bijvoorbeeld voor React |
| `tsconfig.json` | TypeScript-compilerconfiguratie                    |
| `tsc`           | TypeScript-compiler                                |
| npm             | Installeert TypeScript en dependencies             |

Kort gezegd: TypeScript is JavaScript met extra typecontrole, waardoor fouten eerder worden ontdekt en grotere applicaties beter onderhoudbaar zijn.
