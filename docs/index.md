# Handbuch Proto4DigEd: Prototypische Workflows für digitale wissenschaftliche Editionen (DSE)

## 1. Das Handbuch

### Anwendungsbereiche

Das Handbuch unterstützt Forschende und Projekte aus den Geisteswissenschaften  in der Erstellung von digitalen wissenschaftlichen Editionen (digital scientific editions: DSE) in ihrer ganzen Dauer, d.h. von der Planungsphase bis zur Langzeitsicherung. Sein Fokus auf Texteditionen verdankt sich der romanistischen Modelleditin des Open Research Data Projekts [Proto4DigEd](https://www.zde.uzh.ch/de/projects/proto4diged.html) (untersützt durch swissuniversities, 2023-2024). In ihm haben Vertreter:innen der Literatur- und Geschichtschwissenschaften, der Digital Humanities sowie des Bibliothekswesens Edition-Workflows anhand eines Teilkorpus' der Korrespondenz des französischen Philologen Gaston Paris getestet und evaluiert. Im Zentrum standen dabei die Tools **Transkribus** (zur Texterkennung und Transkription) und **TEI-Publisher** (zur Annotation, Kommentierung und Publikation). 

Das Handbuch dokumentiert jedoch nicht nur besagte Tools, seine grundsätzlichen editionswissenschaftlichen Überlegungen zur Planung von Workflows lassen sich mit Einschränkungen auf Editionen nicht-textueller oder multimedialer Medien übertragen. Um auch Forschenden zugänglich zu sein, die bisher an gedruckten Editionen gearbeitet haben, verwendet es bewährte **editorische Begriffe** (Textkonstitution, Kollation, diplomatische Umschrift etc.), reflektiert jedoch deren Übertragung ins Digitale, die zu Bedeutungsverschiebungen oder Erweiterungen führen kann.   

Das Handbuch hat nicht den Anspruch, alle Facetten des Edierens abzudecken, es ergänzt bereits oder bald verfügbare Ressourcen, die einzelne Workflow-Schritte in den Blick nehmen, allen voran als Standard Nachschlagewerk das [KONDE Weißbuch](https://www.digitale-edition.at). Dieses gibt grundlegende Einblicke in verschiedene Themenfelder, bietet jedoch keine prozessuralen Überlegungen zur Planung von Workflows. Das vorliegende Handbuch verweist extensiv auf das KONDE Weißbuch um Doppelungen zu vermeiden. 
Spezifischere Handbücher sind etwa [PATT](https://www.hist.uzh.ch/de/fachbereiche/mittelalter/lehrstuehle/teuscher/forschung/projekte/PATT.html) zur automatischen Texterkennung für Historker:innen, [DigEdTnT](https://digedtnt.github.io/about/) zur Transition zwischen Tools, oder das [Handbuch zur Erstellung diskriminierungsfreier Metadaten für historische Quellen und Forschungsdaten](https://maehr.github.io/diskriminierungsfreie-metadaten/). 


### Ziele

Die hier dokumentierten, prototypischen, d.h. vorbild- und beispielhaften, Schritte in der Erstellung von DSE sollen als Wegweiser dienen. Sie geben eine Übersicht zu erprobten Workflows verfügbarer Tools (zu den Begriffen s.u.), die  unterschiedliche Grade an Fähigkeiten und Ressourcen benötigen. 

Das Handbuch reflektiert deshalb immer eine **Mehrzahl der Möglichkeiten** und hilft DSE-Projekten, diese abzuwägen. Ziel der Dokumentation ist es nicht, *den* perfekten Weg bzw. Workflow für jedes Projekt vorzuzeichnen. Sie gibt stattdessen Hinweise zur  Planung und Umsetzung von DSE, die dem Projektrahmen angemessenen sind. Diese Faktoren haben grundsätzliche Auswirkungen auf die [Planung](1. Planung/01_Projektziele_und_-ressourcen.md). 

## 2. Workflows

Unter einem **Workflow** verstehen wir die Folge aufeinander aufbauender Arbeitsschritte, deren Abschluss bzw. Vollständigkeit jeweils ein editorischer Entscheid zugrunde liegt. So ist der Abschluss der [Textkonsitution](02_Textkonsitution.md) eine - auf der Gesamtplanung beruhende - editorische Entscheidung, die es erlaubt, zur [Transkription](03_Transkription.md) des Korpus voranzuschreiten. Für diese Arbeitsschritte besteht im Handbuch je ein eigener Eintrag. Sie  lassen sich  per se auf verschiedene Mitarbeitende oder Teams aufteilen im Gegensatz zu Unterschritten, die das oftmals verbieten (u.a. weil ihre Abschliessbarkeit weniger von editorischen als von technischen Erwägungen abhängt). Die **Arbeitsteilung** innerhalb des Workflows bedarf jedoch immer genauer Planung und Koordination; sie ist nicht in jedem Fall sinnvoll. Auf besonders eng Verzahnungen von Arbeitsschritten wird im Handbuch hingewiesen.

### Komplexität 

Workflows rückten in den letzten Jahren verstärkt in den **Fokus der Digital Humanities** und insbesondere der Auseinandersetzung mit DSE (vgl. z.B. [DARIAH Annual Event 2024: "Workflows: Digital Methods for Reproducible Research Practices in the Arts and Humanities"](https://www.dariah.eu/2023/12/12/dariah-annual-event-2024-workflows-digital-methods-for-reproducible-research-practices-in-the-arts-and-humanities/)). Der Hintergrund dieses Interesses ist einerseits ein **Komplexitätszuwachs**: Die Anzahl von immer leichter zugänglichen Tools und Plattformen für DSE steigt. Aus ihnen gilt es für spezifische Projektbedürfnisse auszuwählen, um sie in einen Workflow zu integrieren und aufeinander abzustimmen. 

### Standardisierung

Andererseits steht dem Kompexitätszuwachs an verfügbaren Tools und Plattformen eine Vereinheitlichung der (Meta-)Datenformate und -standards gegenüber, insbesondere der Verwendung von [*TEI/XML*](Themen/tei.md) zur Strukturierung und Annotierung von maschinenlesbaren Editionstexten sowie die Verlinkung der Annotationen mit den Metadaten von [*Normdatenbanken*](Themen/authority.md). Diese Standardisierung der Daten und damit einhergehende Standardisierungen der Editionsrichtlinien und Funktionalitäten von DSE, zieht eine **Nachfrage nach der Standardisierung von Workflows** nach sich. Wo ähnliche Daten/Publikationen erarbeitet werden sollen, können auch ähnliche Workflows verwendet werden. Uns interessiert dabei vor allem das *Wie*: Wie und wann ist es weiterhin sinnvoll unterschiedliche, oftmals selbsterstellte Workflows zu generieren? Inwiefern lassen sich Tools und Plattformen  in best practices auf wie einheitliche Weise kombinieren? Und welche editorische und technische Einschränkungen gehen mit dieser Vereinheitlichung einher, d.h. welcher editorische Entscheidnungsspielraum geht durch sie verloren? Das Handbuch  versteht sich weniger als eine Anleitung zur Standardisierung von Workflows, als vielmehr eine Hilfe, um den Standardisierungsgrad zu ermitteln und eine projekteigene best practice zu erarbeiten. Deshalb sind die einzelnen Workflow-Kapitel nach folgendem Muster aufgebaut: 

1. Beschreibung des Workflow-Schrittes 

2. Beschreibung der vorhandenen Standards (und mögliche Alternativen) 

3. Hier sind die momentanen Tools unzureichend
    -  Wir verweien auf 'haute couture' Lösungen, d.h. 'maßgeschneiderte' Funktionalitäten, für die keine Standardisierung vorliegen   


## 3. Tools und Plattformen

Unter einem **Tool** zur Erstellung einer DSE versteht das vorliegende Handbuch jegliche relevanten technische Werkzeuge und Hilfsmittel; dies können neben Desktop- oder webbasierten Programmen auch Add-Ons oder Code-Skripts sein, die in der Anwendung unterschiedliches technisches Vorwissen benötigen. Das Handbuch bietet Hinweise darauf, in welchen Fällen wieviel Vorwissen notwendig ist. In seinem Zentrum stehen die weitverbreiteten Tools [Transkribus](https://app.transkribus.org/) und [TEI-Publisher](https://teipublisher.com/).

Neben der Kategorie der Tools ist diejenige von **(Publikations-) Plattformen** zentral, da sie Zugänglichkeit der DSE bzw. ihrer (Meta-)Daten gewährleisten. Zu ihnen zählen zentral verwaltete  Datenbanken (wie das [Swiss National Data and Service Center for the Humanities DaSCH](https://www.dasch.swiss/)), Metadatenbanken (wie [Metagrid](https://metagrid.ch/) oder [Correspsearch](https://correspsearch.net)) sowie Repositorien für verschiedene Datentypen (nicht DSE-spezifisch: Zenodo, Swissubase, GitHub/GitLab; DSE-spezifisch: TEI und Tranksripitions Datenrepositorien). Wie verschiedene Tools benötigen auch Plattformen unterschiedliche Vorkenntnisse oder Einarbeitungszeiten, vor allem aber richteten sie sich an unterschiedliche Publika und erfüllen verschiedene Zwecke. Im Gegensatz zu Tools, deren Wahl oftmals im Workflow schwer umkehrbare Weichenstellungen darstellt, ist die Verwendung mehrerer Plattformen zur [Publikation](3_Publikation/01_introduction_publication.md) und [Langzeitarchivierung](4_Langzeitarchivierung/01_introduction_preservation.md) der DSE und ihrer Daten  ausdrücklich empfohlen.

### Obszeleszenz und Innovation

Was das Handbuch in technischer Hinsicht *nicht* ist: Die dokumentierten Schritte stellen keine Anleitungen dar, wie bestimmte Tools oder Plattformen im Detail zu verwenden sind. Da die Entwicklung zurzeit so schnell  voranschreitet, führte ein hoher Detailgrad schnell zur Dokumentation von veralteten Features. Da die Handbücher zur gedruckten Editorik heute noch in ihren editorischen Überlegungen gültig sind, ist auch mit diesem Handbuch die Hoffnung verbunden, nach zukünftigen technischen Innovationen weiterhin Hilfe zu bieten.  

Eine grundsätzliche Herausforderung der digitalen Editionsarbeit ist damit bereits angesprochen: Sie ist einerseits von den Einschränkungen und Obszeleszenzen technischer Werkzeuge abhängig, andererseits erwachsen durch deren Weiterentwicklung innovative editorische Möglichkeiten. Die Balance zwischen wissenschaftlicher Notwendigkeit ("wissenschaftlich und editorisch geboten") und innovativem Surplus ("nice to have") ist darum in der Planung, insbesondere in der Abklärung der [Projektziele](1_Planung/01_Projektziele_und_-ressourcen.md) immer im Auge zu behalten.  





