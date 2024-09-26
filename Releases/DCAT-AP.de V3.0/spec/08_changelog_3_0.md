### Klasse: Katalog

Auf Ebene der Klasse [Katalog](#klasse-katalog) (`dcat:Catalog`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Veröffentlichungsdatum](#katalog-veroffentlichungsdatum) (`dcterms:issued`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Aktualisierungsdatum](#katalog-aktualisierungsdatum) (`dcterms:modified`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 


### Klasse: Datensatz

Auf Ebene der Klasse [Datensatz](#klasse-datensatz) (`dcat:Dataset`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Andere ID](#datensatz-andere-id) (`adms:identifier`) | 3.0: Errata: Link der Range korrigiert und Verwendungshinweis überarbeitet. | 
| [Veröffentlichungsdatum](#datensatz-veroffentlichungsdatum) (`dcterms:issued`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Aktualisierungsdatum](#datensatz-aktualisierungsdatum) (`dcterms:modified`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Versionsbezeichnung](#datensatz-versionsbezeichnung) (`dcat:version`) | 3.0: Neu hinzugefügt. | 
| [Versionsbezeichnung (DEPRECATED)](#datensatz-versionsbezeichnung-deprecated) (`owl:versionInfo`) | 3.0: [DEPRECATED](#glossar-deprecated) | 
| [Rechtsgrundlage](#datensatz-rechtsgrundlage) (`dcatap:applicableLegislation`) | 3.0: Neu hinzugefügt. | 
| [Rechtsgrundlage für die Zugangseröffnung (DEPRECATED)](#datensatz-rechtsgrundlage-zugangseroffnung) (`dcatde:legalBasis`) | 3.0: [DEPRECATED](#glossar-deprecated) | 
| [Grad der Zugänglichkeit](#datensatz-grad-zuganglichkeit) (`dcterms:accessRights`) | 3.0: Kontrolliertes Vokabular hinzugefügt. | 
| [Typ](#datensatz-typ) (`dcterms:type`) | 3.0: Kardinalität von `0..1` auf `*` geändert.<br>3.0: Namen vereinfacht.<br>3.0: Optionale Codeliste hinzugefügt. | 
| [Zeitliche Auflösung](#datensatz-zeitliche-auflosung) (`dcat:temporalResolution`) | 3.0: Errata: Anzeige des Wertebereichs korrigiert.<br>3.0: Errata: Weiterführende Dokumentation zu DCAT korrigiert. | 
| [Weitere Version](#datensatz-weitere-version) (`dcat:hasVersion`) | 3.0: Neu hinzugefügt. | 
| [Weitere Version (DEPRECATED)](#datensatz-weitere-version-deprecated) (`dcterms:hasVersion`) | 3.0: [DEPRECATED](#glossar-deprecated) | 
| [Ist Version von (DEPRECATED)](#datensatz-ist-version) (`dcterms:isVersionOf`) | 3.0: [DEPRECATED](#glossar-deprecated) | 
| [Autor](#datensatz-autor) (`dcterms:creator`) | 3.0: Errata: War fälschlicherweise als Ergänzung durch DCAT-AP.de angegeben. | 
| [In Serie](#datensatz-in-serie) (`dcat:inSeries`) | 3.0: Im Zuge der Einführung von `dcat:DatasetSeries` hinzugefügt. | 


### Klasse: Datenservice

Auf Ebene der Klasse [Datenservice](#klasse-datenservice) (`dcat:DataService`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Beschreibung des Endpunktes](#datenservice-beschreibung-endpunkt) (`dcat:endpointDescription`) | 3.0: In Anlehnung an DCAT-AP 3.0 wurde ein neuer Verwendungshinweis aufgenommen. | 
| [Grad der Zugänglichkeit](#datenservice-grad-zuganglichkeit) (`dcterms:accessRights`) | 3.0: Kontrolliertes Vokabular hinzugefügt. | 
| [Format](#datenservice-format) (`dcterms:format`) | 3.0: Eigenschaft aufgenommen. | 
| [Herausgeber](#datenservice-herausgeber) (`dcterms:publisher`) | 3.0: Eigenschaft aufgenommen. | 


### Klasse: Datensatzserie

Auf Ebene der Klasse [Datensatzserie](#klasse-datensatzserie) (`dcat:DatasetSeries`) gibt es 
folgende Änderungen zur Vorversion:

> 3.0: Neu hinzugefügt.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Titel](#datensatzserie-titel) (`dcterms:title`) | 3.0: Neu hinzugefügt. | 
| [Kontakt](#datensatzserie-kontakt) (`dcat:contactPoint`) | 3.0: Neu hinzugefügt. | 
| [Beschreibung](#datensatzserie-beschreibung) (`dcterms:description`) | 3.0: Neu hinzugefügt. | 
| [Rechtsgrundlage](#datensatzserie-rechtsgrundlage) (`dcatap:applicableLegislation`) | 3.0: Neu hinzugefügt. | 
| [Aktualisierungsfrequenz](#datensatzserie-aktualisierungsfrequenz) (`dcterms:accrualPeriodicity`) | 3.0: Neu hinzugefügt. | 
| [Veröffentlichungsdatum](#datensatzserie-veroffentlichungsdatum) (`dcterms:issued`) | 3.0: Neu hinzugefügt. | 
| [Aktualisierungsdatum](#datensatzserie-aktualisierungsdatum) (`dcterms:modified`) | 3.0: Neu hinzugefügt. | 
| [Räumliche Abdeckung](#datensatzserie-raumliche-abdeckung) (`dcterms:spatial`) | 3.0: Neu hinzugefügt. | 
| [Herausgeber](#datensatzserie-herausgeber) (`dcterms:publisher`) | 3.0: Neu hinzugefügt. | 
| [Zeitliche Abdeckung](#datensatzserie-zeitliche-abdeckung) (`dcterms:temporal`) | 3.0: Neu hinzugefügt. | 


### Klasse: Distribution

Auf Ebene der Klasse [Distribution](#klasse-distribution) (`dcat:Distribution`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Aktualisierungsdatum](#distribution-aktualisierungsdatum) (`dcterms:modified`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Format](#distribution-format) (`dcterms:format`) | 3.0: Errata: Wertebereichs auf dcterms:MediaTypeOrExtent geändert. | 
| [Verfügbarkeit](#distribution-verfugbarkeit) (`dcatap:availability`) | 3.0: Errata: Hinterlegte URL für den Wertebereichs auf skos:Concept geändert. | 
| [Größe in Bytes](#distribution-grosse-in-bytes) (`dcat:byteSize`) | 3.0: Änderung der Range von xsd:decimal auf xsd:nonNegativeInteger. | 
| [Veröffentlichungsdatum](#distribution-veroffentlichungsdatum) (`dcterms:issued`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Status](#distribution-status) (`adms:status`) | 3.0: Änderung des kontrollierten Vokabulars. | 
| [Räumliche Auflösung in Meter](#distribution-raumliche-auflosung-in-meter) (`dcat:spatialResolutionInMeters`) | 3.0: Errata: Eigenschaft aufgeführt, existierte bereits in DCAT-AP 2.0. | 
| [Zeitliche Auflösung](#distribution-zeitliche-auflosung) (`dcat:temporalResolution`) | 3.0: Errata: Eigenschaft aufgeführt, existierte bereits in DCAT-AP 2.0. | 


### Klasse: Zeitraum

Auf Ebene der Klasse [Zeitraum](#klasse-zeitraum) (`dcterms:PeriodOfTime`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Startzeitpunkt](#zeitraum-startzeitpunkt) (`dcat:startDate`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Endzeitpunkt](#zeitraum-endzeitpunkt) (`dcat:endDate`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 


### Klasse: Standort

Auf Ebene der Klasse [Standort](#klasse-standort) (`dcterms:Location`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Bounding Box](#standort-bounding-box) (`dcat:bbox`) | 3.0: Errata: Korrektur des zu verwendenden Types. | 
| [Geografischer Mittelpunkt](#standort-geografischer-mittelpunkt) (`dcat:centroid`) | 3.0: Errata: Korrektur des zu verwendenden Types. | 
| [Geometrie](#standort-geometrie) (`locn:geometry`) | 3.0: Wertebereich auf locn:Geometry geändert.<br>3.0: Verwendungshinweis und weiterführende Dokumentation hinzugefügt. | 


### Klasse: Prüfsumme

Auf Ebene der Klasse [Prüfsumme](#klasse-prufsumme) (`spdx:Checksum`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Algorithmus](#prufsumme-algorithmus) (`spdx:algorithm`) | 3.0: Range von `rdfs:Resource` auf `spdx:ChecksumAlgorithm` geändert. | 


### Klasse: Katalogeintrag

Auf Ebene der Klasse [Katalogeintrag](#klasse-katalogeintrag) (`dcat:CatalogRecord`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Aktualisierungsdatum](#katalogeintrag-aktualisierungsdatum) (`dcterms:modified`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Application Profile der Metadaten](#katalogeintrag-konform-zu) (`dcterms:conformsTo`) | 3.0: Kardinalität von `0..1` auf `*` geändert.<br>3.0: Errata: Anzeige des Wertebereichs korrigiert. | 
| [Veröffentlichungsdatum](#katalogeintrag-veroffentlichungsdatum) (`dcterms:issued`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Katalogeintrag](#katalogeintrag-katalogeintrag) (`foaf:primaryTopic`) | 3.0: Aufnahme der Ressource `dcat:DatasetSeries` | 


### Klasse: Lizenzdokument

Auf Ebene der Klasse [Lizenzdokument](#klasse-lizenzdokument) (`dcterms:LicenseDocument`) gibt es 
folgende Änderungen zur Vorversion:

> 3.0: Errata: Label korrigiert.

Bei ihren Eigenschaften gibt es keine Änderungen zur Vorversion.


### Klasse: Kategorie

Auf Ebene der Klasse [Kategorie](#klasse-kategorie) (`skos:Concept`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Bezeichnung](#kategorie-bezeichnung) (`skos:prefLabel`) | 3.0: Verwendungshinweis hinzugefügt. | 


