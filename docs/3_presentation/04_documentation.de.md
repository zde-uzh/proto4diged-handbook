# 3.3 Dokumentation

Die DSE-Dokumentation ist ein zentraler Bestandteil der Erstellung einer DSE, deshalb sollten schon in der **Planungsphase** der Zeitpunkt im Projektplan und die **Dokumentations-Verantwortungen** im Projektteam festgehalten werden. Wenn möglich gibt es eine Hauptverantwortung für die Dokumentation, die einzelne Aspekte (s.u.) von den betreffenden Spezialist:innen zusammenträgt. 
In der Planungsphase sollte auch  geklärt werden, **wie ausführlich und in welchem Datenformat** dokumentiert werden muss (s.u.), da die Dokumentation idealerweise bereits während den dokumentierten Arbeitsprozessen geschieht und am Schluss nur noch minimaler redaktioneller Überarbeitung bedarf.  

Wir verweisen im Folgenden ausführlich in jedem Punkt auf die [Dokumentation der Showcase-Edition](), die viele Erläuterungen in diesem  Handbuchs (insbesondere die Editionsrichtlinien bez. Transkription, Annotation und Kommentierung) gebündelt wiederholt. 

Es gilt zu beachten, dass sich bislang nur bedingt standardisierte Dokumentations-Strukturen oder Bezeichnungen für Aspekte der Dokumentation durchgesetzt haben; dies macht den Vergleich der Dokumentationen zuweilen schwierig. Eine Standardisierung wäre wünschenswert, das vorliegende Kapitel versteht sich jedoch nicht als diesbezüglichen Vorschlag, sondern versucht die Dokumentation von (notwendigen und wünschenswerten) Anforderungen aus zu denken. 

## Was enthält eine DSE-Dokumentation?

Eine DSE-Dokumentation ersetzt gegenüber einer gedruckten Edition den **editorischen Kommentar**(der meist knapp die Grundlagen der Textkonstitution und die editorischen Richtlinien erklärt) oder das **editorische Nachwort** (das zusätzlich die historischen Hintergründe der Edition und editionsphilologische Aspekte erläutert). 

Das **Editionsmodell** der DSE-Dokumentation ergänzt diese klassischen editorischen Erklärungen um **Richtlinien zur Erstellung textkritischer und inhaltlicher Annotationen sowie Kommentare** in TEI/XML. D.h. es wird erläutert, welche Codierung für welche Formen der Annotation und Kommentierung im TEI/XML verwendet wird. 
=> [Editionsmodell der Showcase-Edition]()

Die DSE-Dokumentation dokumentiert zudem digitale Aspekte, die im Druck keine Entsprechung haben:

- alle **verwendeten tools**, idealerweise mit einem Verweis auf deren eigene Dokumentation und ggfls. auf ihr Nutzungsmöglichkeiten; 
=> [Tool-Dokumentation der Showcase-Edition]()

