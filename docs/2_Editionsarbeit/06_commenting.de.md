# 2.5 Kommentierung

## Formen der Kommentierung in DSE

Der Kommentar erlaubt es in gedruckten und digitalen Editionen über textkritische und inhaltliche Annotationen hinaus Texte mit Kontextinformationen anzureichern. Kommentare stellen meistens das Resultat von Forschung dar, seien es Recherchen, die eng mit der [_Textkonsitution_](02_Textkonstitution.de.md) verbunden sind und damit keinen größeren Zusatzaufwand darstellen, oder Recherchen, die parallel zum Editionsvorhaben als eigenständige Forschungsarbeit stattfindet und z.B. auch in Aufsätzen oder Monographien weitergenutzt werden.

In der klassischen Print-Editorik kennt man drei verschiedene Grundformen des Kommentars, die in anderer Form alle auch in DSE zur Anwendung kommen:

1.**Der editorische Kommentar** (oder auch Herausgeberkommentar, editorischer Bericht etc.) erklärt mindestens die editorischen Richtlinien, ggfls. die Auswahl des Corpus aufgrund seiner Entstehungsgeschichte und die Nutzung des textkritischen Apparats. Diese Kommentarform ist in DSE eher als [_Dokumentation_](../3_presentation/05_documentation.de.md) bekannt und wird im Folgenden unter dieser Bezeichnung im Kapitel Publikation behandelt.

