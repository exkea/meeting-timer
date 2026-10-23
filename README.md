# Meeting timer

Timer voor korte, gestructureerde meetings. Eén statisch HTML-bestand, gehost via GitHub Pages.

## Structuur via URL-parameters

Zet alle parameters in de link. Zonder parameters toont de pagina een neutraal voorbeeld en opent het instellingenpaneel.

| Parameter | Betekenis | Standaard |
|---|---|---|
| `title` | Titel bovenaan | Weekly Sync |
| `people` | Deelnemers check-in, komma-gescheiden | `Persoon A,Persoon B,Persoon C` |
| `checkin` | Minuten per persoon | `3` |
| `vragen` | Minuten vragen na de check-in (`0` = geen) | `1` |
| `blocks` | Blokken na de check-in, `Naam:minuten` | `Tensions:10,Actionables:5` |

Voorbeeld:

```
https://exkea.github.io/meeting-timer/?title=Sales%20Weekly&people=Anna,Bert&checkin=2&vragen=0&blocks=Pipeline:8,Deals:5
```

Het paneel **Structuur aanpassen** onderaan de pagina maakt zo'n link voor je.

Sneltoetsen: `Spatie` start/pauze, `→` volgende blok, `←` vorige blok.
