============================================================================================
=============================== dcat-ap.de readme für 2.0 ==================================
============================================================================================

In Version 2.0 ist die größte und offensichtlichste Änderung, die Verwendung von ReSpec, um Spezifikation und Konventionenhandbuch als moderne Web-Version zu veröffentlichen. 
Mit der Umstellung ging eine redaktionelle Überarbeitung der meisten Texte einher.

Detaillierte Changelogs finden Sie unter
Spezifikation:        https://www.dcat-ap.de/def/dcatde/2.0/spec/#anderungen-in-der-version-2-0
Konventionenhandbuch: https://www.dcat-ap.de/def/dcatde/2.0/implRules/#anderungen-in-der-version-2-0


Wesentlichte Änderungen in der Spezifikation:
 - Übernahme von Änderungen aus W3C-DCAT 2.0 und DCAT-AP 2.0, insbesondere:
    - Berücksichtigung von dcat:Resource durch Vererbung
    - Einführung des dcat:DataService
 - Breaking Changes:
    - DEPRECATION von dcat:plannedAvailability (NEU: dcatap:availability)
    - DEPRECATION von dct:type und dct:hasVersion für Datenreihen (KÜNFTIG: dcat:DataSeries)
    - DEPRECATION von dcat:granularity
    - DEPRECATION von schema:startDate und schema:endDate (NEU: dcat:startDate und dcat:endDate)
   
Wesentliche Änderungen im Konventionenhandbuch:
 - Beispiele, wie ein dcat:DataService modelliert werden kann
 - Abgrenzung zwischen dct:license, odrl:hasPolice und dct:rights
 - Vereinfachung von Konvention 31
 - Nutzung des Musterdatenkatalogs für dcat:keyword und dct:references


Beispieldateien:
Anpassung der Beispieldateien entsprechend des Changelogs der Spezifikation und des Konventionenhandbuchs.
Verwendung von example.com-Adressen für Datasätze und Distributionen.

UML-Diagramm: 
Das UML-Diagramm wird nun aus einer PlantUML-Datei generiert. Die maschinenlesbare PlantUML-Datei, sowie eine SVG-Datei werden bereitgestellt.

============================================================================================
=============================== dcat-ap.de readme für 1.1 ==================================
============================================================================================

