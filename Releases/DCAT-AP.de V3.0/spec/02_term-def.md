# Terminologie und Definitionen
Ein Application Profile ist eine Spezifikation, die Begrifflichkeiten bzw. Konzepte eines oder mehrerer grundlegender Standards weiterverwendet. Eine größere Bestimmtheit wird erreicht, indem für eine bestimmte Anwendung Klassen und Klassenattribute (Eigenschaften) als obligatorisch, empfohlen oder optional eingeordnet werden. Zusätzlich werden Empfehlungen für die Verwendung von kontrollierten Vokabularen gegeben.

Ein **Datenportal** ist ein webbasiertes System, welches einen Datenkatalog enthält, in dem Datensätze mittels Metadaten beschrieben werden. Des Weiteren stellt ein Datenportal Dienste zur Recherche und Wiederverwendung von Datensätzen bereit.
Ein **Datensatz (Dataset)** ist eine sinnvolle Sammlung von zusammenhängenden Daten, die von einer einzelnen Quelle veröffentlicht oder kuratiert wird und in einem oder mehreren Formaten erreichbar ist oder als Download zur Verfügung steht.
Ein **Sender** ist ein Bereitsteller von Daten (z.B. ein Datenportal, das Metadaten zur Verfügung stellt).
Ein **Empfänger** ist ein Nutzer von Daten (z.B. eine Anwendung, welche Metadaten eines Datenportals verarbeitet).

Verbindlichkeitsstufen (verpflichtend/empfohlen/optional) gelten allein für die Sender. Empfänger MÜSSEN immer in der Lage sein, Informationen über alle Instanzen aller Klassen sowie alle ihre Eigenschaften zu verarbeiten (nicht aber notwendigerweise zu parsen, zu konvertieren, zu speichern, suchbar zu machen oder anzuzeigen, etc.).</mark>
In den folgenden Abschnitten werden Klassen und Eigenschaften als „verpflichtend“, „empfohlen“ oder „optional“ bezeichnet. Diese Ausdrücke haben die folgende Bedeutung:
- **Verpflichtende Klasse:** Sender MÜSSEN Informationen über Instanzen dieser Klasse zur Verfügung stellen. Empfänger MÜSSEN Informationen über Instanzen dieser Klasse verarbeiten können.
- **Empfohlene Klasse:** Sender SOLLEN Informationen über Instanzen dieser Klasse zur Verfügung stellen. Sender MÜSSEN Informationen über Instanzen dieser Klasse zur Verfügung stellen, falls solche Informationen verfügbar sind. Empfänger MÜSSEN Informationen über Instanzen dieser Klasse verarbeiten können.
- **Optionale Klasse:** Sender KÖNNEN Informationen über Instanzen dieser Klasse zur Verfügung stellen, sind jedoch nicht dazu verpflichtet.
- **Verpflichtende Eigenschaft:** Sender MÜSSEN Informationen über diese Eigenschaft zur Verfügung stellen.
- **Empfohlene Eigenschaft:** Sender SOLLEN Informationen über diese Eigenschaft zur Verfügung stellen, falls diese verfügbar sind.
- **Optionale Eigenschaft:** Sender KÖNNEN Informationen über diese Eigenschaft zur Verfügung stellen, sind jedoch nicht dazu verpflichtet.

Im gegebenen Kontext bedeutet der Begriff „verarbeiten”, dass Empfänger eingehende Daten akzeptieren und transparent für Anwendungen und Dienste zur Verfügung stellen müssen. Dadurch wird nicht vorgeschrieben oder impliziert, welche Art der Datenverarbeitung durch die jeweiligen Anwendungen und Dienste letztendlich ausgeführt wird.

