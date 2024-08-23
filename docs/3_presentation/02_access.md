# 3.1 Einstiege: Seiten, Suchen und Register

Die Form des Einstiegs ist abhängig vom **intendierten Publikum**, dass die DSE ansprechen (oder implizit eben gerade nicht ansprechen) möchte. Innerhalb von DSE-Projekten gibt es zuweilen rege Diskussionen, wie stark der Zugang zur Edition strukturiert werden soll, insbesondere ob der Einstieg zunächst eine Einführung in die Benutzung der Edition und/oder ihr Thema bereithält, bevor Texte oder andere Medien zugänglich gemacht werden, oder ob verschiedene Zugänge möglichst intuitiv und schnell vorgelegt werden.

Wir bevorzugen **niederschwellige Formen** des Einstiegs und versuchen solche im Folgenden anhand von konkreten Beispielen zu evaluieren. Wir sprechen 'vorgelagerten' Einführungen nicht ihre Berechtigung ab, zumal diese der Niederschwelligkeit dienen können; z.B. waren in älteren DSE  für viele Nutzende heute selbstverständliche Funktionen noch erklärungsbedürftig. Niederschwellig bedeutet zudem nicht , dass bereits auf der Einstiegsseite (s.u.) alle Zugänge zur Edition gelegt sind, dies kann auch unübersichtlich wirken und den Einstieg erschweren.
Neben verschiedenen Formen von Einstiegsseiten sind verschiedene Suchfunktionen und Register für den Zugang zu den edierten Texten zentral, weshalb sie ebenfalls im Folgenden behandelt werden. 

## Einstiegsseiten  

Es lassen sich zwei grundsätzliche Konzepte von Einstiegseiten unterscheiden: 

1. **Einstiege in das edierte Material**, d.h. der Zugang zu verscherschiedenen Ressourcen und Registern ist vorrangig und der Weg zu ihnen unmittelbar sichtbar. 