!!! info "Beispielhafte DSE"
In hybriden Ausgaben wie der [Faustedition](https://www.faustedition.net/) sind zuweilen auch der editorische Bericht (der für die digtale und die gedruckte Ausgabe gilt) und die technische Dokumentation voneinander getrennt.

2.**Der Überblickskommentar** (oder auch Einführugnskommentar, Themenkommentar, Sachkommentar zum Gesamttext etc.) bezieht sich auf einen edierten Inhalt als Ganzes, sei dies ein Themengebiet, ein Werkkomplex oder ein Text. In historisch-kritischen Ausgaben dient er oft dazu, Inhalte zusammenzufassen (im Fall von historischen Quelleneditionen und Briefedtionen auch Regest genannt), ihre Entstehung (Textgenese, Intertextualitä), Publikations-und Rezeptionsgeschichte zu beleuchten und zuweilen sogar einen Überblick über Interpretationen in der Sekundärliteratur zu geben. Verschiedene Formen von Übersichtskommentaren existieren auch in DSE, nur sind sie selten als ein Fließtext gebündelt, sondern finden sich auf verschiedenen hierarchischen Ebenen näher am kommentierten Inhalt (z.B.: Einführung in die Abteilung Briefe, Einführung in eine spezifische Korrespondenz, Einzelbriefregeste). Da es sich dabei um einzelne, mit dem edierten Text nur lose verknüpfte Texte handelt (die im idealfall wie der edierte Text als TEI/XML ausgegeben werden können) sind die technischen und editorischen Aspekte wenig komplex und müssen nicht weiter ausgeführt werden.

!!! info "Beispielhafte DSE"
Vorbildhaft sind die Überblickskommentare der [edition humboldt digital](https://edition-humboldt.de), die zu jeder Briefkorrespondenz eine eigene Einführung vorlegt (ähnlich gehen die später erstellten Briefeditionen in [haller.net](https://hallernet.org) vor). Die einzelnen Reisetagebücher Humboldts weisen neben einem solchen "Einstieg" jeweils auch "Forschungsdossiers" auf, die klassische Überblickskommentare durch ihren Detailgrad teilweise übersteigen. Eine solche Anreicherung der Edition durch thematische Aufsätze kann ihren Forschungsnutzen unter Beweis stellen. Letztlich weist die edition humbodlt digital zuweilen auch noch einen detaillierten Überblickskommentar auf der Ebene der Einzeltexte auf. Dieser Kommentar wird "Anmerkung" genannt und erscheint als Hoover-Text, wenn die Metadaten aufgerufen werden. Er beschränkt sich primär auf die Datierung und Struktur des einzelnen Dokuments.  
 Eine Verzweigung in verschiedene Überblickskommentare ist im Falle eines einzelnen edierten Textes wie einem Roman nicht nötig. Der [Überblickskommentar der Lokalbericht Edition](https://www.lokalbericht.ch/kommentar) ist deshalb als Fließtext strukturiert, der durch Verlinkung eng mit einzelnen Editionsabschnitten verbunden ist.

3.**Der Stellenkommentar** bezieht sich auf eine einzelne Textstelle, deren Länge von einem Einzelwort bis zu Passagen von mehreren Absätzen reichen kann. Gedruckte Ausgaben kennen sowohl die Stellenkommentierung in unmittelbarer Nähe des Textes (am Seitenrand, als Fussnote) oder in einem Kommentarapparat (durch Endnoten, Zeilennummern und/oder Lemmata gegliedert). DSE haben auch hier den Vorteil, Stellenkommentare stärker mit dem kommentierten Inhalt zu verknüpfen. Verschiedenen Wege, digitale Stellenkommentare zu erstellen, werden im Folgenden genauer beleuchtet.

## Workflows für Stellenkommentare

Von 'Standard-Workflows' wie in den anderen Kapiteln zu Editionsarbeiten kann an dieser Stelle (noch) nicht die Rede sein, da Editionen **sehr unterschiedliche Bedürfnisse** der Stellen-Kommentierung aufweisen und oftmal sogar ganz darauf verzichten. Die Notwendigkeit für Stellenkommentare hat im Vergleich zu Print-Editionen abgenommen, da sich viele heute durch [_inhaltliche Annotationen_](05_semantic_annotation.de.md) ersetzen lassen.

Falls Stellenkommentare erstellt werden, ist jedoch deren 'Verankerung' bzw. Codierung im TEI-XML sehr einheitlich, da sie einfachheitshalber als `<note>` eingefügt werden. => Hier ev. Code-Snippet aus der Showcase-Edition einfügen oder besser direkt mit TEI-XML verlinken.

Die Codierung in TEI/XML sagt freilich noch nichts darüber aus, **wie der Stellenkommentar letztlich dargestellt wird**; dies hängt von der Wahl des ODDs und der Technik des Publikationstools ab. Im Falle des TEI Publishers werden Stellenkommentare zurzeit als Endnote unter dem edierten Text dargestellt. Der Endnotenanker im Fliesstext ist (wie etwa aus Word bekannt) so mit der Endnote verknüpft, dass bei Daraufklicken die Seite zur Endnote scrollt. Für die Schowcase-Edition haben wir diese Funktion dahingehend erweitert, dass auch ein Hoover-Text erscheint, wenn der Cursor über den Endnotenanker gesteuert wird.

![Kommentierung im TEI Publisher in Endnoten mit TEI-XML](image-5.png)

Da Stellenkommentare auf Seiten der Codierung einfach **als Annotationen zu handhaben** sind, lassen sie sich im TEI-Publisher im Annotations-Editor einfügen. Zurzeit lassen sie sich jedoch im Editor nicht löschen, sondern müssen manuell aus der TEI/XML-Datei gelöscht werden. Um nicht zu oft im TEI/XML arbeiten zu müssen, hat sich die Showcase-Edition dafür entschieden, solche Löschungen zunächst mit einer To-Do-Annotation zu markieren und sie später gebündelt durchzuführen.

Zur einheitlichen Anwendung von Stellenkommentaren ist es sinnvoll, diese in Editionsrichtlinien festzuschreiben.

!!! abstract "Showcase-Editionsrichtlinien: Kommentierung"
=> @ Ursula: Eigentliche Kommentar-Richtlinien haben wir noch nicht festgelegt, das Kommentieren fällt v.a. in Deine Expertise. Warum soll wann was kommentiert werden?
