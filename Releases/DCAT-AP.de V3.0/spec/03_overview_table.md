| Klasse | Verpflichtend | Empfohlen | Optional |
| ------ | ------------- | --------- | -------- |
| [Katalog](#klasse-katalog)<br>(`dcat:Catalog`) |[`dct:title`](#katalog-titel)<br>[`dct:description`](#katalog-beschreibung)<br>[`dcat:dataset`](#katalog-datensatz)<br>[`dct:publisher`](#katalog-herausgeber)<br> | [`dct:issued`](#katalog-veroffentlichungsdatum)<br>[`dct:modified`](#katalog-aktualisierungsdatum)<br>[`dct:language`](#katalog-sprache)<br>[`foaf:homepage`](#katalog-homepage)<br>[`dct:license`](#katalog-lizenz)<br>[`dcat:themeTaxonomy`](#katalog-kategorienschema)<br>[`dcatap:availability`](#katalog-verfugbarkeit)<br>[`dct:spatial`](#katalog-raumliche-abdeckung)<br> | [`dct:rights`](#katalog-nutzungsbestimmungen)<br>[`dcat:catalog`](#katalog-katalog)<br>[`dcat:service`](#katalog-datenservice)<br>[`dct:hasPart`](#katalog-hat-teilkatalog)<br>[`dct:isPartOf`](#katalog-ist-teilkatalog)<br>[`dcat:record`](#katalog-katalogeintrag)<br>[`dct:creator`](#katalog-autor)<br> |

| Klasse | Verpflichtend | Empfohlen | Optional |
| ------ | ------------- | --------- | -------- |
| [Datensatz](#klasse-datensatz)<br>(`dcat:Dataset`) |[`dct:title`](#datensatz-titel)<br>[`dct:description`](#datensatz-beschreibung)<br> | [`dcat:keyword`](#datensatz-schlagwort)<br>[`dcatde:politicalGeocodingLevelURI`](#datensatz-ebene-geopolitischen-abdeckung)<br>[`dcatde:politicalGeocodingURI`](#datensatz-geopolitischen-abdeckung)<br>[`dcat:theme`](#datensatz-kategorie)<br>[`dcat:contactPoint`](#datensatz-kontakt)<br>[`dcatap:availability`](#datensatz-verfugbarkeit)<br>[`dct:spatial`](#datensatz-raumliche-abdeckung)<br>[`dct:temporal`](#datensatz-zeitliche-abdeckung)<br>[`dcat:distribution`](#datensatz-distribution)<br>[`dct:publisher`](#datensatz-herausgeber)<br> | [`dcatde:contributorID`](#datensatz-datenbereitsteller-id)<br>[`dcatde:geocodingDescription`](#datensatz-beschreibung-abdeckung)<br>[`dct:identifier`](#datensatz-id)<br>[`adms:identifier`](#datensatz-andere-id)<br>[`dct:issued`](#datensatz-veroffentlichungsdatum)<br>[`dct:modified`](#datensatz-aktualisierungsdatum)<br>[`owl:versionInfo`](#datensatz-versionsbezeichnung)<br>[`adms:versionNotes`](#datensatz-versionserlauterung)<br>[`dcatde:legalBasis`](#datensatz-rechtsgrundlage-zugangseroffnung)<br>[`dct:relation`](#datensatz-verwandte-ressource)<br>[`dcat:landingPage`](#datensatz-ursprungliche-webseite)<br>[`foaf:page`](#datensatz-dokumentation)<br>[`dct:language`](#datensatz-sprache)<br>[`dct:conformsTo`](#datensatz-konform-zu-standard)<br>[`dct:accessRights`](#datensatz-grad-zuganglichkeit)<br>[`dct:provenance`](#datensatz-provenienz)<br>[`dct:accrualPeriodicity`](#datensatz-aktualisierungsfrequenz)<br>[`dcatde:qualityProcessURI`](#datensatz-qualitatssicherungsprozess)<br>[`dct:type`](#datensatz-typ)<br>[`prov:wasGeneratedBy`](#datensatz-wurde-erzeugt-von)<br>[`dcat:spatialResolutionInMeters`](#datensatz-raumliche-auflosung-in-meter)<br>[`dcat:temporalResolution`](#datensatz-zeitliche-auflosung)<br>[`dcat:granularity`](#datensatz-abgedeckte-zeitliche-granularitat-deprecated)<br>[`prov:qualifiedAttribution`](#datensatz-rollenzuordnung)<br>[`dcat:qualifiedRelation`](#datensatz-qualifizierte-beziehung)<br>[`dct:isReferencedBy`](#datensatz-wird-referenziert)<br>[`dct:references`](#datensatz-referenziert)<br>[`dct:source`](#datensatz-quelle)<br>[`dct:hasVersion`](#datensatz-weitere-version)<br>[`dct:isVersionOf`](#datensatz-ist-version)<br>[`adms:sample`](#datensatz-beispieldistribution)<br>[`dct:creator`](#datensatz-autor)<br>[`dct:contributor`](#datensatz-bearbeiter)<br>[`dcatde:originator`](#datensatz-urheber)<br>[`dcatde:maintainer`](#datensatz-verwalter)<br> |

| Klasse | Verpflichtend | Empfohlen | Optional |
| ------ | ------------- | --------- | -------- |
| [Datenservice](#klasse-datenservice)<br>(`dcat:DataService`) |[`dcat:endpointURL`](#datenservice-url-endpunkt)<br>[`dct:title`](#datenservice-titel)<br> | [`dcat:endpointDescription`](#datenservice-beschreibung-endpunkt)<br>[`dcatap:availability`](#datenservice-verfugbarkeit)<br>[`dcat:servesDataset`](#datenservice-liefert-datensatz-aus)<br> | [`dct:description`](#datenservice-beschreibung)<br>[`dct:license`](#datenservice-lizenz)<br>[`dct:accessRights`](#datenservice-grad-zuganglichkeit)<br> |

| Klasse | Verpflichtend | Empfohlen | Optional |
| ------ | ------------- | --------- | -------- |
| [Distribution](#klasse-distribution)<br>(`dcat:Distribution`) |[`dcat:accessURL`](#distribution-zugangs-url)<br> | [`dct:title`](#distribution-titel)<br>[`dct:modified`](#distribution-aktualisierungsdatum)<br>[`dct:license`](#distribution-lizenz)<br>[`dct:format`](#distribution-format)<br>[`dcatap:availability`](#distribution-verfugbarkeit)<br>[`dcatde:plannedAvailability`](#distribution-verfugbarkeit-deprecated)<br> | [`dcatde:licenseAttributionByText`](#distribution-namensnennungstext-by-clauses)<br>[`dct:description`](#distribution-beschreibung)<br>[`dcat:byteSize`](#distribution-grosse-in-bytes)<br>[`dct:issued`](#distribution-veroffentlichungsdatum)<br>[`dcat:downloadURL`](#distribution-download-url)<br>[`dct:language`](#distribution-sprache)<br>[`foaf:page`](#distribution-dokumentation)<br>[`dct:rights`](#distribution-grad-zuganglichkeit)<br>[`dct:conformsTo`](#distribution-konform-zu-standard)<br>[`dcat:mediaType`](#distribution-medientyp)<br>[`dcat:compressFormat`](#distribution-kompressionsformat)<br>[`dcat:packageFormat`](#distribution-paketformat)<br>[`odrl:hasPolicy`](#distribution-regelwerk)<br>[`adms:status`](#distribution-status)<br>[`dcat:accessService`](#distribution-ausliefernder-datenservice)<br>[`spdx:checksum`](#distribution-prufsumme)<br> |

| Klasse | Verpflichtend | Empfohlen | Optional |
| ------ | ------------- | --------- | -------- |
| [Zeitraum](#klasse-zeitraum)<br>(`dct:PeriodOfTime`) | | [`dcat:startDate`](#zeitraum-startzeitpunkt)<br>[`dcat:endDate`](#zeitraum-endzeitpunkt)<br> | [`time:hasBeginning`](#zeitraum-anfang)<br>[`time:hasEnd`](#zeitraum-ende)<br>[`schema:startDate`](#zeitraum-startzeitpunkt-deprecated)<br>[`schema:endDate`](#zeitraum-endzeitpunkt-deprecated)<br> |

| Klasse | Verpflichtend | Empfohlen | Optional |
| ------ | ------------- | --------- | -------- |
| [Standort](#klasse-standort)<br>(`dct:Location`) | | [`dcat:bbox`](#standort-bounding-box)<br>[`dcat:centroid`](#standort-geografischer-mittelpunkt)<br> | [`locn:geometry`](#standort-geometrie)<br> |

| Klasse | Verpflichtend | Empfohlen | Optional |
| ------ | ------------- | --------- | -------- |
| [Verantwortliche Stelle](#klasse-verantwortliche-stelle)<br>(`foaf:Agent`) |[`foaf:name`](#verantwortliche-stelle-name)<br> |  | [`dct:type`](#verantwortliche-stelle-typ)<br> |

| Klasse | Verpflichtend | Empfohlen | Optional |
| ------ | ------------- | --------- | -------- |
| [Identifier](#klasse-identifier)<br>(`adms:Identifier`) |[`skos:notation`](#identifier-notation)<br> |  |  |

| Klasse | Verpflichtend | Empfohlen | Optional |
| ------ | ------------- | --------- | -------- |
| [Prüfsumme](#klasse-prufsumme)<br>(`spdx:Checksum`) |[`spdx:algorithm`](#prufsumme-algorithmus)<br>[`spdx:checksumValue`](#prufsumme-prufsummenwert)<br> |  |  |

| Klasse | Verpflichtend | Empfohlen | Optional |
| ------ | ------------- | --------- | -------- |
| [Katalogeintrag](#klasse-katalogeintrag)<br>(`dcat:CatalogRecord`) |[`dct:modified`](#katalogeintrag-aktualisierungsdatum)<br>[`foaf:primaryTopic`](#katalogeintrag-katalogeintrag)<br> | [`dct:conformsTo`](#katalogeintrag-konform-zu)<br>[`adms:status`](#katalogeintrag-anderungstyp)<br>[`dct:issued`](#katalogeintrag-veroffentlichungsdatum)<br> | [`dct:title`](#katalogeintrag-titel)<br>[`dct:description`](#katalogeintrag-beschreibung)<br>[`dct:language`](#katalogeintrag-sprache)<br>[`dct:source`](#katalogeintrag-original-metadaten-der-ressource)<br> |

| Klasse | Verpflichtend | Empfohlen | Optional |
| ------ | ------------- | --------- | -------- |
| [Lizenzdokument](#klasse-lizenzdokument)<br>(`dct:LicenceType`) | | [`dct:type`](#lizenzdokument-lizenztyp)<br> |  |

| Klasse | Verpflichtend | Empfohlen | Optional |
| ------ | ------------- | --------- | -------- |
| [Beziehung](#klasse-beziehung)<br>(`dcat:Relationship`) |[`dcat:hadRole`](#beziehung-rolle)<br>[`dct:relation`](#beziehung-beziehung)<br> |  |  |

| Klasse | Verpflichtend | Empfohlen | Optional |
| ------ | ------------- | --------- | -------- |
| [Rollenzuordnung](#klasse-rollenzuordnung)<br>(`prov:Attribution`) |[`dcat:hadRole`](#rollenzuordnung-rolle)<br>[`prov:agent`](#rollenzuordnung-agent)<br> |  |  |

| Klasse | Verpflichtend | Empfohlen | Optional |
| ------ | ------------- | --------- | -------- |
| [Kategorie](#klasse-kategorie)<br>(`skos:Concept`) |[`skos:prefLabel`](#kategorie-bezeichnung)<br> |  |  |

| Klasse | Verpflichtend | Empfohlen | Optional |
| ------ | ------------- | --------- | -------- |
| [Kategorienschema](#klasse-kategorienschema)<br>(`skos:ConceptScheme`) |[`dct:title`](#kategorienschema-bezeichnung)<br> |  |  |