- die **Herkunft der digitalen Ressourcen**, z.B. externer IIIF-Server/Plattformen wie [e-manuscripta](https://www.e-manuscripta.ch/) oder Metadaten-Quellen (neben der **Herkunft physischer Quellen**, d.h. der _digitalisierten Ressourcen_, z.B. einem Archiv); 
=> [Ressourcen-Dokumentation der Showcase-Edition]()

- das **Datenmodell**, das wiederum das **Format der Daten** und die **Strukturierung von Metadaten** enthält; 
=> [Datenmodell der Showcase-Edition]()

- die **Maßnahmen zur Langzeitsicherung**, sowohl betreffend der [_funktionalen Edition mit Frontend_](../4_longterm_preservation/02_static_presentation.de.md) als auch die [_Datenarchivierung_](../4_longterm_preservation/03_archiving_data.de.md) auf anderen Plattformen mit entsprechenden Links zu diesen Ressourcen. 
=> [Langzeitsicherungs-Dokumentation der Showcase-Edition]()

## Zugänglichkeit und Präsentation 

Eine DSE-Dokumentation kann, abhängig von Größe, Komplexität und Innovationsgehalt einer DSE, **unterschiedliche Anforderungen** zu befriedigen haben, sollte aber gewisse Grundvoraussetzungen in ihrer Präsentation erfüllen: 
Sie sollte als Dokumentation  **erkennbar** sein und auf der gleichen Ebene wie die Liste der edierten Texte, das Register oder die Suchfunktionen bereitgestellt werden. 

Grundsätzlich empfehlen wir, die Dokumentation von anderen Informationen, die keinen technischen oder editionsphilologischen Erklärungscharakter haben, zu trennen. Dies betrifft vor allem eine **Trennung** von allgemeinen Informationen zum Projektaufbau (z.B. als [_Projekteinstiegsseite_](../3_presentation/02_access.de.md) über involvierte Institutionen, Team oder Fördermittel) oder von Hintergrundinformationen zu den edierten Inhalten (als wissenschaftliche Ergänzung im Sinne von [_Übersichtskommentaren_](../2_Editionsarbeit/06_commenting.de.md)). Zitiervorschläge können in der Dokumentation enthalten sein, die Minimalanforderung ist jedoch, wie bereits erwähnt, für jede distinkte Seite einen Zitiervorschlag gut sichtbar einzublenden. Zum Zitieren einer DSE sollte nicht zwingend die Dokumentation konsultiert werden müssen. 

## Dokumentationstypen

Die **minimale Anforderung an eine Dokumentation** ist die stichwortartige Erklärung aller sichtbaren/benutzbaren Bestandteile der 
DSE und entspricht damit eher dem editorischen Kommentar im Druck. Die verschiedenen Aspekte können durch einfache Unterkapitel getrennt auf einer einzelnen Seite vereint werden, was das einfache Generieren eines PDFs ermöglicht. Dies kann für eine kleinere oder wenig komplexe DSE ausreichend sein, insbesondere wenn sie bisherige Praxis fortsetzt - in diesem Fall ist es ratsam, in der eigenen Dokumentation auf diejenige [_vorbildhafter DSE_](../1_Planung/02_Vorbildhafte_Editionen.de.md) zu verweisen. 

!!! info "Beispielhafte DSE: Minimale Dokumentation"
    Die [Digitale Edition der Reisetagebücher von Johann Conrad Fischer 1794–1851](https://johannconradfischer.com/de/content/editorial-guidelines){:target="\_blank"} ist eine optisch ansprechende DSE eines gedruckten, bereits in Buchform kritisch edierten Korpus, der nun primär die Vorteile einfacher Verlinkung und visueller Anreicherung nutzt. Da es auf etablierte Funktionen des TEI Publishers aufbaut, begnügt sich die Dokumentation mit minimalen Angaben zu [Editionsgeschichte und Technik](https://johannconradfischer.com/de/content/about){:target="\_blank"}  sowie zu den [Editionsrichtlinien](https://johannconradfischer.com/de/content/editorial-guidelines){:target="\_blank"}.    

Eine **ausführliche Dokumentation** hat demgegenüber eher den Charakter eines editorischen Nachworts und wird zur besseren Übersichtlichkeit in mehrere Unterseiten aufgeteilt. Je stärker ein DSE-Projekt innerhalb einer community Vorbild-Charakter haben soll und/oder je innovativer ein DSE-Projekt ist, desto ausführlicher sollte die Dokumentation ausfallen.  

!!! info "Beispielhafte DSE: Ausführliche Dokumentation"
    Die bereits früher erwähnte Briefkorrespondenz-DSE [hallernet](https://hallernet.org/){:target="\_blank"} ist hinsichtlich ihrer Datenbank eines der ambitioniertesten Projekte der letzten Jahre. Dass es sich hierbei in technischer Hinsicht um eine 'haute couture' Edition handelt, zeigt sich auch in ihrer [Dokumentation](https://docs.hallernet.org/guidelines/conventions/){:target="\_blank"}. Hierfür wurde eine eigene Subdomain fast ausschliesslich auf Englisch geschaffen, die drei Hauptkategorien (Guidelines/System/Usage) mit Unterkapiteln enthält. Die Dokumentation richtet sich primär an ein technisch und editionsphilologisch versiertes Publikum. 


## Tools und Datenformate 

**Verwendung von TEI/XML, z.B. zusammen mit dem TEI Publisher**

DSE können ihre Dokumentation im **selben Datenstandard**, in der Regel TEI/XML, verfassen, wie den edierten Text. Dies ist sinnvoll, wenn die Dokumentation mit demselben Tool publiziert werden soll, etwa mit dem TEI Publisher. Zu beachten ist jedoch, dass TEI/XML ein komplexeres Datenformat als normalerweise für eine Dokumentation notwendig darstellt. Das ist insbesondere relevant, wenn Teile der Dokumentation von Mitarbeitenden geschrieben, die selbst nicht in den editorischen Prozess involviert sind (z.B. technische Mitarbeitende, die für das Frontend oder die Langzeitsicherung zuständig sind) und sich deshalb in TEI/XML alleine zu diesem Zweck einarbeiten müssten. Fazit: In kleinen Teams, die mit TEI/XML vertraut sind, sind das TEI/XML-Datenformat und zugehörige tools sinnvoll. Eine vereinfachte XML Alternative, die etwa in der TEI Publisher Dokumentation verwendet wird, ist das Format [DocBook XML](https://docbook.org/). 

==->@REto: Hast Du mit DocBook Erfahrung? Ist es empfehlenswert?==   

**Verwendung von Markdown, z.B. zusammen mit MKDocs oder ähnlichen Dokumentationstools**

Markdown ist ein Datenstandard für technische Dokumentationen und bietet deshalb genügend Funktionalitäten für DSE-Dokumentationen. Es finden sich zudem verschiedene frei zugängliche Python libraries, die mit relativ einfachen Mitteln erlauben, komplexere Dokumentationen zu schreiben. Eine solche Python library, [MkDocs](https://www.mkdocs.org/) wurde für das vorliegende Handbuch verwendet. Die [Dokumentation von hallernet](https://docs.hallernet.org/guidelines/conventions/){:target="\_blank"} (s.o.) ist mit dem tool ... erstellt worden.

==Ich kläre das noch mit Peter ab==
