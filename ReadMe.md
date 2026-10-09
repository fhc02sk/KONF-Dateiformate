# Datensatz: Buch

Beschreibt einen Buchtitel im Bibliothekskatalog.

## Felder

- `titel` (Text) – Titel des Buchs
- `autoren` (Liste von Text) – eine oder mehrere Personen
- `erscheinungsjahr` (Zahl) – Jahr der Veröffentlichung
- `verfügbar` (Wahrheitswert) – aktuell ausleihbar?
- `bewertung` (Zahl oder leer) – Durchschnittsnote, `null` wenn noch keine
- `genres` (Liste von Text)
- `verlag` (Objekt) – mit `name` und `ort`

## Als JSON (`daten.json`)

```json
{
  "titel": "Datenbanken kompakt",
  "autoren": ["Jörg Meier", "Anna Huber"],
  "erscheinungsjahr": 2023,
  "verfügbar": true,
  "bewertung": null,
  "genres": ["Fachbuch", "Informatik"],
  "verlag": {
    "name": "TechVerlag",
    "ort": "Wien"
  }
}
```

## Als YAML (`daten.yml`)

```yaml
# Buch im Bibliothekskatalog
titel: Datenbanken kompakt
autoren:
  - Jörg Meier
  - Anna Huber
erscheinungsjahr: 2023
verfügbar: true
bewertung: null
genres:
  - Fachbuch
  - Informatik
verlag:
  name: TechVerlag
  ort: Wien
```

## Als XML (`daten.xml`)

```xml
<?xml version="1.0" encoding="UTF-8"?>
<buch>
  <titel>Datenbanken kompakt</titel>
  <autoren>
    <autor>Jörg Meier</autor>
    <autor>Anna Huber</autor>
  </autoren>
  <erscheinungsjahr>2023</erscheinungsjahr>
  <verfügbar>true</verfügbar>
  <bewertung/>
  <genres>
    <genre>Fachbuch</genre>
    <genre>Informatik</genre>
  </genres>
  <verlag>
    <name>TechVerlag</name>
    <ort>Wien</ort>
  </verlag>
</buch>
```

## Als CSV (`daten.csv`)

```csv
titel,autoren,erscheinungsjahr,verfügbar,bewertung,genres,verlag_name,verlag_ort
Datenbanken kompakt,"Jörg Meier|Anna Huber",2023,true,,"Fachbuch|Informatik",TechVerlag,Wien
```