# 2.2 Transkription, ATR und Annotation

## Was bedeutet digitales Transkribieren?

Das Transkribieren in nicht-digitalen Editionen erfolgte nach Transkriptionsregeln, denen Hilfswissenschaftler:innen oder externe Transkriptionsdienstleistungen zu folgen hatten. Demgegenüber ist der Trankskriptionsprozess in DSE durch mehr Einzelschritte und Weichenstellungen für den weiteren Projektverlauf geprägt. Namentlich sind dies, wie im Folgenden beschrieben, die Wahl

1. des Tools und der Datenformate;
2. des Automatisierungsgrads;
3. der Workflows im eigentlichen Transkriptionsprozess (Erstellen eines eigenen Texterkennungs-Modells; Korrekturschritte; mögliche erste Annotationen).

Zum Schluss wird das vorliegende Handbuch-Kapitel auf die Limitationen der verfügbaren Standard-Lösungen zur Transkription eingehen.

#### Transkriptionsrichtlinien

Wie in Print-Editionen gilt es auch für DSE konsequente **Transkriptionsrichtlinien** zu verfolgen, insbesondere hinsichtlich **Transkriptionsumfang** und **diplomatischer Umschrift**, d.h. Deckungsgrad der Abschrift mit dem Original bezüglich sprachlicher und formaler Eigenheiten: Bei Handschriften muss die Frage beantwortet werden, welche Hände, (Sonder-)Zeichen, Text-Eingriffe und Überarbeitungsstufen wie transkribiert werden. Bei Drucken stellt sich zudem die Frage nach druckspezifischen Paratexten wie Seitenzahlen oder Schmutztitel. Das Auszeichnen dieser formalen textualen Aspekte bezeichnet man auch als **textkritische Annotation**, sie kann je nach Tool (s.u.) zusammen mit der Transkription oder erst später zusammen mit der [_inhaltlichen Annotation_](05_semantic_annotation.de.md) erfolgen.

!!! abstract "Showcase-Editionsrichtlinien: Tranksription und textkritische Annotation"

    Die Showcase-Edition versteht sich als hypothetische Vorarbeit zu einer wesentlich größeren Edition der Korrespondenz von Gaston Paris, die ca. 27.000 Seiten umfasst und sich - falls in späteren Projekten umgesetzt - primär an ein **Forschungspublikum** wendet. Da die entwickelten prototypischen Workflows einerseits wissenschaftliche Standards diplomatischer Editionen erfüllen sollen und andererseits im Umfang skalierbar bleiben müssen, konzentriert sie sich auf **größtmögliche Texttreue bei gleichzeitiger Einfachheit textkritischer und inhaltlicher Auszeichnung**.

    Bei der Transkription hielt sich die Showcase-Edition an folgende **textkritische Grundsätze**:

    **Umfang**

    - **Alle Hände**, d.h. alle unterschiedlichen Handschriften, werden transkribiert.
        - Hinzufügungen durch **fremde Hände**, d.h. die in den Brief-Metadaten nicht als Urheberhand ausgewiesen sind, werden als solche durch eine texktritische Annotation (s.u., 3.5) kenntlich gemacht.=> Hier Beispiel aus der Showcase-Edition verlinken.
        - Ausnahme: Fremde Hände werden nicht transkribiert, wenn sie Hinzufügungen von **Archiv-Signaturen oder Archiv-Paginierungen** betreffen. Archiv-Signaturen sind stattdessen in den Metadaten enthalten. 

    - Die Frage nach **textgenetischen Reihenfolgen** (welche Hand welchem Zeitpunkt zugeordnet werden kann) wird nicht während der Transkription durch Sonderzeichen oder Annotationen beantwortet, da die Briefe Gaston Paris' textgenetisch weitgehend 'flach' sind (d.h. kaum eigene oder fremde Überarbeitungsspuren aufweisen). Wo textgenetische Zusammenhänge dargestellt werden müssen, geschieht dies in [_Kommentaren_](06_commenting.de.md).

    - **Vordrucke** (z.B. Briefköpfe von Hotels oder Privatpersonen) auf dem Briefpapier werden in der Regel transkribiert und  als 'Vordrucke' ebenfalls textkritisch annotiert. => Hier Beispiel aus der Showcase-Edition verlinken.
        - Ausnahme 1: Vorgedruckte **Formularzeilen von Postkarten** ('Nom:', 'Prenom:', etc.) werden nicht transkribiert, da sie allen Postkarten eigen sind.
        - Ausnahme 2: **Postkartenstempel oder Briefmarken** werden nicht transkribiert. Die darin enthaltenen Orts- und Datumsangaben können, falls sie von der Datumslinie des Briefes abweisen, in den Metadaten festgehalten werden. Es gibt jedoch Editionen, die sich zwecks Durchsuchbarkeit der Stempel für deren Auszeichnung entschieden haben, z.B. die [Gotthelf-Ausgabe](=> bei Erscheinen hier Link ergänzen).

    **Diplomatische Umschrift**

    - Sonderzeichen, die Gaston Paris insbesondere aus wissenschaftlichen Gründen benutzt oder Fremdsprachen entlehnt, werden stillschweigend verwendet und nicht ausdrücklich in einem textkritischen Apparat aufgeführt. Ihr Verständnis durch das Fachpublikum wird vorausgesetzt.

    - Fehler im Ursprungsmanuskript werden ohne zusätzliche Kennzeichnung übernommen. Die Überprüfung des Fehlers ist durch den Vergleich mit der daneben eingeblendeten Handschrift einfach möglich.

    - Unterstreichungen, auch doppelte und dreifache, sowie Hochstellungen werden als solche transkribiert.

    - Einkreisungen von Wörtern oder Buchstaben werden durch Einkreisungen wiedergegeben. 

    - Auf eine Umwandlung in Sperrung oder Fettdruck wird verzichtet, um die oftmals wissenschaftlich motivierte Hervorhebung von Lemmata zu erhalten.

    - Der französische Leerschlag vor Doppelpunkten, Semikolon und Ausrufezeichen wird stillschweigend in der Transkription angewendet. Dieser letzte Punkt weicht von einer strengen diplomatischen Umschrift ab und orientiert sich an der französischen Druck-Konventionen.