Beispieldateien:
Die nicht-normativen Beispieldateien wurden in RDF Turtle erstellt und mittels des Tools http://rdf-translator.appspot.com/ in die Formate RDF/XML und JSON-LD überführt.
Die Beispiele wurden so angepasst, dass sie zum DCAT-AP.de Validator (BETA, siehe https://www.itb.ec.europa.eu/shacl/dcat-ap.de/upload) valide sind.


Verschärfungen Datentyp:
1.0.2: spdx:algorithm hat als Range ein rdfs:Literal
1.1:   spdx:algorithm hat als Range eine rdfs:Resource


Ergänzungen zur Spezifikation:
Aufnahme eines Kapitels, das auf weitere Projekte verweist, die auf DCAT-AP basieren. (Liste wird zukünftig online bereitgestellt.)


Änderungen im Konventionenhandbuch:
Hinzufügen von Konvention 40: Festlegung, wie dct:modified befüllt werden muss, wenn die Metadaten aus ISO-Metadaten erzeugt werden.
Hinzufügen von neuen Wertelisten für dcatde:politicalGeocodingURI:
   1. Gemeindeschlüssel
   2. Gemeindeverband
   3. Bezirk
Aktualisierung der im Konventionenhandbuch veröffentlichten Wertelisten.


============================================================================================
=============================== dcat-ap.de readme für 1.0.2 ================================
============================================================================================

Beispieldateien:
Die beiliegenden Beispieldateien sind nicht-normativ und enthalten in den verschiedenen technischen Implementierungen (RDF/XML, RDF Turtle, JSON-LD [mit und ohne @context]) verschiedene Attribute in einfacher und fortgeschrittener Ausführung.
Die Beispiele wurden in RDF Turtle konstruiert und mittels des Tools http://rdf-translator.appspot.com/ in die anderen Formate überführt.


Validierung:
Die Validierungsdateien der Version 1.0 entfallen seit Version 1.0.1. JSON, XML sowie JSON-Schema und XSD-Schemavalidierung werden nicht weiter gepflegt. In Version 1.1 ist eine Validierung mit SHACL geplant. 


Migrationshinweise für Version 1.0.1 auf 1.0.2:
Errata für Implementierer der Version 1.0.1 zur Version 1.0.2:


Errata:
1.0.1: spdx:checksumValue wurde als URI in der Klasse spdx:Checksum geführt
1.0.2: spdx:checksumValue ist eine verpflichtende Eigenschaft von spdx:Checksum

1.0.1: Um in den Beispieldateien im JSON-Schema Namenskonflikte zu vermeiden, existierte die zusätzliche Klasse "Andere ID" (other_identifier).
1.0.2: In den neuen Beispieldateien ist dank der namespace-awareness von JSON-LD dieser Workaround nicht mehr notwendig. Mehrere Identifier können über die Klasse "Identifier" abgebildet werden. "Andere ID" wurde daher entfernt.

1.0.1: Klasse dcat:Dataset als verpflichtendes "Attribut"
1.0.2: verpflichtendes Attribut dcat:dataset verweist auf die Klasse dcat:Dataset

1.0.1: Lizenz Dokument führt dct:type in der Abbildung 6 als optional, in der Klassenbeschreibung aber als empfohlen
1.0.2: Lizenz Dokument führt dct:type in beiden Fällen als empfohlen


Hinzugefügt:
1.0.2: dcat:granularity als optionale Eigenschaft zur Klasse dcat:Dataset hinzugefügt


Geändert:
1.0.1: Kardinalität dct:type in LicenseDocument-Klasse: 0..1
1.0.2: Kardinalität dct:type in LicenseDocument-Klasse: 0..n



============================================================================================
=============================== dcat-ap.de readme für 1.0.1 ================================
============================================================================================

Beispieldateien:
Die beiliegenden Beispieldateien sind nicht-normativ und enthalten in den verschiedenen technischen Implementierungen (RDF/XML, RDF Turtle, JSON-LD) verschiedene Attribute in minimaler und maximaler Ausführung.

Validierung:
Die Validierungsdateien der Version 1.0 entfallen zukünftig. JSON, XML sowie JSON-Schema und XSD-Schemavalidierung werden nicht weiter gepflegt. In Version 1.1 ist eine Validierung mit SHACL geplant. 
Zusätzlich wird als Beispieldatei bereitgestellt RDF Turtle Notation, JSON-LD

Migrationshinweise für Version 1.0 auf 1.0.1:
Errata für Implementierer der Version 1.0 zur Version 1.0.1:

Feldumbenennungen:
1.0: (überall) geocodingText
1.0.1: (überall) geocodingDescription

1.0: (überall) legalBasisText
1.0.1: (überall) legalBasis


Verschärfungen Datentyp:
1.0: (UML): plannedAvailability:rdfs:Literal
1.0.1: (UML): plannedAvailability:rdfs:Resource

1.0: (UML): qualityProcessURI:rdfs:Literal
1.0.1: (UML): qualityProcessURI:rdfs:Resource

1.0: (UML): politicalGeocodingURI:rdfs:Literal
1.0.1: (UML): politicalGeocodingURI:rdfs:Resource


Verschärfungen Feldverbindlichkeiten:
- keine -


Vereinfachung Feldverbindlichkeiten:
1.0: distribution.licence 1 - verbindlich
1.0.1: distribution.licence 0..1 - empfohlen

1.0: distribution.contributorID 1 - verbindlich
1.0.1: distribution.contributorID 0..1 - optional


Die Art in der Werteliste als RDF auf dcat-ap.de ausgeliefert werden wurde geändert.



============================================================================================
========================== Links zu den Dokumenten und Artefakten ==========================
============================================================================================

Web-Dokumenten
2.0: Spezifikation:        https://www.dcat-ap.de/def/dcatde/2.0/spec/
2.0: Konventionenhandbuch: https://www.dcat-ap.de/def/dcatde/2.0/implRules/

Spezifikation DCAT-AP.de (PDF):
2.0:   https://www.dcat-ap.de/def/dcatde/2.0/spec/specification.pdf
1.1:   https://www.dcat-ap.de/def/dcatde/1.1/spec/specification.pdf
1.0.2: https://www.dcat-ap.de/def/dcatde/1.0.2/spec/specification.pdf
1.0.1: https://www.dcat-ap.de/def/dcatde/1.0.1/spec/specification.pdf
1.0.0: -

UML Modell (strukturiert):
2.0:   (PlantUML): https://www.dcat-ap.de/def/dcatde/2.0/uml/dcat-ap-de.plantuml
1.1:   -
1.0.2: (Modelio):  https://www.dcat-ap.de/def/dcatde/1.0.2/uml/modelio.zip
1.0.1: (Modelio):  https://www.dcat-ap.de/def/dcatde/1.0.1/uml/modelio.zip
1.0.0: -

UML Modell (graphisch):
2.0:   https://www.dcat-ap.de/def/dcatde/2.0/uml/dcat-ap-de.svg
1.1:   https://www.dcat-ap.de/def/dcatde/1.1/uml/modelio.pdf
1.0.2: https://www.dcat-ap.de/def/dcatde/1.0.2/uml/modelio.pdf
1.0.1: https://www.dcat-ap.de/def/dcatde/1.0.1/uml/modelio.pdf
1.0.0: -

Konventionenhandbuch (PDF):
2.0:   https://www.dcat-ap.de/def/dcatde/2.0/implRules.pdf
1.1:   https://www.dcat-ap.de/def/dcatde/1.1/implRules.pdf
1.0.2: https://www.dcat-ap.de/def/dcatde/1.0.2/implRules.pdf
1.0.1: https://www.dcat-ap.de/def/dcatde/1.0.1/implRules.pdf
1.0.0: -

Beispieldateien:
2.0:   https://www.dcat-ap.de/def/dcatde/2.0/examples.zip
1.1:   https://www.dcat-ap.de/def/dcatde/1.1/examples.zip
1.0.2: https://www.dcat-ap.de/def/dcatde/1.0.2/examples.zip
1.0.1: https://www.dcat-ap.de/def/dcatde/1.0.1/examples.zip
1.0.0: -

URI-Konzept (PDF):
1.0: https://www.dcat-ap.de/def/uriConcept/1.0
