# 3.2 Editionsansichten

Das Herzstück jeder DSE ist die Präsentation des edierten Textes. Über die Minimal-Standards (zweiteiliges Layout und XML-Downloads) scheint sich die DSE-Community in den letzten Jahren einig geworden zu sein, darüber hinaus gibt es jedoch weitere Ansichts- und Download-Funktionen, die im Folgenden ebenfalls diskutiert werden.

## Das zweiteilige Layout

Als Standard-Ansicht hat sich ein **zweiteiliges Layout** etabliert, das aus dem transkribierten und annotierten Text einerseits und dem dreh- und vergrößerbaren Digitalisat andererseits besteht. Der Vorteil dieser Ansicht ist, dass Beziehungen zwischen der Quelle und dem wissenschaftlich aufbereiteten Text unmittelbar erkennbar werden; man spricht hierbei auch vom **autoptischen Vergleich**. Während Druck-Editionen als historisch-kritische Editionen, die in der Regel auf Faksimilie verzichteten, textgenetische Komplexität noch mithilfe eines textkritischen Apparats nachvollziehbar machen mussten, vereinfacht das zweiteilige digitale Layout etwa die Identifizierung fremder Hände, nachträglicher Korrekturen, Poststempel oder paratextueller Ergänzungen. Diese können zwar weiterhin auch im transkribierten Text mittels Annotationen kenntlich gemacht werden, DSE können aber freier abwägen, was durch die Nutzenden identifiziert und was zusätzlich ausgezeichnet werden soll, da die Information des Quellmaterials im Editionsprozess nicht verloren geht.

Der autoptische Vergleich und damit die Beziehung zwischen Digitalisat und Transkriptionstext kann durch die Einblendung von graphischen Elementen auf dem Faksimile unterstützt werden. Da dies eine Präsentationsfunktion ist, die bereits bei der Erstellung der Tranksriptionen vorbereitet werden muss (d.h. auf Datenebene Koordinaten vorliegen müssen), haben wir die **Verknüpfung von Digitalisat und Transkriptionen** bereits im Unterkapitel [_Transkription_](../2_Editionsarbeit/03_Transkription.de.md) vorgestellt.

