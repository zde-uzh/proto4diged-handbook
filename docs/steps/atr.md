# ATR – Automatische Texterkennung

Das Ziel bei der automatischen Texterkennung ist, den Korrekturaufwand möglichst gering, aber auf jeden Fall unter dem Aufwand einer
manuellen Korrektur zu halten.
Dies versucht man üblicherweise mit der schrittweisen Erweiterung der Trainingsdaten durch korrigierte Transkriptionen und dem Trainieren
neuer Modelle für den nächsten Datensatz zu erreichen.

Wenn bereits geeignete Daten bestehen, können die ersten Schritte übersprungen werden.

## Trainingsdaten

Es besteht die Möglichkeit, projektspezifische Modelle zu trainieren.
Die von Transkribus gepflegten Standard-Transkriptionsmodelle werden allerdings immer besser und es ist am besten, vor allen Entscheidungen einen Testdurchlauf mit diesen Modellen zu machen.
Wenn im Projekt spezifische Transkriptionsregeln bestehen oder das Material für eine Schreiberhand viel Material hat, kann ein spezifisches Modell natürlich einen Mehrwert bringen.

Als Trainingsset für Transkriptionsmodelle empfiehlt Transkribus mindestens 75 Seiten.
Dies können bestehende Transkriptionen sein, die in Transkribus importiert werden oder Seiten, die mit den Standardmodellen transkribiert und anschliessend korrigiert wurden.

Das Aufbereiten bestehender Transkriptionen ging in der Vergangenheit mit der Funktion "text2image". Gegenwärtig ist der ideale Weg unklar.
Für die Handschrift von Gaston Paris erwies sich das Standardmodell "The Text Titan I" als geeignet für die Anwendungen auf die Editionsdaten und eine anschliessende Korrekturrunde.
Ab 75 Seiten korrigierten Materials können eigene Modelle darauf trainiert und die Qualität mit dem Standardmodell verglichen werden.

Ein manuelles Einfügen von Transkriptionen in die Trainingsdaten ist nur sinnvoll, wenn der Weg über die Standardmodelle und eine Korrektur nicht möglich ist.

Für ein Transkriptionsmodell sind nur die Zeilen relevant.
Komplexe Anordnungen von Zeilen können zwar für Trainingsdaten verwendet werden, der Mehraufwand bringt aber keine Vorteile.

## Re-Training

Wann wollen wir mit neuen Daten bessere Modelle trainieren?

Faktoren sind:

- Qualitätsverbesserung
- Korrekturaufwand
- Verfügbare Zeit der Projektmitglieder
- Zeit, die für das Trainieren gebraucht wird

## Layoutanalyse

Für die Trainingsdaten scheint die Layoutanalyse "Transkribus LA" die Zeilen am besten zu erkennen.
Im Client ist diese als Vorauswahl zu finden. Stand September 2023 scheint es nicht möglich, über die Webversion diese Layoutanalyse auszuwählen.

In der Webversion muss die Layoutanalyse vor der Handschriftenerkennung nicht gesondert angesteuert werden.
Im Client dagegen ist eine der Fallen, dass man Seiten ohne Textregionen analysiert und damit auch keine Transkriptionen bekommt.

## Korrektur der Layoutanalyse

Nach der Layoutanalyse empfiehlt sich eine Kontrolle der Zeilen, besonders wenn Zeilen zerstückelt erkannt wurden oder Zeilen fehlen.
Mehr zur [Korrektur](../topics/transkribus.md).

Einzelne Korrekturen wie das Verlängern einer Zeile können auch hier vorgenommen werden.
Auf eine komplette Überarbeitung der Zeilen sollte verzichtet werden.

## Handschriftenerkennung

Bei der Handschriftenerkennung triagiert Transkribus mit einer Warteliste.
Es ist nicht gewährleistet, dass man direkt nach dem Auftrag weiterarbeiten kann.
Bezahlte Credits führen jedoch zu einer Bevorzugung.

## Korrektur der Transkription

Fehler in der Transkription können ganz einfach in den Zeilen gemacht werden.

Falsche Zeilenregionen können ebenfalls in diesem Schritt behoben werden.

## Annotation von Textregionen

Einer der letzten Schritte in Transkribus ist die Auszeichnung der Textregionen mit Funktionen.
Damit können Titel, Absätze usw. unterschieden werden und ergeben sich bei der Konvertierung nicht einfach anonyme Blöcke (`<ab>`).
Die wichtigsten Elemente werden standardmässig von Skripten wie Page2TEI erkannt und in die entsprechenden Elemente überführt.
