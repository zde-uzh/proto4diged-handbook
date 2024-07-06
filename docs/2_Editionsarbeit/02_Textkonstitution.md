# Textkonstitution

Die Textkonsitution bezeichnet das Zusammenstellen der zu edierenden Texte. Falls es sich um eine textgenetisch ausgerichtete Edition handelt, d.h. falls die Entstehungs- und Publikationsgeschichte eines Werkes nachvollziehbar gemacht werden soll, umfasst die Textkonstitution das **Auffinden und die Auswahl aller zu edierenden Textstufen** (Manu- oder Typoskripte und Korrekturfahnen, die im Schaffensprozess entstanden sind) **und der Textausgaben** (verschiedene autorisierte oder nichtautorisierte Drucke, ggfls. ebenfalls mit händischen Notizen oder Korrekturen von Autor:innen, Lektor:innen und Herausgeber:innen).

Die editionsphilologischen Überlegungen in der Textkonstitution erscheinen auf den ersten Blick unabhängig davon, ob die angestrebte Edition digital oder gedruckt sein soll. Tatsächlich spielt es jedoch eine Rolle, wo sich die zu edierenden Textzeugen befinden und wie ihre Zugangs- und Publikationsrechte sind, da unterschiedliche Publikationsformen (open/restricted/closed access, mit oder ohne Digitalisat) daraus resultieren können, wie im Folgenden gezeigt wird. 


## Zugang zum Textträger und Publikationsrechte
Die Textkonstitution ist damit verbunden, ob und wie die physischen **Textträger zur Transkription zugänglich sind** bzw. gemacht werden können. Eine Edition kann sich gegen die Edition von Textträgern entscheiden, wenn diese schwer zugänglich und mit großem (finanziellen, logistischen oder rechtlichen) Aufwänden verbunden sind. Möglicherweise sind Textträger sogar schon digitalisiert vorhanden und auf der Datenbank einer Gedächtnisinstitution (s.u.) oder archive.org abrufbar.

Für DSE gehört ein weiterer Schritt zur Textkonstitution, der die Entscheidungen über die Edition eines Textträgers entscheidet: Das Erstellen(-lassen) der Digitalisate und die **rechtlichen Modalitäten**, wie sie der Edition zur Verfügung gestellt werden. Die Besitzer:innen eines Textträgers können eine digitale, breit zugängliche Veröffentlichung des Digitalisats verbieten und/oder starke urheberrechtliche Restriktionen fordern. Dies kann ein Grund sein, ganz von der Edition des Textträgers abzusehen. Versuche, urheberrechtlichen Einschränkungen zu genügen, können dazu führen, dass die Digitalisate der Textträger nur im Arbeitsprozess Verwendung finden und nicht veröffentlicht werden und die Transkriptionen mit einem Kopierschutz ausgestattet sind. 

Dieser Weg geht beispielsweise die online Ausgabe der [Stoffe-Edition](https://fd-stoffe-online.ch/) Friedrich Dürrenmatts: Die Digitalisate lassen sich zwar einblenden, aber nicht als PDF herunterladen, der transkribierte Text lässt nur die Kopie einer bestimmten Zeichenzahl zu und liegt nicht als TEI XML vor. Diese beschränkte Funktionalität, die von mittlerweile etablierten DSE-Daten- und Präsentationtsstandards abweicht, wurden aus einer Open Access Perspektive in einem [Review der Zeitschrift RIDE](https://ride.i-d-e.de/issues/issue-17/duerrenmatt/) (A review journal for digital editions and resources) kritisiert. Das Stoffe-Projekt ist beispielhaft für einen früh in der Planungsphase getroffenen Kompromiss: Die Entscheidung, einen rechtlich geschützten Text überhaupt zugänglich machen zu wollen, kann mit großen Einschränkungen einhergehen. 

## Wege zum Digitalisat

Sind rechtliche Fragen geklärt, stellen sich institutionelle und technische Fragen in der digitalen Textkonstitution, die weitreichende Folgen bis zur langfristigen Publikation und Langzeitsicherung haben . Wir unterschieden drei grundsätzliche Wege zum Digitalisat, seiner Verfügbarmachung und seiner Einbindung in die DSE.  

**1. Digitalisierung und Verfügbarmachungung durch eine Gedächtnisinstitution**

Hierbei handelt es sich um den angestrebenswerten Standard beziehungsweise die *best practis* auf dem Weg zum Digitalisat:  Die Gedächtnisinstitution (Archiv, Bibliothek, Museum o.ä.), welche den Textträger besitzt,  digitalisiert diesen und macht ihn digital öffentlich zugänglich. Die Digitalisierung geschieht nach etablierten Normen (z.B. ISO-Standards) und in gleichbleibender Qualität. Sie wird nach dem Digitalisierungsprozess durch die Gedächtnisinstitution auf einer Datenbank langzeitarchiviert.

 Solche öffentliche Datenbanken werden meist von einen Verbund von Gedächtnisinstitutionen betrieben, für die Schweiz z.B. im Kanton Waadt [Patrinum](https://patrinum.ch/?ln=fr) oder in der Deutschschweiz [e-manuscripta](https://www.e-manuscripta.ch). Dort werden die Bilddaten mit dem [IIIF-Standard](https://www.digitale-edition.at/o:konde.123) zugänglich gemacht. D.h. jedes Bild des digitalisierten Textträgers erhält einen persistente Identifikator (URI) und kann über entsprechende Schnittstellen angesteuert werden.

 Der große Vorteil dieses Wegs ist es, dass die Langzeitsicherung der Bilddaten nicht in der Hand eines temporär begrenzten Projektes liegt. Dies folgt der modularen Logik, den Betrieb und die Sicherung der verschiedenen DSE-Bestandteile voneinander unabhängig zu gestalten und insbesondere Bilddaten, Editions-Datenbank (TEI-XML-Daten) und Editions-Frontend voneinander getrennt zu halten, so dass sie bei Bedarf anderen Institutionen übergeben oder mit neuen technischen Lösungen ersetzt oder ergänzt werden können. 

**2. Digitalisierung durch eine Gedächtnisinstitution, Verfügbarmachung durch das Projekt** 

Sollte die Gedächtnisinstitution das Digitalisat nicht selbst auf einer Datenbank zur Verfügung stellen - sei es, weil sie keine solche Datenbank besitzt oder weil der Textträger nicht aus den eigenen Beständen stammt - ist auch die Verwendung eines IIIF-Servers einer weiteren Institution möglich. Universitätsbibliotheken bieten Projekten mittlerweile oftmals Speicherplatz auf einem solchen Server zum Unkostenbeitrag an. Dieser zusätzliche finanzielle Aufwand muss - wie alle weiteren Server-Kosten - über die Projektlaufzeit hinaus beantragt werden. Die Bilddaten sind in diesem Fall nicht unabhängig über eine Datenbank abrufbar, können aber über eine eigene URI unabhängig übers Internet angesteuert werden (wenn diese URI bekannt ist).   

**3. Digitalisiserung und Sicherung durch das Projekt**
