# Statische Präsentation

Digitale Editionen im Web werden meistens von einer Datenbank gespeist. Die Datenbank kann eine XML-Datenbank wie eXist-db oder eine relationale Datenbank sein.
Die Schnittstellen und Indices der Datenbanken erlauben performante Suchfunktionen in den Beständen der Edition und die Daten können jederzeit über interne Zugänge bearbeitet werden.

Für Editionen in ihrer aktiven Phase ist ein Server mit genügend Arbeitsspeicher kein grosses Hindernis und die Wartung kann gemeinsam mit der Entwicklung gemacht werden.
Nach Projektende fehlen die Mittel für die Infrastruktur und die Pflege und die digitalen Editionen drohen vom Web zu verschwinden.
Statische oder dateibasierte Webseiten sind eine Lösung für dieses Problem. Statt einer ad-hoc-Konvertierung durch die Datenbank werden die Daten einmalig in ein Format konvertiert, das vom Browser verarbeitet werden kann. Das Hosting reduziert sich auf das Lagern und Ausliefern der Dateien für den Browser.

Durch die Konvertierung verlieren die Daten den Grossteil ihrer Semantik und müssen separat für die Wiederverwendung [archiviert](03_archiving_data.de.md) werden.
Das Abweichen vom Single-Source-Prinzip hat zur Folge, dass bei Änderungen in den Daten entweder die Inhalte neu konvertiert werden müssen oder manuell alle betroffenen Stellen bearbeitet werden müssen.

Ein Verzicht auf eine Datenbankanbindung heisst nicht, dass keine dynamischen Darstellungen möglich sind, lediglich, dass die Operationen im Browser mittels JavaScript ausgeführt werden müssen. Wie stark die verschiedenen Ansätze von JavaScript abhängig sind, wird in diesem Kapitel beschrieben.

## HTML-basierte Seiten

Die radikalste Umsetzung ist eine Konvertierung der TEI-Daten in HTML, wobei Inhalt und Form nicht mehr getrennt werden.

Vorteile:

-   Langlebigkeit von HTML
-   offline benutzbar

Nachteile:

-   Verschiedene Ansichten müssen separat konvertiert und über verschiedene Pfade eingebunden werden.
-   Keine Suchfunktion ohne JavaScript oder externe Anbieter wie Suchmaschinen
-   Neuentwicklung von Grund auf

## JSON-basierte Seiten

Weniger radikal ist die Nutzung von JSON-Dateien mit dem Inhalt äquivalent zu den Daten von der Datenbankschnittstelle. HTML wird nur als Format für die einzelnen Properties verwendet.

Vorteile:

-   Umbau bestehender Seiten ist möglich
-   Dynamische Features lassen sich gut nachbilden

Nachteile:

-   Schnelllebigkeit von JavaScript-Libraries
-   auch offline nur mit einem HTTP-Server nutzbar
-   Suchfunktionen müssen im Browser ausgeführt werden. Dafür müssen Indexdaten für den ganzen Datenbestand geladen werden.

## Hybride Ansätze

Zwischen diesen Polen gibt es verschiedene Abstufungen. Mit JavaScript kann bei HTML-basierten Ansätzen auch die Ansicht geändert werden (beispielsweise via Manipulation der CSS-Klassen) oder einzelne Seiten können dynamisch umgesetzt werden, wie zum Beispiel eine Suche.