Die Begriffe MUSS, SOLL und KANN werden in diesem Dokument entsprechend ihren in [RFC2119](https://www.rfc-editor.org/rfc/rfc2119) definierten Bedeutungen verwendet, wenn sie wie hier gezeigt durchgehend groß geschrieben wurden. 

Neben den explizit als nicht-normativ gekennzeichneten Abschnitten sind auch alle Diagramme, Beispiele und Hinweise in diesem Dokument nicht normativ. Alle anderen Angaben sind normativ.


## Verwendete Spezifikationen  

Das Application Profile verwendet Begriffe von verschiedenen existierenden Spezifikationen. Klassen und Eigenschaften, die in den nachfolgenden Abschnitten spezifiziert werden, entstammen den folgenden Namensräumen.

| Namespace | URI des Namespace                       | Name der Spezifikation                                                                                     |
| :-------- | :-------------------------------------- | :--------------------------------------------------------------------------------------------------------- |
| `adms`    | `http://www.w3.org/ns/adms#`            | Asset Description Metadata Schema                                                                          |
| `dcat`    | `http://www.w3.org/ns/dcat#`            | Data Catalog Vocabulary                                                                                    |
| `dcatap`  | `http://data.europa.eu/r5r/`            | DCAT Application profile for data portals in Europe (DCAT-AP)                                              |
| `dcatde`  | `http://dcat-ap.de/def/dcatde/`         | German Adaptation of DCAT-AP                                                                               |
| `dcterms` | `http://purl.org/dc/terms/`             | DCMI (Dublin Core Metadata Initiative) Metadata Terms                                                      |
| `foaf`    | `http://xmlns.com/foaf/0.1/`            | FOAF (Friend of a friend) Vocabulary                                                                       |
| `geo`     | `http://www.opengis.net/ont/geosparql#` | GeoSPARQL Ontology                                                                                         |
| `locn`    | `http://www.w3.org/ns/locn#`            | ISA Programme Location Core Vocabulary                                                                     |
| `odrl`    | `http://www.w3.org/ns/odrl/2/`          | Open Digital Rights Language (ODRL)                                                                        |
| `owl`     | `http://www.w3.org/2002/07/owl#`        | OWL Web Ontology Language                                                                                  |
| `rdfs`    | `http://www.w3.org/2000/01/rdf-schema#` | RDF (Resource Description Framework) Vocabulary Description Language 1.0: RDF Schema                       |
| `schema`  | `http://schema.org/`                    | Vocabulary for structured data on the Internet                                                             |
| `skos`    | `http://www.w3.org/2004/02/skos/core#`  | SKOS Simple Knowledge Organization System – Reference                                                      |
| `spdx`    | `http://spdx.org/rdf/terms#`            | Software Package Data Exchange                                                                             |
| `time`    | `http://www.w3.org/2006/time#`          | OWL-Time is an OWL-2 DL ontology of temporal concepts, for describing the temporal properties of resources |
| `vcard`   | `http://www.w3.org/2006/vcard/ns#`      | File format standard for electronic business cards                                                         |
| `xsd`     | `http://www.w3.org/2001/XMLSchema#`     | XML Schema Part 2: Datatypes Second Edition                                                                |


## Bekannte Nutzungen von DCAT-AP und DCAT-AP.de
Im Rahmen der Verwendung von DCAT-AP entstanden durch Arbeiten der Europäischen Kommission und der Mitgliedsländer weitere Profilierungen. Zusätzlich zur horizontalen Verbreitung in den Mitgliedstaaten (u.a. Italien, Schweden und Spanien) fand eine fachliche Vertiefung durch Ergänzungen in den Application Profiles „GeoDCAT-AP“ und „StatDCAT-AP“ statt.

Diese Arbeiten flossen unter Berücksichtigung weiterer [Best Practices](https://www.w3.org/2013/share-psi/bp/) und [Hinweisen](https://joinup.ec.europa.eu/asset/ogd2_0/issue/dcat-ap) aus [Beteiligungsverfahren](https://joinup.ec.europa.eu/asset/dcat-ap_implementation_guidelines/issue/all) der Plattformen [Github](https://github.com/GovDataOfficial/DCAT-AP.de) und [Joinup](https://joinup.ec.europa.eu/asset/dcat_application_profile/issue/all) in die Erarbeitung der deutschen Erweiterung DCAT-AP.de und damit in dieses Dokument ein.

Um einen Überblick über die Nutzung der deutschen, EU und W3C Spezifikationen zu erhalten, die Möglichkeit des Community-Building zu fördern und das Verständnis über die Bedeutung von DCAT-AP und DCAT-AP.de ausserhalb des GovData Horizontes zu schärfen, wird zukünftig auf http://DCAT-AP.de/def/implementations eine Liste von Projekten geführt, die DCAT-AP oder DCAT-AP.de verwenden.
