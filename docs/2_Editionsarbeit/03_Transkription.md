# Transkription und automatische Texterkennung (ATR)

## Was bedeutet digitales Transkribieren?

Das Transkribieren in nicht-digitalen Editionen erfolgte nach Transkriptionsregeln, denen Hilfswissenschaftler:innen oder externe Transkriptionsdienstleistungen zu folgen hatten. Demgegenüber ist der Trankskriptionsprozess in DSE durch mehr Einzelschritte und Weichenstellungen für den weiteren Projektverlauf geprägt. Namentlich sind dies, wie im Folgenden beschrieben, die Wahl 1. des Tools und der Datenformate, 2. des Automatisierungsgrads und 3. der Workflows im eigentlichen Transkriptionsprozess (Erstellen eines eigenen Texterkennungs-Modells; Korrekturschritte; mögliche erste Annotationen). Letztlich wird das vorliegende Handbuch-Kapitel auf die Limitationen der verfügbaren Standard-Lösungen zur Transkription eingehen.  

Wie in Print-Editionen gilt es auch für DSE konsequente **Transkriptionsrichtlinien** zu verfolgen, insbesondere hinsichtlich **Transkriptionsumfang** und **diplomaticher Umschrift**, d.h. Genauigkeitsgrad der Umschrift. Bei Handschriften muss die Frage beantwortet werden, welche Hände, (Sonder-)Zeichen, Text-Eingriffe und Überarbeitungsstufen wie transkribiert werden. Bei Drucken stellt sich zudem die Frage nach druckspezifischen Paratexten wie Seitenzahlen oder Schmutztitel. 

!!! abstract "Modell-Editionsrichtlinien: Tranksription"

    Die Modell-Edition versteht sich als hypothetische Vorarbeit zu einer wesentlich größeren Edition der Korrespondenz von Gaston Paris, die 27.000 Seiten umfasst und sich - falls in späteren Projekten umgesetzt - primär an ein **Forschungspublikum** wendet. Da die entwickelten prototypischen Workflows einereseits wissenschaftliche Standards diplomatischer Editionen erfüllen sollen, anderersetits im Umfang skalierbar bleiben müssen, konzentriert sie sich um **größtmöglich Texttreue bei gleichzeitiger Einfachheit textkritischer und inhaltlicher Auszeichnung**. 

    Bei der Transkription hielt sich die Modell-Ediiton an folgende **textkritische Grundsätze**: 

    **Umfang**
        
    - Abgesehen von eindeutig durch Archivar:innen hinzugefügte Signaturen oder Paginierungen werden alle Hände transkribiert, insbesondere Datumsergänzungen. Archivsignaturen sind in den Metadaten ersichtlich. 

    - Hinzufügungen durch 'fremde Händ', d.h. die in den Brief-Metadaten nicht als Urheberhand ausgewiesen sind, werden als solche durch Annotation (siehe 3.5) kenntlich gemacht.=> Hier beispiel aus der Modell-Edition verlinken.    

    - Die Frage nach textgenetischen Zusammenhängen (welche Hand welchem Zeitpunkt zugeordnet werden kann) wird nicht während der Transkritpion durch Sonderzeichen oder Annotationen beantwortet, da die Breife Gaston Paris' textgenetisch weitgehend 'flach' sind (d.h. kaum eigene oder fremde Überarbeitungsspuren aufweisen). Wo textgenetische Zusammenhänge dargestellt werden müssen, würde dies in [Kommentaren](06_commenting.md) geschehen.  

    - Vordrucke (z.B. Briefköpfe von Hotels oder Privatpersonen) auf dem Briefpapier werden in der Regel transkribiert und  als 'Vordrucke' ebenfalls annotiert. => Hier beispiel aus der Modell-Edition verlinken.  
        - Ausnahme 1: Vorgedruckte Formularzeilen bei Postkarten ('Nom:','Prenom:' etc.) werden nicht transkribiert, da sie allen Postkarten eigen sind.
        - Ausnahme 2: Postkartenstempel oder Briefmarken werden nicht transkribiert. Die darin enthaltenen Orst- und Datumsangaben können, falls sie von der Datumslinie des Briefes abweisen, in den Metadaten festgehalten werden. Es gibt jedoch Editionen, die sich zwecks Durchsuchbarkeit der Stempel für ihre Auszeichnung entschieden haben, z.B. die [Gotthelf-Ausgabe](bei Erscheinen hier Link ergänzen).


    **Diplomatische Umschrift**

    - Sonderzeichen, die Gaston Paris' insbesondere aus wissenschaftlichen Hintergründen oder Fremdsprachen entlehnt, werden verwendet und nicht ausdrücklich in einem textkritischen Apparat aufgeführt [Verständnis durch das Fachpublikum wird vorausgesetzt].
    
    - Fehler im Ursprungsmanuskript werden ohne zusätzliche Kennzeichnung übernommen [Überprüfung des Fehlers ist durch den Vergleich mit der daneben eingeblendeten Handschrift einfach möglich]. 
    
    - Unterstreichungen, Hochstellungen und Sonderzeichen werden als solche transkribiert. 
    
    - Einkreisungen von Wörtern oder Buchstaben werden durch eckige Kasten wiedergegeben. Auf eine Umwandlung in Sperrung oder Fettdruck wird verzichtet, um die oftmals wissenschaftlich motivierte Hervorhebung von Lemmata zu erhalten.  
    
    - Der französische Leerschlag vor Doppelpunkten, Semikolon und Ausrufuezeichen wird stillschweigend in der Transkription angewendet. [Dieser letzte Punkt weicht von einer strengen diplomatischen Umschrift ab und ist bereits eine Konzession an eine mögliche gedruckte Leseausgabe]. 

