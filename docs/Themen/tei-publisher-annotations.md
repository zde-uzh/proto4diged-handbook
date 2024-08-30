# Annotationen mit TEI-Publisher

TEI Publisher bietet eine Grundkonfiguration für die Annotation von XML-Daten an, die von reinen Layoutannotationen über die Verlinkung mit Registereinträgen bis zur Erstellung eines Registers gehen.
Die mitgelieferte Konfiguration kann direkt verwendet werden oder als Beispiel für Erweiterungen an die Bedürfnisse eines Projekts dienen.

Die zugrundeliegende XML-Datei wird in ein spezifisches HTML-Format übertragen und die Leerzeichen analysiert, sodass Annotationen an der richtigen Position eingefügt werden können.

## Anpassungen

Da die Annotationsansicht auf der gleichen Technologie wie die Präsentation basiert, ist die Anpassung ähnlich wie diejenige der Editionsansichten.

## Limitationen

Besonders für die Annotation mit Verknüpfung zum Register sind im Hintergrund einige Mechanismen im Gang, die um Beispiel lokale Einträge bevorzugen, häufigere Annotation priorisieren und so weiter, die bei Anpassungen berücksichtigt werden müssen. Erfahrung mit TEI Publisher sind deshalb eine Voraussetzung.

Weitere Limitationen sind interne Abhängigkeiten in Ordnern, deren Veränderung nicht empfohlen wird ([Best Practice Recommendations](https://teipublisher.com/exist/apps/tei-publisher/documentation/customization-best-practice#){:target="\_blank"}) oder Abhängigkeiten von Werten in den Webcomponents ([Webcomponent Documentation](https://teipublisher.com/exist/apps/tei-publisher/documentation/webcomponents-docs){:target="\_blank"}, vgl. auch [Changing and Debugging Webcomponents](https://faq.teipublisher.com/webcomponents/debug/){:target="\_blank"}, [Creating Custom Web Components](https://teipublisher.com/exist/apps/tei-publisher/documentation/custom-components#){:target="\_blank"}), wenn zum Beispiel eine Normdaten-API nicht unterstützt wird oder eine komplexe Annotation besondere Funktionalitäten für die Bearbeitung oder Löschung benötigt.

## Dokumentation

Folgendes Kapitel der Dokumentation ist für alle editorischen Mitarbeitenden relevant:

-   [Annotating Documents](https://teipublisher.com/exist/apps/tei-publisher/documentation/web-annotations){:target="\_blank"}

Für technische Mitarbeitende sind ausserdem folgende Kapitel zu beachten:

-   [Configuring the Annotation Editor](https://teipublisher.com/exist/apps/tei-publisher/documentation/configuring-annotation-editor){:target="\_blank"}

-   [Local authority registers](https://teipublisher.com/exist/apps/tei-publisher/documentation/registers){:target="\_blank"}
