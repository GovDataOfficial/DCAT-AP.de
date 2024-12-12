### Klasse: Katalog

Auf Ebene der Klasse [Katalog](#klasse-katalog) (`dcat:Catalog`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Veröffentlichungsdatum](#katalog-veroffentlichungsdatum) (`dcterms:issued`) | Errata: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Aktualisierungsdatum](#katalog-aktualisierungsdatum) (`dcterms:modified`) | Errata: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Rechte](#katalog-rechte) (`dcterms:rights`) | Weiterentwicklung: In "Rechte" umbenannt und Verwendungshinweis hinzugefügt. | 
| [Rechtsgrundlage](#katalog-rechtsgrundlage) (`dcatap:applicableLegislation`) | Harmonisierung: Neu hinzugefügt. | 
| [Datensatz](#katalog-datensatz) (`dcat:dataset`) | Harmonisierung: Kardinalität von `1..*` auf `*` geändert. Verbindlichkeit auf "Empfohlen" gesenkt. | 


### Klasse: Datensatz

Auf Ebene der Klasse [Datensatz](#klasse-datensatz) (`dcat:Dataset`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Geopolitische Abdeckung (DEPRECATED)](#datensatz-geopolitischen-abdeckung) (`dcatde:politicalGeocodingURI`) | Weiterentwicklung: [DEPRECATED](#glossar-deprecated) | 
| [Beschreibung der Abdeckung (DEPRECATED)](#datensatz-beschreibung-abdeckung) (`dcatde:geocodingDescription`) | Weiterentwicklung: [DEPRECATED](#glossar-deprecated) | 
| [Andere ID](#datensatz-andere-id) (`adms:identifier`) | Errata: Link der Range korrigiert und Verwendungshinweis überarbeitet. | 
| [Veröffentlichungsdatum](#datensatz-veroffentlichungsdatum) (`dcterms:issued`) | Errata: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Aktualisierungsdatum](#datensatz-aktualisierungsdatum) (`dcterms:modified`) | Errata: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Versionsbezeichnung](#datensatz-versionsbezeichnung) (`dcat:version`) | Harmonisierung: Neu hinzugefügt. | 
| [Versionsbezeichnung (DEPRECATED)](#datensatz-versionsbezeichnung-deprecated) (`owl:versionInfo`) | Harmonisierung: [DEPRECATED](#glossar-deprecated) | 
| [Rechtsgrundlage](#datensatz-rechtsgrundlage) (`dcatap:applicableLegislation`) | Harmonisierung: Neu hinzugefügt. | 
| [Rechtsgrundlage für die Zugangseröffnung (DEPRECATED)](#datensatz-rechtsgrundlage-zugangseroffnung) (`dcatde:legalBasis`) | Weiterentwicklung: [DEPRECATED](#glossar-deprecated) | 
| [Grad der Zugänglichkeit](#datensatz-grad-zuganglichkeit) (`dcterms:accessRights`) | Harmonisierung: Kontrolliertes Vokabular hinzugefügt. | 
| [Qualitätssicherungsprozess (DEPRECATED)](#datensatz-qualitatssicherungsprozess) (`dcatde:qualityProcessURI`) | Weiterentwicklung: [DEPRECATED](#glossar-deprecated) | 
| [Typ](#datensatz-typ) (`dcterms:type`) | Harmonisierung: Kardinalität von `0..1` auf `*` geändert.<br>Harmonisierung: Optionale Codeliste hinzugefügt.<br>Weiterentwicklung: Namen vereinfacht. | 
| [Räumliche Auflösung in Meter](#datensatz-raumliche-auflosung-in-meter) (`dcat:spatialResolutionInMeters`) | Errata: Kardinalität von `[*]` wie bei DCAT-AP auf `[0..1]` angepasst. | 
| [Zeitliche Auflösung](#datensatz-zeitliche-auflosung) (`dcat:temporalResolution`) | Errata: Kardinalität von `[*]` wie bei DCAT-AP auf `[0..1]` angepasst.<br>Errata: Anzeige des Wertebereichs korrigiert und weiterführende Dokumentation zu DCAT korrigiert. | 
| [Weitere Version](#datensatz-weitere-version) (`dcat:hasVersion`) | Harmonisierung: Neu hinzugefügt. | 
| [Weitere Version (DEPRECATED)](#datensatz-weitere-version-deprecated) (`dcterms:hasVersion`) | Harmonisierung: [DEPRECATED](#glossar-deprecated) | 
| [Ist Version von (DEPRECATED)](#datensatz-ist-version) (`dcterms:isVersionOf`) | Harmonisierung: [DEPRECATED](#glossar-deprecated) | 
| [Herausgeber](#datensatz-herausgeber) (`dcterms:publisher`) | Weiterentwicklung: Nutzung verpflichtend gemacht. | 
| [Autor](#datensatz-autor) (`dcterms:creator`) | Errata: War fälschlicherweise als Ergänzung durch DCAT-AP.de angegeben. | 
| [Urheber (DEPRECATED)](#datensatz-urheber) (`dcatde:originator`) | Weiterentwicklung: [DEPRECATED](#glossar-deprecated). Wird ersetzt durch [`geodcatap:originator`](#datensatz-geodcatap-urheber). | 
| [Urheber (GeoDCAT-AP)](#datensatz-geodcatap-urheber) (`geodcatap:originator`) | Weiterentwicklung: Neu hinzugefügt. Ersetzt `dcatde:originator`. | 
| [Verwalter (DEPRECATED)](#datensatz-verwalter) (`dcatde:maintainer`) | Weiterentwicklung: [DEPRECATED](#glossar-deprecated). Wird ersetzt durch [`geodcatap:custodian`](#datensatz-geodcatap-verwalter). | 
| [Verwalter (GeoDCAT-AP)](#datensatz-geodcatap-verwalter) (`geodcatap:custodian`) | Weiterentwicklung: Neu hinzugefügt. Ersetzt `dcatde:maintainer`. | 
| [In Serie](#datensatz-in-serie) (`dcat:inSeries`) | Harmonisierung: Im Zuge der Einführung von `dcat:DatasetSeries` hinzugefügt. | 


### Klasse: Datenservice

Auf Ebene der Klasse [Datenservice](#klasse-datenservice) (`dcat:DataService`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Grad der Zugänglichkeit](#datenservice-grad-zuganglichkeit) (`dcterms:accessRights`) | Harmonisierung: Kontrolliertes Vokabular hinzugefügt. | 
| [Format](#datenservice-format) (`dcterms:format`) | Harmonisierung: Eigenschaft aufgenommen. | 
| [Rechtsgrundlage](#datenservice-rechtsgrundlage) (`dcatap:applicableLegislation`) | Harmonisierung: Neu hinzugefügt. | 
| [Herausgeber](#datenservice-herausgeber) (`dcterms:publisher`) | Harmonisierung: Eigenschaft aufgenommen.<br>Weiterentwicklung: Nutzung verpflichtend gemacht. | 


### Klasse: Datensatzserie

Auf Ebene der Klasse [Datensatzserie](#klasse-datensatzserie) (`dcat:DatasetSeries`) gibt es 
folgende Änderungen zur Vorversion:

> Harmonisierung: Neu hinzugefügt.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Titel](#datensatzserie-titel) (`dcterms:title`) | Harmonisierung: Neu hinzugefügt. | 
| [Beschreibung](#datensatzserie-beschreibung) (`dcterms:description`) | Harmonisierung: Neu hinzugefügt. | 
| [Aktualisierungsfrequenz](#datensatzserie-aktualisierungsfrequenz) (`dcterms:accrualPeriodicity`) | Harmonisierung: Neu hinzugefügt. | 
| [Veröffentlichungsdatum](#datensatzserie-veroffentlichungsdatum) (`dcterms:issued`) | Harmonisierung: Neu hinzugefügt. | 
| [Aktualisierungsdatum](#datensatzserie-aktualisierungsdatum) (`dcterms:modified`) | Harmonisierung: Neu hinzugefügt. | 
| [Rechtsgrundlage](#datensatzserie-rechtsgrundlage) (`dcatap:applicableLegislation`) | Harmonisierung: Neu hinzugefügt. | 
| [Räumliche Abdeckung](#datensatzserie-raumliche-abdeckung) (`dcterms:spatial`) | Harmonisierung: Neu hinzugefügt. | 
| [Herausgeber](#datensatzserie-herausgeber) (`dcterms:publisher`) | Harmonisierung: Neu hinzugefügt.<br>Weiterentwicklung: Nutzung verpflichtend gemacht. | 
| [Zeitliche Abdeckung](#datensatzserie-zeitliche-abdeckung) (`dcterms:temporal`) | Harmonisierung: Neu hinzugefügt. | 
| [Kontakt](#datensatzserie-kontakt) (`dcat:contactPoint`) | Harmonisierung: Neu hinzugefügt. | 


### Klasse: Distribution

Auf Ebene der Klasse [Distribution](#klasse-distribution) (`dcat:Distribution`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Lizenz](#distribution-lizenz) (`dcterms:license`) | Weiterentwicklung: Kardinalität von `[0..1]` auf `[1]` geändert und die Eigenschaft damit verpflichtend gemacht. | 
| [Aktualisierungsdatum](#distribution-aktualisierungsdatum) (`dcterms:modified`) | Errata: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Format](#distribution-format) (`dcterms:format`) | Errata: Wertebereichs auf dcterms:MediaTypeOrExtent geändert. | 
| [Verfügbarkeit](#distribution-verfugbarkeit) (`dcatap:availability`) | Errata: Hinterlegte URL für den Wertebereichs auf skos:Concept geändert. | 
| [Größe in Bytes](#distribution-grosse-in-bytes) (`dcat:byteSize`) | Harmonisierung: Änderung der Range von xsd:decimal auf xsd:nonNegativeInteger. | 
| [Veröffentlichungsdatum](#distribution-veroffentlichungsdatum) (`dcterms:issued`) | Errata: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Rechte](#distribution-rechte) (`dcterms:rights`) | Weiterentwicklung: In "Rechte" umbenannt und Verwendungshinweis hinzugefügt. | 
| [Status](#distribution-status) (`adms:status`) | Harmonisierung: Änderung des kontrollierten Vokabulars. | 
| [Räumliche Auflösung in Meter](#distribution-raumliche-auflosung-in-meter) (`dcat:spatialResolutionInMeters`) | Errata: Eigenschaft aufgeführt, existierte bereits in DCAT-AP 2.0. | 
| [Zeitliche Auflösung](#distribution-zeitliche-auflosung) (`dcat:temporalResolution`) | Errata: Eigenschaft aufgeführt, existierte bereits in DCAT-AP 2.0. | 
| [Rechtsgrundlage](#distribution-rechtsgrundlage) (`dcatap:applicableLegislation`) | Harmonisierung: Neu hinzugefügt. | 
| [Prüfsumme](#distribution-prufsumme) (`spdx:checksum`) | Harmonisierung: Verwendungshinweis hinzugefügt. | 


### Klasse: Zeitraum

Auf Ebene der Klasse [Zeitraum](#klasse-zeitraum) (`dcterms:PeriodOfTime`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Startzeitpunkt](#zeitraum-startzeitpunkt) (`dcat:startDate`) | Errata: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Endzeitpunkt](#zeitraum-endzeitpunkt) (`dcat:endDate`) | Errata: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 


### Klasse: Standort

Auf Ebene der Klasse [Standort](#klasse-standort) (`dcterms:Location`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Bounding Box](#standort-bounding-box) (`dcat:bbox`) | Errata: Korrektur des zu verwendenden Types. | 
| [Geografischer Mittelpunkt](#standort-geografischer-mittelpunkt) (`dcat:centroid`) | Errata: Korrektur des zu verwendenden Types. | 
| [Geometrie](#standort-geometrie) (`locn:geometry`) | Harmonisierung: Wertebereich auf locn:Geometry geändert.<br>Harmonisierung: Verwendungshinweis von DCAT hinzugefügt. | 


### Klasse: Verantwortliche Stelle

Auf Ebene der Klasse [Verantwortliche Stelle](#klasse-verantwortliche-stelle) (`foaf:Agent`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Typ](#verantwortliche-stelle-typ) (`dcterms:type`) | Errata: Link zur zu verwendenden Codeliste hinzugefügt, war zuvor bei `foaf:name` angegeben. | 


### Klasse: Kontaktinformationen

Auf Ebene der Klasse [Kontaktinformationen](#klasse-kontaktinformationen) (`vcard:Kind`) gibt es 
folgende Änderungen zur Vorversion:

> Weiterentwicklung: Neu hinzugefügt.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Name](#kontaktinformationen-name) (`vcard:fn`) | Weiterentwicklung: Neu hinzugefügt. | 
| [E-Mail](#kontaktinformationen-email) (`vcard:hasEmail`) | Weiterentwicklung: Neu hinzugefügt. | 
| [Kontaktformular/Chatbot](#kontaktinformationen-url) (`vcard:hasURL`) | Weiterentwicklung: Neu hinzugefügt. | 
| [Telefon](#kontaktinformationen-telefon) (`vcard:hasTelephone`) | Weiterentwicklung: Neu hinzugefügt. | 


### Klasse: Prüfsumme

Auf Ebene der Klasse [Prüfsumme](#klasse-prufsumme) (`spdx:Checksum`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Algorithmus](#prufsumme-algorithmus) (`spdx:algorithm`) | Errata: Range von `rdfs:Resource` auf `spdx:ChecksumAlgorithm` geändert. | 


### Klasse: Katalogeintrag

Auf Ebene der Klasse [Katalogeintrag](#klasse-katalogeintrag) (`dcat:CatalogRecord`) gibt es 
keine Änderungen zur Vorversion.

Bei ihren Eigenschaften gibt es folgende Änderungen zur Vorversion:

| Eigenschaft           | Änderungen                      |
|:----------------------|:--------------------------------|
| [Aktualisierungsdatum](#katalogeintrag-aktualisierungsdatum) (`dcterms:modified`) | Errata: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Application Profile der Metadaten](#katalogeintrag-konform-zu) (`dcterms:conformsTo`) | Harmonisierung: Kardinalität von `0..1` auf `*` geändert.<br>Errata: Anzeige des Wertebereichs korrigiert. | 
| [Veröffentlichungsdatum](#katalogeintrag-veroffentlichungsdatum) (`dcterms:issued`) | Errata: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
| [Katalogeintrag](#katalogeintrag-katalogeintrag) (`foaf:primaryTopic`) | Harmonisierung: Aufnahme der Ressource `dcat:DatasetSeries` | 


