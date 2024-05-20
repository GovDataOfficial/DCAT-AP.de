### Klasse: Katalog

Auf Ebene der Klasse [Katalog](#klasse-katalog) (`dcat:Catalog`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Veröffentlichungsdatum](#katalog-veroffentlichungsdatum) (`dct:issued`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Aktualisierungsdatum](#katalog-aktualisierungsdatum) (`dct:modified`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 


### Klasse: Datensatz

Auf Ebene der Klasse [Datensatz](#klasse-datensatz) (`dcat:Dataset`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Veröffentlichungsdatum](#datensatz-veroffentlichungsdatum) (`dct:issued`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Aktualisierungsdatum](#datensatz-aktualisierungsdatum) (`dct:modified`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Versionsbezeichnung](#datensatz-versionsbezeichnung) (`dcat:version`) | 3.0: Neu hinzugefügt. | 
| [Versionsbezeichnung (DEPRECATED)](#datensatz-versionsbezeichnung-deprecated) (`owl:versionInfo`) | 3.0: [DEPRECATED](#glossar-deprecated) | 
| [Rechtsgrundlage](#datensatz-rechtsgrundlage) (`dcatap:applicableLegislation`) | 3.0: Neu hinzugefügt. | 
| [Rechtsgrundlage für die Zugangseröffnung (DEPRECATED)](#datensatz-rechtsgrundlage-zugangseroffnung) (`dcatde:legalBasis`) | 3.0: [DEPRECATED](#glossar-deprecated) | 
| [Grad der Zugänglichkeit](#datensatz-grad-zuganglichkeit) (`dct:accessRights`) | 3.0: Kontrolliertes Vokabular hinzugefügt. | 
| [Typ des Datensatzes](#datensatz-typ) (`dct:type`) | 3.0: Kardinalität von `0..1` auf `*` geändert. | 
| [Zeitliche Auflösung](#datensatz-zeitliche-auflosung) (`dcat:temporalResolution`) | 3.0: Errata: Anzeige des Wertebereichs korrigiert. | 
| [Weitere Version](#datensatz-weitere-version) (`dcat:hasVersion`) | 3.0: Neu hinzugefügt. | 
| [Weitere Version (DEPRECATED)](#datensatz-weitere-version-deprecated) (`dct:hasVersion`) | 3.0: [DEPRECATED](#glossar-deprecated) | 
| [Ist Version von (DEPRECATED)](#datensatz-ist-version) (`dct:isVersionOf`) | 3.0: [DEPRECATED](#glossar-deprecated) | 


### Klasse: Datenservice

Auf Ebene der Klasse [Datenservice](#klasse-datenservice) (`dcat:DataService`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Grad der Zugänglichkeit](#datenservice-grad-zuganglichkeit) (`dct:accessRights`) | 3.0: Kontrolliertes Vokabular hinzugefügt. | 


### Klasse: Distribution

Auf Ebene der Klasse [Distribution](#klasse-distribution) (`dcat:Distribution`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Aktualisierungsdatum](#distribution-aktualisierungsdatum) (`dct:modified`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Format](#distribution-format) (`dct:format`) | 3.0: Errata: Wertebereichs auf dct:MediaTypeOrExtent geändert. | 
| [Größe in Bytes](#distribution-grosse-in-bytes) (`dcat:byteSize`) | 3.0: Änderung der Range von xsd:decimal auf xsd:nonNegativeInteger. | 
| [Veröffentlichungsdatum](#distribution-veroffentlichungsdatum) (`dct:issued`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Räumliche Auflösung in Meter](#distribution-raumliche-auflosung-in-meter) (`dcat:spatialResolutionInMeters`) | 3.0: Errata: Eigenschaft aufgeführt, existierte bereits in DCAT-AP 2.0. | 
| [Zeitliche Auflösung](#distribution-zeitliche-auflosung) (`dcat:temporalResolution`) | 3.0: Errata: Eigenschaft aufgeführt, existierte bereits in DCAT-AP 2.0. | 


### Klasse: Zeitraum

Auf Ebene der Klasse [Zeitraum](#klasse-zeitraum) (`dct:PeriodOfTime`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Startzeitpunkt](#zeitraum-startzeitpunkt) (`dcat:startDate`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Endzeitpunkt](#zeitraum-endzeitpunkt) (`dcat:endDate`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 


### Klasse: Standort

Auf Ebene der Klasse [Standort](#klasse-standort) (`dct:Location`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
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
| [Aktualisierungsdatum](#katalogeintrag-aktualisierungsdatum) (`dct:modified`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Application Profile der Metadaten](#katalogeintrag-konform-zu) (`dct:conformsTo`) | 3.0: Kardinalität von `0..1` auf `*` geändert. | 
| [Veröffentlichungsdatum](#katalogeintrag-veroffentlichungsdatum) (`dct:issued`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Katalogeintrag](#katalogeintrag-katalogeintrag) (`foaf:primaryTopic`) | 3.0: Aufnahme der Ressource `dcat:DatasetSeries` | 


### Klasse: Lizenzdokument

Auf Ebene der Klasse [Lizenzdokument](#klasse-lizenzdokument) (`dct:LicenseDocument`) gibt es 
folgende Änderungen zur Vorversion:

> 3.0: Errata: Label korrigiert.

Bei ihren Eigenschaften gibt es keine Änderungen zur Vorversion.


