# 2.4 Inhaltliche Annotation

## Was bedeutet digitales inhaltliches Annotieren?
Unter der _inhaltlichen Annotation_ verstehen wir die Auszeichnung eines Wortes oder einer Wortfolge hinsichtlich ihrer **semantischen Referenzen**. Diese können sich auf denselben Text (intratextuell), andere Texte/Werke (intertextuell) oder beliebiege Fakten (kontextuell) beziehen. Das vorliegende Kapitel wird sich primär mit der inter- und kontextuellen Referenzierung befassen, da diese editorisch bezüglich Forschungsaufwand und technisch bezüglich Tools und Schnittstellen am anspruchsvollsten sind. Trotzdem sollten Projekte intratextuelle Verweise nicht ausser Acht lassen, da sie insbesondere die Navigation innerhalb eines größeren Textes sehr erleichtert. 

Verbreitete Beispiele: 

- Intratextuelle inhaltliche Annotationen:
    - Verweis einer Briefpassage auf den darin angesprochenen Briefanhang
    - Verweis eines Inhaltsverzeichnises auf die darin angegebenen Kapitel

- Intertextuelle inhaltliche Annotationen: 
    - Verweis eines in einem Brief implizit oder explizit thematisierten Werkes auf einen bibliographischen Eintrag im DSE-Register und/oder auf eine Bibliotheksdatenbank oder - idealerweise - eine [Normdatenbank](/Themen/authority)
    - Verweis einer Textstelle auf einen anderen Text in derselben DSE oder auf einen Text, der in einer anderen DSE ediert wurde