!!! info "Beispielhafte DSE"
Für diese Verknüpfung liegt mit der [Escher-Briefedition](https://www.briefedition.alfred-escher.ch/home.html) eine Best Practice vor. Es ist jedoch zu beachten, dass die Escher-Briefedition die Entscheidung fordert, entweder die zweiteilige Layout mit Digitalisat und diplomatischer Umschrift oder eine einteilige Darstellung mit dem inhaltlich annotierten Text ("Edierter Text (mit Registereinträgen)") darzustellen. Dies führt einerseits zu mehr Übersichtlichkeit, weil in der Darstellung des annotierten Textes die Register auf der Seite gut sichtbar dargestellt werden können. Andererseits kann an dieser Lösung kritisiert werden, dass inhaltliche Annotation und Digitalisat so nicht gleichzeitig durchgesehen werden kann. Das Beispiel zeigt den typischen Konflikt zwischen Übersichtlichkeit und Informationsdichte, der an verschiedenen Stellen in der Präsentation von DSE auftaucht.
![alt text](../2_Editionsarbeit/image-3.png)

## Lesefassungen

Neben dem Digitalisat und dem transkribierten und annotierten Text bieten viele DSE auch eine **Lesefassung** an, die auf der diplomatischen Umschrift (siehe [_Transkription_](../2_Editionsarbeit/03_Transkription.de.md)) aufbaut, jedoch eine **Normalisierung** durchlaufen ist. Das heisst, dass Fehler im Originaltext, inkongruente oder historische Schreibweisen und textkritische Annotationen wie Streichungen oder Unterstreichungen nach klar definierten Editionsrichtlinien korrigiert bzw. einer heute im Druck gebräuchlichen Schreibweise angenähert werden. Fehler werden getilgt, Schreibweisen modernisiert und vereinheitlicht, textkritische Annotationen weggelassen oder vereinfacht (Streichungen fallen weg, Unterstreichungen in Kursivierungen geändert). Zudem werden Zeilenumbrüche variabel auf die Bildschirmgröße angepasst und entsprechen nicht länger den Zeilenumbrüchen des Digitalisats (Ausnahmen: Verse und Dramentexte).

Die Lesefassung kann auf Datenebene entweder auf einer neuen XML-Datei basieren, oder die XML-Datei der diplomatischen Umschrift wird mithilfe des ODDs anders ausgelesen. Für zweitere Variante ist es nötig, spätestens während der inhaltlichen Annotation im Falle von Korrekturen die korrekte Wortvarianten für die Lesefassung zu annotieren.

=> @Reto: Ist es besser, eine eigene XML-Datei für die Lesefassung zu erstellen oder den komplexeren zweiten Weg zu wählen? Welche technischen Erwägung gibt es zu beachten und welche Detail-Arbeitsschritte zum Erstellen der Lesefassung sind sinnvoll anzufügen? Wollen wir bereits im Unterkapitel "Inhaltliche Annotation" (wo es erst einen kurzen Verweis auf die Lesefassung gibt) dokumentieren oder reicht das?

## Mehrteilige, variable Layouts

Die **Präsentation der Lesefassung** kann entweder alleinstehend dargestellt werden (ähnlich der oben beschreibenen Präsentation des annotierten Textes in der Escher-Edition) oder in ein **zwei-, drei- bzw. mehrteiliges Layout** mit anderen Ansichten kombiniert werden.

!!! info "Beispielhafte DSE"
Ein Beispiel für eine wahlweise ein-, zweiteilige Ansicht stellt die [Lokalbericht-Edition](https://www.lokalbericht.ch/synopsis/LB.TEIL1.0010-d/LB.TEIL1.0010-d) dar. Im Gegensastz zur Escher-Briefedition lässt sie in der "Parallelansicht" frei wählen, ob die zwei Teile je aus Digitalisat, Transkription oder Lesefassung einer Seite bestehen. In der "Synopsis"-Ansicht ist es auch möglich, zwei unterschiedliche Digitalisate zu kombinieren, oder eine Lesefassung mit einem Digitalisat, das zu einer anderen Seite gehört, darzustellen.
![Ansichten Lokalbericht](image.png)

Auch hier gilt es abzuwägen, wie viel **visuelle und konzeptuelle Komplexität** DSE-Nutzenden zugemutet werden soll. Das beginnt bereits bei der Standard-Einsteillung der Ansicht, betrifft aber vor allem die Auswahl, wie viele Ansichten möglich sind. Nicht jede mögliche Darstellung ist auch tatsächlich für Nutzende sinnvoll.

!!! info "Beispielhafte DSE"
Ein Extrem-Beispiel einer mehrteiligen Editionsansicht stellt das Editionsportal des Deutschen Literaturarchivs Marbach [Edview](https://edview.dla-marbach.de/) dar. Edview ist nicht wie eine herkömmliche Website, sondern im Stil einer webbasierten Ansichts-Anwendung aufgebaut, die innerhalb des Browsers 'Fenster' öffnet und den Nutzenden viele Konfigurationsmöglichkeiten bietet.

     Komplex ist hier bereits der Einstieg, in dem für die Recherche wahlweise mehrere Editionen ausgewählt werden können. In der eigentlichen Editionsansicht lassen sich so Texte von verschiedenen Editionen gleichzeitig in mehreren Fenstern darstellen. Sichtbar sind wahlweise ein bis vier Fenster, jeder neue Ansichtstyp (XML, Faksimilie, Editionstext, Kommentar etc.) erzeugt ein neues Fenster und schiebt bereits geöffnete in einen nicht-sichbtaren Bereich nach links. Die Anzahl Fenster, die durch Miniatur-Symbole zur Ansicht ausgewählt werden können, scheint unbegrenzt. Fenster können für den späteren Gebrauch auch einer virtuellen Ablage hinzugefügt wrden.
    ![Edview Editionsansicht](image-1.png)

## Download der Text-Daten: XML, JPG, PDF, ebooks

DSE bieten mittlerweile oft einfache Möglichkeiten, unterschiedliche Editionsdaten direkt aus der Editionsansicht herunterzuladen (anstatt sie etwa aus einem Repository für Langzeitarchivierung zu holen). Standard ist die Download-Funktion der XML-Datei, interessante Angebote sind aber auch JPGs oder PDFs des Digitalisats sowie PDFs der diplomatischen Umschrift oder der Lesefassung. Noch selten ist die Möglichkeit, Lesefassungen als ebooks (im dafür typischen epub- oder mobi-Format) herunterzuladen. Dies mag daran liegen, dass sich ebooks bislang kaum als wissenschaftliches Arbeitsinstrument etabliert haben.

!!! info "Beispielhafte DSE"
Die (Missiven-Edition)[https://missiven.stadtarchiv.ch/index.html] des Stadtarchivs und der Vadianischen Sammlung St. Gallen ist mit dem TEI-Publisher erstellt und bietet den Download von XML-, JPG- und PDF-Daten jeder Missive an.
![alt text](image-2.png)
