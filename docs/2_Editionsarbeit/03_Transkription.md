# Transkription (ATR – Automatische Texterkennung)

## Was bedeutet digitales Tranksribieren?

Das Transkribieren in nicht-digitalen Editionen erfolgte nach klaren Transkriptionsregeln, denen Hilfswissenschaftler:innen oder externe Transkriptionsdienstleistungen zu folgen hatten. Demgegenüber ist der Trankskriptionsprozess von DSE durch mehr Einzelschritte und Weichenstellungen für den weiteren Projektverlauf geprägt. Namentlich sind dies die Wahl 1. des Tools und der Datenformate, 2. des Automatisierungsgrads und 3. der Workflows im eigentlichen Transkriptionsprozess (Erstellen eines eigenen Texterkennungs-Modells; Korrekturschritte, mögliche erste Annotationen). 

Es gilt freilich auch in diesen digitalen Einzelschritten wie in Print-Editionen eine konsequente Transkriptionsrichtlinie zu verfolgen, insbesondere hinsichtlich dessen, was transkribiert werden soll (bei Handschriften: alle Hände, alle Text-Eingriffe und Überarbeitungsstufen? bei Drucken: auch Paratexte wie Seitenzahlen?) und wie Digitalisat und transkribierter Text im Frontend aufeinander verweisen sein sollen (durch Einblendung, Wort- oder Zeilenkorrespondenz?). Da sich ein Zeilen-genauer Text-Bild-Verweis, der den autoptischen Vergleich vereinfacht z.B. durch Aufblinken der Textzeile im Digitalisat, zum Standard von DSE entwickelt, wird er im Folgenden auch zu den dokumentierten Standardlösungen gezählt. 

## 1. Standardlösungen für Transkriptionen

Sind die Textträger ausgewählt und digitalisiert, d.h. ist die [Textkonstitution](docs\2_Editionsarbeit\02_Textkonstitution.md) beendet, gilt es die Texte selbst maschinenlesbar zu machen. Hierfür werden die Bilddaten der Digitalisate, die z.B. im JPEG- oder TIFF-Format vorliegen, in Textdaten umgewandelt bzw. eben transkribiert. Dies kann manuell oder automatisiert geschehen (s.u.), in beiden Fällen können mittlerweile  dieselben Transkriptionstools und damit dieselben XML-Standard-Datenformate verwendet werden. 

