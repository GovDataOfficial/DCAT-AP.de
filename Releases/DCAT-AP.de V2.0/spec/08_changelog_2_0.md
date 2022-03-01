### Klasse: Katalog

Auf Ebene der Klasse [Katalog](#klasse-katalog) (`dcat:Catalog`) gibt es 
keine Änderungen zur Vorversion.


Bei ihren Eigenschaften gibt es 
folgende Änderungen zur Vorversion:


| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Sprache](#katalog-sprache) (`dct:language`) | Kontrolliertes Vokabular angegeben. | 
| [Verfügbarkeit](#katalog-verfugbarkeit) (`dcatap:availability`) | Neu hinzugefügt. | 
| [Katalog](#katalog-katalog) (`dcat:catalog`) | Neu hinzugefügt. | 



### Klasse: Datensatz

Auf Ebene der Klasse [Datensatz](#klasse-datensatz) (`dcat:Dataset`) gibt es 
keine Änderungen zur Vorversion.


Bei ihren Eigenschaften gibt es 
folgende Änderungen zur Vorversion:


| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Verfügbarkeit](#datensatz-verfugbarkeit) (`dcatap:availability`) | Neu hinzugefügt. | 
| [Datenbereitsteller ID](#datensatz-datenbereitsteller-id) (`dcatde:contributorID`) | Beschreibung angepasst, Pflicht, bestehende IDs zu erhalten entfernt. | 
| [Konform zu Standard](#datensatz-konform-zu-standard) (`dct:conformsTo`) | Label der Eigenschaft von &quot;Application Profile der Metadaten&quot; zu &quot;Konform zu Standard&quot; geändert, um Verwendung an DCAT-AP anzugleichen. | 
| [Typ des Datensatzes](#datensatz-typ) (`dct:type`) | Beschreibung überarbeitet. Die Eigenschaft soll nicht mehr für Collections verwendet werden ([DEPRECATED](#glossar-deprecated)). Hierfür soll künftig [&#x60;dcat:DatasetSeries&#x60;](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#sammlungen-und-reihen-von-datensatzen) verwendet werden. | 
| [Wurde erzeugt von](#datensatz-wurde-erzeugt-von) (`prov:wasGeneratedBy`) | Neu hinzugefügt. | 
| [Räumliche Auflösung in Meter](#datensatz-raumliche-auflosung-in-meter) (`dcat:spatialResolutionInMeters`) | Neu hinzugefügt. | 
| [Zeitliche Auflösung](#datensatz-zeitliche-auflosung) (`dcat:temporalResolution`) | Neu hinzugefügt. | 
| [Abgedeckte zeitliche Granularität (DEPRECATED)](#datensatz-abgedeckte-zeitliche-granularitat-deprecated) (`dcat:granularity`) | [DEPRECATED](#glossar-deprecated) | 
| [Rollenzuordnung](#datensatz-rollenzuordnung) (`prov:qualifiedAttribution`) | Neu hinzugefügt. | 
| [Qualifizierte Beziehung](#datensatz-qualifizierte-beziehung) (`dcat:qualifiedRelation`) | Neu hinzugefügt. | 
| [Wird Referenziert](#datensatz-wird-referenziert) (`dct:isReferencedBy`) | Neu hinzugefügt. | 
| [Referenziert](#datensatz-referenziert) (`dct:references`) | Neu durch DCAT-AP.de hinzugefügt. | 
| [Räumliche Abdeckung](#datensatz-raumliche-abdeckung) (`dct:spatial`) | Änderung von optional auf recommended. Umbenennung von &quot;Standort&quot; in &quot;Räumliche Abdeckung&quot;. | 
| [Zeitliche Abdeckung](#datensatz-zeitliche-abdeckung) (`dct:temporal`) | Verbindlichkeit wurde von optional auf empfohlen hochgestuft. Umbenennung von &quot;Zeitraum&quot; in &quot;Zeitliche Abdeckung&quot;. | 
| [Weitere Version](#datensatz-weitere-version) (`dct:hasVersion`) | Beschreibung überarbeitet. Die Eigenschaft soll nicht mehr für Collections verwendet werden ([DEPRECATED](#glossar-deprecated)). Hierfür soll künftig [&#x60;dcat:DatasetSeries&#x60;](https://www.w3.org/TR/vocab-dcat-3/#Class:Dataset_Series) verwendet werden. | 



### Klasse: Datenservice

Auf Ebene der Klasse [Datenservice](#klasse-datenservice) (`dcat:DataService`) gibt es 
folgende Änderungen zur Vorversion:


> Neu hinzugefügt.


Bei ihren Eigenschaften gibt es 
folgende Änderungen zur Vorversion:


| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [URL des Endpunktes](#datenservice-url-endpunkt) (`dcat:endpointURL`) | Neu hinzugefügt. | 
| [Titel](#datenservice-titel) (`dct:title`) | Neu hinzugefügt. | 
| [Beschreibung des Endpunktes](#datenservice-beschreibung-endpunkt) (`dcat:endpointDescription`) | Neu hinzugefügt. | 
| [Verfügbarkeit](#datenservice-verfugbarkeit) (`dcatap:availability`) | Neu hinzugefügt. | 
| [Beschreibung](#datenservice-beschreibung) (`dct:description`) | Neu hinzugefügt. | 
| [Lizenz](#datenservice-lizenz) (`dct:license`) | Neu hinzugefügt. | 
| [Grad der Zugänglichkeit](#datenservice-grad-zuganglichkeit) (`dct:accessRights`) | Neu hinzugefügt. | 
| [Liefert Datensatz aus](#datenservice-liefert-datensatz-aus) (`dcat:servesDataset`) | Neu hinzugefügt. | 



### Klasse: Distribution

Auf Ebene der Klasse [Distribution](#klasse-distribution) (`dcat:Distribution`) gibt es 
keine Änderungen zur Vorversion.


Bei ihren Eigenschaften gibt es 
folgende Änderungen zur Vorversion:


| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Verfügbarkeit](#distribution-verfugbarkeit) (`dcatap:availability`) | Neu hinzugefügt. | 
| [Verfügbarkeit (DEPRECATED)](#distribution-verfugbarkeit-deprecated) (`dcatde:plannedAvailability`) | [DEPRECATED](#glossar-deprecated). | 
| [Sprache](#distribution-sprache) (`dct:language`) | Beschreibung klarer formuliert. Kontrolliertes Vokabular angegeben. | 
| [Konform zu Standard](#distribution-konform-zu-standard) (`dct:conformsTo`) | Beschreibung angepasst. Label der Eigenschaft von &quot;Application Profile der Metadaten&quot; zu &quot;Konform zu Standard&quot; geändert. | 
| [Kompressionsformat](#distribution-kompressionsformat) (`dcat:compressFormat`) | Neu hinzugefügt. | 
| [Paketformat](#distribution-paketformat) (`dcat:packageFormat`) | Neu hinzugefügt. | 
| [Regelwerk](#distribution-regelwerk) (`odrl:hasPolicy`) | Neu hinzugefügt. | 
| [Ausliefernder Datenservice](#distribution-ausliefernder-datenservice) (`dcat:accessService`) | Neu hinzugefügt. | 



### Klasse: Zeitraum

Auf Ebene der Klasse [Zeitraum](#klasse-zeitraum) (`dct:PeriodOfTime`) gibt es 
keine Änderungen zur Vorversion.


Bei ihren Eigenschaften gibt es 
folgende Änderungen zur Vorversion:


| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Startzeitpunkt](#zeitraum-startzeitpunkt) (`dcat:startDate`) | Neu hinzugefügt. Zudem sind bei dieser Eigenschaft auch &#x60;xsd:gYear&#x60; und &#x60;xsd:gYearMonth&#x60; erlaubt. | 
| [Endzeitpunkt](#zeitraum-endzeitpunkt) (`dcat:endDate`) | Neu hinzugefügt. Zudem sind bei dieser Eigenschaft auch &#x60;xsd:gYear&#x60; und &#x60;xsd:gYearMonth&#x60; erlaubt. | 
| [Anfang](#zeitraum-anfang) (`time:hasBeginning`) | Neu hinzugefügt. | 
| [Ende](#zeitraum-ende) (`time:hasEnd`) | Neu hinzugefügt. | 
| [Startzeitpunkt (DEPRECATED)](#zeitraum-startzeitpunkt-deprecated) (`schema:startDate`) | [DEPRECATED](#glossar-deprecated). | 
| [Endzeitpunkt (DEPRECATED)](#zeitraum-endzeitpunkt-deprecated) (`schema:endDate`) | [DEPRECATED](#glossar-deprecated). | 



### Klasse: Standort

Auf Ebene der Klasse [Standort](#klasse-standort) (`dct:Location`) gibt es 
keine Änderungen zur Vorversion.


Bei ihren Eigenschaften gibt es 
folgende Änderungen zur Vorversion:


| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Bounding Box](#standort-bounding-box) (`dcat:bbox`) | Neu hinzugefügt. | 
| [Geografischer Mittelpunkt](#standort-geografischer-mittelpunkt) (`dcat:centroid`) | Neu hinzugefügt. | 



### Klasse: Identifier

Auf Ebene der Klasse [Identifier](#klasse-identifier) (`adms:Identifier`) gibt es 
keine Änderungen zur Vorversion.


Bei ihren Eigenschaften gibt es 
folgende Änderungen zur Vorversion:


| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Notation des Identifier](#identifier-notation) (`skos:notation`) | Range neu formuliert. Auf &quot;mandatory&quot; korrigiert. | 



### Klasse: Katalogeintrag

Auf Ebene der Klasse [Katalogeintrag](#klasse-katalogeintrag) (`dcat:CatalogRecord`) gibt es 
keine Änderungen zur Vorversion.


Bei ihren Eigenschaften gibt es 
folgende Änderungen zur Vorversion:


| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Änderungstyp](#katalogeintrag-anderungstyp) (`adms:status`) | Zu verwendendes Vokabular entfernt. | 



### Klasse: Beziehung

Auf Ebene der Klasse [Beziehung](#klasse-beziehung) (`dcat:Relationship`) gibt es 
folgende Änderungen zur Vorversion:


> Neu hinzugefügt.


Bei ihren Eigenschaften gibt es 
folgende Änderungen zur Vorversion:


| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Hatte Rolle](#beziehung-rolle) (`dcat:hadRole`) | Neu hinzugefügt. | 
| [Beziehung](#beziehung-beziehung) (`dct:relation`) | Neu hinzugefügt. | 



### Klasse: Rollenzuordnung

Auf Ebene der Klasse [Rollenzuordnung](#klasse-rollenzuordnung) (`prov:Attribution`) gibt es 
folgende Änderungen zur Vorversion:


> Neu hinzugefügt.


Bei ihren Eigenschaften gibt es 
folgende Änderungen zur Vorversion:


| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Hatte Rolle](#rollenzuordnung-rolle) (`dcat:hadRole`) | Neu hinzugefügt. | 
| [Agent](#rollenzuordnung-agent) (`prov:agent`) | Neu hinzugefügt. | 

