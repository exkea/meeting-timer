# Meeting timer

Timer voor korte, gestructureerde meetings. Eén statisch HTML-bestand, gehost via GitHub Pages.

## Structuur via URL-parameters

Zet de structuur in de link: een `title` en één `slot` per blok, in de volgorde van de meeting.

| Parameter | Formaat | Voorbeeld |
|---|---|---|
| `title` | Naam van de meeting | `Weekly Sync` |
| `slot` | `Titel:Slot:minuten`, herhaal per blok | `Check-in:Kenneth:3` |

- **Titel** groepeert slots in de balk, bijvoorbeeld drie check-in-slots onder `Check-in`.
- **Slot** is de naam die groot in beeld staat.
- **Minuten** mag een halve minuut zijn: `2.5`.
- `Slot:minuten` mag ook; dan is de titel gelijk aan de slotnaam.

Voorbeeld:

```
https://exkea.github.io/meeting-timer/?title=Weekly%20Sync&slot=Check-in:Kenneth:3&slot=Check-in:Nick:3&slot=Check-in:Joey:3&slot=Check-in:Vragen:1&slot=Tensions:Tensions:10&slot=Actionables:Actionables:5
```

Zonder parameters toont de pagina een neutraal voorbeeld en opent het paneel **Structuur aanpassen**. Daar voeg je slot per slot toe en kopieer je de link.

Sneltoetsen: `Spatie` start/pauze, `→` volgende blok, `←` vorige blok.
