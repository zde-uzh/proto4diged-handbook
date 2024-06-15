# Barrierefreiheit im Web

Mit der Transkription von historischen Dokumenten leisten Editionsprojekte einen Beitrag zur Barrierefreiheit zum historischen Erbe, der nicht durch eine nicht-navigierbare Plattform verloren gehen darf.
Die englische Entsprechung "Accessibility" wird im Bereich von Forschungsdaten oft im Kontext der FAIR-Prinzipien verstanden, während die Abkürzung "a11y" sich ausschliesslich auf die Barrierefreiheit bezieht.

Die Barrierefreiheit einer digitalen Edition beginnt bereits bei den Daten und zieht sich über die Konzeption der Plattform bis zur Umsetzung.

## Überlegungen beim Erarbeiten der Editionsdaten

-   Wahl der Sprache(n)
-   Alternativtexte für Bilder
-   Semantisches oder nicht-semantisches Markup (`<strong>` oder `<span style="font-weight: bold;">`)
-   Semantsiches Markup statt einfacher Text (`<app><lem wit="#h">froh</lem><rdg wit="#V">frei</rdg></app>` statt `froh ] h; frei V`)
-   Orientierung der Struktur am Dokument (Seiten und Zeilen) oder am Inhalt (Kapitel und Absätze)

## Besondere Herausforderungen bei Texten in digitalen Editionen

-   Index-Annotationen:

    -   Viele Links in einem Text können störend wirken. Dropdowns verdienen besondere Aufmerksamkeit beim Überprüfen nach Barrieren.
    -   Eine Alternative bzw. Ergänzung zu Dropdowns ist eine Liste der Relevanten Einträge pro Dokument.

-   Fussnoten und Kommentare:

    -   Fussnoten sind nur mit ihrem Kontext verständlich. Bei der Anzeige in einer separaten Liste müssen sie beidseitig verlinkt sein (wie bei TEI-Publisher).
    -   Fussnoten im Dropdown haben den Kontext aber die oben beschriebenen Probleme.
    -   Editorische Kommentare mit einem Lemma sind auch ohne Primärtext verständlich.

-   Unterstreichungen, Additionen, Streichungen, Hochstellungen ...
-   Parallele Texte ...
-   Konkurrierende Hierarchien: Darstellung in der digitalen Edition vs. Struktur des Originaldokuments

## Herausforderungen in der Navigation in digitalen Editionen

-   Paginierung bei längeren Dokumenten:

    -   Jede Ansicht ist ein Dokument und braucht einen eigenen Titel zur Identifikation.
    -   Der Wechsel zwischen Ansichten macht die Navigation undurchsichtig.

-   Informationsgehalt pro Bildschirm

## Links

-   [Accessibility im CMS der Universität Zürich](https://t.uzh.ch/access) mit diversen Links zu Anleitungen und Werkzeugen
