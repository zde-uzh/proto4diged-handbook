# Konvertierung von PAGE nach TEI

1. Warum Konvertierung?

PAGE XML ist ein Standard von ATR, der ein XML Dokument pro transkribierte Seit ausgibt, TEI XML ein Editionsstandard, der es erlaubt beliebig viele Seiten in einer Edition zu annotieren und auszugeben. Beide sind maschinenlesbar, TEI XML zudem einfacher auch für Menschen zu lesen und zu manipulieren.

2. Standard-Konvertierungsmöglichkeiten

    - mit Transkribus (Exports)
    - mit eScriptorium (PAGE, ALTO)
    - mit vorhandenen Scripts (trans2tei, page2tei)

3. Limitationen

Kein/Minimalstes Tag-Set: benötigt kaum Nachjustierung.
Dann jedoch keine Layout-Analyse vorbereitet, Verknüpfung zur Handschrift fehlt: keine Koordinaten. Ob das sinnvoll ist, kann mit einem anfänglichen Mock-Up hergeleitet werden.

Manuell ansonsten Nachjustierungen: Nachkonvertierung für Übereinstimmung des TEI-Schemas.

Für projektspezifische Konvertierungen können Pipelines wie bei [trans2tei](https://github.com/biblhertz/trans2tei) entwickelt werden.
Basis davon ist [page2tei](https://github.com/dariok/page2tei), das bereits bei der Exportfunktion von Transkribus zur Verfügung steht.
