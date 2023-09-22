# Normdaten

## Unterstützung durch TEI-Publisher-Annotation

- Airtable: Projektspezifische Datenbank
- Anton: Projektspezifische Datenbank
- Custom: Projektspezifische XML-Daten
- Geonames: Orte
- GND: Gemeinsame Normdatei
- KBGA: Karl-Barth-Gesamtausgabe
- Metagrid 
- Reconciliation: Interne Daten?

Out of the box kann für die Annotation von Personen GND oder Metagrad (mit GND und Helveticat) verwendet werden.

## Interne und externe ID

Für die Annotation und interne Verlinkung sind lokale IDs zu empfehlen, die auf ein eigenes Verzeichnis verweisen.
Auf diese Weise sind die Daten auch offline verständlich.

### Ein Beispiel aus der Wölfflin-Edition:

Die **Referenz im Text** verweist auf eine interne ID, die aber auf der GND-Nummer basiert und damit eindeutig ist.

```xml
Am 10. Dezember 1889 bestellt <rs type="person" ref="#gnd-118634496">Wölfflin</rs> ein Konvolut von ...
```

Im von TEI-Publisher mit GND-Daten generierten **Index-Eintrag** wird auf den GND-Eintrag verlinkt.
An dieser Stelle können weitere Normdaten eingebunden werden.
Die Daten im Index-Eintrag können auf der Seite zur Person oder in einem Dropdown bei der Annotation angezeigt werden.

```xml
<person xml:id="gnd-118634496">
    <persName type="full">Wölfflin, Heinrich</persName>
    <birth when="1864-06-21"/>
    <death when="1945-07-19"/>
    <note>Kunsthistoriker</note>
    <occupation>Kunsthistoriker</occupation>
    <occupation>Geheimer Rat</occupation>
    <ptr type="gnd" target="https://d-nb.info/gnd/118634496"/>
</person>
```

## Mapping auf weitere Normdateien


