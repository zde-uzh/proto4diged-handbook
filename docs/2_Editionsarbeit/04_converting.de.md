# 2.3 Konvertierung von PAGE nach TEI

## 1. Warum Konvertierung?

Wie bereits im Zusammenhang mit der Transkription beschrieben, sind ALTO- und PAGE-XML Standards von ATR. Sie geben ein XML Dokument pro transkribierte Seite aus, im Gegensatz zu TEI/XML, das eine unbegrenzte Anzahl von Seiten umfassen kann. TEI erlaubt, inhaltsorientierte Strukturen und mehrere Quellen in einem Dokument, PAGE bildet nur das Faksimile ab. TEI/XML ist deshalb der Editionsstandard, der es erlaubt beliebig lange Editionen zu annotieren und zu publizieren. Alle XML-Formate sind maschinenlesbar, TEI/XML zudem einfacher für Menschen zu lesen und zu manipulieren, weshalb DSE-Projekte auch die Möglichkeit haben, ihre TEI/XML Daten direkt in XML-Editoren wie [Oxygen](https://www.oxygenxml.com/){:target="\_blank"}  aufzubereiten. Auch in letzterem Fall ist eine Konversion nötig.

## 2. Standard-Konvertierungsmöglichkeiten

### Transkribus (Exports)

Transkribus bietet eine Vielzahl an Exportmöglichkeiten (PDF, Textfile, Docx, Excel/CSV, PAGE-XML, ALTO-XML, TEI/XML); nur die drei letztgenannten lassen sich jedoch für die Entwicklung einer DSE nach heutigen Standards weiterverwenden. Während PAGE-XML und ALTO-XML selbst noch in ein TEI/XML umgewandelt werden müssen, entspricht das durch einen Transkribus Export zur Verfügung gestellte TEI/XML leider noch nicht der angestrebten Qualität. Wenn in Transkribus viele eigene Tags vergeben wurden, muss das der Export deshalb noch überarbeitet werden.


### eScriptorium (PAGE, ALTO)

eScriptorium hat zurzeit zwei Exportmöglichkeiten: PAGE-XML und ALTO-XML.

### Vorhandene Scripts (trans2tei, page2tei)

Weil Exporte im TEI XML Format in den verbreiteten Transkriptionstools entweder fehlen oder unzureichend sind, wurde in den letzten Jahren Code-Scripts entwickelt um die Konversion nicht manuell durchzuführen (z.B. in einem XML Editor wie Oxygen. Die beiden hier vorgestellt Scripts automatisieren  die Konversion. 

Grundlegend ist [**page2tei**](https://github.com/dariok/page2tei), das PAGE-XML in TEI/XML umwandelt.
Das grösste Hindernis bei page2tei ist ein TODO bei Tags der Zeilen. Sobald das gelöst ist, kann die eigene Konvertierung als folgender Schritt gemacht werden (Kaskade). Andere editionsspezifische Tags werden in anonyme Blöcke (Tag ab) mit Type-Attribut gesetzt, was bestens weiterverarbeitet werden kann.

[**trans2tei**](https://github.com/biblhertz/trans2tei){:target="\_blank"} ist spezifisch auf die PAGE XMLAusgabe aus Transkribus zugeschnitten. Esbeinhaltet alle Schritte vom Export-Zip bis zum TEI-XML und deckt auch die Erkennungen von gedruckten Hervorhebungen mittels Sonderzeichen ab.
trans2tei zielt auf die Bedürfnisse der Bibliotheca Herziana ab. Für Editionsprojekte ist es am besten einfach eine Inspiration.

=> Hier erschient später das Script proto2tei, das auf die Showcase-Edition zugeschnitten ist. 

## 3. Limitationen

Wenn kein oder nur ein minimales Tag-Set vorliegt, benötigt der TEI-XML Export von Transkribus kaum Nachjustierung. In diesem Fall fällt jedoch eine wichtige Funktion des Tools weg: Die Annotation von Text oder Textregionen.

Noch gravierender ist, dass die **Verknüpfung zur Handschrift**, die mittlerweile zum Standard von vielen DSE gehört, fehlt, da auch die Koordinaten in diesem Fall wegfallen. 

Als Lösung dieses Problems können **manuelle Nachjustierungen** durchgeführt werden, um die Übereinstimmung mit dem angestrebten TEI-Schema zu erreichen. Solche manuelle Überarbeitungen können je nach Komplexität des Schemas jedoch aufwändig werden.

Letztlich können bei genügendem technischem Fachwissen projektspezifische Konvertierungen mithilfe von Pipelines wie [trans2tei](https://github.com/biblhertz/trans2tei){:target="\_blank"}  entwickelt werden.
Basis davon ist [page2tei](https://github.com/dariok/page2tei){:target="\_blank"}, das bereits bei der Exportfunktion von Transkribus zur Verfügung steht.


Edit 30.9.24. Anregung Peter Dängeli: Python-page-to-tei von Ismail Ziegler Prada: https://github.com/raykyn/page2tei/ (oder habt ihr das absichtlich nicht mit drin?)