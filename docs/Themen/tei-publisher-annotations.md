# Annotationen mit TEI-Publisher

## Dateien, die für einen neuen Annotationstyp angepasst werden müssen (am Beispiel `person`)

-   `resources/odd/annotations.odd`: Markierung der Annotationen im Annotationsviewer
    -   Model für die Annotation im Text ergänzen:
        -   Model für den Elementnamen (`persName`)
        -   CSS-Klassen: `annotation` (Annotationsmöglichkeit), `annotation-person` (Unterscheidung), `authority` (bei Verlinkung mit Index)
    -   (bei Verlinkung) Zweites Model für die Anzeige des Indexeintrags (`person`) im Dropdown erstellen
-   `templates/pages/annotate.html`: Layout des Annotationsviewers
    -   Button im Menü hinzufügen: Wichtig sind die Attribute `data-type` für die Funktionalität und `icon` für die Abbildung.
    -   Formular für Attribute in der Annotation: Eintrag in `iron-form#edit-form`
    -   (Bei Verlinkung) Falls ein Formular für den Index-Eintrag verwendet wird: `<authority-forms>person</authority-forms>` (?)
    -   (Bei Verlinkung) Bei verschiedenen Keys (`@ref`, `@corresp`) können diese bei `pb-view-annotate` im Attribut `key-map` genauer definiert werden.
-   `modules/annotation-config.xqm`: Konfiguration des Annotationstyps
    -   `anno:entity-type`: Typ vom Element ableiten (?)
    -   `anno:annotations`: Format des Elements, das in den Text gesetzt wird
    -   `anno:occurrences`: (bei Verlinkung) Selektor für obiges Format für die Anzahl bestehender Annotationen

Nur für verlinkte Annotationen zusätzlich

-   `collection.xconf`: Indexierung des Eintrags im Index für den Lookup bereits erfasster Einträge
-   `modules/registers.xql`:
    -   `rapi:insert-point`: Wo ein Eintrag gespeichert wird
    -   `rapi:prepare-record`: Bei Verwendung eines Templates
    -   `rapi:next`: Bei Verwendung eines Templates
    -   `rapi:query`: Laden von Properties für Annotationen
    -   `rapi:create-record`: Format des Indexeintrags
    -   `rapi:local-search-strings` (optional?): alternative Names

Bei Verwendung eines Formulars für den Index-Eintrag zusätzlich

-   `template/pages/annotation/person-editor.html`: (?)
-   `data/registers/persons.xml`: Clear examples, move, ...
-   `data/registers/templates/person-template.xml`: (?)
-   `data/registers/templates/person-default.xml`: (?)

Nur bei Verwendung von SpaCy

-   `modules/nlp-config.xqm` bei Verwendung von SpaCy
    -   Mapping zwischen Key von SpaCy und TEI-Element
