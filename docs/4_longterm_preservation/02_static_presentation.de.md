# 4.1 Statische Präsentation

## Warum statische Präsentationen von DSE?
Wie in der Einleitung zur Langzeitsicherung beschrieben, erscheinen statische Präsentationsformen zurzeit (Stand 2024) als erfolgsversprechende Lösung, um eine **langfristige Sicherung einer DSE inklusive der meisten ihrer Nutzerfunktionen** zu gewährleisten. Eine statische DSE-Präsentation besteht primär aus HTML-Dateien, die vorgeneriert wurden. Dadurch fällt die Wartung einer Datenbank, wie sie für dynamische Präsentationen notwendig ist, weg. Domänenspezifisches Wissen über XML-Datenbanken und ihre Langzeitwartung sind somit nicht mehr nötig. Statische Websites können von technischen DH- und DSE-Spezialist:innen z.B. an einen **generalistischen IT-Dienst** einer Forschungs- oder Gedächtnisinstitution übergeben werden, der auch mit der Wartung anderer einfacher Websites betraut ist.  

???+ question "Statische vs. dynamische Webpräsentationen"
    **Dynamische Präsentation mit Datenbank**

    ![alt text](Web_server_serving_static_and_dynamic_content.png)

    CC BY-SA 4.0: Ade56facc [https://commons.wikimedia.org/wiki/File:Web_server_serving_static_and_dynamic_content.png](https://commons.wikimedia.org/wiki/File:Web_server_serving_static_and_dynamic_content.png){:target="\_blank"} 

    **Statische Präsentation ohne Datenbank** 
    
    ![alt text](Web_server_serving_static_content.png)

    CC BY-SA 4.0: Ade56facc [https://commons.wikimedia.org/wiki/File:Web_server_serving_static_content.png](https://commons.wikimedia.org/wiki/File:Web_server_serving_static_content.png){:target="\_blank"}



## Statische Präsentation mit dem TEI Publisher 10

In der Version 9 des TEI Publisher ist eine Publikation der DSE nur als dynamische Präsentation vorgesehen. Hierfür wird im TEI Publisher [eine dynamische App generiert](https://teipublisher.com/exist/apps/tei-publisher/documentation/create-app){:target="\_blank"}, die danach gewartet werden muss. Für die Version 10 des Publishers soll ein **statischer Generator** zum zentralen Bestandteil der Publikationsmöglichkeiten werden. Hinzu kommt ein **App Manager**, der den Prozess, eine custom App einer Edition zu machen, automatisiert. 
Idealerweise wird es so möglich, verschiedene Versionen von statischen Präsentationen im Verlaufe des Projektes auszugeben und zu testen. 

Vorgesehen sind auch Zwischenformen, die gewisse dynamische Funktionen der Präsentation erhalten. Falls diese Funktionen nicht länger gewartet werden können, soll die restliche DSE funktional bleiben.  

## Andere statische Präsentationstools

Schon heute existieren tools bzw. scripts, welche die Umwandlung von dynamischen Websites in statische Websites erlauben. Deren Anwendung ist jedoch mit einem größeren technischen Wissen verbunden, als es die Anwendung des oben angekündigten statischen Generators in TEI Publisher verspricht.

- Bereits für ältere Versionen des TEI Publisher zur Anwendung gekommen ist [Eleventy](https://www.11ty.dev/){:target="\_blank"}. e-editiones hat 2022 ein eigenes [Plugin von Eleventy für den TEI Publisher](https://github.com/eeditiones/tei-publisher-eleventy){:target="\_blank"} entwickelt und seine Benutzung ausführlich [dokumentiert](https://www.e-editiones.org/posts/community-event-going-static/){:target="\_blank"}.

-  Das [Austrian Centre for Digital Humanities and Cultural Heritage (ACDH-CH)](https://www.oeaw.ac.at/acdh/acdh-ch-home){:target="\_blank"} hat mit dem tool [DSE-Static-Cookiecutter](https://github.com/acdh-oeaw/dse-static-cookiecutter?tab=readme-ov-file){:target="\_blank"} einen statischen Website-Generator für DSE entwickelt, der z.B. für verschiedene Editionen zu Arthur Schnitzler zum Einsatz kommt oder kommen soll (Schnitzlers [Tagebuch](https://schnitzler-tagebuch.acdh.oeaw.ac.at){:target="\_blank"}, seine [Briefe](https://schnitzler-briefe.acdh.oeaw.ac.at/){:target="\_blank"} sowie [Briefe und Materialien seiner Korrespondenz mit Hermann Bahr](https://schnitzler-bahr.acdh.oeaw.ac.at/){:target="\_blank"}). Der Vorteil dieses tool ist, dass es direkt über eine GitHub-Instanz TEI/XML-Quelldaten auf einem GitHub-Repositorium als statische Website veröffentlichen kann (die [_Archivierung der Daten_](../4_longterm_preservation/03_archiving_data.de.md){:target="\_blank"} und ihre Präsentation sind somit direkt miteinander verknüpft und eine neue Version des Datenstandes führt automatisch zu einer neuen Version der Präsentation). 

    ==->@Reto: Du hast mir mal von dieser Lösung erzählt, als sie noch in Planung war, ich habe es nun genauer angeschaut und bin sehr überzeugt, kann aber v.a. die Limitationen (falls es welche gibt) nicht abschätzen - ausser dass es ev. mehr technisches Know-How als der TEI Publisher 10 braucht.== 

- Zu den weitverbreitetsten tools, die statische Websites generieren, gehört [Jekyll](https://jekyllrb.com/){:target="\_blank"}, das tool hinter der Ausgabe von GitHub-Pages. Eine Anwendung für DSE-Projekte ist uns bislang jedoch nicht bekannt.  

    ==->@Reto: liegt das ggfls. daran, dass es primär zur Ausgabe von MD-Dateien dient, d.h. XML gar nicht abgedeckt wird? Falls ja: Soll es überhaupt hier aufgeführt werden? Gibt es andere static generators, die sinnvoller wären?==

## Limitationen 

Für komplexe Editionen, die auf eine **große Datenbank** angewiesen sind und diese **konstant erweitern** möchten, ist das Generieren einer statischen Präsentation wenig sinnvoll. Zwar ist der Aufruf einer statischen Website schneller, sie bildet jedoch immer nur eine vorgenerierte Momentaufnahme ab, die bei fortlaufendem work in progress schnell veraltet. 

Bei der Umwandlung in statische Präsentationen ist ferner zu beachten, dass gewisse **Suchfunktionen** sowie die **Darstellung von Zeitstrahl- oder geografischen Karten-Visualisierungen** wegfallen können. So ist eine statische Präsentation mit dem oben erwähnte TEI Publisher-Plugin von Eleventy auf einfache Suchen beschränkt, d.h. die Möglichkeit einer [Facettensuche](https://de.wikipedia.org/wiki/Facettensuche), wie sie Datenbanken ermöglichen, fällt weg. Visualisierungs-tools, die auf externe Ressourcen zurückgreifen müssen, könnne zwar in eine statische Präsentation integriert blieben, ihr Funktionieren hängt jedoch von der externen Ressource ab.     