DSE-spezifische Transkriptionsrichtlinien betreffen die **Verknüpfung von Digitalisat und Transkriptionen** im Frontend, d.h. die Einblendung von visuellen Wort- oder Zeilenkorrespondenzen zwischen Faksimile und Text. Diese wird idealerweise bereits im Schritt der Transkription vorbereitet, alle unten erwähnten Tools weisen einfache Formen dieser Verknüpfung auf. Der Zeilen-genaue Text-Bild-Verweis, der den autoptischen Vergleich vereinfacht z.B. durch Aufblinken der Textzeile im Digitalisat, hat sich zum Standard von DSE entwickelt, und wird im Folgenden zu den dokumentierten Standardlösungen gezählt. 

!!! success "Best Practice" 
    ![screenshot Escher](image-3.png){ width="400" align=right } 
    Vorbildhaft für die Verknüpfung von Digitalisat und Transkription für DSE, die den TEI-Publisher verwenden, ist die [Briefedition Alfred Escher](https://www.briefedition.alfred-escher.ch/home.html). 
    
    Die Modell-Edition hat sich an dieser Form der Zeilen-Korrespondenz orientiert und den hierfür vorhandenen [Quellcode der Briefedition Alfred Escher](https://github.com/stazh/briefedition-escher) nachgenutzt. 

## 1. Standardlösungen für Transkriptionen

Sind die Textträger ausgewählt und digitalisiert, d.h. ist die [Textkonstitution](02_Textkonstitution.md) beendet, gilt es die Texte selbst maschinenlesbar zu machen. Hierfür werden die Bilddaten der Digitalisate, die z.B. im JPEG- oder TIFF-Format vorliegen, in Textdaten umgewandelt bzw. eben transkribiert. Dies kann manuell oder automatisiert geschehen (s.u.), in beiden Fällen können mittlerweile  dieselben Transkriptionstools und damit dieselben XML-Standard-Datenformate verwendet werden. 

Es ist deshalb von Vorteil sowohl für die manuelle wie die automatisierte digitale Transkription ein wissenschaftliches Tranksriptionstool und kein Textverarbeitungsprogramm wie Word zu wählen. Letzteres verwendet keinen offenen XML-Standard, erlaubt keine Text-Bild-Verweise durch Koordinaten im XML oder macht dazu weitere Daten-Konversionen nötig. 

Im Folgenden protraitieren wir die verbreitetsten  wissenschaftliche Transkriptionstools (weitere Tools finden sich [hier](https://www.adfontes.uzh.ch/ressourcen/quellen-erschliessen/digitale-transkriptionstools)): 

- [Transkribus](https://app.transkribus.org/): Das Stand 2024 weitverbreitetste Transkriptionstool wird von der internationalen Genossenschaft [READ-COOP](https://readcoop.org/de) vertrieben, deren Inhaber diverse akademische Institutionen sind. Es weist einen ausgebauten Kundensupport und eine große Nutzercommunity auf. Deshalb kann das Tool auch am meisten (von Einzelprojekten erarbeitete und Transkribus zur Verfügung gestellte) KI-Modelle zur Texterkennung anbieten. Transkribus ist jedoch ohne Bezahlung von Abonnement-Angeboten nur sehr eingeschränkt nutzbar.
- [eScriptorium](https://escriptorium.inria.fr/): Der Code dieser Tranksribus-Alternative wird kostenlos von der Université PSL in Paris zur Verfügung gestellt. Er kann lokal installiert werden, bedarf jedoch zum vollumfänglichen Betrieb eine eigene Server-Infrastruktur oder den institutionellen Zugang zu einem eScriptorium-Server, wie er zurzeit von verschiedenen Universtitäten betrieben wird (z.B. ist die eScriptorium-Instanz [fondue](https://fondue.unige.ch/) der Universität Genf an den meisten Schweizer Universitäten nutzbar). 
- [OCR4all](https://www.ocr4all.org/): Das kostenlose Transkriptionstool der Universität Würzburg benötigt wie eScriptorium die Installation auf einem lokalen Gerät oder einem eigenen Server. Es ist im Moment institutionell schlechter verankert als Transkribus und eScriptorium. Eine Besonderheit von OCR4all ist die Automatisierung nicht nur des Text-Tranksriptionsschrittes, sondern ganzer Workflows von der bis zum speichern im gewünschten Format. 
- [Transkribo](https://tcdh.uni-trier.de/de/projekt/transcribo) ist ein Angebot des Trier Center for digital Humanities der Universität Trier und Teil von dessen Forschungsplattform FuD (vergleichbar mit [Textgrid](https://textgrid.de), einem deutschen Forschungsverbundsprojekt). Im Gegensatz zu den obigen Tools erlaubt es die Transkription auf Wort- anstatt nur auf Zeilenebene, d.h. jedes transkribierte Wort verweist durch Koordinatenangaben auf das Wort im Digitalisat. Dadurch kann mehr Genauigkeit hergestellt werden, der Prozess einer manuellen Transkription wird jedoch komplexer. Eine DSE, die das Tool verwendet, ist die [Johann Caspar Lavater Online Briefedition](https://www.jclavater-briefwechsel.ch/home).

 Den geringsten (projekteigenen) technischen Support benötigt das Tool Transkribus, weshalb im Folgenden auf dessen Workflows fokussiert wird. Viele Arbeitsschritte wie  das Trainieren eines Modells sind jedoch auf andere Tools übertragbar. 
 
 Wie erwähnt, gleichen sich die Tools auch bezüglich Datenstandards: Die Transkriptionsdaten lassen sich in der Regel in einem  [XML-Format](https://www.digitale-edition.at/o:konde.215) ausgeben, z.B. in [PAGE-XML](https://www.digitale-edition.at/o:konde.154) oder in [ALTO-XML](https://altoxml.github.io/). Diese sind erst Vorstufen für den DSE-Datenstandard [TEI-XML](https://www.digitale-edition.at/o:konde.79), in dem die Edition letztlich lesbar gemacht wird. Zwischen dem Workflow-Schritt der Transkription in XML (inklusive hier bereits möglicher textritischer Annotation) und der inhaltlichen [Annotation](05_semantic_annotation.md) und [Kommentierung](06_commenting.md) in TEI-XML und muss  deshalb noch eine [Datenkonversion](04_converting.md) stattfinden. 

## 2. Automatisierte oder manuelle Transkription?

Es gibt Fälle, in denen manuelle Transkriptionen weiterhin empfehlenswert sind. Dies betrifft insbesondere Editionen von Handschriften: Je schwieriger zu entziffern die Hand und je kleiner die Handschriften-Menge ist, umso weniger lohnt sich der ATR-Einsatz. Zwar existieren insbesondere für Transkribus sehr fähige allgemeine Texterkennungsmodelle, die sowohl Drucke wie Handschriften - sogar im selben Dokument - erkennen. Für **schwierige Hände** reichen diese jedoch oft nicht aus, weshalb ein Hand-spezifisches ATR-Modell tainiert werden muss (s.u.). Für das Training dieses Modells ist eine Textmenge von mindestens 75, in schwierigen Fällen sogar 200-300 Training-Seiten ('Ground Truth' - vorbereitete, korrekte Transkriptionen) nötig, bis sich der ATR-Prozess (Training und Nachkorrekturen eingerechnet) nicht mehr den manuellen Aufwand übersteigt. Erst die Transkription eines Mehrfachen der benötigten Training-Seiten rechtfertigt den Einsatz eines spezifischen ATR-Modells.  

Die Entscheidung für die Automatisation hängt also von einer Kosten-Nutzen-Rechnung ab: Das Ziel der automatischen Texterkennung ist, den Korrekturaufwand möglichst gering, aber auf jeden Fall unter dem Aufwand einer manuellen Korrektur zu halten.
Dies versucht man üblicherweise mit der schrittweisen Erweiterung der Trainingsdaten durch korrigierte Transkriptionen und dem Trainieren
neuer Texterkennungs-Modelle für den nächsten Datensatz zu erreichen. 


## 3. Standard-Schritte im ATR-Prozess

Falls die Entscheidung für ATR gefallen ist, gilt es zu testen, ob ein bereits verfügbares ATR-Modell zufriedenstellende Resultate zeitigt oder ein eigenes Modell trainiert werden soll. Die von Transkribus gepflegten Standard-Transkriptionsmodelle werden immer besser und es ist sinnvoll, einen Testdurchlauf mit diesen Modellen zu machen (wenn kein eigenes Modell angestrebt wird, kann mit Schritt 3.3 fortgefahren werden).

Falls im Projekt spezifische Transkriptionsregeln bestehen oder das Material für eine Schreiberhand viel Material hat, bringt ein spezifisches Modell gegenüber bestehenden Modellen einen Mehrwert und kann die Korrektur verkürzen.

### 3.1 Trainieren eines ATR-Modells 

Als Trainingsset für eigene Transkriptionsmodelle empfiehlt Transkribus, wie erwähnt, mindestens 75 Seiten Ground Truth. Dies können bestehende Transkriptionen sein, die in Transkribus importiert werden oder Seiten, die mit den Standardmodellen transkribiert und anschliessend korrigiert wurden.

Das Aufbereiten bestehender Transkriptionen in Transkribus stand in der Vergangenheit die Funktion **"text2image"** zur Verfügung, die bestehende Transkriptionen zeilengenau dem Digitalisat zugeordnet hat. Gegenwärtig müssen die Zeilen-Korrespondenzen zu Trainingszwecken manuell hergestellt werden. Ein solches manuelles Einfügen von Transkriptionen in die Trainingsdaten ist nur sinnvoll, wenn der Weg über die Standardmodelle und einer Korrektur nicht möglich ist. Transkribus hat jedoch die Wiedereinführung von "text2image" Ende 2024 in Aussicht gestellt.

!!! note "Erfahrung aus der Modell-Edition"
    Für die Handschrift von Gaston Paris erwies sich das Standardmodell "The Text Titan I" als geeignet für die Anwendungen auf die Editionsdaten und eine anschliessende Korrekturrunde. Es handelt sich dabei um ein KI-Modell, das ähnlich ChatGPT auf der Transformer-Technologie beruht und herkömmlichen generellen ATR-Modellen, die ältere KI-Technologien nutzen, überlegen ist. Das eigene Training von Transformer-Modellen ist bislang noch auf keinem Transkriptionstool möglich, selbsterstellte ATR-Modelle können trotzdem durch das Training mit projektspezifischer Ground Truth Tansformer-Modelle konkurrenzieren (siehe nächster Kasten).


### 3.2 Wiederholtes Training, Re-Training

Grundsätzlich empfiehlt es sich, **mehr als ein spezifisches Modell mit derselben Ground Truth** zu erstellen. Obschon sich die Datengrundlage dabei nicht ändert, erstellt die KI mit ihrer Hilfe in jedem Training ein anderes Modell, das sich in der Qualität der Texterkennung stark vom vorhergehenden untrscheiden kann. Als Faustregel gilt, mit einer Ground Truth mindesten vier separate Trainingsdurchgänge durchzuführen um die Zufälligkeit des KI Trainings zu minimieren. So kann bereits das erste Training das gute Resultate zeitigen, während das zweite wesentlich schlechter, das dritte am besten und das vierte wieder schlechter ist. 

Vom wiederholten Training mit derselben Ground Truth unterscheidet sich das **Re-Training mit einer größeren Ground Truth"". Wann sollen mit neuen Daten bessere Modelle trainiert werden? Auch diese Frage kann nur projektspezifisch beantwortet werden. Faktoren sind:

-   Qualitätsverbesserung
-   Korrekturaufwand
-   Verfügbare Zeit der Projektmitglieder
-   Zeit, die für das Trainieren gebraucht wird

!!! note "Erfahrung aus der Modell-Edition"
    Mithilfe von immer größerer Ground Truth Sammlungen (manuell korrigierten Transkriptionen, die wir mit  "The Text Titan I" erstellt haben) wurden mehrere Serien von Re-Trainings gemacht; das zweite Modell der zweiten Serie überstieg in gewissen Fähigkeiten "The Text Titan I", namentlich in eher aussergewöhnlichen Idiosynkrasien von Gaston Paris' Handschrift. Das allgemeine Modell 'schlug' das eigene jedoch weiterhin in der Erkennung von Zahlen und verschiedener Sprachen.  

### 3.3 Layoutanalyse

In der Layoutanalyse erkennt ein Algorithmus die Anordnung der Zeilen, bevor die eigentliche Texterkennung durchgeführt wird; es ist deshalb kein optionaler Schritt wie die Anootation von Text oder Textregionen (siehe 3.5). Während ältere Versionen von Transkribus  die Layoutanalyse als eigenen, vorgängigen Schritt vor der ATR nötig gemacht haben, so ist diese Mehrstufigkeit mittlerweile optional und es kann direkt mit der Texterkennung (durch ein spezifisches oder ein allgemeines Modell) gestartet werden. Erst bei schlechten Transkriptionsresultaten, in denen Zeilen teilweise oder ganz ausgelassen wurden, ist es empfehlenswert, verschiedene Modelle und Konfigurationen zur Layoutanalyse auszutesten.

### 3.4 Korrektur der Layoutanalyse und der Transkription

Im Korrekturdurchgang empfiehlt sich zunächst eine Kontrolle der Zeilen, besonders wenn Zeilen zerstückelt erkannt wurden oder Zeilen fehlen. Sehr schlechte Resultate der Layoutanalyse rechtfertigen Test mit verschiedenen Layoutanalyse-Modellen (s.o.). 

Wenn  dies keine Verbesserung bringt, können die Zeilen auch manuell verbessert oder ganz gezogen werden. Solche Layout-Korrekturen wie das Verlängern einer Zeile verbessern einen erneuten ATR-Durchlauf und die visuelle Korrespondenz zwischen Transkription und Digitalisat im Frontend (siehe hierzu unsere [Tipps](../Themen/transkribus.md)). Eine genaue Überarbeitung der Zeilen stellt u.U. jedoch einen nicht zu rechtfertigenden Mehraufwand da, da der autoptische Vergleich durch die visuelle Einblendung der Zeilen-Korrespondenz auch ohne diese Einblendung möglich ist. 

Fehler in der Transkription können einfach in den Zeilen korrigiert werden. Falsche Zeilenregionen können ebenfalls in diesem Schritt behoben werden.

### 3.5 Annotationen im Transkriptionstool

Der letzte, bereits optionale Schritte in Transkribus und ähnlichen Transkriptionstools ist die **Auszeichnung ('Tagging') von Text und Textregionen**. Optional ist dieser Schritt jedoch nur hinsichtlich der Frage, wann, nicht ob er geschieht. Das Auszeichnen des Transkriptionstextes gehört zum Standard einer DSE, da er den Text grundlegend strukturiert (z.B. in Paragraphen, Hände etc.). Dieser Arbeitsschritt stellt technisch gesehen keine Transkription des Textes mehr dar, sondern könnte auch erst später im TEI-XML geschehen. Es gibt jedoch Gründe dafür, warum er schon während der Transkription (oder ihrer Korrektur) geschieht: Die Auszeichnung verschiedener Hände, Unterstreichungen, Titel, Absätze usw. ist bereits eng mit ihr verbunden. Wenn das Digitalisat und der fertige oder entstehend transkribierte Text genau miteinander verglichen werden müssen, ist es sinnvoll, neben der korrekten (z.B. diplomatischen) Zeilenfolge auch die strukturellen Eigenheiten des Textes festzuhalten. 

 ![alt text](image.png){align=left width="250" } Transkribus unterscheidet 'Structural Tags' und 'Textual Tags'. Mit **'Structural Tags'** können selbstdefinierbare Textregionen und automatisch von der Layoutanalyse generierte Zeilenregionen ('base lines' und zugehörige 'line polygons') direkt auf dem Digitalisat, d.h. auf der linken Seite der Benutzeroberfläche, ausgezeichnet werden. Auch wenn diese Tags einfachheitshalber auf dem Digitalisat erscheinen, werden sie in derselben XML-Datei wie die Transkription gespeichert. 

 ![alt text](image-2.png){align=right width="250" }**'Textual Tags'** erlauben das Auszeichnen auf der Wortebene der Tranksription und werden deshalb am Transkriptionstext auf der rechten Seite der Benutzeroberfläche angebracht. 'Textual Tags' können neben formalen Aspekten (Unterstreichungen, fremde Hände) auch bereits inhaltliche Aspekte (Tagging von Ortsbezeichnungen oder Schlagwörtern beinhalten). Wir raten jedoch dazu, die komplexere inhaltliche Annotation erst im TEI-XML vorzunehmen, um den Konversionsaufwand zu minimieren (s.u.). 

 Transkriptionstools bieten also bereits eine Auszeichnung in PAGE-XML oder ALTO-XML an, die bei der Konversion in TEI-XML berücksichtigt werden muss. 
Es ist deshalb empfehlenswert, sich in der Auszeichnung im Transkriptionstool an der Nomenklatur des angestrebten TEI-XML zu orientieren. So entstehen bei der Konvertierung in TEI-XML  TEI-Syntax-konforme Elemente statt frei erfundene Ausdrücke oder - bei Nichtauszeichnung - anonyme Blöcke (`<ab>`). Die wichtigsten Elemente werden standardmässig von Skripten wie Page2TEI erkannt und in die entsprechenden Elemente überführt. Dies stellt ein Komplexitätszuwachs dar, der einen engermaschigen technischen Support des Projektes benötigt. 

Der Vorteil von Annotationen in Transkriptionstools ist, dass in der ersten, oberflächlichen Auseinandersetzung mit dem Text bereits die wichtigsten formalen Aspekte geklärt werden können. In den nächsten Schritten nach der Konvertierung, der kritischen Annotation und KOmmentierung, - die hier primär anhand des TEI-Publishers beschreiben werden - können sich die Mitarbeitenden dann verstärkt mit den inhaltlichen Aspekten auseinandersetzen. 
Ob und wie eingehend mit den einfach zu bedienenden, aber im Konversionsprozess anspruchsvollen Tags der Transkriptionstools gearbeitet werden soll, sollten Projekte möglichst früh abwägen.   

!!! note "Erfahrung aus der Modell-Edition"
    Wir haben uns entschieden, mit 'Structual' und 'Textual' Tags in Transkribus nur textkritische Aspekte auszuzeichnen (siehe Modell-Editionsrichtlinien oben). In dieser Auszeichnung der Briefe von Gaston Paris halten wir uns an die Element-Namen, die das [deutsche Textarchiv](https://www.deutschestextarchiv.de/) als [Basisformat zur Auszeichnung von Briefen](https://deutschestextarchiv.de/doku/basisformat/brief.html) vorschlägt. Hierfür haben wir z.T. eigene Tags in Transkribus geschaffen und in der Auszeichnung der Textregionen auf dem Digitalisat angewendet: Der Briefkopf ist beispielsweise als die Textregion 'opener' definiert, in dieser Textregion zeichnen wir die Zeile mit Datum und ggfls. Ort als 'dateline' aus. Der Textkörper selbst ist in verschiedene Paragraphen (= 'paragraph') unterteilt.
    
    ![alt text](image-1.png)

## 4. Limitationen

### Das ideale Transkriptionstool?
Zurzeit gibt es nicht *die* Lösung zur Transkription. Die oben aufgeführten Tools benötigen vor allem unterschiedlich viel Support und technisches Wissen, haben aber ähnliche Funktionalitäten. Es erscheint uns ratsam, in der Wahl des Tools zunächst stärker vom vorhandenen institutionellen Know-How und den technischen Ressourcen auszugehen. Sind diese sehr limitiert und erlaubt die finanzielle Lage ein Transkribus-Abonnement, so würden wir für ein solches plädieren.  

### ATR als Lösung?
Die großen Hoffnungen, die in wissenschaftliche Anwendungen von KI gesetzt werden, gelten auch für ATR-Modelle, die zuweilen auf derselben Technologie wie große Sprachmodelle (z.B. ChatGPT) basieren. Zwar sind die Fortschritte der ATR zurzeit sehr groß, trotzdem sind sie v.a. bezüglich älterer und/oder schwieriger Handschriften noch nicht groß genug, als dass ihre Anwendung in jedem DSE-Projekt sinnvoll erscheint. 
Auch bei der Anwendung der besten verfügbaren ATR-Modelle kann der Korrekturaufwand eine von Beginn an manuelle Transkription übersteigen. Das Training von eigenen Modellen ist zeitintensiv und führt nicht zwingend zu besseren Resultaten. Projekte müssen deshalb zwingend eine Testphase einplanen, in der sie die Optionen sondieren, bevor große Ground Truth Sammlungen erstellt und trainiert werden. 

### Annotieren in Transkriptionstools?
Auch die Frage, wie viel bereits in PAGE-XML oder ALTO-XML ausgezeichnet werden soll, hängt vom verfügabren technischen Support ab. Uns sind Projekte bekannt, deren Workflow extensive, nicht nur textkritische, sondern auch inhaltliche Annotationen in Transkribus vorsahen und aufgrund Konversionsschwierigkeiten große Verzögerungen und Anpassungen im Workflow hinnehmen mussten. Schon bei Projektbeginn muss deshalb klar werden, wo welche Auszeichnungen stattfinden können, um die Komplexität der Datenkonversion an die Projektressourcen anzupassen. 


