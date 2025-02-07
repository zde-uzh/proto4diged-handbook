# Barrierefreiheit im Web

Mit der Transkription von historischen Dokumenten leisten Editionsprojekte einen Beitrag zum barrierearmen Zugang zum historischen Erbe, der nicht durch eine nicht-navigierbare Plattform verloren gehen darf.
Die englische Entsprechung "Accessibility" wird im Bereich von Forschungsdaten oft im Kontext der FAIR-Prinzipien verstanden, während die Abkürzung "a11y" sich ausschliesslich auf die Barrierefreiheit bezieht.

Die Barrierefreiheit einer digitalen Edition beginnt bereits bei den Daten und zieht sich über die Konzeption der Plattform bis zur Umsetzung.

## Überlegungen beim Erarbeiten der Editionsdaten

-   Wahl der Sprache(n)
-   Alternativtexte für Bilder
-   Semantisches oder nicht-semantisches Markup (`<strong>` oder `<span style="font-weight: bold;">`)
-   Semantisches Markup statt einfacher Text (`<app><lem wit="#h">frey</lem><rdg wit="#V">frei</rdg></app>` statt `frey ] h; frei V`)
-   Orientierung der Struktur am Dokument (Seiten und Zeilen) oder am Inhalt (Kapitel und Absätze)

## Besondere Herausforderungen bei Texten in digitalen Editionen

-   Index-Annotationen:

    -   Viele Links in einem Text können störend wirken. Dropdowns verdienen besondere Aufmerksamkeit beim Überprüfen nach Barrieren.
    -   Eine Alternative bzw. Ergänzung zu Dropdowns ist eine Liste der Relevanten Einträge pro Dokument.

-   Fussnoten und Kommentare:

    -   Fussnoten sind nur mit ihrem Kontext verständlich. Bei der Anzeige in einer separaten Liste müssen sie beidseitig verlinkt sein (wie bei TEI-Publisher).
    -   Fussnoten im Dropdown haben den Kontext aber die gleichen Probleme wie bei Index-Annotationen.
    -   Editorische Kommentare mit einem Lemma sind auch ohne Primärtext verständlich.

-   Unterstreichungen, Additionen, Streichungen, Hochstellungen

    -   Vermeidung von Interpretation von Markup und blosse visuelle Nachbildung kann dieses unsichtbar machen.

-   Parallele Texte

    -   Je nach Intention der Edition und Länge der parallelen Texte sind Tabellen oder Kapitel geeignet.

-   Konkurrierende Hierarchien: Darstellung in der digitalen Edition vs. Struktur des Originaldokuments

## Herausforderungen in der Navigation in digitalen Editionen

-   Paginierung bei längeren Dokumenten:

    -   Jede Ansicht ist ein Dokument und braucht einen eigenen Titel zur Identifikation.
    -   Der Wechsel zwischen Ansichten macht die Navigation undurchsichtig.

-   Informationsgehalt pro Bildschirm

## Links

-   [Web Content Accessibility Guidelines (WCAG) 2.1](https://www.w3.org/TR/WCAG21/){:target="\_blank"} mit international gültige Empfehlungen von W3C
-   [eCH-0059 Accessibility Standard](https://www.ech.ch/de/ech/ech-0059/3.0){:target="\_blank"} für Gemeinwesen und konzessionierte Unternehmen in der Schweiz
-   [Accessibility im CMS der Universität Zürich](https://t.uzh.ch/access){:target="\_blank"} mit diversen Links zu Anleitungen und Werkzeugen
-   [Handreichungen des Zentrums für Digitale Editionen ZDE Zürich](https://www.zde.uzh.ch/de/offers/handout.html)