#### Lesefassung

Ein Schritt, der technisch mit der textkritischen und/oder inhaltlichen Annotation zusammenfällt, aber nichts Sichtbares oder Inhaltliches auszeichnet, ist das Erstellen der **Lesefassung**, die der texttreueren diplomatischen Umschrift zur Seite gestellt ist (siehe dazu auch [_Editionsansichten_](../3_presentation/03_edition_views.de.md)). Damit der Text in einer Lesefassung normalisiert dargestellt werden kann, müssen im Falle von fehlerhaften oder veralteten Schreibweisen die Worte mit einer korrekten bzw. modernisierten Wortvariante annotiert werden - was hierbei als fehlerhaft bzw. veraltet verstanden wird, muss im Detail [_dokumentiert_](../3_presentation\05_documentation.de.md) werden. 

!!! abstract "Showcase-Editionsrichtlinien: Lesefassung"
    Da sich die Showcase-Edition der Briefe Gaston Paris' primär an ein wissenschaftliches Publikum richtet, wird von der Einrichtung einer Lesefassung während der inhaltichen Annotation abgesehen. Eine solche ist jedoch auch nachträglich machbar, da die TEI/XML-Daten auch zu späteren Zeitpunkten mit unterschiedlichen Tools angereichert werden können.

#### Verknüpfung Digitalisat und Transkription

DSE-spezifische Transkriptionsrichtlinien betreffen die **Verknüpfung von Digitalisat und Transkription** im Frontend, d.h. die Einblendung von visuellen Wort- oder Zeilenkorrespondenzen zwischen Faksimile und Text. Diese wird idealerweise bereits im Schritt der Transkription vorbereitet, alle unten erwähnten Tools weisen einfache Formen dieser Verknüpfung auf, in dem sie die XML-Datei der Transkription mit Bild-Koordinaten anreichern. Der zeilengenaue Text-Bild-Verweis, der den autoptischen Vergleich vereinfacht, z.B. durch Aufblinken der Textzeile im Digitalisat, hat sich zum Standard von DSE entwickelt, und wird im Folgenden zu den dokumentierten Standardlösungen gezählt.

