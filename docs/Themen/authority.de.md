# Normdaten

## Unterstützung durch TEI-Publisher-Annotation

-   Airtable: Projektspezifische Datenbank
-   Anton: Projektspezifische Datenbank
-   Custom: Projektspezifische XML-Daten  
    Geeignet beispielsweise für Retrodigitalisierung, wo bereits ein Register existiert
-   Geonames: Orte  
    International und mit Koordinaten, Suche nach Namen am besten auf Englisch
-   GND: Gemeinsame Normdatei
    Standard im deutschsprachigen Raum, gut für historische Daten und alternative Schreibweisen
-   KBGA: Karl-Barth-Gesamtausgabe
-   Metagrid  
    Verbindung mit schweizerischen Datenquellen
-   Reconciliation: Interne Daten?

Out of the box kann für die Annotation von Personen GND oder Metagrid (mit GND und Helveticat) verwendet werden.

## Interne und externe ID

Annotationen können theoretisch auch aus Weblinks direkt auf Normdaten bestehen, der Standard ist jedoch die Aggregierung eines lokalen Verzeichnisses.
Ein lokales Verzeichnis schützt vor dem Ausfall von Normdaten und mach eine Edition darüber hinaus auch offline lesbar.

### Ein Beispiel aus in einem Brief von Gaston Paris:

Die **Referenz im Text** verweist auf eine interne ID, die aber auf der GND-Nummer basiert und damit eindeutig ist.

```xml
<closer facs="#facs_1_TextRegion_1701785821837_2221" xml:space="preserve">
    <signed><lb facs="#facs_1_tr_1_tl_16" n="N001"/><rs type="person" ref="gnd-118789627">GParis</rs></signed>
</closer>
```

Im von TEI-Publisher mit GND-Daten generierten **Index-Eintrag** wird auf den GND-Eintrag verlinkt.
An dieser Stelle können weitere Normdaten eingebunden werden.
Die Daten im Index-Eintrag können auf der Seite zur Person oder in einem Dropdown bei der Annotation angezeigt werden.

```xml
<person xml:id="gnd-118789627" when="2024-04-29" resp="p4de">
    <persName type="main">Paris, Gaston</persName>
    <persName type="sort">Paris, Gaston</persName>
    <gender value="M">male</gender>
    <birth>
        <date when="1839-08-09"/>
    </birth>
    <death>
        <date when="1903-03-05"/>
        <placeName ref="https://d-nb.info/gnd/4009413-3">Cannes</placeName>
    </death>
    <note type="bio">philologue et linguiste français</note>
    <occupation ref="https://d-nb.info/gnd/4199236-2">Philologe</occupation>
    <occupation ref="https://d-nb.info/gnd/4219681-4">Romanist</occupation>
</person>
```

## Mapping auf weitere Normdateien

Über VIAF lassen sich die Normdaten verschiedener Quellen aufeinander mappen.
Ein Mapping kann auf [VIAF Dataset](https://viaf.org/viaf/data/){:target="\_blank"} heruntergeladen werden.
Der GND-Nummer [118789627](https://d-nb.info/gnd/118789627){:target="\_blank"} entspricht die VIAF-ID [39382261](http://viaf.org/viaf/39382261){:target="\_blank"}, über die man wiederum zur IdRef [027058352](https://www.idref.fr/027058352){:target="\_blank"} kommt.

Die Anreicherung eines bereits mit GND-Daten angereicherten Indexes geht am einfachsten mit einem Python-Skript.
Einträge, für die keine Identifier gefunden werden, können manuell nachbearbeitet werden.

Ideen für die Sicherung der Datenqualität:

-   nicht-eindeutige Einträge (GND zu VIAF, VIAF zu GND, IdRef zu VIAF etc.) können manuell ergänzt werden.
-   Mappings mit Kurzansichten der verlinkten Einträge machen das Überprüfen einfacher