!!! info "Beispielhafte DSE" 
    Das Standard-Beispiel ist die Hauptseite des TEI Publishers, das alle Texte in alphabetischer bzw. numerischer Reihenfolge aufführt.

    - Z.B. lässt sich nach einer sehr einfachen Einstiegsseite, die das Projekt kurz umreisst, in der [Coseriu-Ediiton](https://coseriu.uzh.ch/static/home.xml) auf der Hauptseite ein Überblick über alle Texte finden, was angesichts des eher kleinen Korrespondenz-Volumens einleuchtet. Ähnlich verfährt die St. Gallter [Missiven-Edition](https://missiven.stadtarchiv.ch/start.html). 
    - Die Einstiegsseite der [Escher Briefedition](https://www.briefedition.alfred-escher.ch/home.html) ist etwas komplexer, aber bleibt übersichtlich und erlaubt ebenfalls den Zugang zur Textauswahl mit einem Klick. 

    Typisch für viele Editionen im TEI-Publisher ist, dass das **Suchfeld und die Register-Menü** (z.T. als 'Kontexte') ab der Einstiegsseite immer sichtbar sind.

2. **Einstiege in das Projekt**, d.h. die Beschreibung des Projektrahmens, der Benutzung und ggfls. der Zugang zur Dokumentation ist vor- oder gleichrangig. Der Weg zum edierten Text wird oft erst durch eine Lektüre der Einstiegsseite klar und/oder verläuft über mehrere Unterseiten. 

!!! info "Beispielhafte DSE" 
    Insbesondere wenn eine Edition erst wenige edierte Dokumente aufweist, kann ein Einstieg ins Projekt von Anfang an klären, dass es sich um eine unabgeschlossenes 'work in progress' handelt. Auch ein Edition von sehr spezialisierten, komplex aufgbeauten Beständen, die z.B. die Funktion eines digitalen Archivs haben, kann einen ausführlichen Einstieg rechtfertigen. 
    
    - Ein Beispiel hierfür ist das [Niklas Luhmann Archiv](https://niklas-luhmann-archiv.de), dessen Kern eine Edition der Zettelkasten und der Arbeits-Typoskripte bzw. Manuskripte des Wissenschaftlers ausmachen. Da es damit selbst bereits komplex angelegte analoge Arbeitswerkzeuge ins Digitale zu übersetzen galt, weist die Edition [Lesewege](https://niklas-luhmann-archiv.de/bestand/zettelkasten/lesewege) und [Tutorials](https://niklas-luhmann-archiv.de/bestand/zettelkasten/tutorial) auf, die mit dem Editionstext selbst mindestens gleichwertig präsentiert werden.

    - Für extensive Einstiege gibt es Beispiele im TEI Publisher, etwa [Louis Ginzbergs "Legende der Juden"](https://www.ginzberg.ethz.ch/index.html), das zwei Hauptseiten ("About the Edition" und "Edition") umfasst und erstere priorisiert. 

Die Einstiegseite des TEI-Publisher lässt sich **konfigurieren**, wie in der [TEI Publisher-Dokumentation] detailliert beschrieben wird. => @Reto Ich habe die entsprechende Dokumentation noch nicht gefunden.  

Die Showcase-Edition stellt ihre - weitgehend den Standard-Einstellungen entsprechende - Einstiegsseite auch als Quellcode zu verfügung: => Hier Verlinkung auf Github, wenn wir soweit sind. 

## Suchfunktionen

Je komplexer die Edition, desto mehr Suchfunktionen sind sinnvoll. Neben der Hauptfunktion - der Volltextsuche im edierten Text - kann die gezielte Suche in den Kommentaren, Registern oder Bibliographien sinnvoll sein. Eine vorbildhafte Auswahl bietet die [edition-humboldt](https://edition-humboldt.de/). Wo kaum Kommentare zum Einsatz kommen und Register sich einfach in kurzer Zeit durchgehen lassen, sind diese Funktionen jedoch nicht nötig. 
=> @ Reto: Gibt Aspekte aus technischer Sicht zum TEI Publisher zu ergänzen?

## Register

Neben einer Liste der Dokumente und der Suchfunktion stellen Register den wichtigsten Zugang zur Edition dar. Wie bereits im Zusammenhang mit der [*inhaltlichen Annotation*](../2_Editionsarbeit/05_semantic_annotation.md) gesehen, sind die üblichsten Register diejenigen für Orte, Personen und Schlagworte. Zwar  gehören auch Zeitdaten zur Standard-Kategorie der inhaltlichen Auszeichnung, diese werden in der Regel jedoch nicht als Register, sondern als [*Zeitstrahl*](04_timelines_maps.md) dargestellt. Der TEI Publisher erlaubt es, diesen Zeitstrahl auf der Hauptseite einzublenden. Von dieser Lösung macht z.B. die St. Galler [Missiven-Edition](https://missiven.stadtarchiv.ch/start.html?query=&subtype=document&dates=&collection=&start=1) Gebrauch.

**Einfache Register** sind in der Regel alphabetisch nach Eintrag (Ortsnamen, Nachname einer Person etc.) geordnet, dies gilt auch für die Standard Register im TEI-Publisher (unten das Beispiel der Namensregister der St.Galler Missiven Edition).
![Namensregister Missiven](image-4.png)


**Komplexere Register** wie diejenige von [hallernet](https://hallernet.org/), die nicht mit Standard-Tools erstellt sind,  erlauben auch dynamische Anpassungen der Reihenfolge, etwa in dem Personeneinträge auch nach Geburtsort und Sterbeort geordnet werden können. hallernet betont die Vernetzung ihrer Datenbestände und hat den Chrakter einer Forschungdatenbank, deshlab sind auch auf der Einstiegsseite die unterschiedlichen Register im Vordergrund.
![Personenregister hallernet](image-3.png) 

Jeder Registereintrag ist mit einer spezifischen Registerseite verknüpft. Diese können wie das Register selbst unterschiedlich komplex ausgestaltet sein; im Standard-Fall (die auch für den TEI Publisher gilt) sind **auf einer Registerseite alle Vorkommnisse des Eintrags in der Edition sowie eine Verlinkung zu Ressourcen und Normdaten-Einträge außerhalb der Edition** aufgeführt (unten das Beispiel einer Namensregister-Seite der Missiven-Edition).
![Namensregister-Seite der Missiven-Edition](image-6.png)


Wo wie in hallernet die Datenbank-Struktur zentral ist, sind Registerseiten auch mit weiteren Informationen zur Entität angereichert sein, im Falle einer Person z.B. Metadaten über Publikationen oder beruflichen Funktionen. Solche 'haute-couture'-Lösungen benötigen eine **komplexe Datenbank im Hintergrund** und entsprechendes technisches Know-How über die Erstellung und Wartung von Datenbanken.
![Personenregister-Seite hallernet](image-5.png) 