- Kontextuelle inhaltliche Annotation: 
    - Verweis einer Textstelle auf einen Eintrag in im DSE-eigenen Ortsregister und/oder eine Normdatenbank für geographische Daten wie z.B. [geonames.org](https://www.geonames.org/). 
    - Verweis einer Textstelle auf einen Eintrag in im DSE-eigenen Personenregister und/oder eine Normdatenbank für Personen-Daten wie z.B.einen Personeneintrag in der [Gemeinsame Normdatei](https://gnd.network/Webs/gnd/DE/Home/home_node.html), die größte Normdatensammlung für Kultur- und Forschungsdaten im deutschsprachigen Raum. 


Das inhaltliche Annotieren ist eine Editionsarbeit, die spezifisch durch digitale Werkzeuge, insbesondere die Möglichkeit der Verlinkung entsteht. Im Gegensatz  zur textkritischen Annotation, die oft schon während der [*Transkription*](/03_Transkription) (siehe dort 3.5) gemacht wird, erscheint die inhaltlich annotierte Textstelle als Link, der diese Referenz durch einen Klick zugänglich macht (alternativ kann sie auch durch einen Hoover-Text kenntlich werden). Im Gegensatz zur [*Kommentierung*](06_commenting.md) ist eine inhaltliche Annotation ein **einfacher Verweis**, der **selbsterklärend** sein sollte oder zumindest erklärt wird durch die Weiterleitung zu einer editionsinternen Ressource (z.B. ein Eintrag in einem Register oder in einer Karte) oder einer externen Ressource (z.B. einer [*Normdatenbank*](/Themen/authority) wie GND oder Metagrid).


## 1. Standardlösungen für inhaltliches Annotieren
Die inhaltliche Annotation kann normalerweise im gleichen Tool wie die Kommentierung gemacht werden, eine genaue Betrachtung des Digitalisats ist für beide Arbeitsschritte nicht mehr zwingend nötig. Transkriptionstools wie Transkribus bieten diese Arbeitsschritte (noch) nicht an, d.h. sie weisen bislang nicht die Möglichkeit auf, inhaltliche Annotationen als Links oder Kommentare zu erstellen. Solche Funktionen sind zwar Stand Sommer 2024 geplant. Sie sollten jedoch, falls implementiert, mit großer Vorsicht angewendet werden, weil jede zusätzliche Annotationsfunktion im Transkriptionstool neue Herausforderungen in der [*Konversion*](04_converting.md) nach sich ziehen können - zumindest solange Transkriptionstools noch nicht die Funktion besitzen, TEI/XML-Daten selbst zu [*publizieren*](/3_Publikation/01_introduction_publication).  

Zwei technische Standardlösung stehen zur Verfügung und werden im nächsten Unterkapitel in ihren Workflows dokumentiert:

1. Die Nutzung eines Tools, das sowohl **Edition und Publikation** erlaubt. Die hierfür im Detail getestete Lösung ist der TEI-Publisher. 

2. Die Nutzung eines **TEI/XML-Editors** wie Oxygen: Er stellt in diesem Fall ein Verbindungsglied zwischen Transkriptionstool und Publikationstool dar. 


## 2. Standard-Workflow-Schritte 

### 2.1. Erstellen der Editionsrichtlinien
Weitgehend unabhängig vom verwendeten Tool sollte am Anfang des Arbeitsschrittes geklärt werden, welche Inhalte zu welchem Zweck ausgezeichnet werden müssen. Anleitend sollte die Frage sein, welche Nutzungsszenarien die DSE zu erfüllen hat:

- Soll sie möglichst viele inhaltliche Daten möglichst breit sammeln oder sind ganz spezifische Daten im Vordergrund? 
- Welche Daten sind das?

Fünf Hauptkategorien inter- und kontextueller Referenzen, wie in den Beispielen eingangs schon aufgetaucht, haben sich in den letzten Jahren ausgebildet: **Personendaten, Ortsdaten, Zeitdaten, Werkdaten und Schlagworte**. Während Werkdaten und Schlagworte jedoch nicht in jeder DSE auftauchen, sind Personen, Orte und Zeiten mittlerweile Standard. 

Etwas exotischer ist die Referenzierung weiterer Kategorien, denen technisch im Grunde keine Grenzen gesetzt sind, z.B. frei gewählte Themen (spezifischer als Schlagworte), historische Ereignissen oder linguistischer Eigenarten (z.B. die Nutzung von Fremdsprachen). 

!!! warning "Herausforderung"
    Aus editorischer Sicht ist eine Entgrenzung der Kategorien immer mit dem Problem verknüpft, dass eine einmal eingeführte Kategorie sinnvollerweise konsequent angewendet werden muss, was zu viel Aufwand führen kann. Im Fall von mehreren Edierenden bedingt es das genaue Befolgen von komplexen Editionsrichtlinien bzw. die ständige Koordination zur ihrer Anpassung. Komplexe Sachverhalte, die nur in wenigen Texten nachvollziehbar gemacht werden müssen, sollten deshalb eher im Stellen- oder Text-[*Kommentar*](06_commenting) dargestellt werden. 

- Sind vor allem der DSE-eigene Register zentral, etwa weil es kaum andere Datensätze dazu auf dem Internet gibt? 
- Oder soll das Register in den meisten Fällen ein 'Zwischenhalt' darstellen, um eine Information zu bündeln und mit externen Ressourcen zu verknüpfen? 

Beide Tool-Standardlösungen erlauben die **Einbindung von Konnektoren**, d.h. die halb-automatisierte Verlinkung der Annotation im TEI-XML mit einer Normdatenbank. Die Edierenden können aus den Vorschlägen des Konnektors den korrekten Normdatensatz auswählen und müssen die Verlinkung nicht selbst recherchieren und im TEI/XML verfassen. Sollte jedoch die Aussicht klein sein, überhaupt externe Normdaten zu finden, so ist die Anwendung von Konnektoren zweitrangig. 

Im Detail sollte erwägt werden, wie oft welche Daten in einem Text ausgezeichnet werden sollen. Es ist beispielsweise nicht sinnvoll, Anreden (z.B. Du/Ihr) in Briefen jedes Mal zu annotieren, v.a. wenn die angesprochene Person mit dem:der Empfänger:in des Briefes identisch ist. Solche Erwägungen, auch wenn sie trivial erscheinen mögen, sollten ebenfalls in Editionsrichtlinien aufgenommen und den DSE-Nutzenden zur Verfügung gestellt werden. 

!!! abstract "Showcase-Editionsrichtlinien: Inhaltliche Annotation"
    Das Projekt hat sich dazu entschieden, die drei Kategorien Ort, Person und Werk zu annotieren, da sich diese im Falle der historischen Wissenschaftler-Korrespondenzen von Gaston Paris am besten dazu eignen, das Forschungsnetzwerk des Gelehrten, das im Zentrum der eigenen Forschung der Projektleiterin steht, nachzuvollziehen.
        
    - **Orte** werden, wenn möglich, mit ihrem heutigen Ortsnamen auf geonames verlinkt.
        - Orte werden nicht ausgezeichnet, wenn sie bereits in den Metadaten des Briefes vorhanden sind (Absende- oder Empfangsort).
        - Alle anderen Orte werden nur bei ihrer ersten Nennung ausgezeichnet. Da die Briefe kurz sind, sind die weiteren Nennungen einfach findbar.  
        
    - **Personen** werden in einem ersten Schritt mit den Personendaten in GND verknüpft, in einem zweiten Schritt soll auch eine Verknüpfung mit VIAF hergestellt werden. Personendaten, die auf GND noch nicht verzeichnet sind, werden mithilfe eines Bibliothekservices der Zentralbibliothek Zürich in GND ergänzt und werden so verknüpfbar. 
        - Personen werden nicht im Text ausgezeichnet, wenn sie bereits Teil der Metadaten sind (Verfasser:in oder Empfänger:in)
        - Alle anderen Personen werden nur bei ihrer ersten Nennung im Brief ausgezeichnet. 

    - **Werke** werden aus der umfangreichen Bibliographie der Projektleiterin aus dem Bibliographie-Tool Zotero importiert. Das dadurch entstehende Register könnte in einem zweiten Schritt mit Werkdaten aus GND verknüpft werden, dies ist jedoch in der Showcase-Edition nicht umgesetzt. 
        - Werke werden pro Brief nur bei ihrer ersten Nennung ausgezeichnet

### 2.2. Die inhaltliche Annotation im TEI-Publisher

Die open source software [TEI Publisher](https://teipublisher.com/) bietet seit Version 7 (Stand Sommer 2024: Version 9) die Möglichkeit, mithilfe einer graphischen Oberfläche TEI/XML-Daten mit Annotationen anzureichern. Das bedeutet, dass der zu bearbeitende Text nicht als TEI/XML erscheint und als Code bearbeitet werden muss, sondern ähnlich dem Textverarbeitungsprogramm Word darstellbar ist. Die Codierung in TEI/XML lässt sich jedoch jederzeit überprüfen und auch direkt manipulieren, was zuweilen notwendig ist, aber zusätzliches Fachwissen benötigt. 

#### Wahl der ODDs 
Nach dem Importieren der TEI/XML-Daten in den TEI Publisher können diese mithilfe unterschiedlicher ODDs (**O**ne **D**ocument **D**oes it all) auf der Benutzeroberfläche des Tools dargestellt werden. ODD-Dateien (eine genaue Beschreibung finden sich [im Konde-Weissbuch](https://www.digitale-edition.at/o:konde.150)) sind in der ODD-Schema-Sprache verfasst; sie geben den TEI/XML-Code aufgrund unterschiedlicher, festgelegter Schemata aus: Im Falle der (in diesem Fall textkritischen) Annotation ```<hi rend="underline">rassuré</hi>``` 'erkennt' das ODD beispielsweise, dass das Wort "rassuré" unterstrichen werden soll. 
[Das TEI-Konsortium bietet verschiedene ODDs an und dokumentiert deren Verwendung](https://tei-c.org/guidelines/customization/getting-started-with-p5-odds/); da TEI-XML ein flexibler Standard ist, muss und kann nicht jede Annotation für dasselbe verwendet werden. Im deutschsprachigen Raum hat sich neben den Standard-ODDS des Konsortiums das [ODD des deutschen Textarchivs](https://www.deutschestextarchiv.de/doku/basisformat/schema.html) für Edtionen durchgesetzt. ODDs können für jedes Projekt angepasst werden, etwa mithilfe des Online-Tools [ROMA](https://roma.tei-c.org/).

#### Annotatons-Editor

Der TEI Publisher hat verschiedene Standard-ODDS vorinstalliert; auch der Überarbeitungsmodus zur Annotation hat die Form eines ODDS. Dieses hat den Datei-Namen 'annotations.odd' und kann einfach aus einem Seitenreiter ausgewählt haben. Die dadurch aktivierte Annotations-Editor kann angepasst werden, siehe hierzu die [Dokumentation des TEI-Publishers](https://teipublisher.com/exist/apps/tei-publisher/documentation/configuring-annotation-editor?action=search&view=div&odd=docbook.odd#3.42.13.63.3); wichtige Hinweise haben wir zudem im Kapitel "Themen "im Unterkapitel ["Annotationen mit TEI-Publisher"](../Themen/tei-publisher-annotations/) zusammengefasst. 

!!! note "Erfahrungen aus der Showcase-Edition"
    Um alle benötigten Annotationen im Editions-Editor zu aktivieren, waren mehrere Versuche, Besprechungen und Überarbeitungsrunden notwendig. Das Projekt hat u.a. die Notwendigkeit erkannt, die Faksimile, die in der Standard-Einstellung des Annotations-Editors relativ klein am unteren Bildrand platziert ist, grösser rechts vom annotierten Text einzublenden. Somit können auch textkritische Annotationen oder Korrekturen an der Transkription, für die der Vergleich mit dem Faksilie nötig ist, nachgetragen werden. 
    Das angepasste Annotations-ODD des Projektes ist über GitLab öffentlich verfügbar: 
    => HIER PROJEKTRESSOURCEN EINFÜGEN. ![Annotations-Editor TEI Publisher](image-4.png)


### 2.3. Die inhaltliche Annotation in Oxygen mit und ohne ediarum

Nach dem Import der TEI-XML-Daten in den Editor wird mithilfe der Arbeitsumgebung [ediarum](https://www.ediarum.org) die Auszeichnung durchgeführt. Ediarum stellt TEI-XML-Daten ähnlich wie eine Word-Datei dar und hat entsprechende Formatierungs-Buttons. Eine ausführliche ediarum-[Dokumentation](https://www.ediarum.org/docs.html) existiert für das [Aufsetzen](https://www.ediarum.org/docs/set-up/), [Konfigurieren](https://github.com/ediarum/ediarum.SKOS.edit?tab=readme-ov-file#installation) und [Verwenden]( https://www.ediarum.org/docs/ediarum.BASE.manual) der Editionsumgebung und wird vom ediarum-Team regelmässig ergänzt. 

=> Dieser Punkt wird durch Erfahrungen aus dem Schwarzenbach-Projekt angereichert, wobei die Benutzung von ediarum sich voraussichtlich auf sehr wenige Funktionen beschränkt. 

## 4. Limitationen

Die aufgeführten Standard-Wege zur inhaltlichen Annotation haben grundsätzlich dieselbe **editorische Limitation**: Je mehr Annotations-Kategorien in der Edition eingeführt werden, desto schwieriger wird die konsequente Einhaltung der Editionsrichtlinien. 

Auf technischer Seite lassen sich grundsätzlich zwei Limitationen unterscheiden:

1. Wird eine **benutzerfreundliche Annotations-Oberfläche** wie der Annotations-Editor des TEI Publisher oder die ediarum-Erweiterung zu Oxygen verwendet, geht die einfachere Bedienung mit einer Eingrenzung der Annotationsmöglichkeiten einher. Sollen diese erweitert werden, benötigt es reglmässigen Support durch eine technische Fachkraft und womöglich aufwändigere Versuchsphasen. 

2. Wird ein **XML-Editor** wie Oxygen verwendet, so ist die Einführung in die Codier-Arbeit zwecks Annotationserstellung mit  Aufwand verbunden; die Editionsumgebung ist nicht 'ready to use', das Annotieren muss eingeübt werden. Eine Erweiterung und Anpassung der Editionsrichtlinien ist hingegen mit weniger technischem Support verbunden.

Welche der beiden Wege insgesamt weniger Aufwand auf technischer und editorischer Seite benötigt, hängt von der **Dynamik bezüglich der Komplexität eines Projektes** ab: Sind die Editionsrichtlinien zur inhaltlichen Annotation einfach und von Anfang an gesetzt, so ist der erste Weg vorzuziehen; ist das Projekt komplex (z.B. durch ein anwachsendes, anfänglich noch schwer abschätzbares Corpus) und die Anforderungen an die Annotationen anfänglich schwer festzulegen, ist die Arbeit im TEI/XML-Code selbst wahrscheinlich sinnvoller. Die längere technische Einarbeitungszeit der Editionsmitarbeitenden zahlt sich dann durch größere Flexibilität aus. 