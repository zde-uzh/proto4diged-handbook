# 3.3 Dokumentation

Die DSE-Dokumentation ist ein zentraler Bestandteil der Erstellung einer DSE, deshalb sollten schon in der **Planungsphase** der Zeitpunkt im Projektplan und die **Dokumentations-Verantwortungen** im Projektteam festgehalten werden. Wenn möglich gibt es eine Hauptverantwortung für die Dokumentation, die einzelne Aspekte (s.u.) von den betreffenden Spezialist:innen zusammenträgt. 
In der Planungsphase sollte auch  geklärt werden, **wie ausführlich und in welchem Datenformat** dokumentiert werden muss (s.u.), da die Dokumentation idealerweise bereits während den dokumentierten Arbeitsprozessen geschieht und am Schluss nur noch minimaler redaktioneller Überarbeitung bedarf.  

Wir verweisen im Folgenden ausführlich in jedem Punkt auf die [Dokumentation der Showcase-Edition](), die viele Erläuterungen in diesem  Handbuchs (insbesondere die Editionsrichtlinien bez. Transkription, Annotation und Kommentierung) gebündelt wiederholt. 

Es gilt zu beachten, dass sich bislang nur bedingt standardisierte Dokumentations-Strukturen oder Bezeichnungen für Aspekte der Dokumentation durchgesetzt haben; dies macht der Vergleich mit anderen Dokumentationen zuweilen schwierig. Eine Standardisierung wäre wünschenswert, das vorliegende Kapitel versteht sich jedoch nicht als diesbezüglichen Vorschlag, sondern versucht die Dokumentation von (notwendigen und wünschenswerten) Anforderungen aus zu denken. 

## Was enthält eine DSE-Dokumentation?

Eine DSE-Dokumentation ersetzt gegenüber einer gedruckten Edition, deren **editorischen Kommentar**(der meist knapp die Grundlagen der Textkonstitution und die editorischen Richtlinien erklärt) oder deren **editorisches Nachwort** (das zusätzlich die historischen Hintergründe der Edition und editionsphilologische Aspekte auch auf einer abstrakten Ebene erläutert). 

Das **Editionsmodell** der DSE-Dokumentation ergänzt diese klassischen editorischen Erklärungen  um die Richtlinien der Verwendung von **Regeln zur Erstellung textkritischer und inhaltlicher Annotationen sowie Kommentare** in TEI/XML. D.h. es wird Erläutert, welche Codierung für welche Formen der Annotation und Kommentierung im TEI/XML verwendet wird. 
=> [Editionsmodell der Showcase-Edition]()

Die DSE-Dokumentation dokumentiert zudem digitale Aspekte, die im Druck keine Entsprechung haben:

- alle **verwendeten tools**, idealerweise mit einem Verweis auf deren Dokumentation und ggfls. auf ihr Nutzungsmöglichkeiten; 
=> [Tool-Dokumentation der Showcase-Edition]()

- die **Herkunft der digitalen Ressourcen**, z.B. externer IIIF-Server/Plattformen wie [e-manuscripta](https://www.e-manuscripta.ch/) oder Metadaten-Quellen wie  (neben der **Herkunft physischer Quellen**, d.h. der _digitalisierten Ressourcen_, z.B. einem Archiv); 
=> [Ressourcen-Dokumentation der Showcase-Edition]()

- das **Datenmodell**, das wiederum das **Format der Daten** und die **Strukturierung von Metadaten** enthält; 
=> [Datenmodell der Showcase-Edition]()

- die **Maßnahmen zur Langzeitsicherung**, sowohl betreffend der funktionalen Edition mit Frontend als auch die Datenarchivierung auf anderen Plattformen mit entsprechenden Links zu diesen Ressourcen. 
=> [Langzeitsicherungs-Dokumentation der Showcase-Edition]()

## Zugänglichkeit und Präsentation der Dokumentation

Eine DSE-Dokumentation kann, abhängig von Größe, Komplexität und Innovationsgehalt einer DSE, **unterschiedliche Anforderungen** zu befriedigen haben (s.u.), sollte aber gewisse Grundvoraussetzungen in ihrer Präsentation erfüllen: 
Sie sollte als Dokumentation  **erkennbar** sein und auf der gleichen Ebene wie die Liste der edierten Texte, das Register oder die Suchfunktionen bereitgestellt werden. 

Grundsätzlich empfehlen wir, die Dokumentation von anderen Informationen, die keinen technischen oder editionsphilologischen Erklärungscharakter haben, zu trennen. Dies betrifft vor allem eine Trennung von allgemeinen Informationen zum Projektaufbau (z.B. als [Projekteinstiegsseite](../3_presentation/02_access.de.md) über involvierte Institutionen, Team oder Fördermittel) oder von Hintergrundinformationen zu den edierten Inhalten (als wissenschaftliche Ergänzung im Sinne von [Übersichtskommentaren](../2_Editionsarbeit/06_commenting.de.md)). Zitiervorschläge können nötigenfalls in der Dokumentation enthalten sein, besser ist jedoch, wie bereits erwähnt, für jede distinkte Seite einen Zitiervorschlag gut sichtbar einzublenden. 

## Verschiedene Dokumentationstypen

Die **minimale Anforderung an eine Dokumentation** ist die stichwortartige Erklärung aller sichtbaren/benutzbaren Bestandteile der 
DSE und entspricht damit eher dem editorischen Kommentar im Druck. Die verschiedenen Aspekte können durch einfache Unterkapitel getrennt auf einer einzelnen Seite vereint werden, was das einfache Generieren eines PDFs ermöglicht. Dies kann für eine kleinere oder wenig komplexe DSE ausreichend sein, insbesondere wenn sie bisherige Praxis fortsetzt - in diesem Fall ist es ratsam, in der eigenen Dokumentation auf diejenige [_vorbildhafter DSE_](../1_Planung/02_Vorbildhafte_Editionen.de.md) zu verweisen. 

!!! info "Beispielhafte DSE: Minimale Dokumentation
    https://johannconradfischer.com/de/content/editorial-guidelines 

Eine **ausführliche Dokumentation** hat demgegenüber eher den Charakter eines editorischen Nachworts und wird zur besseren Übersichtlichkeit in mehrere Unterseiten aufgeteilt. Je stärker ein DSE-Projekt innerhalb einer community Vorbild-Charakter haben soll und/oder je innovativer ein DSE-Projekt ist, desto ausführlicher sollte die Dokumentation ausfallen.  

## Tools und Datenformate zur Erstellung einer Dokumentation

- **Verwendung von TEI/XML, z.B. zusammen mit dem TEI Publisher**
    - Vorteil: derselbe Datenstandard
    - Nachteile : Unnötige Komplexität, viele Facetten von TEI/XML werden nicht verwendet, Teile der Dokumentation werden womöglich von Mitarbeitenden geschrieben, die selbst nicht in den editorischen Prozess involviert sind (z.B. technische Mitarbeitende, die für das Frontend oder die Langzeitsicherung zuständig sind) und sich deshalb in TEI/XML alleine zu diesem Zweck einarbeiten müssen.
    - Fazit: In kleinen Teams, die alle mit TEI/XML vertraut sind, sinnvoll.  

- Verwendung von Markdown, z.B. zusammen mit MKDocs oder ähnlichen Dokumentationstools
