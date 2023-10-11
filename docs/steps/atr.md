# ATR – Automatische Texterkennung

Das Ziel bei der automatischen Texterkennung ist, den Korrekturaufwand möglichst gering, aber auf jeden Fall unter dem Aufwand einer
manuellen Korrektur zu halten.
Dies versucht man üblicherweise mit der schrittweisen Erweiterung der Trainingsdaten durch korrigierte Transkriptionen und dem Trainieren
neuer Modelle für den nächsten Datensatz zu erreichen.

Wenn bereits geeignete Daten bestehen, können die ersten Schritte übersprungen werden.

## Trainingsdaten

Für ein Transkriptionsmodell sind nur die Zeilen relevant.
Komplexe Anordnungen von Zeilen können zwar für Trainingsdaten verwendet werden, der Mehraufwand bringt aber keine Vorteile.

Transkribus empfiehlt Trainingsdaten im Umfang von mindestens 75 Seiten.

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

# Korrektur der Transkription

Fehler in der Transkription können ganz einfach in den Zeilen gemacht werden.

Falsche Zeilenregionen können ebenfalls in diesem Schritt behoben werden.
