# 1.1 Festlegung der Projektziele

Anders als zumindest ideell ergebnisoffene geisteswissenschaftliche Forschung müssen DSE **von ihrem Endprodukt aus gedacht** werden. Die Planung hat sich an einem Modell der fertigen Edition und deren Verwendungszwecken zu orientieren und vom angestrebten Ergebnis aus die notwendigen Workflow-Schritte zurückzugehen - freilich nicht, ohne dieses Ergebnis im Planungsprozess kontinuierlich anzupassen.

Wir skizzieren im Folgenden Fragen und Herausforderungen, die ein Projekt in der Planungsphase für sich im Sinne einer **Requirement-Prüfung** klären sollte. Die provisorischen Antworten sollen mithilfe dieses Handbuchs in der Planungsphase konkretisiert werden.

### 1. Ausgangslage: Projektrahmen und Ressourcen

Bevor eine Detailplanung des Endproduktes beginnen kann, sollten folgende Faktoren evaluiert werden:

-   Beschaffenheit und Quantität der zu edierenden Medien (siehe [_Textkonstitution_](../2_Editionsarbeit/02_Textkonstitution.de.md))
-   Teamgröße und -fähigkeiten

-   Projektdauer

Inwiefern diese Faktoren anpassbar sind, hängt von der institutionellen und finanziellen Ausgangslage ab, insbesondere möglicher Fördermittel. Im Falle der Schweiz ist Stand Sommer 2024 z.B. eine öffentliche Förderung von größeren DSE nur im Rahmen eines 4-jährigen [Projektantrags beim Schweizer Nationalfonds](https://www.snf.ch/de/WAvYcY7awAUGolST/foerderung/projekte/projekte-in-allen-disziplinen){:target="\_blank"} möglich.

### 2. Zusammenspiel der technischen Komponenten

Ein technischer Grundsatz von DSE ist die **modulare Logik**, den Betrieb und die Sicherung der verschiedenen DSE-Bestandteile voneinander unabhängig zu gestalten. Insbesondere Bilddaten, Editions-Datenbank (TEI/XML-Daten) und Editions-Frontend sollten voneinander getrennt gehalten werden, so dass sie bei Bedarf anderen Institutionen übergeben oder mit neuen technischen Lösungen ersetzt oder ergänzt werden können.

Bevor Tools und Plattformen festgelegt werden, sollten sich DSE-Projekte Gedanken über das Zusammenspiel der technischen Komponenten machen.

-   Gibt es eine **technische Leitung**, die sich mit allen Komponenten auskennt?

    -   Falls nicht, wie wird das Zusammenspiel koordiniert?

-   Werden alle verfügbaren **technischen Komponenten wirklich benötigt**?
    -   Kleine Projekte können z.B. auf Metadaten-Datenbanken verzichten und ihre Metadaten in Excel- bzw. CSV-Files kuratieren.

### 3. Rolle des Frontends

-   Muss am Schluss eine möglichst einfach zu wartende digitale Publikation der Oberfläche vorliegen (siehe [_statische Präsentation_](../4_longterm_preservation/02_static_presentation.de.md))?
-   Werden physische Prints vorgesehen, die auf einer [_Lesefassung_](../3_presentation/03_edition_views.de.md) aufbauen? Ist das Frontend eine Zwischenstufe?

### 4. Verschiedene Formen des Outputs (Publikation und Nachnutzung)

-   Wie sollen die **Daten** der Edition genutzt werden?

    -   Zur qualitativen Analyse (z.B. historische Quellenauswertung, philologische textgenetische oder hermeneutische Methoden)? Dann lohnt sich wahrscheinlich eine Konzentration auf eine komplexe [_digitale Präsentation_](../3_presentation/01_introduction_presentation.de.md).
    -   Zur quantitativen Analyse (z.B. korpuslinguistische Analysen, philologische distant-readings, statistische Fragestellungen)? Dann steht die [_Langzeitsicherung in Datenbanken_](../4_longterm_preservation/03_archiving_data.de.md) im Vordergrund.

### 5. Wo lohnen sich für das Projekt Automatisierungen?

Repetitive Arbeiten sind für **Automatisierung** prädestiniert, aber nicht jede repetitive Arbeit lohnt sich zu automatisieren (konkret: was dauert länger: das Anpassen/neu Schreiben eines python scripts oder die repetitive Arbeit einer wissenschaftlichen Hilfsassistenz?). Entsprechendes technisches Wissen muss für das Projekt angeworben werden.
