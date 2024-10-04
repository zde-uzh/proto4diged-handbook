# 2. Datenarchivierung

## Wozu dient die Archivierung von DSE-Datensätzen?

Wie in der Einleitung zur Langzeitsicherung erwähnt, eröffnet die Archivierung von DSE als Datensätze verschiedene Nutzungsmöglichkeiten für distant-reading Ansätze oder computerlinguistische Methoden. Die Daten lassen sich für verschiedene Zwecke neu visualisieren, wie es etwa das entstehende Visualisierungs- und Forschungstool [ORD-Explore](https://libraries.dsi.uzh.ch/project/ord-xplore/#content){:target="\_blank"} für eine Vielzahl von DSE durch den Upload ihrer TEI/XML-Daten ermöglichen soll. 

Schließlich erlaubt eine vollständige Daten-Archivierung eine spätere Neuveröffentlichung mithilfe neuer tools in einem neuen bzw. nachgebauten Frontend. Voraussetzung für eine solche 'Wiederbelebung' archivierter Daten ist jedoch eine lückenlose technische [_Dokumentation_](../3_presentation/04_documentation.de.md), die das korrekte Zusammenspiel der Datensätze erklärt. 

## Kuratierte Archivierung 

Auf geisteswissenschaftliche Daten spezialisierte Institutionen können eine kuratierte Archivierung der Daten anbieten, d.h. sie haben ein fachspezifisches Wissen für die Standarddatenformate und machen diese entsprechend präsentier- bzw. durchsuchbar. Zudem garantieren sie in der Regel eine **Mindestsicherung von 10 Jahren**. Es kann jedoch davon ausgegangen werden, dass die Daten über wesentlich längere Zeiträume verfügbar bleiben, so lange diese Institutionen existieren. 

Die derzeit in der **Schweiz** praktizierte und durch den Schweizer Nationalfonds unterstützte Standardlösung ist eine Archivierung der kompletten Daten im [Swiss National Data and Service Center for the Humanities DaSCH](https://www.dasch.swiss/){:target="\_blank"}. Unterschiedliche Projekte sind in derselben Datenbank, der Data Service Plattform (DSP), abgelegt, was mit zunehmender Datenmenge den Vorteil einer breiten übergreifenden Suche in DaSCH Ressourcen ermöglicht. Neben DSEs befinden sich dort auch andere geisteswissenschaftliche Datensätze wie Lexika, Fotografiesammlungen oder Bibliographien. Das DaSCH vergibt zudem für die einzelenen Projektdaten einen [ARK-Identifier](https://arks.org/){:target="\_blank"}, d.h. einen persistenten, zentral registrierten Ansteuerungspunkt im Internet.     
Die Archivierung im DaSCH kann auf zwei verschiedene Weisen geschehen: 

- Als **einfaches Datenmodell**: Dem DaSCH werden die TEI/XML Dateien plus elementare Metadaten geliefert. Diese Metadaten sind dann auf der Data Service Plattform (DSP) im Volltext durchsuchbar. 

- Als **elaboriertes Datenmodell**: In Zusammenarbeit mit dem DSE-Projekt modelliert das DaSCH einen Teilen der Daten als RDF-Datenbank auf der DSP. Dadurch werden komplexere Suchen nach Relationen zwischen den Datensätzen möglich. Ein Beispiel hierfür ist die [Briefedition Bernoulli-Euler Online](https://app.dasch.swiss/project/yTerZGyxjZVqFMNNKXCDPF){:target="\_blank"}. Sie erlaubt neben der Darstellung der Faksimiles (die auf dem DaSCH-eigenen IIF-Server gespeichert werden können) auch eine generische Publikation des TEI/XML Dokuments sowie eine Durchsuchbarkeit nach Register.    

==-> @Rita: ist das korrekt so?== 

In **Österreich** ist eine Langzeitarchivierung der Daten im [Geisteswissenschaftliches Asset Management System GAMS der Universität Graz](https://gams.uni-graz.at/){:target="\_blank"} möglich, jedoch ist dies Dienstleistung primär für Projekte und Kooperationen der Universität Graz vorgesehen. Ähnlich archiviert das [Austrian Centre for Digital Humanities and Cultural Heritage (ACDH-CH)](https://www.oeaw.ac.at/de/acdh/acdh-ch-home) der österreichischen Akademie der Wissenschaften die Daten ihrer DSE in der Datenbank [ARCHE](https://arche.acdh.oeaw.ac.at/browser/){:target="\_blank"}.  

==-> @alle: Gibt es diesbezüglich bundesdeutsche Äquivalente?==

## Archivierung als Datensicherung

Neben disziplinär spezifischen Datenbanken wie dem DaSCH oder GAMS ist es auch möglich, die Daten **ohne fremde Kuratierung** in einer wissenschaftlichen Datenbank abzulegen. Hierfür bietet sich etwa die von CERN und OpenAIRE gewartete Datenbank [**Zenodo**](https://zenodo.org/). Eine Strukturierung oder Kuratierung der Daten ist nur bedingt möglich und muss durch das Projekt selbst durchgeführt werden. Viele Projekte entscheiden sich darum, 'Datenbankdumps', also unkuratierte Abbilder der eigenen Datenbank, auf Zenodo abzulegen. Diese Kopien können versioniert werden und erhalten als ganzes eine [DOI](https://www.doi.org/), d.h. ebenfalls einen persistenten, zentral registrierten Ansteuerungspunkt im Internet.  Ein Beispiel ist etwa der Datenbankdump des etwas älteren Projektes [Cædmon’s Hymn
A multimedia study, edition and archive](https://caedmon.seenet.org/), das unter der DOI [10.5281/zenodo.1226549](https://zenodo.org/records/1226549) auf Zenodo gesichert wurde.

Auf ähnliche Weise wie Zenodo können auch andere wissenschaftliche Daten-Repositorien wie wie [**GitHub**](https://github.com/){:target="\_blank"} oder [**OLOS**](https://access.olos.swiss/portal/home){:target="\_blank"} genutzt werden. Ein bereits erwähntes Beispiel, in dem die Datenarchivierung und die  statische Präsentation der Daten Hand in Hand geht, ist das [GitHub-Repositorium](https://github.com/arthur-schnitzler){:target="\_blank"} der DSE [Arthur Schnitzler Briefe](https://schnitzler-briefe.acdh.oeaw.ac.at/index.html){:target="\_blank"} und weiterer Projekte, die das tool [DSE-Static-Cookiecutter](https://github.com/acdh-oeaw/dse-static-cookiecutter?tab=readme-ov-file){:target="\_blank"} verwenden. Die Quelldaten auf GitHub werden mit de  ssen Hilfe über eine weitere [GitHub-Instanz](https://github.com/arthur-schnitzler/schnitzler-briefe-static/){:target="\_blank"} zu einer statischen Website weiterverarbeitet. 

Der SNF gibt eine [**Übersicht über empfehlenswerte Repositorien**](https://www.snf.ch/en/WtezJ6qxuTRnSYgF/topic/open-research-data-which-data-repositories-can-be-used), die ihre Anforderungen an open research data Standards erfüllen. 

## Archivierung von Transkriptionsdaten

Für den spezifischen Nachnutzungszweck, [_ATR-Modelle zu trainieren_](../2_Editionsarbeit/03_Transkription.de.md), können im Repositorium [htr-united](https://htr-united.github.io/){:target="\_blank"} PAGE- und Alto-XML-Daten abgelegt werden (auch txt-Daten sind dort willkommen, solche Fallen aber in den hier beschriebenen Workflows nicht an).

Einen breiteren Nachnutzungszweck verfolgt [transcriptiones](https://transcriptiones.ch/){:target="\_blank"}, das es primär Historiker:innen erlaubt, anderswo nicht veröffentlichte Transkriptionen von Quellen einfach abzulegen und zugänglich zu machen. Eine Beschränkung von Datenformaten gibt es nicht, die rechtlichen und technischen Hürden zur Publikation werden absichtlich sehr niedrig gehalten (generische Darstellung, keine Faksimiles). Da  DSE-Projekten in der Regel ihre Daten bereits anderswo präsentieren und archivieren, ist transcriptiones eher als zusätzliche Ablagemöglichkeit zu verstehen.  

## Archivierung/Teilen von Metadaten

Sogenannte Metadaten-[Aggregatoren](https://www.digitale-edition.at/o:konde.49){:target="\_blank"} vernetzen Metadaten miteinander und Verweisen auf deren Ressourcen zurück. Besonders hervorzuheben ist der Aggregator [**correspSearch**](https://correspsearch.net/de/start.html){:target="\_blank"}, der Korrespondenz-Metadaten (Personen, Orte, Sende- und Empfangsdaten etc.) von 490 DSE zusammenträgt (Stand 2024). Die Metadaten müssen vor Übergabe an correspSearch aus der TEI/XML-Codierung [CorrespDesc](https://tei-c.org/release/doc/tei-p5-doc/en/html/ref-correspDesc.html){:target="\_blank"} in das [Correspondence Metadata Interchange-Format (CMIF)](https://correspsearch.net/en/documentation.html){:target="\_blank"} übertragen werden. Wichtig für das Teilen der Metadaten mit correspSearch ist deshalb, von Anfang an Korrespondenzen nach den Codierungsrichtlinien CorrespDesc auszuzeichnen.   

Ein weiterer Metadaten-Aggregatoren ist die Schweizer Plattform [**Metagrid**](https://metagrid.ch/){:target="\_blank"}, die die biographische Daten geisteswissenschaftlicher Online-Ressourcen vernetzt. Es ist besonders attraktiv für Schweizer DSE-Projekte, da bereits verschiedene Schweizer DSE, Datenbanken, Archive und Bibliotheken ihre Metadaten hier teilen.  

==-> @alle: Gibt es weitere Metadaten-Aggregatoren, die für DSE relevant sind?==

## Bekannt- und Zugänglichmachen

Das Teilen der Metadaten dient nicht nur der Vernetzung von open linked data, es macht auch auf ein Projekt aufmerksam. Letztlich sollten zu diesem Zweck Projektinformationen **möglichst breit gestreut** werden. Dies kann dadurch geschehen, indem das Projekt bei Fertigstellung den großen [**_Übersichten und Sammlungen von DSE_**](../1_Planung/02_Vorbildhafte_Editionen.de.md), die in diesem Handbuch erwähnt wurden, gemeldet werden. Besonders wichtig erscheint uns dabei der [**Catalogue Digital Editions**](https://dig-ed-cat.acdh.oeaw.ac.at/), da dieser die Editionsdaten mit dem **German Library Network (DBIS)** vernetzt; es ist zu hoffen, dass ähnliche Lösungen auch für nicht-deutsche **Bibliotheksnetzwerke** gefunden werden. 

==-> @Yann ist da glaubs dran, ist da schon was spruchreif?== 

Ansonsten ist es sinnvoll, DSE selbst den relevanten Bibliotheksnetzwerken als Online-Ressource zu melden, so dass sie über Bibliothekssuchen einfach auffindbar sind. 
