# Konvertierung von PAGE nach TEI

## 1. Warum Konvertierung?

Wie bereits im Zusammenhang der Transkription beschriebenn, sind ALTO- und PAGE-XML Standards von ATR. Sie geben ein XML Dokument pro transkribierte Seit aus, im Gegensatz zu TEI-XML, das eine unbegrenzte Anzahl von Seiten umfassen kann. TEI-XML ist deshalb der Editionsstandard, der es erlaubt beliebig lange Edition zu annotieren und zu publizieren. Alle XML-Formate sind maschinenlesbar, TEI-XML zudem einfacher für Menschen zu lesen und zu manipulieren, weshalb DSE-Projekte auch die Möglichkeit haben, ihre TEI-XML Daten direkt in XML-Editoren wie [Oxygen](https://www.oxygenxml.com/) aufzubereiten. Auch in letzterem Fall ist eine Konversion nötig. 

## 2. Standard-Konvertierungsmöglichkeiten

### Transkribus (Exports)
Transkribus bietet eine Vielzahl Exportmöglichkeiten (PDF, Textfile, Docx, Excel/CSV, PAGE-XML, ALTO-XML, TEI-XML); nur die drei letztgenannten lassen sich jedoch für die Entwicklung einer DSE nach heutigen Standards weiterverwenden. Während PAGE-XML und ALTO-XML selbst noch in ein TEI-XML umgewandelt werden müssen, entspricht das durch einen Transkribus Export zur Verfügung gestellte TEI-XML leider noch nicht der angestrebten Qualität, wenn in Transkribus viele Tags vergeben wurden, und muss deshalb selbst noch überarbeitet werden.
=> @Reto: Könntest Du hier bitte ergänzen, warum der TEI-XML Export (auch derjenige mit trans2tei) aus technischer Sicht nicht zufriedenstellend ist?

### eScriptorium (PAGE, ALTO)


### Vorhandene Scripts (trans2tei, page2tei)

## 3. Limitationen

Wenn kein oder nur ein minimalstes Tag-Set vorliegt, benötigt der TEI-XML Export in Transkribus kaum Nachjustierung. In diesem Fall fällt jedoch eine wichtige Funktion des Tools weg: Die Annotation von Text oder Textregionen. 

Noch gravierender ist, dass die **Verknüpfung zur Handschrift**, die mittlerweile zum Standard von vielen DSE gehört, fehlt, da auch die Koordinaten in diesem Fall wegfallen. Ob das sinnvoll ist, kann mit einem anfänglichen Mock-Up hergeleitet werden.
=> @Reto: Ist es korrekt, dass die Koordinaten wegfallen müssen? Ich ging bislang davon aus, dass Koordinaten und Tags völlig unabhängig voneinander sind und Koordinaten in einem minimal ausgezeichneten TEI-XML kein Problem darstellen.

Als Lösung dieses Problems können **manuelle Nachjustierungen** durchgeführt werden, umn die Übereinstimmung mit dem angestrebten TEI-Schema zu erreichen. Solche manuelle Überarbeitungen können je nach Komplexität des Schemas jedoch aufwändig werden. 

Letztlich können bei genügendem technischem Fachwissen projektspezifische Konvertierungen mithilfe von Pipelines wie [trans2tei](https://github.com/biblhertz/trans2tei) entwickelt werden.
Basis davon ist [page2tei](https://github.com/dariok/page2tei), das bereits bei der Exportfunktion von Transkribus zur Verfügung steht.
=> @Reto: Was sind die projektspezifischen Vorteile von trans2tei? 