!!! success "Best Practice"
    Vorbildhaft für die Verknüpfung von Digitalisat und Transkription für DSE, die den TEI-Publisher verwenden, ist die [Briefedition Alfred Escher](https://www.briefedition.alfred-escher.ch/home.html){:target="\_blank"} .

    Die Showcase-Edition hat sich an dieser Form der Zeilen-Korrespondenz orientiert und den hierfür vorhandenen [Quellcode der Briefedition Alfred Escher](https://github.com/stazh/briefedition-escher){:target="\_blank"}  nachgenutzt.
    <figure markdown="span">

    ![screenshot Escher](image-3.png){ width="1000" }
    <figcaption>Jung Joseph (Hrsg.), Digitale Briefedition Alfred Escher, Relaunch Januar 2022, Zürich. Abgerufen am 22.9.2024. [https://briefedition.alfred-escher.ch/briefe/B0056](https://briefedition.alfred-escher.ch/briefe/B0056?view1=1){:target="\_blank"} </figure>


## 1. Standardlösungen für Transkriptionen

Sind die Textträger ausgewählt und digitalisiert, d.h. ist die [_Textkonstitution_](02_Textkonstitution.de.md) beendet, gilt es die Texte selbst maschinenlesbar zu machen. Hierfür werden die Bilddaten der Digitalisate, die z.B. im JPEG- oder TIFF-Format vorliegen, in Textdaten umgewandelt bzw. eben transkribiert. Dies kann manuell oder automatisiert geschehen (s.u.), in beiden Fällen können mittlerweile dieselben Transkriptionstools und damit dieselben XML-Standard-Datenformate verwendet werden.

Es ist deshalb von Vorteil sowohl für die manuelle wie die automatisierte digitale Transkription ein wissenschaftliches Tranksriptionstool und kein Textverarbeitungsprogramm wie Word zu wählen. Letzteres verwendet keinen offenen XML-Standard, erlaubt keine Verknüpfung von Transkription und Digitalisat durch Koordinaten im XML oder macht dazu weitere Daten-Konversionen nötig.

Im Folgenden portraitieren wir die verbreitetsten wissenschaftlichen Transkriptionstools (eine Liste weiterer Tools finden sich [hier](https://www.adfontes.uzh.ch/ressourcen/quellen-erschliessen/digitale-transkriptionstools){:target="\_blank"} ):

-   [Transkribus](https://app.transkribus.org/){:target="\_blank"} : Das Stand 2024 **weitverbreitetste Transkriptionstool** wird von der internationalen Genossenschaft [READ-COOP](https://readcoop.org/de) vertrieben, deren Inhaber diverse akademische Institutionen sind. Es weist einen ausgebauten Kundensupport und eine große Nutzercommunity auf. Deshalb kann das Tool auch am meisten (von Einzelprojekten erarbeitete und Transkribus zur Verfügung gestellte) KI-Modelle zur Texterkennung anbieten. Mit dem fortschrittlichsten allgemeinen KI-Modell "The Text Titan 1" ist es Stand Sommer 2024 allen anderen uns bekannten Transkriptionstools überlegen, zumindest was weitverbreitete Handschriften-Arten anbelangt. Transkribus ist jedoch ohne Bezahlung von Abonnement-Angeboten nur eingeschränkt nutzbar.
-   [eScriptorium](https://escriptorium.inria.fr/){:target="\_blank"} : Der Code dieser Tranksribus-Alternative wird kostenlos von der Université PSL in Paris zur Verfügung gestellt. Er kann lokal installiert werden, bedarf jedoch zum vollumfänglichen Betrieb eine **eigene Server-Infrastruktur** oder den institutionellen Zugang zu einem eScriptorium-Server, wie er zurzeit von verschiedenen Universitäten betrieben wird (z.B. ist die eScriptorium-Instanz [fondue](https://fondue.unige.ch/){:target="\_blank"}  der Universität Genf an den meisten Schweizer Universitäten nutzbar). Die Anzahl der zur Verfügung gestellten KI-Modell wächst zurzeit stark.
-   [OCR4all](https://www.ocr4all.org/){:target="\_blank"} : Das kostenlose Transkriptionstool der Universität Würzburg benötigt wie eScriptorium die Installation auf einem lokalen Gerät oder einem eigenen Server. Es ist im Moment institutionell schlechter verankert als Transkribus und eScriptorium. Eine Besonderheit von OCR4all ist die Automatisierung nicht nur des Text-Tranksriptionsschrittes, sondern ganzer Workflows vom Hochladen bis zum Speichern im gewünschten Format.
-   [Transcribo](https://tcdh.uni-trier.de/de/projekt/transcribo){:target="\_blank"}  ist ein Angebot des Trier Center for Digital Humanities der Universität Trier und Teil von dessen Forschungsplattform FuD (vergleichbar mit [Textgrid](https://textgrid.de){:target="\_blank"} , einem deutschen Forschungsverbundsprojekt). Im Gegensatz zu den obigen Tools erlaubt es die Transkription auf Wort- anstatt nur auf Zeilenebene, d.h. jedes transkribierte Wort verweist durch Koordinatenangaben auf das Wort im Digitalisat. Dadurch kann grössere Genauigkeit erzielt werden, der Prozess einer manuellen Transkription wird jedoch komplexer. Eine DSE, die das Tool verwendet, ist die [Johann Caspar Lavater Online Briefedition](https://www.jclavater-briefwechsel.ch/home){:target="\_blank"} .

Den geringsten (projekteigenen) technischen Support benötigt das Tool Transkribus, weshalb im Folgenden auf seine Workflows fokussiert wird. Viele Arbeitsschritte, wie das Trainieren eines Modells, sind jedoch auch auf andere Tools übertragbar.

Wie erwähnt, gleichen sich die Tools auch bezüglich **Datenstandards**: Die Transkriptionsdaten lassen sich in der Regel in einem [XML-Format](https://www.digitale-edition.at/o:konde.215) ausgeben, z.B. in [PAGE-XML](https://www.digitale-edition.at/o:konde.154) oder in [ALTO-XML](https://altoxml.github.io/). Diese sind erst Vorstufen für den DSE-Datenstandard [TEI/XML](https://www.digitale-edition.at/o:konde.79), in dem die Edition letztlich lesbar gemacht wird. Zwischen dem Workflow-Schritt der Transkription in XML (inklusive hier bereits möglicher Annotation) und der weitergehenden [_inhaltlichen Annotation_](05_semantic_annotation.de.md) und [_Kommentierung_](06_commenting.de.md) in TEI-XML muss deshalb noch eine [_Datenkonversion_](04_converting.de.md) stattfinden.

## 2. Automatisierte oder manuelle Transkription?

Es gibt Fälle, in denen manuelle Transkriptionen weiterhin empfehlenswert sind. Dies betrifft insbesondere Editionen von Handschriften: Je schwieriger zu entziffern die Hand und je kleiner die Handschriften-Menge ist, umso weniger lohnt sich der ATR-Einsatz. Zwar existieren insbesondere für Transkribus sehr fähige allgemeine Texterkennungsmodelle wie "The Text Titan 1", die sowohl Drucke wie Handschriften - sogar im selben Dokument - erkennen. Für **schwierige Hände** reichen diese jedoch oft nicht aus, weshalb ein Hand-spezifisches ATR-Modell trainiert werden muss (s.u.). Für das Training dieses Modells ist eine Textmenge von mindestens 75, in schwierigen Fällen sogar 200-300 Trainings-Seiten (sogenannter 'Ground Truth' = ein Corpus vorbereiteter, korrekter Transkriptionen) nötig, bis sich der ATR-Prozess (Training und Nachkorrekturen eingerechnet) nicht mehr den manuellen Aufwand übersteigt. Erst die Transkription eines Mehrfachen der benötigten Trainings-Seiten rechtfertigt in diesen Fällen den Einsatz eines spezifischen ATR-Modells.

Die Entscheidung für die Automatisation hängt also von einer Kosten-Nutzen-Rechnung ab: Das Ziel der automatischen Texterkennung ist, den Korrekturaufwand möglichst gering, aber auf jeden Fall unter dem Aufwand einer manuellen Transkription zu halten.
Dies versucht man üblicherweise mit der schrittweisen Erweiterung der Trainingsdaten durch korrigierte Transkriptionen und dem Trainieren
neuer Texterkennungs-Modelle für den nächsten Datensatz zu erreichen.

## 3. Standard-Schritte im ATR-Prozess

Falls die Entscheidung für ATR gefallen ist, gilt es zu testen, ob ein bereits verfügbares ATR-Modell zufriedenstellende Resultate zeigt oder ein eigenes Modell trainiert werden soll. Die von Transkribus gepflegten Standard-Transkriptionsmodelle werden immer besser und es ist sinnvoll, einen Testdurchlauf mit diesen Modellen zu machen (wenn kein eigenes Modell angestrebt wird, kann mit Schritt 3.3 fortgefahren werden).


### 3.1 Trainieren eines ATR-Modells

Als Trainingsset für eigene Transkriptionsmodelle empfiehlt Transkribus, wie erwähnt, mindestens 75 Seiten Ground Truth. Dies können bestehende Transkriptionen sein, die in Transkribus importiert werden oder Seiten, die mit den Standardmodellen transkribiert und anschliessend korrigiert wurden.

Für Aufbereiten bestehender Transkriptionen in Transkribus stand in der Vergangenheit die Funktion **"text2image"** zur Verfügung, die bestehende Transkriptionen, z.B. aus alten Druck-Editionen, zeilengenau dem Digitalisat zugeordnet hat. Gegenwärtig müssen die Zeilen-Korrespondenzen zu Trainingszwecken manuell hergestellt werden. Ein solches manuelles Einfügen von Transkriptionen in die Trainingsdaten ist nur sinnvoll, wenn der Weg über die Standardmodelle und eine Korrektur nicht möglich ist. Transkribus hat jedoch die Wiedereinführung von "text2image" Ende 2024 in Aussicht gestellt.

!!! note "Erfahrung aus der Showcase-Edition"
    Für die Handschrift von Gaston Paris erwies sich das Standardmodell "The Text Titan I" als geeignet, um mithilfe von Korrekturen eine Ground Truth herzustellen, die wiederum das Trainieren eines eigenen Modells erlaubte (siehe nächste Informationsbox). Es handelt sich dabei um ein KI-Modell, das, ähnlich ChatGPT, auf der Transformer-Technologie beruht und herkömmlichen generellen ATR-Modellen, die ältere KI-Technologien nutzen, überlegen ist. Das eigene Training von Transformer-Modellen ist bislang noch auf keinem Transkriptionstool möglich, selbsterstellte ATR-Modelle können trotzdem durch das Training mit projektspezifischer Ground Truth Tansformer-Modelle konkurrenzieren. 

### 3.2 Wiederholtes Training, Re-Training

Grundsätzlich empfiehlt es sich, **mehr als ein spezifisches Modell mit derselben Ground Truth** zu erstellen. Obschon sich die Datengrundlage dabei nicht ändert, erstellt die KI mit ihrer Hilfe in jedem Training ein anderes Modell, das sich in der Qualität der Texterkennung stark vom vorhergehenden unterscheiden kann. Als Faustregel gilt, mit einer Ground Truth mindesten vier separate Trainingsdurchgänge durchzuführen um die Zufälligkeit des KI Trainings zu minimieren. So kann bereits das erste Training ein gutes Resultat ergeben, während das zweite wesentlich schlechter, das dritte am besten und das vierte wieder schlechter ist.

Vom wiederholten Training mit derselben Ground Truth unterscheidet sich das **Re-Training mit einer größeren Ground Truth**. Wann sollen mit neuen Daten bessere Modelle trainiert werden? Auch diese Frage kann nur projektspezifisch beantwortet werden. Faktoren sind:

-   Qualitätsverbesserung;
-   Korrekturaufwand;
-   Verfügbare Zeit der Projektmitglieder;
-   Zeit, die für das Trainieren gebraucht wird.

!!! note "Erfahrung aus der Showcase-Edition"
Mithilfe von immer größeren Ground Truth Sammlungen (manuell korrigierten Transkriptionen, die wir mit "The Text Titan I" erstellt haben) wurden mehrere Serien von Re-Trainings gemacht; das zweite Modell der zweiten Serie überstieg in gewissen Erkennungsleistungen "The Text Titan I", namentlich in eher aussergewöhnlichen Idiosynkrasien von Gaston Paris' Handschrift. Das allgemeine Modell 'schlug' das eigene jedoch weiterhin in der Erkennung von Zahlen und verschiedener Sprachen.

### 3.3 Layoutanalyse

In der Layoutanalyse erkennt ein Algorithmus **die Anordnung der Zeilen**, bevor die eigentliche Texterkennung durchgeführt wird; es ist deshalb kein optionaler Schritt wie die Annotation von Text oder Textregionen (s.u., 3.5). Während ältere Versionen von Transkribus die Layoutanalyse als eigenen, vorgängigen Schritt vor der ATR nötig gemacht haben, ist diese Mehrstufigkeit mittlerweile optional und es kann direkt mit der Texterkennung (durch ein spezifisches oder ein allgemeines Modell) gestartet werden. Erst bei schlechten Transkriptionsresultaten, in denen Zeilen teilweise oder ganz ausgelassen wurden, ist es empfehlenswert, verschiedene Modelle und Konfigurationen zur Layoutanalyse auszutesten.

### 3.4 Korrektur der Layoutanalyse und der Transkription

Im Korrekturdurchgang empfiehlt sich zunächst eine Kontrolle der Zeilen, besonders wenn Zeilen zerstückelt erkannt wurden oder Zeilen fehlen. Sehr schlechte Resultate der Layoutanalyse rechtfertigen Tests mit verschiedenen Layoutanalyse-Modellen (s.o.).

Wenn dies keine Verbesserung bringt, können die **Zeilen auch manuell verbessert oder ganz von Hand gezogen** werden. Solche Layout-Korrekturen wie das Verlängern einer Zeile verbessern einen erneuten ATR-Durchlauf und die visuelle Korrespondenz zwischen Transkription und Digitalisat im Frontend (siehe hierzu unsere [_Tipps_](../Themen/transkribus.de.md)). Eine genaue Überarbeitung der Zeilen stellt u.U. jedoch einen nicht zu rechtfertigenden Mehraufwand dar, da der Vergleich durch die visuelle Einblendung der Zeilen-Korrespondenz auch ohne diese Einblendung möglich ist.

Fehler in der Transkription können einfach in den Zeilen korrigiert werden. Falsche Zeilenregionen können ebenfalls in diesem Schritt behoben werden. Es ist jedoch zu beachten, dass bei der Nutzung der optionalen Wort-Segmentierung die einzelnen Wörter nicht korrigiert werden können - für diesen Schritt ist eine Nachbearbeitung in Transcribo (https://tcdh.uni-trier.de/de/projekt/transcribo){:target="\_blank"}  eine Option. 

### 3.5 Annotationen im Transkriptionstool

Der letzte, bereits optionale Schritt in Transkribus und ähnlichen Transkriptionstools ist die **Annotation ('Tagging') zunächst von Textregionen und schliesslich des Textes selbst**. Optional ist der erste Schritt, die Textregion-Bestimmung, jedoch nur hinsichtlich der Frage, wann, nicht ob er geschieht. Die **Annotation auf Regionen-Ebene** gehört zum Standard einer DSE, da er den Text grundlegend strukturiert, z.B. in Paragraphen, Postskripta, Verse etc.

Auch die feinteiligere Annotation von Wortfolgen oder Wörtern gehört zum Standard, ihr Detailgrad ist jedoch weniger standardisiert, sie kann, je nach Editionsrichtlinien, nur ein minimales Set umfassen. Grundsätzlich unterscheidet man **zwei Annotationsformen auf Wort-Ebene**:

-   **Textkritische Annotationen** zeichnen sichtbare Eigenschaften des Schriftbildes aus, wie z.B. Unterstreichungen.
-   **Inhaltliche Annotationen** zeichnen semantische Eigenschaften des Textes aus, wie z.B. die Bestimmung eines geographischen Ortes. Auf diese Form der Annotation wird [_später_](05_semantic_annotation.de.md) vertieft eingegangen.

Diese Arbeitsschritte stellen technisch gesehen keine Transkription des Textes mehr dar, sondern könnten auch erst später im TEI/XML geschehen. Es gibt jedoch Gründe dafür, warum die Annotation von Regionen und textkritischen Aspekten - also im Schriftbild erkennbare Eigenschaften - schon während der Transkription (oder ihrer Korrektur) geschieht: Die Auszeichnung verschiedener Hände, Unterstreichungen, Titel, Absätze usw. ist bereits eng mit ihr verbunden. Wenn das Digitalisat und der fertige oder entstehende transkribierte Text genau miteinander verglichen werden müssen, ist es sinnvoll, neben der korrekten (z.B. diplomatischen) Zeichenfolge auch die **sichtbaren Eigenheiten des Textes** festzuhalten.

Transkribus unterscheidet 'Structural Tags' und 'Textual Tags', dies entspricht der oben gezogenen Unterscheidung zwischen der Annotation auf Regionen-Ebene und  der Annotation auf Wort-Ebene.

![alt text](image.png){align=left width="250" } Mit **'Structural Tags'** können selbstdefinierbare Textregionen und automatisch von der Layoutanalyse generierte Zeilenregionen ('base lines' und zugehörige 'line polygons') direkt auf dem Digitalisat, d.h. auf der linken Seite der Benutzeroberfläche, ausgezeichnet werden. Auch wenn diese Tags einfachheitshalber auf dem Digitalisat erscheinen, werden sie in derselben XML-Datei wie die Transkription gespeichert.

![alt text](image-2.png){align=right width="250" }**'Textual Tags'** erlauben das Auszeichnen auf der Wortebene der Tranksription und werden deshalb am Transkriptionstext auf der rechten Seite der Benutzeroberfläche angebracht. 'Textual Tags' können neben formalen Aspekten (Unterstreichungen, fremde Hände) auch bereits inhaltliche Aspekte (Tagging von Ortsbezeichnungen oder Schlagwörtern beinhalten). Wir raten jedoch dazu, die komplexere inhaltliche Annotation erst im TEI-XML vorzunehmen, um den Konversionsaufwand zu minimieren (s.u.). Auch ist Transkribus zurzeit (noch) nicht fähig, inhaltliche Annotationen automatisiert mit externen Ressourcen wie Normdaten zu verlinken. Auch wenn sich dies in Zukunft, wie offenbar geplant, ändern sollte, ist aufgrund des Konversionsaufwandes Vorsicht geboten. 

!!! warning "Herausforderung"
    Wie gesagt, bieten Transkriptionstools eine Auszeichnung in PAGE-XML oder ALTO-XML an, die bei der Konversion in TEI-XML berücksichtigt werden muss.
    Es ist deshalb empfehlenswert, sich **in der Auszeichnung im Transkriptionstool an der Nomenklatur des angestrebten TEI/XML zu orientieren**. So entstehen bei der Konvertierung in TEI/XML TEI-Syntax-konforme Elemente statt frei erfundene Ausdrücke oder - bei Nichtauszeichnung - anonyme Blöcke (`<ab>`). Die wichtigsten Elemente werden standardmässig von Skripten wie Page2TEI erkannt und in die entsprechenden Elemente überführt. Dies stellt einen Komplexitätszuwachs dar, der einen engermaschigen technischen Support des Projektes benötigt.

Der Vorteil von Annotationen in Transkriptionstools ist, dass in der ersten, oberflächlichen Auseinandersetzung mit dem Text bereits die wichtigsten formalen Aspekte geklärt werden können. In den nächsten Schritten nach der Konvertierung, der inhaltlichen Annotation und Kommentierung, - die in folgenden Kapiteln primär anhand des TEI Publishers beschrieben werden - können sich die Mitarbeitenden dann verstärkt mit den semantischen Aspekten auseinandersetzen.
Ob und wie eingehend mit den einfach zu bedienenden, aber im Konversionsprozess anspruchsvollen Tags der Transkriptionstools gearbeitet werden soll, sollten Projekte möglichst früh abwägen.

!!! note "Erfahrung aus der Showcase-Edition"
    Wir haben uns entschieden, mit 'Structual' und 'Textual' Tags in Transkribus nur textkritische Aspekte auszuzeichnen (siehe Showcase-Editionsrichtlinien oben). In dieser Auszeichnung der Briefe von Gaston Paris halten wir uns an die Element-Namen, die das [deutsche Textarchiv](https://www.deutschestextarchiv.de/){:target="\_blank"} als [Basisformat zur Auszeichnung von Briefen](https://deutschestextarchiv.de/doku/basisformat/brief.html){:target="\_blank"} vorschlägt. Hierfür haben wir z.T. eigene Tags in Transkribus geschaffen und in der Auszeichnung der Textregionen auf dem Digitalisat angewendet: Der Briefkopf ist beispielsweise als die Textregion 'opener' definiert, in dieser Textregion zeichnen wir die Zeile mit Datum und ggfls. Ort als 'dateline' und die Begrüssung ("Mon cher ami") als 'salute' aus. Der Textkörper selbst ist in verschiedene Paragraphen (= 'paragraph') unterteilt.

    ![alt text](image-1.png)

## 4. Limitationen

### 4.1 Das ideale Transkriptionstool?

Zurzeit gibt es nicht _die_ Lösung zur Transkription. Die oben aufgeführten Tools benötigen vor allem **unterschiedlich viel Support und technisches Wissen**, haben aber ähnliche Funktionalitäten. Es erscheint uns ratsam, in der Wahl des Tools zunächst stärker vom vorhandenen institutionellen Know-How und den technischen Ressourcen auszugehen als von den Fähigkeiten des Tools (insbesondere weil diese Fähigkeiten bei den oben portraitierten ähnlich sind). Ist das institutionelle Know-How sehr limitiert und erlaubt die finanzielle Lage ein Transkribus-Abonnement, so würden wir für ein solches plädieren.

### 4.2 ATR als Lösung?

Die großen Hoffnungen, die in wissenschaftliche Anwendungen von KI gesetzt werden, gelten auch für ATR-Modelle, die zuweilen auf derselben Technologie wie große Sprachmodelle (z.B. ChatGPT) basieren. Zwar sind die Fortschritte der ATR zurzeit sehr groß, trotzdem sind sie v.a. bezüglich älterer und/oder schwieriger Handschriften noch nicht groß genug, als dass ihre Anwendung in jedem DSE-Projekt sinnvoll erscheint.
Auch bei der Anwendung der besten verfügbaren ATR-Modelle kann der Korrekturaufwand eine von Beginn an manuelle Transkription übersteigen. Das Training von eigenen Modellen ist zeitintensiv und führt nicht immer zu besseren Resultaten. Projekte müssen deshalb zwingend eine **Testphase** einplanen, in der sie die Optionen evaluieren, bevor große Ground Truth Sammlungen erstellt und trainiert werden.

### 4.3 Annotieren in Transkriptionstools?

Auch die Frage, wie viel bereits in PAGE-XML oder ALTO-XML ausgezeichnet werden soll, hängt vom verfügabren technischen Support ab. Uns sind Projekte bekannt, deren Workflow extensive, nicht nur textkritische, sondern auch inhaltliche Annotationen in Transkribus vorsah und aufgrund von Konversionsschwierigkeiten große Verzögerungen und Anpassungen im Workflow hinnehmen mussten. Schon bei Projektbeginn muss deshalb klar werden, **wo welche Auszeichnungen stattfinden** sollen, um die Komplexität der Datenkonversion an die Projektressourcen anzupassen.
Die Showcase-Edition hat die Oberfläche des Annotations-Editors so erweitert, dass textkritische Annotationen auch komplett im TEI-Publisher möglich wären. Das Vorgehen ist dabei dasselbe wie von uns für die [_inhaltliche Annotation_](05_semantic_annotation.de.md) beschrieben.
