### Klasse: Katalog

Auf Ebene der Klasse [Katalog](#klasse-katalog) (`dcat:Catalog`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Veröffentlichungsdatum](#katalog-veroffentlichungsdatum) (`dcterms:issued`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Aktualisierungsdatum](#katalog-aktualisierungsdatum) (`dcterms:modified`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Rechte](#katalog-rechte) (`dcterms:rights`) | 3.0: In "Rechte" umbenannt und Verwendungshinweis hinzugefügt. | 
| [Datensatz](#katalog-datensatz) (`dcat:dataset`) | 3.0: Harmonisierung: Kardinalität von `1..*` auf `*` geändert. Verbindlichkeit auf "Empfohlen" gesenkt. | 


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
| [Räumliche Auflösung in Meter](#datensatz-raumliche-auflosung-in-meter) (`dcat:spatialResolutionInMeters`) | 3.0: Errata: Kardinalität von `[*]` wie bei DCAT-AP auf `[0..1]` angepasst. | 
| [Zeitliche Auflösung](#datensatz-zeitliche-auflosung) (`dcat:temporalResolution`) | 3.0: Errata: Kardinalität von `[*]` wie bei DCAT-AP auf `[0..1]` angepasst.<br>3.0: Errata: Anzeige des Wertebereichs korrigiert und weiterführende Dokumentation zu DCAT korrigiert. | 
| [Weitere Version](#datensatz-weitere-version) (`dcat:hasVersion`) | 3.0: Neu hinzugefügt. | 
| [Weitere Version (DEPRECATED)](#datensatz-weitere-version-deprecated) (`dcterms:hasVersion`) | 3.0: [DEPRECATED](#glossar-deprecated) | 
| [Ist Version von (DEPRECATED)](#datensatz-ist-version) (`dcterms:isVersionOf`) | 3.0: [DEPRECATED](#glossar-deprecated) | 
| [Herausgeber](#datensatz-herausgeber) (`dcterms:publisher`) | 3.0: Anforderung: Nutzung verpflichtend gemacht. | 
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
| [Herausgeber](#datenservice-herausgeber) (`dcterms:publisher`) | 3.0: Eigenschaft aufgenommen.<br>3.0: Anforderung: Nutzung verpflichtend gemacht. | 


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
| [Herausgeber](#datensatzserie-herausgeber) (`dcterms:publisher`) | 3.0: Neu hinzugefügt.<br>3.0: Anforderung: Nutzung verpflichtend gemacht. | 
| [Zeitliche Abdeckung](#datensatzserie-zeitliche-abdeckung) (`dcterms:temporal`) | 3.0: Neu hinzugefügt. | 


### Klasse: Distribution

Auf Ebene der Klasse [Distribution](#klasse-distribution) (`dcat:Distribution`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Lizenz](#distribution-lizenz) (`dcterms:license`) | 3.0: Kardinalität von `[0..1]` auf `[1]` geändert und die Eigenschaft damit verpflichtend gemacht. | 
| [Aktualisierungsdatum](#distribution-aktualisierungsdatum) (`dcterms:modified`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Format](#distribution-format) (`dcterms:format`) | 3.0: Errata: Wertebereichs auf dcterms:MediaTypeOrExtent geändert. | 
| [Verfügbarkeit](#distribution-verfugbarkeit) (`dcatap:availability`) | 3.0: Errata: Hinterlegte URL für den Wertebereichs auf skos:Concept geändert. | 
| [Größe in Bytes](#distribution-grosse-in-bytes) (`dcat:byteSize`) | 3.0: Änderung der Range von xsd:decimal auf xsd:nonNegativeInteger. | 
| [Veröffentlichungsdatum](#distribution-veroffentlichungsdatum) (`dcterms:issued`) | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Rechte](#distribution-rechte) (`dcterms:rights`) | 3.0: In "Rechte" umbenannt und Verwendungshinweis hinzugefügt. | 
| [Status](#distribution-status) (`adms:status`) | 3.0: Änderung des kontrollierten Vokabulars. | 
| [Räumliche Auflösung in Meter](#distribution-raumliche-auflosung-in-meter) (`dcat:spatialResolutionInMeters`) | 3.0: Errata: Eigenschaft aufgeführt, existierte bereits in DCAT-AP 2.0. | 
| [Zeitliche Auflösung](#distribution-zeitliche-auflosung) (`dcat:temporalResolution`) | 3.0: Errata: Eigenschaft aufgeführt, existierte bereits in DCAT-AP 2.0. | 
| [Prüfsumme](#distribution-prufsumme) (`spdx:checksum`) | 3.0: Harmonisierung: Verwendungshinweis hinzugefügt. | 


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
| [Geometrie](#standort-geometrie) (`locn:geometry`) | 3.0: Wertebereich auf locn:Geometry geändert.<br>3.0: Verwendungshinweis von DCAT hinzugefügt. | 


### Klasse: Verantwortliche Stelle

Auf Ebene der Klasse [Verantwortliche Stelle](#klasse-verantwortliche-stelle) (`foaf:Agent`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Typ](#verantwortliche-stelle-typ) (`dcterms:type`) | 3.0: Errata: Link zur zu verwendenden Codeliste hinzugefügt, war zuvor bei `foaf:name` angegeben. | 


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


