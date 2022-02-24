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

Spezifikation DCAT-AP.de (PDF):
1.1:   https://www.dcat-ap.de/def/dcatde/1.1/spec/specification.pdf
1.0.2: https://www.dcat-ap.de/def/dcatde/1.0.2/spec/specification.pdf
1.0.1: https://www.dcat-ap.de/def/dcatde/1.0.1/spec/specification.pdf
1.0.0: -

UML Modell (ZIP):
1.1:   -
1.0.2: https://www.dcat-ap.de/def/dcatde/1.0.2/uml/modelio.zip
1.0.1: https://www.dcat-ap.de/def/dcatde/1.0.1/uml/modelio.zip
1.0.0: -

UML Modell (PDF):
1.1:   https://www.dcat-ap.de/def/dcatde/1.1/uml/modelio.pdf
1.0.2: https://www.dcat-ap.de/def/dcatde/1.0.2/uml/modelio.pdf
1.0.1: https://www.dcat-ap.de/def/dcatde/1.0.1/uml/modelio.pdf
1.0.0: -

Konventionenhandbuch (PDF):
1.1:   https://www.dcat-ap.de/def/dcatde/1.1/implRules.pdf
1.0.2: https://www.dcat-ap.de/def/dcatde/1.0.2/implRules.pdf
1.0.1: https://www.dcat-ap.de/def/dcatde/1.0.1/implRules.pdf
1.0.0: -

Beispieldateien:
1.1:   https://www.dcat-ap.de/def/dcatde/1.1/examples.zip
1.0.2: https://www.dcat-ap.de/def/dcatde/1.0.2/examples.zip
1.0.1: https://www.dcat-ap.de/def/dcatde/1.0.1/examples.zip
1.0.0: -

URI-Konzept (PDF):
1.0: https://www.dcat-ap.de/def/uriConcept/1.0