Es ist deshalb von Vorteil sowohl für die manuelle wie die automatisierte digitale Transkription ein wissenschaftliches Tranksriptionstool und kein Textverarbeitungsprogramm wie Word zu wählen. Letzteres verwendet keinen offenen XML-Standard, erlaubt keine Text-Bild-Verweise oder macht dazu weitere Daten-Konversionen nötig. Im Folgenden protraitieren wir die verbreitetsten  wissenschaftliche Transkriptionstools (weitere Tools finden sich [hier](https://www.adfontes.uzh.ch/ressourcen/quellen-erschliessen/digitale-transkriptionstools)): 

- [Transkribus](https://app.transkribus.org/): Das Stand 2024 weitverbreitetste Transkriptionstool wird von der internationalen Genossenschaft [READ-COOP](https://readcoop.org/de) vertrieben, deren Inhaber diverse akademische Institutionen sind. Es weist einen ausgebauten Kundensupport und eine große Nutzercommunity auf. Deshalb kann das Tool auch am meisten (von Einzelprojekten erarbeitete und Transkribus zur Verfügung gestellte) Modelle zur Texterkennung anbieten. Transkribus ist jedoch ohne Bezahlung von Abonnement-Angeboten nur sehr eingeschränkt nutzbar.
- [eScriptorium](https://escriptorium.inria.fr/): Der Code dieser Tranksribus-Alternative wird kostenlos von der Université PSL in Paris zur Verfügung gestellt. Er kann lokal installiert werden, bedarf jedoch zum vollumfänglichen Betrieb eine eigene Server-Infrastruktur oder den institutionellen Zugang zu einem eScriptorium-Server, wie er zurzeit von verschiedenen Universtitäten betrieben wird (z.B. ist die eScriptorium-Instanz [fondue](https://fondue.unige.ch/) der Universität Genf an den meisten Schweizer Universitäten nutzbar). 
- [OCR4all](https://www.ocr4all.org/): Das kostenlose Transkriptionstool der Universität Würzburg benötigt wie eScriptorium die Installation auf einem lokalen Gerät oder einem eigenen Server. Es ist im Moment institutionell schlechter verankert als Transkribus und eScriptorium. Eine Besonderheit von OCR4all ist die Automatisierung nicht nur des Text-Tranksriptionsschrittes, sondern ganzer Workflows von der bis zum speichern im gewünschten Format. 
- [Transkribo](https://tcdh.uni-trier.de/de/projekt/transcribo) ist ein Angebot des Trier Center for digital Humanities der Universität Trier und Teil von dessen Forschungsplattform FuD (vergleichbar mit [Textgrid](https://textgrid.de)). Im Gegensatz zu den obigen Tools erlaubt es die Transkription auf Wort- anstatt nur auf Zeilenebene, d.h. jedes transkribierte Wort verweist durch Koordinatenangaben auf das Wort im Digitalisat. Dadurch kann mehr Genauigkeit hergestellt werden, der Prozess einer manuellen Transkription wird jedoch komplexer.  

 Den geringsten (projekteigenen) technischen Support benötigt das Tool Transkribus, weshalb im Folgenden vor allem auf die Workflows mit diesem fokussiert wird. Viele Arbeitsschritte wie  das Trainieren eines Modells sind jedoch auf andere Tools übertragbar. 
 
 Auch bezüglich Datenstandards gleichen sich die Tools: Die Transkriptionsdaten befinden sich in der Regel in einem  [XML-Format](https://www.digitale-edition.at/o:konde.215), z.B. in [PAGE-XML](https://www.digitale-edition.at/o:konde.154) oder in [ALTO-XML](https://altoxml.github.io/). Diese sind erst Vorstufen für den DSE-Datenstandard [TEI-XML](https://www.digitale-edition.at/o:konde.79), in dem die Edition letztlich lesbar gemacht wird. Zwischen dem Workflow-Schritt der Transkription in XML und der textkritischen Editionsarbeit in TEI-XML ([Annotation](docs\2_Editionsarbeit\05_critical_annotation.md) und [Kommentierung](docs\2_Editionsarbeit\06_semantic_annotation.md)) muss  deshalb noch eine [Datenkonversion](docs\2_Editionsarbeit\04_converting.md) stattfinden. 

## 2. Automatisierte oder manuelle Transkription?

Es gibt weiterhin Fälle, in denen manuelle Transkriptionen empfehlenswert sind. Dies betrifft insbesondere Editionen von Handschriften: Je schwieriger zu entziffern die Hand und je kleiner die Handschriften-Menge ist, umso weniger lohnt sich der ATR-Einsatz. Zwar existieren insbesondere für Transkribus sehr fähige allgemeine Texterkennungsmodelle , die sowohl Drucke wie Handschriften - sogar im selben Dokument - erkennen. Für **schwierige Hände** reichen diese jedoch oft nicht aus, weshalb ein Hand-spezifisches ATR-Modell tainiert werden muss (s.u.). Für das Training dieses Modells ist eine Textmenge von mindestens 75, in schwierigen Fällen sogar 200-300 Training-Seiten ('Ground Truth') nötig, bis sich der ATR-Prozess (Training und Nachkorrekturen eingerechnet) nicht mehr den manuellen Aufwand übersteigt. Erst die Transkription eines Mehrfachen der benötigten Training-Seiten rechtfertigt den Einsatz eines spezifischen ATR-Modells.  

Die Entscheidung für die Automatisation hängt also von einer Kosten-Nutzen-Rechnung ab: Das Ziel der automatischen Texterkennung ist, den Korrekturaufwand möglichst gering, aber auf jeden Fall unter dem Aufwand einer manuellen Korrektur zu halten.
Dies versucht man üblicherweise mit der schrittweisen Erweiterung der Trainingsdaten durch korrigierte Transkriptionen und dem Trainieren
neuer Texterkennungs-Modelle für den nächsten Datensatz zu erreichen. Wenn bereits geeignete Daten bestehen, können die ersten Schritte übersprungen werden.

## 3. Schritte im ATR-Prozess

Falls die Entscheidung für ATR gefallen ist, gilt es auszutesten, ob ein bereits verfügbares ATR-Modell zufriedenstellende Resultate zeitigt oder ein eigenes Modell trainiert werden soll. Die von Transkribus gepflegten Standard-Transkriptionsmodelle werden immer besser und es ist sinnvoll, einen Testdurchlauf mit diesen Modellen zu machen (wenn kein eigenes Modell angestrebt wird, kann mit Schritt 3.3 fortgefahren werden).

Falls im Projekt spezifische Transkriptionsregeln bestehen oder das Material für eine Schreiberhand viel Material hat, bringt ein spezifisches Modell gegenüber bestehenden Modellen einen Mehrwert und kann die Korrektur verkürzen.

### 3.1 Trainieren eines ATR-Modells 

Als Trainingsset für eigene Transkriptionsmodelle empfiehlt Transkribus mindestens 75 Seiten. Dies können bestehende Transkriptionen sein, die in Transkribus importiert werden oder Seiten, die mit den Standardmodellen transkribiert und anschliessend korrigiert wurden.

Das Aufbereiten bestehender Transkriptionen in Transkribus stand in der Vergangenheit die Funktion **"text2image"** zur Verfügung, die bestehende Transkriptionen zeilengenau dem Digitalisat zugeordnet hat. Gegenwärtig müssen die Zeilen-Korrespondenzen zu Trainingszwecken manuell hergestellt werden. Ein solches manuelles Einfügen von Transkriptionen in die Trainingsdaten ist nur sinnvoll, wenn der Weg über die Standardmodelle und eine Korrektur nicht möglich ist. Transkribus hat jedoch die Wiedereinführung von "text2image" Ende 2024 in Aussicht gestellt.

Für die Handschrift von Gaston Paris erwies sich das Standardmodell "The Text Titan I" als geeignet für die Anwendungen auf die Editionsdaten und eine anschliessende Korrekturrunde.


### 3.2 Re-Training

Wann sollen mit neuen Daten bessere Modelle trainiert werden? Auch diese Frage kann nur projektspezifisch beantwortet werden. Faktoren sind:

-   Qualitätsverbesserung
-   Korrekturaufwand
-   Verfügbare Zeit der Projektmitglieder
-   Zeit, die für das Trainieren gebraucht wird

### 3.3 Layoutanalyse

In der Layoutanalyse erkennt ein Algorithmus die Anordnung der Zeilen, bevor die eigentliche Texterkennung durchgeführt wird. Während ältere Versionen von Transkribus  die Layoutanalyse als eigenen, vorgängigen Schritt vor der ATR nötig gemacht haben, so ist diese Mehrstufigkeit mittlerweile optional und es kann direkt mit der Texterkennung (durch ein spezifisches oder ein allgemeines Modell) gestartet werden. Erst bei schlechten Transkriptionsresultaten, in denen Zeilen teilweise oder ganz ausgelassen wurden, ist es empfehlenswert, verschiedene Modelle und Konfigurationen zur Layoutanalyse auszutesten.

### 3.4 Korrektur der Layoutanalyse und der Transkription

Im Korrekturdurchgang empfiehlt sich zunächst eine Kontrolle der Zeilen, besonders wenn Zeilen zerstückelt erkannt wurden oder Zeilen fehlen. Sehr schlechte Resultate der Layoutanalyse rechtfertigen Test mit verschiedenen Layoutanalyse-Modellen (s.o.). 

Wenn  dies keine Verbesserung bringt, können die Zeilen auch manuell verbessert oder ganz gezogen werden. Solche Layout-Korrekturen wie das Verlängern einer Zeile verbessern einen erneuten ATR-Durchlauf und die visuelle Korrespondenz zwischen Transkription und Digitalisat im Frontend(siehe hierzu unsere [Tipps](../Themen/transkribus.md)). Eine genaue Überarbeitung der Zeilen stellt u.U. jedoch einen nicht zu rechtfertigenden Mehraufwand da, da der autoptische Vergleich durch die visuelle Einblendung der Zeilen-Korrespondenz auch ohne diese Einblendung möglich ist. 

Fehler in der Transkription können einfach in den Zeilen korrigiert werden. Falsche Zeilenregionen können ebenfalls in diesem Schritt behoben werden.

### 3.5 Annotation von Textregionen

Der letzte Schritte in Transkribus ist die Auszeichnung der Textregionen mit Funktionen. Dies stellt keine eigentliche Transkription des Textes mehr dar, sondern bereits eine erste Auszeichnung der Textform: Damit können Titel, Absätze usw. unterschieden werden. So ergeben sich bei der Konvertierung in TEI-XML nicht einfach anonyme Blöcke (`<ab>`).
Es ist empfehlenswert, sich in der Auszeichnung der Form bereits an der Nomenklatur des angestrebten TEI-XML zu orientieren. 
Die wichtigsten Elemente werden standardmässig von Skripten wie Page2TEI erkannt und in die entsprechenden Elemente überführt.
