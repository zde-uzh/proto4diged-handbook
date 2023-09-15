# ATR – Automatische Texterkennung

Das Ziel bei der automatischen Texterkennung ist, den Korrekturaufwand möglichst gering, aber auf jeden Fall unter dem Aufwand einer
manuellen Korrektur zu halten.
Dies versucht man üblicherweise mit der schrittweisen Erweiterung der Trainingsdaten durch korrigierte Transkriptionen und dem Trainieren
neuer Modelle für den nächsten Datensatz zu erreichen.

Wenn bereits geeignete Daten bestehen, können die ersten Schritte übersprungen werden.

## Trainingsdaten

Für ein Transkriptionsmodell sind nur die Zeilen relevant.
Komplexe Anordnungen von Zeilen können zwar für Trainingsdaten verwendet werden, der Mehraufwand bringt aber keine Vorteile.
