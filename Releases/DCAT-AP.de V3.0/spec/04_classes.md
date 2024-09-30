## Klasse: Katalog

> | *URI der Klasse* | [`dcat:Catalog`](http://www.w3.org/ns/dcat#Catalog)      |
> |:-----------------|:-----------------------------------------------------|
> | Beschreibung     | Eine Sammlung oder Quelle, welche die beschriebenen Datensätze, Datenservices oder Kataloge zur Verfügung stellt.     |
> | eingebunden über | dcat:catalog, dcterms:hasPart, dcterms:isPartOf (dcat:Catalog)         | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Catalogue), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Class:Catalog) |

<br>

Die folgenden Eigenschaften wurden von DCAT-AP.de hinzugefügt oder verändert: 
[`dcatap:availability`](#katalog-verfugbarkeit), [`dcterms:isPartOf`](#katalog-ist-teilkatalog), [`dcat:record`](#katalog-katalogeintrag), [`dcterms:publisher`](#katalog-herausgeber).<br>


|                                 | Eigenschaft  | Wertebereich      | <small>Verbind&shy;lichkeit</small> | Mult. | Interop. |
|:--------------------------------|:-------------|:------------------|:------------------------------------|:-----:|:--------:|
| [Titel](#katalog-titel) | `dcterms:title` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Pflicht</small> | `[1..*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Beschreibung](#katalog-beschreibung) | `dcterms:description` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Pflicht</small> | `[1..*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Herausgeber](#katalog-herausgeber) | `dcterms:publisher` | [`foaf:Agent`](http://xmlns.com/foaf/0.1/Agent) | <small>Pflicht</small> | `[1]` | <abbr title='Eigenes ergänzt.'>E</abbr> |
| [Veröffentlichungsdatum](#katalog-veroffentlichungsdatum) | `dcterms:issued` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Empfohlen</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Aktualisierungsdatum](#katalog-aktualisierungsdatum) | `dcterms:modified` | [`rdfs:Literal`]() | <small>Empfohlen</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Sprache](#katalog-sprache) | `dcterms:language` | [`dcterms:LinguisticSystem`](http://purl.org/dc/terms/LinguisticSystem) | <small>Empfohlen</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Homepage](#katalog-homepage) | `foaf:homepage` | [`foaf:Document`](http://xmlns.com/foaf/0.1/Document) | <small>Empfohlen</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Lizenz](#katalog-lizenz) | `dcterms:license` | [`dcterms:LicenseDocument`](http://purl.org/dc/terms/LicenseDocument) | <small>Empfohlen</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Kategorienschema](#katalog-kategorienschema) | `dcat:themeTaxonomy` | [`skos:ConceptScheme`](http://www.w3.org/2004/02/skos/core#ConceptScheme) | <small>Empfohlen</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Verfügbarkeit](#katalog-verfugbarkeit) | `dcatap:availability` | [`skos:Concept`](http://www.w3.org/2000/01/rdf-schema#Resource) | <small>Empfohlen</small> | `[0..1]` | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
| [Räumliche Abdeckung](#katalog-raumliche-abdeckung) | `dcterms:spatial` | [`dcterms:Location`](http://purl.org/dc/terms/Location) | <small>Empfohlen</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Datensatz](#katalog-datensatz) | `dcat:dataset` | [`dcat:Dataset`](http://www.w3.org/ns/dcat#Dataset) | <small>Empfohlen</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Rechte](#katalog-rechte) | `dcterms:rights` | [`dcterms:RightsStatement`](http://purl.org/dc/terms/RightsStatement) | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Katalog](#katalog-katalog) | `dcat:catalog` | [`dcat:Catalog`](http://www.w3.org/ns/dcat#Catalog) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Datenservice](#katalog-datenservice) | `dcat:service` | [`dcat:DataService`](http://www.w3.org/ns/dcat#DataService) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Hat Teilkatalog](#katalog-hat-teilkatalog) | `dcterms:hasPart` | [`dcat:Catalog`](http://www.w3.org/ns/dcat#Catalog) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Ist Teilkatalog](#katalog-ist-teilkatalog) | `dcterms:isPartOf` | [`dcat:Catalog`](http://www.w3.org/ns/dcat#Catalog) | <small>Optional</small> | `[0..1]` | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
| [Katalogeintrag](#katalog-katalogeintrag) | `dcat:record` | [`dcat:CatalogRecord`](http://www.w3.org/ns/dcat#CatalogRecord) | <small>Optional</small> | `[*]` | <abbr title='Eigenes ergänzt.'>E</abbr> |
| [Autor](#katalog-autor) | `dcterms:creator` | [`foaf:Agent`](http://xmlns.com/foaf/0.1/Agent) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |


<br> Die folgenden weiteren Eigenschaften wurden von der Superklasse [`dcat:Resource`](#klasse-ressource) geerbt, werden aber nicht genauer betrachtet: [`odrl:hasPolicy`](#distribution-regelwerk).


<br>
<hr>
<br>

###  Katalog: Titel {#katalog-titel}
> | *URI*                      | [`dcterms:title`](http://purl.org/dc/terms/title) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1..*]`                   |
> | Beschreibung               | Diese Eigenschaft bezeichnet den einem Katalog zugewiesenen Titel. |
> | Verwendungshinweis | Diese Eigenschaft kann für parallele Sprachversionen des Katalogtitels wiederholt werden. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Catalogue.title), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_title)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Katalog: Beschreibung {#katalog-beschreibung}
> | *URI*                      | [`dcterms:description`](http://purl.org/dc/terms/description) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1..*]`                   |
> | Beschreibung               | Diese Eigenschaft enthält eine Beschreibung des Kataloges als Freitext. |
> | Verwendungshinweis | Diese Eigenschaft kann für parallel existierende Sprachversionen der Katalogbeschreibung wiederholt werden. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Catalogue.description), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_description)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Katalog: Herausgeber {#katalog-herausgeber}
> | *URI*                      | [`dcterms:publisher`](http://purl.org/dc/terms/publisher) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`foaf:Agent`](http://xmlns.com/foaf/0.1/Agent) |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf die Stelle oder Person, die verantwortlich für Bereitstellung des Kataloges ist. |
> | Verwendungshinweis | Es ist zugleich die Stelle oder Person, die über die Einräumung von Zugang und Nutzungsrechten für Dritte entschieden hat.<br>Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#angaben-zum-herausgeber) genauer beschrieben. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Catalogue.publisher), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_publisher)  | 
> | Interoperabilitätslevel    | <abbr title='Eigenes ergänzt.'>E</abbr> |
> | Änderungen durch DCAT-AP.de | Erweiterung des Verwendungshinweises. | 
<br>

###  Katalog: Veröffentlichungsdatum {#katalog-veroffentlichungsdatum}
> | *URI*                      | [`dcterms:issued`](http://purl.org/dc/terms/issued) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) getyped als `xsd:gYear`, `xsd:gYearMonth`, `xsd:date` oder `xsd:dateTime` |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft enthält das Datum der Herausgabe/Emission (z.B. in Form einer Veröffentlichung) des Kataloges. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Catalogue.releasedate), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_release_date)  | 
> | Änderungen zur Vorversion | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Katalog: Aktualisierungsdatum {#katalog-aktualisierungsdatum}
> | *URI*                      | [`dcterms:modified`](http://purl.org/dc/terms/modified) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) getyped als `xsd:gYear`, `xsd:gYearMonth`, `xsd:date` oder `xsd:dateTime` |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft erfasst das Datum der letzten Aktualisierung bzw. Modifikation des Kataloges. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Catalogue.modificationdate), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_update_date)  | 
> | Änderungen zur Vorversion | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Katalog: Sprache {#katalog-sprache}
> | *URI*                      | [`dcterms:language`](http://purl.org/dc/terms/language) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:LinguisticSystem`](http://purl.org/dc/terms/LinguisticSystem) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf die Sprache, die in den textuellen Beschreibungen der dem Katalog zugehörigen DCAT-Ressourcen Verwendung findet (z.B. Titel, Beschreibungen usw.).  |
> | Verwendungshinweis | Diese Eigenschaft kann wiederholt werden, falls die Metadaten in verschiedenen Sprachen zur Verfügung stehen. | 
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-languages) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Catalogue.language), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_language)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Katalog: Homepage {#katalog-homepage}
> | *URI*                      | [`foaf:homepage`](http://xmlns.com/foaf/0.1/homepage) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`foaf:Document`](http://xmlns.com/foaf/0.1/Document) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf eine Homepage, welche die zentrale Homepage des Kataloges ist. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Catalogue.homepage), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:catalog_homepage)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Katalog: Lizenz {#katalog-lizenz}
> | *URI*                      | [`dcterms:license`](http://purl.org/dc/terms/license) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:LicenseDocument`](http://purl.org/dc/terms/LicenseDocument) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf die Lizenz, mit welcher der Katalog verwendet oder wiederverwendet werden kann. |
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-licenses) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Catalogue.licence), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_license)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Katalog: Kategorienschema {#katalog-kategorienschema}
> | *URI*                      | [`dcat:themeTaxonomy`](http://www.w3.org/ns/dcat#themeTaxonomy) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`skos:ConceptScheme`](http://www.w3.org/2004/02/skos/core#ConceptScheme) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf das eingesetzte Schema zur Klassifizierung der dem Katalog zugewiesenen DCAT-Ressourcen in Form von Kategorien. |
> | Verwendungshinweis | Für DCAT-AP.de muss dieser Wert immer mindestens http://publications.europa.eu/resource/authority/data-theme sein. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Catalogue.themes), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:catalog_themes)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Katalog: Verfügbarkeit {#katalog-verfugbarkeit}
> | *URI*                      | [`dcatap:availability`](http://data.europa.eu/r5r/availability) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`skos:Concept`](http://www.w3.org/2000/01/rdf-schema#Resource) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Geplante Verfügbarkeit des Katalogs als Auswahl aus einer festen Liste von Werten via DCAT-AP URIs. |
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-availability) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.availability)  | 
> | Interoperabilitätslevel    | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
> | Änderungen durch DCAT-AP.de | DCAT-AP.de ordnet diese Eigenschaft allen DCAT-Ressourcen und Distributionen zu. | 
<br>

###  Katalog: Räumliche Abdeckung {#katalog-raumliche-abdeckung}
> | *URI*                      | [`dcterms:spatial`](http://purl.org/dc/terms/spatial) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:Location`](http://purl.org/dc/terms/Location) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf einen vom Katalog abgedeckten geographischen Bereich. |
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-spatial) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Catalogue.geographicalcoverage), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:dataset_spatial)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Katalog: Datensatz {#katalog-datensatz}
> | *URI*                      | [`dcat:dataset`](http://www.w3.org/ns/dcat#dataset) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcat:Dataset`](http://www.w3.org/ns/dcat#Dataset) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft verknüpft den Katalog mit einem Datensatz, welcher somit Teil des Kataloges wird. |
> | Verwendungshinweis | Da leere Kataloge in der Regel auf Probleme hinweisen, sollte diese Eigenschaft mit der Eigenschaft "Datenservice" kombiniert werden, um eine Überprüfung auf leere Kataloge zu implementieren. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Catalogue.dataset), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:catalog_dataset)  | 
> | Änderungen zur Vorversion | 3.0: Harmonisierung: Kardinalität von `1..*` auf `*` geändert. Verbindlichkeit auf "Empfohlen" gesenkt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Katalog: Rechte {#katalog-rechte}
> | *URI*                      | [`dcterms:rights`](http://purl.org/dc/terms/rights) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:RightsStatement`](http://purl.org/dc/terms/RightsStatement) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf eine juristische Darlegung, welche die mit dem Katalog assoziierten Nutzungsbestimmungen spezifiziert. |
> | Verwendungshinweis | Gemeint ist damit zum Beispiel ein Link zu Nutzungsbedingungen, wie "Terms of Use", die zusätzlich zu oder statt einer Lizenz bestehen. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Catalogue.rights), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_rights)  | 
> | Änderungen zur Vorversion | 3.0: In "Rechte" umbenannt und Verwendungshinweis hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Katalog: Katalog {#katalog-katalog}
> | *URI*                      | [`dcat:catalog`](http://www.w3.org/ns/dcat#catalog) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcat:Catalog`](http://www.w3.org/ns/dcat#Catalog) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Ein Katalog, dessen Inhalt im Kontext dieses Katalogs von Interesse ist. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Catalogue.catalogue), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:catalog_catalog)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Katalog: Datenservice {#katalog-datenservice}
> | *URI*                      | [`dcat:service`](http://www.w3.org/ns/dcat#service) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcat:DataService`](http://www.w3.org/ns/dcat#DataService) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft verknüpft den Katalog mit einem Datenservice, welcher somit Teil des Kataloges wird. |
> | Verwendungshinweis | Da leere Kataloge in der Regel auf Probleme hinweisen, sollte diese Eigenschaft mit der Eigenschaft "Datensatz" kombiniert werden, um eine Überprüfung auf leere Kataloge zu implementieren. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Catalogue.service), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:catalog_service)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Katalog: Hat Teilkatalog {#katalog-hat-teilkatalog}
> | *URI*                      | [`dcterms:hasPart`](http://purl.org/dc/terms/hasPart) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcat:Catalog`](http://www.w3.org/ns/dcat#Catalog) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf einen in Beziehung stehenden Unterkatalog, der Teil des beschriebenen Kataloges ist. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Catalogue.haspart), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:catalog_has_part)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Katalog: Ist Teilkatalog {#katalog-ist-teilkatalog}
> | *URI*                      | [`dcterms:isPartOf`](http://purl.org/dc/terms/isPartOf) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcat:Catalog`](http://www.w3.org/ns/dcat#Catalog) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf einen in Beziehung stehenden Hauptkatalog, in welchem der beschriebene Katalog physikalisch oder logisch eingebunden ist. |
> | Verwendungshinweis | Nicht Teil von W3C-DCAT, wurde ursprünglich von DCAT-AP hinzugefügt und mit der Version 3.0 wieder entfernt. | 
> | Weiterführende Dokumentationen | [DCMI Metadata Terms](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/#http://purl.org/dc/terms/isPartOf)  | 
> | Interoperabilitätslevel    | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
> | Änderungen durch DCAT-AP.de | Eigenschaft wird für Kataloge beibehalten. | 
<br>

###  Katalog: Katalogeintrag {#katalog-katalogeintrag}
> | *URI*                      | [`dcat:record`](http://www.w3.org/ns/dcat#record) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcat:CatalogRecord`](http://www.w3.org/ns/dcat#CatalogRecord) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf den Katalogeintrag, welcher Teil des Kataloges ist. |
> | Verwendungshinweis | Diese Eigenschaft darf nur mit der besonderen Klasse [`dcat:CatalogRecord`](#klasse-katalogeintrag) verwendet werden. Es handelt sich dabei nicht um einen gewöhnlichen Datensatz. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Catalogue.record), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:catalog_catalog_record)  | 
> | Interoperabilitätslevel    | <abbr title='Eigenes ergänzt.'>E</abbr> |
> | Änderungen durch DCAT-AP.de | DCAT-AP.de bindet einen zusätzlichen Verwendungshinweis ein. | 
<br>

###  Katalog: Autor {#katalog-autor}
> | *URI*                      | [`dcterms:creator`](http://purl.org/dc/terms/creator) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`foaf:Agent`](http://xmlns.com/foaf/0.1/Agent) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf Stellen oder Personen, die den Katalog erstellt haben. |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#weitere-wichtige-rollen) genauer beschrieben. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Catalogue.creator), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_creator)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>



***


## Klasse: Datensatz

> | *URI der Klasse* | [`dcat:Dataset`](http://www.w3.org/ns/dcat#Dataset)      |
> |:-----------------|:-----------------------------------------------------|
> | Beschreibung     | Eine logische Entität, welche die veröffentlichten Informationen repräsentiert.     |
> | eingebunden über | dcat:dataset (dcat:Catalog), dcterms:hasVersion, dcterms:isVersionOf, dcterms:source, (dcat:Dataset), dcat:servesDataset (dcat:DataService), foaf:primaryTopic (dcat:CatalogRecord)         | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Class:Dataset) |

<br>

Die folgenden Eigenschaften wurden von DCAT-AP.de hinzugefügt oder verändert: 
[`dcatde:politicalGeocodingLevelURI`](#datensatz-ebene-geopolitischen-abdeckung), [`dcatde:politicalGeocodingURI`](#datensatz-geopolitischen-abdeckung), [`dcatap:availability`](#datensatz-verfugbarkeit), [`dcatde:contributorID`](#datensatz-datenbereitsteller-id), [`dcatde:geocodingDescription`](#datensatz-beschreibung-abdeckung), [`dcat:version`](#datensatz-versionsbezeichnung), [`dcatap:applicableLegislation`](#datensatz-rechtsgrundlage), [`dcatde:legalBasis`](#datensatz-rechtsgrundlage-zugangseroffnung), [`dcterms:provenance`](#datensatz-provenienz), [`dcatde:qualityProcessURI`](#datensatz-qualitatssicherungsprozess), [`prov:wasGeneratedBy`](#datensatz-wurde-erzeugt-von), [`dcat:spatialResolutionInMeters`](#datensatz-raumliche-auflosung-in-meter), [`dcterms:references`](#datensatz-referenziert), [`dcterms:spatial`](#datensatz-raumliche-abdeckung), [`dcterms:publisher`](#datensatz-herausgeber), [`dcterms:contributor`](#datensatz-bearbeiter), [`dcatde:originator`](#datensatz-urheber), [`dcatde:maintainer`](#datensatz-verwalter).<br>


|                                 | Eigenschaft  | Wertebereich      | <small>Verbind&shy;lichkeit</small> | Mult. | Interop. |
|:--------------------------------|:-------------|:------------------|:------------------------------------|:-----:|:--------:|
| [Titel](#datensatz-titel) | `dcterms:title` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Pflicht</small> | `[1..*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Beschreibung](#datensatz-beschreibung) | `dcterms:description` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Pflicht</small> | `[1..*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Herausgeber](#datensatz-herausgeber) | `dcterms:publisher` | [`foaf:Agent`](http://xmlns.com/foaf/0.1/Agent) | <small>Pflicht</small> | `[1]` | <abbr title='Eigenes ergänzt.'>E</abbr> |
| [Schlagwort](#datensatz-schlagwort) | `dcat:keyword` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Empfohlen</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Ebene der geopolitischen Abdeckung](#datensatz-ebene-geopolitischen-abdeckung) | `dcatde:politicalGeocodingLevelURI` | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) | <small>Empfohlen</small> | `[*]` | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
| [Geopolitische Abdeckung (DEPRECATED)](#datensatz-geopolitischen-abdeckung) | `dcatde:politicalGeocodingURI` | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) | <small>Empfohlen</small> | `[*]` | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
| [Kategorie](#datensatz-kategorie) | `dcat:theme` | [`skos:Concept`](http://www.w3.org/2004/02/skos/core#Concept) | <small>Empfohlen</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Kontakt](#datensatz-kontakt) | `dcat:contactPoint` | [`vcard:Kind`](http://www.w3.org/TR/vcard-rdf/#Kind) | <small>Empfohlen</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Verfügbarkeit](#datensatz-verfugbarkeit) | `dcatap:availability` | [`skos:Concept`](http://www.w3.org/2000/01/rdf-schema#Resource) | <small>Empfohlen</small> | `[0..1]` | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
| [Räumliche Abdeckung](#datensatz-raumliche-abdeckung) | `dcterms:spatial` | [`dcterms:Location`](http://purl.org/dc/terms/Location) | <small>Empfohlen</small> | `[*]` | <abbr title='Eigenes ergänzt.'>E</abbr> |
| [Zeitliche Abdeckung](#datensatz-zeitliche-abdeckung) | `dcterms:temporal` | [`dcterms:PeriodOfTime`](http://purl.org/dc/terms/PeriodOfTime) | <small>Empfohlen</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Distribution](#datensatz-distribution) | `dcat:distribution` | [`dcat:Distribution`](http://www.w3.org/ns/dcat#Distribution) | <small>Empfohlen</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Datenbereitsteller ID](#datensatz-datenbereitsteller-id) | `dcatde:contributorID` | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) | <small>Optional</small> | `[*]` | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
| [Beschreibung der Abdeckung (DEPRECATED)](#datensatz-beschreibung-abdeckung) | `dcatde:geocodingDescription` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Optional</small> | `[*]` | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
| [ID](#datensatz-id) | `dcterms:identifier` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Andere ID](#datensatz-andere-id) | `adms:identifier` | [`adms:Identifier`](http://www.w3.org/ns/adms#Identifier) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Veröffentlichungsdatum](#datensatz-veroffentlichungsdatum) | `dcterms:issued` | [`rdfs:Literal`]() | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Aktualisierungsdatum](#datensatz-aktualisierungsdatum) | `dcterms:modified` | [`rdfs:Literal`]() | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Versionsbezeichnung](#datensatz-versionsbezeichnung) | `dcat:version` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Optional</small> | `[*]` | <abbr title='Eigenes ergänzt.'>E</abbr> |
| [Versionsbezeichnung (DEPRECATED)](#datensatz-versionsbezeichnung-deprecated) | `owl:versionInfo` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Versionserläuterung](#datensatz-versionserlauterung) | `adms:versionNotes` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Rechtsgrundlage](#datensatz-rechtsgrundlage) | `dcatap:applicableLegislation` | [`eli:LegalResource`](http://data.europa.eu/eli/ontology#LegalResource) | <small>Optional</small> | `[*]` | <abbr title='Eigenes ergänzt.'>E</abbr> |
| [Rechtsgrundlage für die Zugangseröffnung (DEPRECATED)](#datensatz-rechtsgrundlage-zugangseroffnung) | `dcatde:legalBasis` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Optional</small> | `[*]` | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
| [Verwandte Ressource](#datensatz-verwandte-ressource) | `dcterms:relation` | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Ursprüngliche Webseite](#datensatz-ursprungliche-webseite) | `dcat:landingPage` | [`foaf:Document`](http://xmlns.com/foaf/0.1/Document) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Dokumentation](#datensatz-dokumentation) | `foaf:page` | [`foaf:Document`](http://xmlns.com/foaf/0.1/Document) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Sprache](#datensatz-sprache) | `dcterms:language` | [`dcterms:LinguisticSystem`](http://purl.org/dc/terms/LinguisticSystem) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Konform zu Standard](#datensatz-konform-zu-standard) | `dcterms:conformsTo` | [`dcterms:Standard`](http://purl.org/dc/terms/Standard) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Grad der Zugänglichkeit](#datensatz-grad-zuganglichkeit) | `dcterms:accessRights` | [`dcterms:RightsStatement`](http://purl.org/dc/terms/RightsStatement) | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Provenienz](#datensatz-provenienz) | `dcterms:provenance` | [`dcterms:ProvenanceStatement`](http://purl.org/dc/terms/ProvenanceStatement) | <small>Optional</small> | `[*]` | <abbr title='Eigenes ergänzt.'>E</abbr> |
| [Aktualisierungsfrequenz](#datensatz-aktualisierungsfrequenz) | `dcterms:accrualPeriodicity` | [`dcterms:Frequency`](http://purl.org/dc/terms/Frequency) | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Qualitätssicherungsprozess (DEPRECATED)](#datensatz-qualitatssicherungsprozess) | `dcatde:qualityProcessURI` | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) | <small>Optional</small> | `[0..1]` | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
| [Typ](#datensatz-typ) | `dcterms:type` | [`skos:Concept`](http://www.w3.org/2004/02/skos/core#Concept) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Wurde erzeugt von](#datensatz-wurde-erzeugt-von) | `prov:wasGeneratedBy` | [`prov:Activity`](https://www.w3.org/TR/prov-o/#Activity) | <small>Optional</small> | `[*]` | <abbr title='Eigenes ergänzt.'>E</abbr> |
| [Räumliche Auflösung in Meter](#datensatz-raumliche-auflosung-in-meter) | `dcat:spatialResolutionInMeters` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Optional</small> | `[0..1]` | <abbr title='Eigenes ergänzt.'>E</abbr> |
| [Zeitliche Auflösung](#datensatz-zeitliche-auflosung) | `dcat:temporalResolution` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Rollenzuordnung](#datensatz-rollenzuordnung) | `prov:qualifiedAttribution` | [`prov:Attribution`](https://www.w3.org/TR/prov-o/#Attribution) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Qualifizierte Beziehung](#datensatz-qualifizierte-beziehung) | `dcat:qualifiedRelation` | [`dcat:Relationship`](https://www.w3.org/TR/vocab-dcat-3/#Class:Relationship) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Wird Referenziert](#datensatz-wird-referenziert) | `dcterms:isReferencedBy` | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Referenziert](#datensatz-referenziert) | `dcterms:references` | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) | <small>Optional</small> | `[*]` | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
| [Quelle des Datensatzes](#datensatz-quelle) | `dcterms:source` | [`dcat:Dataset`](http://www.w3.org/ns/dcat#Dataset) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Weitere Version](#datensatz-weitere-version) | `dcat:hasVersion` | [`dcat:Dataset`](http://www.w3.org/ns/dcat#Dataset) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Weitere Version (DEPRECATED)](#datensatz-weitere-version-deprecated) | `dcterms:hasVersion` | [`dcat:Dataset`](http://www.w3.org/ns/dcat#Dataset) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Ist Version von (DEPRECATED)](#datensatz-ist-version) | `dcterms:isVersionOf` | [`dcat:Dataset`](http://www.w3.org/ns/dcat#Dataset) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Beispieldistribution](#datensatz-beispieldistribution) | `adms:sample` | [`dcat:Distribution`](http://www.w3.org/ns/dcat#Distribution) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Autor](#datensatz-autor) | `dcterms:creator` | [`foaf:Agent`](http://xmlns.com/foaf/0.1/Agent) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Bearbeiter](#datensatz-bearbeiter) | `dcterms:contributor` | [`foaf:Agent`](http://xmlns.com/foaf/0.1/Agent) | <small>Optional</small> | `[*]` | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
| [Urheber (DEPRECATED)](#datensatz-urheber) | `dcatde:originator` | [`foaf:Agent`](http://xmlns.com/foaf/0.1/Agent) | <small>Optional</small> | `[*]` | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
| [Verwalter (DEPRECATED)](#datensatz-verwalter) | `dcatde:maintainer` | [`foaf:Agent`](http://xmlns.com/foaf/0.1/Agent) | <small>Optional</small> | `[*]` | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
| [In Serie](#datensatz-in-serie) | `dcat:inSeries` | [`dcat:DatasetSeries`](http://www.w3.org/ns/dcat#DatasetSeries) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |


<br> Die folgenden weiteren Eigenschaften wurden von der Superklasse [`dcat:Resource`](#klasse-ressource) geerbt, werden aber nicht genauer betrachtet: [`dcterms:license`](#distribution-lizenz), [`dcterms:rights`](#distribution-grad-zuganglichkeit) und [`odrl:hasPolicy`](#distribution-regelwerk).


<br>
<hr>
<br>

###  Datensatz: Titel {#datensatz-titel}
> | *URI*                      | [`dcterms:title`](http://purl.org/dc/terms/title) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1..*]`                   |
> | Beschreibung               | Diese Eigenschaft bezeichnet den einem Datensatz zugewiesenen Titel. |
> | Verwendungshinweis | Diese Eigenschaft kann für parallele Sprachversionen des Datensatztitels wiederholt werden.<br>Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#redundante-angaben-im-titel) genauer beschrieben. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.title), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_title)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Beschreibung {#datensatz-beschreibung}
> | *URI*                      | [`dcterms:description`](http://purl.org/dc/terms/description) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1..*]`                   |
> | Beschreibung               | Diese Eigenschaft enthält eine Beschreibung des Datensatzes als Freitext. |
> | Verwendungshinweis | Diese Eigenschaft kann für parallel existierende Sprachversionen der Datensatzbeschreibung wiederholt werden. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.description), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_description)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Herausgeber {#datensatz-herausgeber}
> | *URI*                      | [`dcterms:publisher`](http://purl.org/dc/terms/publisher) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`foaf:Agent`](http://xmlns.com/foaf/0.1/Agent) |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf die Stelle oder Person, die für Bereitstellung des Datensatzes verantwortlich ist. |
> | Verwendungshinweis | Es ist zugleich die Stelle oder Person, die über die Einräumung von Zugang und Nutzungsrechten für Dritte entschieden hat.<br>Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#angaben-zum-herausgeber) genauer beschrieben. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.publisher), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_publisher)  | 
> | Änderungen zur Vorversion | 3.0: Anforderung: Nutzung verpflichtend gemacht. | 
> | Interoperabilitätslevel    | <abbr title='Eigenes ergänzt.'>E</abbr> |
> | Änderungen durch DCAT-AP.de | Erweiterung des Verwendungshinweises. Nutzung verpflichtend gemacht. | 
<br>

###  Datensatz: Schlagwort {#datensatz-schlagwort}
> | *URI*                      | [`dcat:keyword`](http://www.w3.org/ns/dcat#keyword) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft enthält ein Schlagwort oder Schlüsselbegriff zur Beschreibung des Datensatzes.  |
> | Verwendungshinweis | Diese Eigenschaft kann für unterschiedliche Schlagworte und parallel existierende Sprachversionen wiederholt werden. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.keyword), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_keyword)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Ebene der geopolitischen Abdeckung {#datensatz-ebene-geopolitischen-abdeckung}
> | *URI*                      | [`dcatde:politicalGeocodingLevelURI`](http://dcat-ap.de/def/dcatde/politicalGeocodingLevelURI) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Geopolitische Abdeckung des Datensatzes, etwa durch Kennzeichnung der Verwaltungsebene Bund, Bundesland, Kreis oder Kommune, als dcat-ap.de URI. |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#ebene-des-verwaltungspolitischen-geobezug-als-uri) genauer beschrieben. | 
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-political-geocoding-level) |
> | Interoperabilitätslevel    | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
> | Änderungen durch DCAT-AP.de | Von DCAT-AP.de eingeführte Eigenschaft. | 
<br>

###  Datensatz: Geopolitische Abdeckung (DEPRECATED) {#datensatz-geopolitischen-abdeckung}
> | *URI*                      | [`dcatde:politicalGeocodingURI`](http://dcat-ap.de/def/dcatde/politicalGeocodingLevelURI) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | DEPRECATED: Diese Eigenschaft verknüpft einen Datensatz mit dem von ihm abgedeckten administrativen Gebiet der Bundesrepublik Deutschland, etwa ein konkretes Bundesland, eine Kommune oder ein Landkreis repräsentiert durch eine URI. |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#verwaltungspolitischer-geobezug-als-uri) genauer beschrieben. | 
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-political-geocoding-uri) |
> | Änderungen zur Vorversion | 3.0: [DEPRECATED](#glossar-deprecated) | 
> | Interoperabilitätslevel    | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
> | Änderungen durch DCAT-AP.de | Von DCAT-AP.de eingeführte Eigenschaft. | 
<br>

###  Datensatz: Kategorie {#datensatz-kategorie}
> | *URI*                      | [`dcat:theme`](http://www.w3.org/ns/dcat#theme) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`skos:Concept`](http://www.w3.org/2004/02/skos/core#Concept) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf die dem Datensatz zugewiesenen Kategorien.  |
> | Verwendungshinweis | Mit einem Datensatz können mehrere Kategorien assoziiert sein.<br>Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#angaben-zu-kategorien) genauer beschrieben. | 
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-data-theme) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.theme), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_theme)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Kontakt {#datensatz-kontakt}
> | *URI*                      | [`dcat:contactPoint`](http://www.w3.org/ns/dcat#contactPoint) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`vcard:Kind`](http://www.w3.org/TR/vcard-rdf/#Kind) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft umfasst Kontaktinformationen, welche für das Zusenden von Kommentaren zum jeweiligen Datensatz verwendet werden können. |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#ansprechstelle) genauer beschrieben. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.contactpoint), [DCAT](https://www.w3.org/TR/vocab-dcat-2/#Property:resource_contact_point)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Verfügbarkeit {#datensatz-verfugbarkeit}
> | *URI*                      | [`dcatap:availability`](http://data.europa.eu/r5r/availability) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`skos:Concept`](http://www.w3.org/2000/01/rdf-schema#Resource) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Geplante Verfügbarkeit des Datensatzes als Auswahl aus einer festen Liste von Werten via DCAT-AP URIs. |
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-availability) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.availability)  | 
> | Interoperabilitätslevel    | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
> | Änderungen durch DCAT-AP.de | DCAT-AP.de ordnet diese Eigenschaft allen DCAT-Ressourcen und Distributionen zu. | 
<br>

###  Datensatz: Räumliche Abdeckung {#datensatz-raumliche-abdeckung}
> | *URI*                      | [`dcterms:spatial`](http://purl.org/dc/terms/spatial) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:Location`](http://purl.org/dc/terms/Location) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Ein räumlicher Bereich oder ein bezeichneter Ort. Er kann durch ein kontrolliertes Vokabular oder mit geographischen Koordinaten repräsentiert werden. |
> | Verwendungshinweis | Im letzteren Fall wird die Verwendung des Core Location Vocabulary empfohlen, wie in der GeoDCAT-AP-Spezifikation beschrieben.<br>Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#angaben-zur-geografischen-abdeckung) genauer beschrieben. | 
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-spatial) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.geographicalcoverage), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:dataset_spatial)  | 
> | Interoperabilitätslevel    | <abbr title='Eigenes ergänzt.'>E</abbr> |
> | Änderungen durch DCAT-AP.de | DCAT-AP.de bindet einen zusätzlichen Verwendungshinweis ein | 
<br>

###  Datensatz: Zeitliche Abdeckung {#datensatz-zeitliche-abdeckung}
> | *URI*                      | [`dcterms:temporal`](http://purl.org/dc/terms/temporal) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:PeriodOfTime`](http://purl.org/dc/terms/PeriodOfTime) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Ein Zeitintervall, welches durch Start- und Endzeitpunkt bezeichnet bzw. definiert ist. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.temporalcoverage), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:dataset_temporal)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Distribution {#datensatz-distribution}
> | *URI*                      | [`dcat:distribution`](http://www.w3.org/ns/dcat#distribution) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcat:Distribution`](http://www.w3.org/ns/dcat#Distribution) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft verknüpft den Datensatz mit einer verfügbaren Distribution. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.datasetdistribution), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:dataset_distribution)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Datenbereitsteller ID {#datensatz-datenbereitsteller-id}
> | *URI*                      | [`dcatde:contributorID`](http://dcat-ap.de/def/dcatde/contributorID) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft übermittelt die ID des Bereitstellers der Daten aus dem jeweils portaleigenem Access- und Identitymanagement (wenn vorhanden). |
> | Verwendungshinweis | Ihre genaue Verwendung ist nur für die Anlieferung an GovData festgelegt und wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#eindeutige-kennzeichnung-der-datenbereitsteller) genauer beschrieben. | 
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-contributors) |
> | Interoperabilitätslevel    | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
> | Änderungen durch DCAT-AP.de | Von DCAT-AP.de eingeführte Eigenschaft. | 
<br>

###  Datensatz: Beschreibung der Abdeckung (DEPRECATED) {#datensatz-beschreibung-abdeckung}
> | *URI*                      | [`dcatde:geocodingDescription`](http://dcat-ap.de/def/dcatde/geocodingDescription) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | DEPRECATED: Diese Eigenschaft enthält die geografische Abdeckung eines Datensatzes, repräsentiert durch die Bezeichnung eines administrativen Gebiets oder eines fachlichen Bezugs als Freitext. |
> | Verwendungshinweis | Ergänzend als Text bzw. alleinstehend für alle Fälle bei denen die geopolitische Abdeckung nicht durch eine URI angegeben werden kann (z.B. bei komplexeren Bund-Länder-Kooperationen oder auf kommunaler Ebene). <br>Beispiele: "Gemeinden des Wasserzweckverbands Straubing-Land" oder "Verband Region Rhein-Neckar".<br>Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#geobezug-als-beschreibender-text) genauer beschrieben. Sie kann für parallele Sprachversionen wiederholt werden. | 
> | Änderungen zur Vorversion | 3.0: [DEPRECATED](#glossar-deprecated) | 
> | Interoperabilitätslevel    | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
> | Änderungen durch DCAT-AP.de | Von DCAT-AP.de eingeführte Eigenschaft. | 
<br>

###  Datensatz: ID {#datensatz-id}
> | *URI*                      | [`dcterms:identifier`](http://purl.org/dc/terms/identifier) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft enthält die Haupt-ID des Datensatzes im Kontext des jeweiligen Kataloges (z.B. die URI-Adresse oder eine andere eindeutige ID). |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#identifier) genauer beschrieben. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.identifier), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_identifier)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Andere ID {#datensatz-andere-id}
> | *URI*                      | [`adms:identifier`](http://purl.org/dc/terms/identifier) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`adms:Identifier`](http://www.w3.org/ns/adms#Identifier) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf sekundäre IDs des Datensatzes. |
> | Verwendungshinweis | Beispiele dafür sind [DataCite](http://www.datacite.org/), [DOI (Digital Object Identifier)](http://www.doi.org/), [EZID](https://ezid.cdlib.org/), [W3ID: Permanent Identifiers for the Web](https://w3id.org/) oder andere fachspezifische Identifier.<br>Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#identifier) genauer beschrieben. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.otheridentifier), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#dereferenceable-identifiers)  | 
> | Änderungen zur Vorversion | 3.0: Errata: Link der Range korrigiert und Verwendungshinweis überarbeitet. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Veröffentlichungsdatum {#datensatz-veroffentlichungsdatum}
> | *URI*                      | [`dcterms:issued`](http://purl.org/dc/terms/issued) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) getyped als `xsd:gYear`, `xsd:gYearMonth`, `xsd:date` oder `xsd:dateTime` |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft enthält das Datum der Herausgabe/Emission (z.B. in Form einer Veröffentlichung) des Datensatzes. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.releasedate), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_release_date)  | 
> | Änderungen zur Vorversion | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Aktualisierungsdatum {#datensatz-aktualisierungsdatum}
> | *URI*                      | [`dcterms:modified`](http://purl.org/dc/terms/modified) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) getyped als `xsd:gYear`, `xsd:gYearMonth`, `xsd:date` oder `xsd:dateTime` |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft erfasst das Datum der letzten Aktualisierung bzw. Modifikation des Datensatzes. |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#erkennung-von-dubletten) genauer beschrieben. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.modificationdate), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_update_date)  | 
> | Änderungen zur Vorversion | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Versionsbezeichnung {#datensatz-versionsbezeichnung}
> | *URI*                      | [`dcat:version`](http://www.w3.org/ns/dcat#version) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft enthält eine Versionsnummer oder anderweitige Versionskennzeichnung des Datensatzes. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.version), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_version)  | 
> | Änderungen zur Vorversion | 3.0: Neu hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Eigenes ergänzt.'>E</abbr> |
> | Änderungen durch DCAT-AP.de | TBD: DCAT-AP.de gibt eine Kardinalität von `*` statt `0..1` an. | 
<br>

###  Datensatz: Versionsbezeichnung (DEPRECATED) {#datensatz-versionsbezeichnung-deprecated}
> | *URI*                      | [`owl:versionInfo`](http://www.w3.org/2002/07/owl#versionInfo) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft enthält eine Versionsnummer oder anderweitige Versionskennzeichnung des Datensatzes. |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#angaben-zur-versionierung) genauer beschrieben. | 
> | Weiterführende Dokumentationen | [OWL](https://www.w3.org/TR/owl-ref/#versionInfo-def)  | 
> | Änderungen zur Vorversion | 3.0: [DEPRECATED](#glossar-deprecated) | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Versionserläuterung {#datensatz-versionserlauterung}
> | *URI*                      | [`adms:versionNotes`](http://www.w3.org/ns/adms#versionNotes) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft enthält eine Beschreibung der Unterschiede zwischen dieser und den vorbestehenden Versionen des Datensatzes. |
> | Verwendungshinweis | Dieses Eigenschaft kann für parallele Sprachversionen der Versionsbeschreibung wiederholt werden.<br>Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#angaben-zur-versionierung) genauer beschrieben. | 
> | Weiterführende Dokumentationen | [ADMS](https://www.w3.org/TR/vocab-adms/#adms-versionnotes)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Rechtsgrundlage {#datensatz-rechtsgrundlage}
> | *URI*                      | [`dcatap:applicableLegislation`](http://data.europa.eu/r5r/applicableLegislation) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`eli:LegalResource`](http://data.europa.eu/eli/ontology#LegalResource) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Die Rechtsvorschriften, die die Erstellung oder Verwaltung des Datensatzes vorschreiben. |
> | Verwendungshinweis | Handelt es sich um ein High Value Dataset, muss `http://data.europa.eu/eli/reg_impl/2023/138/oj` angegeben werden.<br>Ansonsten wird die Verwendung eine ELI-Identifiers empfohlen. Ist dieser nicht bekannt, soll ein möglichst stabiler Link zum Gesetz verwendet werden. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.applicablelegislation)  | 
> | Änderungen zur Vorversion | 3.0: Neu hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Eigenes ergänzt.'>E</abbr> |
> | Änderungen durch DCAT-AP.de | Verwendungshinweis ergänzt. | 
<br>

###  Datensatz: Rechtsgrundlage für die Zugangseröffnung (DEPRECATED) {#datensatz-rechtsgrundlage-zugangseroffnung}
> | *URI*                      | [`dcatde:legalBasis`](http://dcat-ap.de/def/dcatde/legalBasis) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Dieses Feld dokumentiert als Freitext optional die Rechtsgrundlage für den Zugang zu den Informationen (die Zugangseröffnung), d.h. die originäre Rechtsgrundlage für den Zugang zu Daten der Verwaltung. |
> | Verwendungshinweis | Diese Eigenschaft kann für parallele Sprachversionen wiederholt werden.<br>Beispiele: Public Sector Information Directive (PSI-Direktive), Umweltinformationsgesetz (UIG), deutsche Informationsfreiheits- (IFG) und Transparenzgesetze. | 
> | Änderungen zur Vorversion | 3.0: [DEPRECATED](#glossar-deprecated) | 
> | Interoperabilitätslevel    | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
> | Änderungen durch DCAT-AP.de | Von DCAT-AP.de eingeführte Eigenschaft. | 
<br>

###  Datensatz: Verwandte Ressource {#datensatz-verwandte-ressource}
> | *URI*                      | [`dcterms:relation`](http://purl.org/dc/terms/relation) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf eine verwandte Ressource. |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#andere-beziehungen-zwischen-datensatzen-dct-relation) genauer beschrieben. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.relatedresource), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_relation)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Ursprüngliche Webseite {#datensatz-ursprungliche-webseite}
> | *URI*                      | [`dcat:landingPage`](http://www.w3.org/ns/dcat#landingPage) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`foaf:Document`](http://xmlns.com/foaf/0.1/Document) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf eine Webseite, welche Zugriff auf den Datensatz, seine Distributionen und/oder weitere Informationen ermöglicht.  |
> | Verwendungshinweis | Es ist beabsichtigt, auf die Webseite des originären Datenbereitstellers zu verweisen und nicht auf zwischengeschaltete Intermediäre. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.landingpage), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_landing_page)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Dokumentation {#datensatz-dokumentation}
> | *URI*                      | [`foaf:page`](http://xmlns.com/foaf/0.1/page) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`foaf:Document`](http://xmlns.com/foaf/0.1/Document) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf eine Seite oder ein Dokument für den jeweiligen Datensatz. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.documentation), [FOAF](http://xmlns.com/foaf/spec/#term_page)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Sprache {#datensatz-sprache}
> | *URI*                      | [`dcterms:language`](http://purl.org/dc/terms/language) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:LinguisticSystem`](http://purl.org/dc/terms/LinguisticSystem) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf die innerhalb des Datensatzes verwendete Sprache. |
> | Verwendungshinweis | Diese Eigenschaft kann wiederholt werden, falls mehrere Sprachen im Datensatz Verwendung finden. | 
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-languages) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.language), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_language)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Konform zu Standard {#datensatz-konform-zu-standard}
> | *URI*                      | [`dcterms:conformsTo`](http://purl.org/dc/terms/conformsTo) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:Standard`](http://purl.org/dc/terms/Standard) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf eine Implementierungsregel oder eine andere Spezifikation, zu welcher der Datensatz konform ist. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.conformsto), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_conforms_to)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Grad der Zugänglichkeit {#datensatz-grad-zuganglichkeit}
> | *URI*                      | [`dcterms:accessRights`](http://purl.org/dc/terms/accessRights) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:RightsStatement`](http://purl.org/dc/terms/RightsStatement) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf Informationen, die darlegen, ob der Datensatz öffentlich zugänglich ist, Zugriffseinschränkungen existieren oder er nicht-öffentlich ist. |
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-access-right) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.accessrights), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_access_rights)  | 
> | Änderungen zur Vorversion | 3.0: Kontrolliertes Vokabular hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Provenienz {#datensatz-provenienz}
> | *URI*                      | [`dcterms:provenance`](http://purl.org/dc/terms/provenance) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:ProvenanceStatement`](http://purl.org/dc/terms/ProvenanceStatement) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft umfasst eine Angabe zur Entwicklungsgeschichte des Datensatzes.  |
> | Verwendungshinweis | Insbesondere ist relevant, in wessen Besitz oder Obhut die Ressource sich bislang befunden hat, soweit die Wechsel signifikanten Einfluss auf die Authentizität, Integrität und Interpretierbarkeit dieser Ressource hat. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.provenance), [DCMI Metadata Terms](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/#http://purl.org/dc/terms/provenance)  | 
> | Interoperabilitätslevel    | <abbr title='Eigenes ergänzt.'>E</abbr> |
> | Änderungen durch DCAT-AP.de | Ergänzung eines Verwendungshinweises. | 
<br>

###  Datensatz: Aktualisierungsfrequenz {#datensatz-aktualisierungsfrequenz}
> | *URI*                      | [`dcterms:accrualPeriodicity`](http://purl.org/dc/terms/accrualPeriodicity) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:Frequency`](http://purl.org/dc/terms/Frequency) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft beschreibt die Aktualisierungsfrequenz des Datensatzes. |
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-frequency) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.frequency), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:dataset_frequency)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Qualitätssicherungsprozess (DEPRECATED) {#datensatz-qualitatssicherungsprozess}
> | *URI*                      | [`dcatde:qualityProcessURI`](http://dcat-ap.de/def/dcatde/qualityProcessURI) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | DEPRECATED: Eine URI, die auf den Prozess zur Qualitätssicherung des Datensatzes verweist. Es handelt sich idealerweise um die URL einer Webseite. |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#webseite-mit-beschreibung-des-qualitatssicherungsprozesses) genauer beschrieben. | 
> | Änderungen zur Vorversion | 3.0: [DEPRECATED](#glossar-deprecated) | 
> | Interoperabilitätslevel    | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
> | Änderungen durch DCAT-AP.de | Von DCAT-AP.de eingeführte Eigenschaft. | 
<br>

###  Datensatz: Typ {#datensatz-typ}
> | *URI*                      | [`dcterms:type`](http://purl.org/dc/terms/type) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`skos:Concept`](http://www.w3.org/2004/02/skos/core#Concept) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf den Typ des Datensatzes. |
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-dataset-type) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.type), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_type)  | 
> | Änderungen zur Vorversion | 3.0: Kardinalität von `0..1` auf `*` geändert.<br>3.0: Namen vereinfacht.<br>3.0: Optionale Codeliste hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Wurde erzeugt von {#datensatz-wurde-erzeugt-von}
> | *URI*                      | [`prov:wasGeneratedBy`](https://www.w3.org/TR/prov-o/#wasGeneratedBy) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`prov:Activity`](https://www.w3.org/TR/prov-o/#Activity) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf die Aktivität, die zur Erstellung des Datensatzes geführt hat. |
> | Verwendungshinweis | Eine Aktivität ist typischer Weise eine Initiative, ein Projekt, eine Umfrage oder dauerhafte Handlung ("business as usual"). | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.wasgeneratedby), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:dataset_was_generated_by)  | 
> | Interoperabilitätslevel    | <abbr title='Eigenes ergänzt.'>E</abbr> |
> | Änderungen durch DCAT-AP.de | Ergänzung eines Verwendungshinweises. | 
<br>

###  Datensatz: Räumliche Auflösung in Meter {#datensatz-raumliche-auflosung-in-meter}
> | *URI*                      | [`dcat:spatialResolutionInMeters`](http://www.w3.org/ns/dcat#spatialResolutionInMeters) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) getyped als [`xsd:decimal`](https://www.w3.org/TR/xmlschema11-2/#decimal) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf den kleinstmöglichen räumlichen Abstand, der in einem Datensatz auflösbar ist, gemessen in Metern. |
> | Verwendungshinweis | Kann die räumliche Auflösung nicht in Metern beschrieben werden, können stattdessen die spezielleren Eigenschaften verwendet werden, die [GeoDCAT-AP](https://semiceu.github.io/GeoDCAT-AP/releases/2.0.0/#spatial-resolution-spatial-resolution-of-the-dataset) hierfür zur Verfügung stellt. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.spatialresolution), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:dataset_spatial_resolution)  | 
> | Änderungen zur Vorversion | 3.0: Errata: Kardinalität von `[*]` wie bei DCAT-AP auf `[0..1]` angepasst. | 
> | Interoperabilitätslevel    | <abbr title='Eigenes ergänzt.'>E</abbr> |
> | Änderungen durch DCAT-AP.de | Verwendungshinweis hinzugefügt. | 
<br>

###  Datensatz: Zeitliche Auflösung {#datensatz-zeitliche-auflosung}
> | *URI*                      | [`dcat:temporalResolution`](http://www.w3.org/ns/dcat#temporalResolution) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) getyped als [`xsd:duration`](https://www.w3.org/TR/xmlschema11-2/#duration) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf den kürzesten im Datensatz auflösbaren Zeitraum. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.temporalresolution), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:dataset_temporal_resolution)  | 
> | Änderungen zur Vorversion | 3.0: Errata: Kardinalität von `[*]` wie bei DCAT-AP auf `[0..1]` angepasst.<br>3.0: Errata: Anzeige des Wertebereichs korrigiert und weiterführende Dokumentation zu DCAT korrigiert. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Rollenzuordnung {#datensatz-rollenzuordnung}
> | *URI*                      | [`prov:qualifiedAttribution`](https://www.w3.org/TR/prov-o/#qualifiedAttribution) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`prov:Attribution`](https://www.w3.org/TR/prov-o/#Attribution) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Verbindet den Datensatz über die Klasse `prov:Attribution` mit einem Agenten, der in beschriebener Weise Verantwortung für ihn trägt. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.qualifiedattribution), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_qualified_attribution)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Qualifizierte Beziehung {#datensatz-qualifizierte-beziehung}
> | *URI*                      | [`dcat:qualifiedRelation`](http://www.w3.org/ns/dcat#qualifiedRelation) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcat:Relationship`](https://www.w3.org/TR/vocab-dcat-3/#Class:Relationship) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Link zu einer Beschreibung (in Form der Klasse `dcat:Relationship`) einer Beziehung zu einer anderen Ressource. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.qualifiedrelation), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_qualified_relation)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Wird Referenziert {#datensatz-wird-referenziert}
> | *URI*                      | [`dcterms:isReferencedBy`](http://purl.org/dc/terms/isReferencedBy) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf eine Ressource, zum Beispiel eine Veröffentlichung, die ihrerseits auf den Datensatz referenziert, ihn verlinkt oder zitiert. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.isreferencedby), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_is_referenced_by)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Referenziert {#datensatz-referenziert}
> | *URI*                      | [`dcterms:references`](http://purl.org/dc/terms/references) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft kann verwendet werden, um auf Referenzdatensätze wie ein High Value Dataset (HVD) oder einen Musterdatensatz des Musterdatenkatalogs zu verweisen. |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#verweis-auf-referenzobjekte) genauer beschrieben. | 
> | Interoperabilitätslevel    | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
> | Änderungen durch DCAT-AP.de | Von DCAT-AP.de eingeführte Eigenschaft. | 
<br>

###  Datensatz: Quelle des Datensatzes {#datensatz-quelle}
> | *URI*                      | [`dcterms:source`](http://purl.org/dc/terms/source) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcat:Dataset`](http://www.w3.org/ns/dcat#Dataset) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf einen verwandten Datensatz, von dem der beschriebene Datensatz abgeleitet ist. |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#quelle-von-metadaten) genauer beschrieben. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.source), [DCMI Metadata Terms](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/#http://purl.org/dc/terms/source)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Weitere Version {#datensatz-weitere-version}
> | *URI*                      | [`dcat:hasVersion`](http://www.w3.org/ns/dcat#hasVersion) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcat:Dataset`](http://www.w3.org/ns/dcat#Dataset) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf einen verwandten Datensatz in Form einer weiteren/nachfolgenden Version, Edition oder Adaption des beschriebenen Datensatzes. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.hasversion), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_has_version)  | 
> | Änderungen zur Vorversion | 3.0: Neu hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Weitere Version (DEPRECATED) {#datensatz-weitere-version-deprecated}
> | *URI*                      | [`dcterms:hasVersion`](http://purl.org/dc/terms/hasVersion) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcat:Dataset`](http://www.w3.org/ns/dcat#Dataset) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf einen verwandten Datensatz in Form einer weiteren/nachfolgenden Version, Edition oder Adaption des beschriebenen Datensatzes. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#deprecated-properties-and-classes), [DCMI Metadata Terms](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/#http://purl.org/dc/terms/hasVersion)  | 
> | Änderungen zur Vorversion | 3.0: [DEPRECATED](#glossar-deprecated) | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Ist Version von (DEPRECATED) {#datensatz-ist-version}
> | *URI*                      | [`dcterms:isVersionOf`](http://purl.org/dc/terms/isVersion) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcat:Dataset`](http://www.w3.org/ns/dcat#Dataset) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf einen verwandten Datensatz, der vom beschriebenen Datensatz eine vorherige Version, Edition oder Adaption ist. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#deprecated-properties-and-classes), [DCMI Metadata Terms](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/#http://purl.org/dc/terms/isVersion)  | 
> | Änderungen zur Vorversion | 3.0: [DEPRECATED](#glossar-deprecated) | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Beispieldistribution {#datensatz-beispieldistribution}
> | *URI*                      | [`adms:sample`](http://www.w3.org/ns/adms#sample) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcat:Distribution`](http://www.w3.org/ns/dcat#Distribution) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf eine Beispieldistribution des Datensatzes. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.sample), [ADMS](https://www.w3.org/TR/vocab-adms/#adms-sample)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Autor {#datensatz-autor}
> | *URI*                      | [`dcterms:creator`](http://purl.org/dc/terms/creator) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`foaf:Agent`](http://xmlns.com/foaf/0.1/Agent) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf Stellen oder Personen, die die Daten erstellt haben. Die Autorenschaft umfasst für gewöhnlich das Recht am geistigen Eigentum |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#weitere-wichtige-rollen) genauer beschrieben. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.creator), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_creator)  | 
> | Änderungen zur Vorversion | 3.0: Errata: War fälschlicherweise als Ergänzung durch DCAT-AP.de angegeben. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatz: Bearbeiter {#datensatz-bearbeiter}
> | *URI*                      | [`dcterms:contributor`](http://purl.org/dc/terms/contributor) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`foaf:Agent`](http://xmlns.com/foaf/0.1/Agent) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf Stellen oder Personen, die die Daten bearbeitet haben (z.B. durch Formatierung derselben). |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#weitere-wichtige-rollen) genauer beschrieben. | 
> | Weiterführende Dokumentationen | [DCMI Metadata Terms](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/#http://purl.org/dc/terms/contributor)  | 
> | Interoperabilitätslevel    | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
> | Änderungen durch DCAT-AP.de | Von DCAT-AP.de eingeführte Eigenschaft. | 
<br>

###  Datensatz: Urheber (DEPRECATED) {#datensatz-urheber}
> | *URI*                      | [`dcatde:originator`](http://dcat-ap.de/def/dcatde/originator) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`foaf:Agent`](http://xmlns.com/foaf/0.1/Agent) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | DEPRECATED: Diese Eigenschaft verweist auf die Personen, die Urheberrechte am Datensatz haben. Geschützt ist laut Urheberrecht ein Werk, das einer persönlichen geistigen Schöpfung seines Urhebers entspringt.<br>Vgl.: https://de.wikipedia.org/wiki/Urheberrecht_(Deutschland). |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#weitere-wichtige-rollen) genauer beschrieben. | 
> | Änderungen zur Vorversion | 3.0: [DEPRECATED](#glossar-deprecated). Wird ersetzt durch [`geodcat:originator`](#datensatz-geodcat-urheber). | 
> | Interoperabilitätslevel    | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
> | Änderungen durch DCAT-AP.de | Von DCAT-AP.de eingeführte Eigenschaft. | 
<br>

###  Datensatz: Verwalter (DEPRECATED) {#datensatz-verwalter}
> | *URI*                      | [`dcatde:maintainer`](http://dcat-ap.de/def/dcatde/maintainer) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`foaf:Agent`](http://xmlns.com/foaf/0.1/Agent) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | DEPRECATED: Diese Eigenschaft verweist auf die Stellen oder Personen, die Verantwortung und Rechenschaftspflicht für die Daten und ihre angemessene Pflege übernehmen. |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#weitere-wichtige-rollen) genauer beschrieben. | 
> | Änderungen zur Vorversion | 3.0: [DEPRECATED](#glossar-deprecated). Wird ersetzt durch [`geodcat:custodian`](#datensatz-geodcat-verwalter). | 
> | Interoperabilitätslevel    | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
> | Änderungen durch DCAT-AP.de | Von DCAT-AP.de eingeführte Eigenschaft. | 
<br>

###  Datensatz: In Serie {#datensatz-in-serie}
> | *URI*                      | [`dcat:inSeries`](http://www.w3.org/ns/dcat#inSeries) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcat:DatasetSeries`](http://www.w3.org/ns/dcat#DatasetSeries) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf die Datensatzserie zu der der Datensatz gehört. |
> | Verwendungshinweis | Pflichteigenschaft, wenn es sich um einen Datensatz handelt, der zu einer Datensatzserie gehören soll. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Dataset.inseries), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:dataset_in_series)  | 
> | Änderungen zur Vorversion | 3.0: Im Zuge der Einführung von `dcat:DatasetSeries` hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>



***


## Klasse: Datenservice

> | *URI der Klasse* | [`dcat:DataService`](http://www.w3.org/ns/dcat#DataService)      |
> |:-----------------|:-----------------------------------------------------|
> | Beschreibung     | Ein Datenservice ermöglicht den Zugang zu einem oder mehreren Datensätzen oder stellt Datenverarbeitungsverfahren zur Verfügung.     |
> | eingebunden über | dcat:service (dcat:Catalog), dcat:accessService (dcat:Distribution), foaf:primaryTopic (dcat:CatalogRecord)         | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#DataService), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Class:Data_Service) |

<br>

Die folgenden Eigenschaften wurden von DCAT-AP.de hinzugefügt oder verändert: 
[`dcatap:availability`](#datenservice-verfugbarkeit), [`dcterms:publisher`](#datenservice-herausgeber).<br>


|                                 | Eigenschaft  | Wertebereich      | <small>Verbind&shy;lichkeit</small> | Mult. | Interop. |
|:--------------------------------|:-------------|:------------------|:------------------------------------|:-----:|:--------:|
| [URL des Endpunktes](#datenservice-url-endpunkt) | `dcat:endpointURL` | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) | <small>Pflicht</small> | `[1..*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Titel](#datenservice-titel) | `dcterms:title` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Pflicht</small> | `[1..*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Herausgeber](#datenservice-herausgeber) | `dcterms:publisher` | [`foaf:Agent`](http://xmlns.com/foaf/0.1/Agent) | <small>Pflicht</small> | `[1]` | <abbr title='Eigenes ergänzt.'>E</abbr> |
| [Beschreibung des Endpunktes](#datenservice-beschreibung-endpunkt) | `dcat:endpointDescription` | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) | <small>Empfohlen</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Verfügbarkeit](#datenservice-verfugbarkeit) | `dcatap:availability` | [`skos:Concept`](http://www.w3.org/2000/01/rdf-schema#Resource) | <small>Empfohlen</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Liefert Datensatz aus](#datenservice-liefert-datensatz-aus) | `dcat:servesDataset` | [`dcat:Dataset`](http://www.w3.org/ns/dcat#Dataset) | <small>Empfohlen</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Beschreibung](#datenservice-beschreibung) | `dcterms:description` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Lizenz](#datenservice-lizenz) | `dcterms:license` | [`dcterms:LicenseDocument`](http://purl.org/dc/terms/LicenseDocument) | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Grad der Zugänglichkeit](#datenservice-grad-zuganglichkeit) | `dcterms:accessRights` | [`dcterms:RightsStatement`](http://purl.org/dc/terms/RightsStatement) | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Format](#datenservice-format) | `dcterms:format` | [`dcterms:MediaTypeOrExtent`](http://purl.org/dc/terms/MediaTypeOrExtent) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |


<br> Die folgenden weiteren Eigenschaften wurden von der Superklasse [`dcat:Resource`](#klasse-ressource) geerbt, werden aber nicht genauer betrachtet: [`dcterms:modified`](#datensatz-aktualisierungsdatum), [`dcterms:creator`](#datensatz-autor), [`dcterms:publisher`](#datensatz-herausgeber), [`dcterms:identifier`](#datensatz-id), [`dcat:theme`](#datensatz-kategorie), [`dcterms:conformsTo`](#datensatz-konform-zu-standard), [`dcat:contactPoint`](#datensatz-kontakt), [`dcat:qualifiedRelation`](#datensatz-qualifizierte-beziehung), [`prov:qualifiedAttribution`](#datensatz-rollenzuordnung), [`dcat:keyword`](#datensatz-schlagwort), [`dcterms:language`](#datensatz-sprache), [`dcterms:type`](#datensatz-typ), [`dcat:landingPage`](#datensatz-ursprungliche-webseite), [`dcterms:issued`](#datensatz-veroffentlichungsdatum), [`dcterms:relation`](#datensatz-verwandte-ressource), [`dcterms:rights`](#distribution-grad-zuganglichkeit), [`odrl:hasPolicy`](#distribution-regelwerk) und [`dcterms:isReferencedBy`](#datensatz-wird-referenziert). Zusätzliche, durch die deutschen Erweiterung von [`dcat:Resource`](#klasse-ressource), geerbte Eigenschaften: [`dcatde:contributorID`](#datensatz-datenbereitsteller-id), [`dcatde:qualityProcessURI`](#datensatz-qualitatssicherungsprozess), [`dcatde:originator`](#datensatz-urheber), [`dcatde:maintainer`](#datensatz-verwalter), [`dcatde:politicalGeocodingLevelURI`](#datensatz-ebene-geopolitischen-abdeckung), [`dcatde:politicalGeocodingURI`](#datensatz-geopolitischen-abdeckung), [`dcatde:geocodingDescription`](#datensatz-beschreibung-abdeckung), [`dcatde:legalBasis`](#datensatz-rechtsgrundlage-zugangseroffnung), [`dcterms:contributor`](#datensatz-bearbeiter) und [`dcterms:references`](#datensatz-referenziert).


<br>
<hr>
<br>

###  Datenservice: URL des Endpunktes {#datenservice-url-endpunkt}
> | *URI*                      | [`dcat:endpointURL`](http://www.w3.org/ns/dcat#endpointURL) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1..*]`                   |
> | Beschreibung               | Die URL unter der API-Endpunkt eines Datenservices erreichbar ist. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#DataService.endpointURL), [DCAT](https://www.w3.org/TR/vocab-dcat-2/#Property:data_service_endpoint_url)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datenservice: Titel {#datenservice-titel}
> | *URI*                      | [`dcterms:title`](http://purl.org/dc/terms/title) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1..*]`                   |
> | Beschreibung               | Diese Eigenschaft bezeichnet den einem Datenservice zugewiesenen Titel.  |
> | Verwendungshinweis | Sie kann für parallele Sprachversionen wiederholt werden. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#DataService.title), [DCAT](https://www.w3.org/TR/vocab-dcat-2/#Property:resource_title)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datenservice: Herausgeber {#datenservice-herausgeber}
> | *URI*                      | [`dcterms:publisher`](http://purl.org/dc/terms/publisher) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`foaf:Agent`](http://xmlns.com/foaf/0.1/Agent) |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf die Stelle oder Person, die für Bereitstellung des Datenservices verantwortlich ist. |
> | Verwendungshinweis | Es ist zugleich die Stelle oder Person, die über die Einräumung von Zugang und Nutzungsrechten für Dritte entschieden hat. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#DataService.publisher), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_publisher)  | 
> | Änderungen zur Vorversion | 3.0: Eigenschaft aufgenommen.<br>3.0: Anforderung: Nutzung verpflichtend gemacht. | 
> | Interoperabilitätslevel    | <abbr title='Eigenes ergänzt.'>E</abbr> |
> | Änderungen durch DCAT-AP.de | Erweiterung des Verwendungshinweises. Nutzung verpflichtend gemacht. | 
<br>

###  Datenservice: Beschreibung des Endpunktes {#datenservice-beschreibung-endpunkt}
> | *URI*                      | [`dcat:endpointDescription`](http://www.w3.org/ns/dcat#endpointDescription) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Die Beschreibung der Services, die unter den angebenen Endpunkten erreicht werden können. |
> | Verwendungshinweis | Diese Eigenschaft gibt spezifische Details zu den Endpunkten an, während die Eigenschaft "Katalogeintrag: Application Profile der Metadaten (dct:conformsTo)" verwendet wird, um den allgemeinen Standard oder die Spezifikation anzugeben, den die Endpunkte anwenden. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#DataService.endpointdescription), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:data_service_endpoint_description)  | 
> | Änderungen zur Vorversion | 3.0: In Anlehnung an DCAT-AP 3.0 wurde ein neuer Verwendungshinweis aufgenommen. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datenservice: Verfügbarkeit {#datenservice-verfugbarkeit}
> | *URI*                      | [`dcatap:availability`](http://data.europa.eu/r5r/availability) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`skos:Concept`](http://www.w3.org/2000/01/rdf-schema#Resource) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Geplante Verfügbarkeit des Datenservices als Auswahl aus einer festen Liste von Werten via DCAT-AP URIs. |
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-availability) |
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |
> | Änderungen durch DCAT-AP.de | DCAT-AP.de ordnet diese Eigenschaft allen DCAT-Ressourcen und Distributionen zu. | 
<br>

###  Datenservice: Liefert Datensatz aus {#datenservice-liefert-datensatz-aus}
> | *URI*                      | [`dcat:servesDataset`](http://www.w3.org/ns/dcat#servesdataset) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcat:Dataset`](http://www.w3.org/ns/dcat#Dataset) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Verweist auf einen Datensatz, der vom Datenservice ausgeliefert werden kann. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#DataService.servesdataset), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:data_service_serves_dataset)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datenservice: Beschreibung {#datenservice-beschreibung}
> | *URI*                      | [`dcterms:description`](http://purl.org/dc/terms/description) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft enthält eine Beschreibung des Datenservices als Freitext.  |
> | Verwendungshinweis | Sie kann für parallel existierende Sprachversionen wiederholt werden. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#DataService.description), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_description)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datenservice: Lizenz {#datenservice-lizenz}
> | *URI*                      | [`dcterms:license`](http://purl.org/dc/terms/license) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:LicenseDocument`](http://purl.org/dc/terms/LicenseDocument) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf die Lizenz, mit welcher der Datenservice verwendet oder seine Inhalte wiederverwendet werden können. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#DataService.licence), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_license)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datenservice: Grad der Zugänglichkeit {#datenservice-grad-zuganglichkeit}
> | *URI*                      | [`dcterms:accessRights`](http://purl.org/dc/terms/accessRights) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:RightsStatement`](http://purl.org/dc/terms/RightsStatement) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf Informationen, die darlegen, ob der Datenservice öffentlich zugänglich ist, Zugriffseinschränkungen existieren oder er nicht-öffentlich ist. |
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-access-right) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#DataService.accessrights), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_access_rights)  | 
> | Änderungen zur Vorversion | 3.0: Kontrolliertes Vokabular hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datenservice: Format {#datenservice-format}
> | *URI*                      | [`dcterms:format`](http://purl.org/dc/terms/format) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:MediaTypeOrExtent`](http://purl.org/dc/terms/MediaTypeOrExtent) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Die Datenformate, die beim Abruf der `dcat:endpointURL` zurückgegeben werden können. |
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-file-type) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#DataService.format), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:distribution_format)  | 
> | Änderungen zur Vorversion | 3.0: Eigenschaft aufgenommen. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>



***


## Klasse: Datensatzserie

> | *URI der Klasse* | [`dcat:DatasetSeries`](http://www.w3.org/ns/dcat#DatasetSeries)      |
> |:-----------------|:-----------------------------------------------------|
> | Beschreibung     | Eine Sammlung von Datasätzen, die zwar separat veröffentlicht werden aber, eine gemeinsame Merkmale aufweisen, die sie zusammenfassen.     |
> | eingebunden über | dcat:inSeries (dcat:Dataset)         | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#DatasetSeries), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Class:Dataset_Series) |
> | Änderungen zur Vorversion | 3.0: Neu hinzugefügt. |

<br>

Die folgenden Eigenschaften wurden von DCAT-AP.de hinzugefügt oder verändert: 
[`dcterms:publisher`](#datensatzserie-herausgeber).<br>


|                                 | Eigenschaft  | Wertebereich      | <small>Verbind&shy;lichkeit</small> | Mult. | Interop. |
|:--------------------------------|:-------------|:------------------|:------------------------------------|:-----:|:--------:|
| [Titel](#datensatzserie-titel) | `dcterms:title` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Pflicht</small> | `[1..*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Herausgeber](#datensatzserie-herausgeber) | `dcterms:publisher` | [`foaf:Agent`](http://xmlns.com/foaf/0.1/Agent) | <small>Pflicht</small> | `[1]` | <abbr title='Eigenes ergänzt.'>E</abbr> |
| [Kontakt](#datensatzserie-kontakt) | `dcat:contactPoint` | [`vcard:Kind`](http://www.w3.org/TR/vcard-rdf/#Kind) | <small>Empfohlen</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Räumliche Abdeckung](#datensatzserie-raumliche-abdeckung) | `dcterms:spatial` | [`dcterms:Location`](http://purl.org/dc/terms/Location) | <small>Empfohlen</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Zeitliche Abdeckung](#datensatzserie-zeitliche-abdeckung) | `dcterms:temporal` | [`dcterms:PeriodOfTime`](http://purl.org/dc/terms/PeriodOfTime) | <small>Empfohlen</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Beschreibung](#datensatzserie-beschreibung) | `dcterms:description` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Rechtsgrundlage](#datensatzserie-rechtsgrundlage) | `dcatap:applicableLegislation` | [`eli:LegalResource`](http://data.europa.eu/eli/ontology#LegalResource) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Aktualisierungsfrequenz](#datensatzserie-aktualisierungsfrequenz) | `dcterms:accrualPeriodicity` | [`dcterms:Frequency`](http://purl.org/dc/terms/Frequency) | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Veröffentlichungsdatum](#datensatzserie-veroffentlichungsdatum) | `dcterms:issued` | [`rdfs:Literal`]() | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Aktualisierungsdatum](#datensatzserie-aktualisierungsdatum) | `dcterms:modified` | [`rdfs:Literal`]() | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |


<br>
<hr>
<br>

###  Datensatzserie: Titel {#datensatzserie-titel}
> | *URI*                      | [`dcterms:title`](http://purl.org/dc/terms/title) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1..*]`                   |
> | Beschreibung               | Diese Eigenschaft bezeichnet den einer Datensatzserie zugewiesenen Titel. |
> | Verwendungshinweis | Diese Eigenschaft kann für parallele Sprachversionen des Datensatztitels wiederholt werden. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#DatasetSeries.title), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Class:Dataset_Series)  | 
> | Änderungen zur Vorversion | 3.0: Neu hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatzserie: Herausgeber {#datensatzserie-herausgeber}
> | *URI*                      | [`dcterms:publisher`](http://purl.org/dc/terms/publisher) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`foaf:Agent`](http://xmlns.com/foaf/0.1/Agent) |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf die Stelle oder Person, die für Bereitstellung der Datensatzserie verantwortlich ist. |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#angaben-zum-herausgeber) genauer beschrieben.<br>Der Herausgeber der Datensatzserie ist möglicherweise nicht der Herausgeber aller Datensätze.  So könnte z. B. ein digitales Archiv die Veröffentlichung älterer Datensätze der Reihe übernehmen.   | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#DatasetSeries.publisher), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_publisher)  | 
> | Änderungen zur Vorversion | 3.0: Neu hinzugefügt.<br>3.0: Anforderung: Nutzung verpflichtend gemacht. | 
> | Interoperabilitätslevel    | <abbr title='Eigenes ergänzt.'>E</abbr> |
> | Änderungen durch DCAT-AP.de | Nutzung verpflichtend gemacht. | 
<br>

###  Datensatzserie: Kontakt {#datensatzserie-kontakt}
> | *URI*                      | [`dcat:contactPoint`](http://www.w3.org/ns/dcat#contactPoint) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`vcard:Kind`](http://www.w3.org/TR/vcard-rdf/#Kind) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft umfasst Kontaktinformationen, welche für das Zusenden von Kommentaren zur jeweiligen Datensatzserie verwendet werden können. |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#ansprechstelle) genauer beschrieben. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#DatasetSeries.contactpoint), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_contact_point)  | 
> | Änderungen zur Vorversion | 3.0: Neu hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatzserie: Räumliche Abdeckung {#datensatzserie-raumliche-abdeckung}
> | *URI*                      | [`dcterms:spatial`](http://purl.org/dc/terms/spatial) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:Location`](http://purl.org/dc/terms/Location) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Ein räumlicher Bereich der durch die Datensatzserie abgedeckt wird. |
> | Verwendungshinweis | Wenn die räumliche Abdeckung eine Dimension der Datensatzserie ist, sollte die räumliche Abdeckung jedes Datensatzes in der Serie Teil der räumlichen Abdeckung sein.<br>In diesem Fall wird ein unspezifischer Wert empfohlen, z. B. die EU oder eine große Bounding Box, die die erwarteten Werte abdeckt.  | 
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-spatial) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#DatasetSeries.geographicalcoverage), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:dataset_spatial)  | 
> | Änderungen zur Vorversion | 3.0: Neu hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatzserie: Zeitliche Abdeckung {#datensatzserie-zeitliche-abdeckung}
> | *URI*                      | [`dcterms:temporal`](http://purl.org/dc/terms/temporal) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:PeriodOfTime`](http://purl.org/dc/terms/PeriodOfTime) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Ein Zeitintervall, welches durch Start- und Endzeitpunkt bezeichnet bzw. definiert ist. |
> | Verwendungshinweis | Wenn die zeitliche Abdeckung eine Dimension in der Datensatzserie ist, sollte die zeitliche Abdeckung jedes enthaltenen Datensatzes Teil der zeitlichen Abdeckung sein der Serie. In diesem Fall wird ein offener Wert empfohlen, z. B. nach 2012.  | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#DatasetSeries.temporalcoverage), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:dataset_temporal)  | 
> | Änderungen zur Vorversion | 3.0: Neu hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatzserie: Beschreibung {#datensatzserie-beschreibung}
> | *URI*                      | [`dcterms:description`](http://purl.org/dc/terms/description) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft enthält eine Beschreibung der Datensatzserie als Freitext. |
> | Verwendungshinweis | Diese Eigenschaft kann für parallel existierende Sprachversionen der Beschreibung wiederholt werden.<br>Es wird empfohlen, eine Angabe zu den Dimensionen zu machen, über die sich die Datensatzserie erstreckt. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#DatasetSeries.description), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_description)  | 
> | Änderungen zur Vorversion | 3.0: Neu hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatzserie: Rechtsgrundlage {#datensatzserie-rechtsgrundlage}
> | *URI*                      | [`dcatap:applicableLegislation`](http://data.europa.eu/r5r/applicableLegislation) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`eli:LegalResource`](http://data.europa.eu/eli/ontology#LegalResource) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Die Rechtsvorschriften, die die Erstellung oder Verwaltung der Datensatzserie vorschreiben. |
> | Verwendungshinweis | Handelt es sich um ein High Value Dataset, muss `http://data.europa.eu/eli/reg_impl/2023/138/oj` angegeben werden.<br>Ansonsten wird die Verwendung eine ELI-Identifiers empfohlen. Ist dieser nicht bekannt, soll ein möglichst stabiler Link zum Gesetz verwendet werden. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#DatasetSeries.applicablelegislation)  | 
> | Änderungen zur Vorversion | 3.0: Neu hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatzserie: Aktualisierungsfrequenz {#datensatzserie-aktualisierungsfrequenz}
> | *URI*                      | [`dcterms:accrualPeriodicity`](http://purl.org/dc/terms/accrualPeriodicity) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:Frequency`](http://purl.org/dc/terms/Frequency) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft beschreibt die Aktualisierungsfrequenz der Datensatzserie. |
> | Verwendungshinweis | Die Aktualisierungsfrequenz der Datensatzserie ist nicht identisch zur Aktualisierungsfrequenz enthaltener Datensätze. | 
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-frequency) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#DatasetSeries.frequency), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:dataset_frequency)  | 
> | Änderungen zur Vorversion | 3.0: Neu hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatzserie: Veröffentlichungsdatum {#datensatzserie-veroffentlichungsdatum}
> | *URI*                      | [`dcterms:issued`](http://purl.org/dc/terms/issued) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) getyped als `xsd:gYear`, `xsd:gYearMonth`, `xsd:date` oder `xsd:dateTime` |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft enthält das Datum der Herausgabe/Emission (z.B. in Form einer Veröffentlichung) der Datensatzserie. |
> | Verwendungshinweis | Der Zeitpunkt, zu dem die Datensatzserie als verwaltete Ressource eingerichtet wurde. Dies ist nicht gleich dem Veröffentlichungsdatum des ältesten Datensatzes in der Serie.  | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#DatasetSeries.releasedate), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_release_date)  | 
> | Änderungen zur Vorversion | 3.0: Neu hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Datensatzserie: Aktualisierungsdatum {#datensatzserie-aktualisierungsdatum}
> | *URI*                      | [`dcterms:modified`](http://purl.org/dc/terms/modified) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) getyped als `xsd:gYear`, `xsd:gYearMonth`, `xsd:date` oder `xsd:dateTime` |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft erfasst das Datum der letzten Aktualisierung bzw. Modifikation der Datensatzserie. |
> | Verwendungshinweis | Dies ist nicht identisch mit dem zuletzt modifizierten Datensatz der Serie. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#DatasetSeries.modificationdate), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_update_date)  | 
> | Änderungen zur Vorversion | 3.0: Neu hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>



***


## Klasse: Distribution

> | *URI der Klasse* | [`dcat:Distribution`](http://www.w3.org/ns/dcat#Distribution)      |
> |:-----------------|:-----------------------------------------------------|
> | Beschreibung     | Eine physische Verkörperung/Repräsentanz des Datensatzes in einem spezifischen Format.     |
> | eingebunden über | dcat:distribution, adms:sample (dcat:Distribution)         | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Class:Distribution) |

<br>

Die folgenden Eigenschaften wurden von DCAT-AP.de hinzugefügt oder verändert: 
[`dcterms:license`](#distribution-lizenz), [`dcterms:title`](#distribution-titel), [`dcterms:modified`](#distribution-aktualisierungsdatum), [`dcatde:licenseAttributionByText`](#distribution-namensnennungstext-by-clauses), [`dcterms:description`](#distribution-beschreibung), [`dcat:spatialResolutionInMeters`](#distribution-raumliche-auflosung-in-meter), [`spdx:checksum`](#distribution-prufsumme).<br>


|                                 | Eigenschaft  | Wertebereich      | <small>Verbind&shy;lichkeit</small> | Mult. | Interop. |
|:--------------------------------|:-------------|:------------------|:------------------------------------|:-----:|:--------:|
| [Zugangs-URL](#distribution-zugangs-url) | `dcat:accessURL` | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) | <small>Pflicht</small> | `[1..*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Lizenz](#distribution-lizenz) | `dcterms:license` | [`dcterms:LicenseDocument`](http://purl.org/dc/terms/LicenseDocument) | <small>Pflicht</small> | `[1]` | <abbr title='Eigenes ergänzt.'>E</abbr> |
| [Titel](#distribution-titel) | `dcterms:title` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Empfohlen</small> | `[*]` | <abbr title='Eigenes ergänzt.'>E</abbr> |
| [Aktualisierungsdatum](#distribution-aktualisierungsdatum) | `dcterms:modified` | [`rdfs:Literal`]() | <small>Empfohlen</small> | `[0..1]` | <abbr title='Eigenes ergänzt.'>E</abbr> |
| [Format](#distribution-format) | `dcterms:format` | [`dcterms:MediaTypeOrExtent`](http://purl.org/dc/terms/MediaTypeOrExtent) | <small>Empfohlen</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Verfügbarkeit](#distribution-verfugbarkeit) | `dcatap:availability` | [`skos:Concept`](https://www.w3.org/2009/08/skos-reference/skos.html#Concept) | <small>Empfohlen</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Namensnennungstext für By-Clauses](#distribution-namensnennungstext-by-clauses) | `dcatde:licenseAttributionByText` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Optional</small> | `[*]` | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
| [Beschreibung](#distribution-beschreibung) | `dcterms:description` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Optional</small> | `[*]` | <abbr title='Eigenes ergänzt.'>E</abbr> |
| [Größe in Bytes](#distribution-grosse-in-bytes) | `dcat:byteSize` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Veröffentlichungsdatum](#distribution-veroffentlichungsdatum) | `dcterms:issued` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Download-URL](#distribution-download-url) | `dcat:downloadURL` | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Sprache](#distribution-sprache) | `dcterms:language` | [`dcterms:LinguisticSystem`](http://purl.org/dc/terms/LinguisticSystem) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Dokumentation](#distribution-dokumentation) | `foaf:page` | [`foaf:Document`](http://xmlns.com/foaf/0.1/Document) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Rechte](#distribution-rechte) | `dcterms:rights` | [`dcterms:RightsStatement`](http://purl.org/dc/terms/RightsStatement) | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Konform zu Standard](#distribution-konform-zu-standard) | `dcterms:conformsTo` | [`dcterms:Standard`](http://purl.org/dc/terms/Standard) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Medientyp](#distribution-medientyp) | `dcat:mediaType` | [`dcterms:MediaType`](http://purl.org/dc/terms/MediaType) | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Kompressionsformat](#distribution-kompressionsformat) | `dcat:compressFormat` | [`dcterms:MediaType`](http://purl.org/dc/terms/MediaType) | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Paketformat](#distribution-paketformat) | `dcat:packageFormat` | [`dcterms:MediaType`](http://purl.org/dc/terms/MediaType) | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Regelwerk](#distribution-regelwerk) | `odrl:hasPolicy` | [`odrl:Policy`](https://www.w3.org/TR/odrl-vocab/#term-Policy) | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Status](#distribution-status) | `adms:status` | [`skos:Concept`](http://www.w3.org/2004/02/skos/core#Concept) | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Räumliche Auflösung in Meter](#distribution-raumliche-auflosung-in-meter) | `dcat:spatialResolutionInMeters` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Optional</small> | `[0..1]` | <abbr title='Eigenes ergänzt.'>E</abbr> |
| [Zeitliche Auflösung](#distribution-zeitliche-auflosung) | `dcat:temporalResolution` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Ausliefernder Datenservice](#distribution-ausliefernder-datenservice) | `dcat:accessService` | [`dcat:DataService`](http://www.w3.org/ns/dcat#DataService) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Prüfsumme](#distribution-prufsumme) | `spdx:checksum` | [`spdx:Checksum`](http://spdx.org/rdf/terms#Checksum) | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |


<br>
<hr>
<br>

###  Distribution: Zugangs-URL {#distribution-zugangs-url}
> | *URI*                      | [`dcat:accessURL`](http://www.w3.org/ns/dcat#accessURL) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1..*]`                   |
> | Beschreibung               | Diese Eigenschaft enthält eine URL-Adresse, die Zugriff auf die Distribution eines Datensatzes ermöglicht.  |
> | Verwendungshinweis | Die mit der Zugangs-URL erreichbare Ressource kann Informationen zur Verfügung stellen, wie die Distribution erreicht werden kann oder direkt auf eine Datei verweisen, die die Daten im angegebenen Format beinhaltet. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.accessURL), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:distribution_access_url)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Distribution: Lizenz {#distribution-lizenz}
> | *URI*                      | [`dcterms:license`](http://purl.org/dc/terms/license) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:LicenseDocument`](http://purl.org/dc/terms/LicenseDocument) |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf die Lizenz, unter welcher die Distribution zur Verfügung gestellt wird. |
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-licenses) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.licence), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:distribution_license)  | 
> | Änderungen zur Vorversion | 3.0: Kardinalität von `[0..1]` auf `[1]` geändert und die Eigenschaft damit verpflichtend gemacht. | 
> | Interoperabilitätslevel    | <abbr title='Eigenes ergänzt.'>E</abbr> |
> | Änderungen durch DCAT-AP.de | Kardinalität von `[0..1]` auf `[1]` geändert und die Eigenschaft damit verpflichtend gemacht. | 
<br>

###  Distribution: Titel {#distribution-titel}
> | *URI*                      | [`dcterms:title`](http://purl.org/dc/terms/title) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft bezeichnet den einer Distribution zugewiesenen Titel. Diese Eigenschaft kann für parallele Sprachversionen des Distributionstitels wiederholt werden. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.title), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:distribution_title)  | 
> | Interoperabilitätslevel    | <abbr title='Eigenes ergänzt.'>E</abbr> |
> | Änderungen durch DCAT-AP.de | Verbindlichkeit wurde von optional auf empfohlen hochgestuft. | 
<br>

###  Distribution: Aktualisierungsdatum {#distribution-aktualisierungsdatum}
> | *URI*                      | [`dcterms:modified`](http://purl.org/dc/terms/modified) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) getyped als `xsd:gYear`, `xsd:gYearMonth`, `xsd:date` oder `xsd:dateTime` |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft erfasst das Datum der letzten Aktualisierung bzw. Modifikation der Distribution. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.modificationdate), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:distribution_update_date)  | 
> | Änderungen zur Vorversion | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Eigenes ergänzt.'>E</abbr> |
> | Änderungen durch DCAT-AP.de | Verbindlichkeit wurde von optional auf empfohlen hochgestuft. | 
<br>

###  Distribution: Format {#distribution-format}
> | *URI*                      | [`dcterms:format`](http://purl.org/dc/terms/format) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:MediaTypeOrExtent`](http://purl.org/dc/terms/MediaTypeOrExtent) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf das Datenformat der Distribution. |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#angaben-zu-dateiformaten) genauer beschrieben. | 
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-file-type) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.format), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:distribution_format)  | 
> | Änderungen zur Vorversion | 3.0: Errata: Wertebereichs auf dcterms:MediaTypeOrExtent geändert. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Distribution: Verfügbarkeit {#distribution-verfugbarkeit}
> | *URI*                      | [`dcatap:availability`](http://data.europa.eu/r5r/availability) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`skos:Concept`](https://www.w3.org/2009/08/skos-reference/skos.html#Concept) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Verfügbarkeit der Distribution eines Datensatzes, als Auswahl aus einer festen Liste von Werten via DCAT-AP URIs. |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#status-und-erwartete-verfugbarkeit) genauer beschrieben. | 
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-availability) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.availability)  | 
> | Änderungen zur Vorversion | 3.0: Errata: Hinterlegte URL für den Wertebereichs auf skos:Concept geändert. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Distribution: Namensnennungstext für By-Clauses {#distribution-namensnennungstext-by-clauses}
> | *URI*                      | [`dcatde:licenseAttributionByText`](http://dcat-ap.de/def/dcatde/licenseAttributionByText) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft speichert den verpflichtenden Namensnennungstext bei Lizenzangaben. |
> | Verwendungshinweis | Diese Eigenschaft kann für parallele Sprachversionen des Namensnennungstextes wiederholt werden.<br>Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#angabe-von-by-texten) genauer beschrieben. | 
> | Interoperabilitätslevel    | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
> | Änderungen durch DCAT-AP.de | Hilfskonstrukt bis zur Lösung in DCAT-AP. | 
<br>

###  Distribution: Beschreibung {#distribution-beschreibung}
> | *URI*                      | [`dcterms:description`](http://purl.org/dc/terms/description) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft enthält eine Freitextbeschreibung der Distribution. |
> | Verwendungshinweis | Diese Eigenschaft kann für unterschiedliche Sprachversionen wiederholt werden. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.description), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:distribution_description)  | 
> | Interoperabilitätslevel    | <abbr title='Eigenes ergänzt.'>E</abbr> |
> | Änderungen durch DCAT-AP.de | Verbindlichkeit wurde von empfohlen auf optional gesenkt. | 
<br>

###  Distribution: Größe in Bytes {#distribution-grosse-in-bytes}
> | *URI*                      | [`dcat:byteSize`](http://www.w3.org/ns/dcat#byteSize) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) getyped als `xsd:nonNegativeInteger` |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft enthält die Größe der Distribution in Bytes. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.bytesize), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:distribution_size)  | 
> | Änderungen zur Vorversion | 3.0: Änderung der Range von xsd:decimal auf xsd:nonNegativeInteger. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Distribution: Veröffentlichungsdatum {#distribution-veroffentlichungsdatum}
> | *URI*                      | [`dcterms:issued`](http://purl.org/dc/terms/issued) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) getyped als `xsd:gYear`, `xsd:gYearMonth`, `xsd:date` oder `xsd:dateTime` |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft enthält das Datum der Herausgabe/Emission (z.B. in Form einer Veröffentlichung) der Distribution. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.releasedate), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:distribution_release_date)  | 
> | Änderungen zur Vorversion | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Distribution: Download-URL {#distribution-download-url}
> | *URI*                      | [`dcat:downloadURL`](http://www.w3.org/ns/dcat#downloadURL) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Resource) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft enthält eine URL-Adresse, welche einen direkten Zugriff/Link auf die herunterladbare Datei im beschriebenen Format liefert. |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#zugriff-auf-eine-herunterladbare-datei) genauer beschrieben. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.downloadURL), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:distribution_download_url)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Distribution: Sprache {#distribution-sprache}
> | *URI*                      | [`dcterms:language`](http://purl.org/dc/terms/language) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:LinguisticSystem`](http://purl.org/dc/terms/LinguisticSystem) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf die in der Distribution verwendete Sprache. |
> | Verwendungshinweis | Diese Eigenschaft kann wiederholt werden, sofern die Distribution in mehreren Sprachen vorliegt. | 
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-languages) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.language)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Distribution: Dokumentation {#distribution-dokumentation}
> | *URI*                      | [`foaf:page`](http://xmlns.com/foaf/0.1/page) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`foaf:Document`](http://xmlns.com/foaf/0.1/Document) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf eine Webseite oder ein Dokument (enthält eine URL-Adresse) mit Informationen über die Distribution. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.documentation), [FOAF](http://xmlns.com/foaf/spec/#term_page)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Distribution: Rechte {#distribution-rechte}
> | *URI*                      | [`dcterms:rights`](http://purl.org/dc/terms/accessRights) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:RightsStatement`](http://purl.org/dc/terms/RightsStatement) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf eine juristische Quelle, welche die mit der Distribution assoziierten Rechte spezifiziert. |
> | Verwendungshinweis | Gemeint ist damit zum Beispiel ein Link zu Nutzungsbedingungen, wie "Terms of Use", die zusätzlich zu oder statt einer Lizenz bestehen. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.rights), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:distribution_rights)  | 
> | Änderungen zur Vorversion | 3.0: In "Rechte" umbenannt und Verwendungshinweis hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Distribution: Konform zu Standard {#distribution-konform-zu-standard}
> | *URI*                      | [`dcterms:conformsTo`](http://purl.org/dc/terms/conformsTo) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:Standard`](http://purl.org/dc/terms/Standard) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf ein etabliertes Schema, zu dem die Distribution konform ist. |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#konformitat-zu-bestehenden-standards) genauer beschrieben. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.linkedschemas), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:distribution_conforms_to)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Distribution: Medientyp {#distribution-medientyp}
> | *URI*                      | [`dcat:mediaType`](http://www.w3.org/ns/dcat#mediaType) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:MediaType`](http://purl.org/dc/terms/MediaType) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf den Medientyp der Distribution. |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#angaben-zu-dateiformaten) genauer beschrieben. | 
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-iana-media-types) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.mediatype), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:distribution_media_type)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Distribution: Kompressionsformat {#distribution-kompressionsformat}
> | *URI*                      | [`dcat:compressFormat`](http://www.w3.org/ns/dcat#mediaType) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:MediaType`](http://purl.org/dc/terms/MediaType) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf das Dateiformat, in dem die Daten der Distribution in komprimierter Form, z.B. um die Größe zu reduzieren, zum Download angeboten werden. |
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-iana-media-types) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.compressionformat), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:distribution_compression_format)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Distribution: Paketformat {#distribution-paketformat}
> | *URI*                      | [`dcat:packageFormat`](http://www.w3.org/ns/dcat#mediaType) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:MediaType`](http://purl.org/dc/terms/MediaType) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf das Dateiformat, in dem die Daten der Distribution zusammengeschnürt zum Download angeboten werden. Zum Beispiel, um den Download zu erleichtern. |
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-iana-media-types) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.packagingformat), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:distribution_packaging_format)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Distribution: Regelwerk {#distribution-regelwerk}
> | *URI*                      | [`odrl:hasPolicy`](https://www.w3.org/TR/odrl-vocab/#term-hasPolicy) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`odrl:Policy`](https://www.w3.org/TR/odrl-vocab/#term-Policy) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf ein Regelwerk, das die Rechte die mit dieser Distribution assoziiert werden unter Verwendung des ODRL Vokabulars beschreibt. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.haspolicy), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:distribution_has_policy)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Distribution: Status {#distribution-status}
> | *URI*                      | [`adms:status`](http://www.w3.org/ns/adms#status) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`skos:Concept`](http://www.w3.org/2004/02/skos/core#Concept) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf den Status bzw. Reifegrad der Distribution. |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#status-und-erwartete-verfugbarkeit) genauer beschrieben. | 
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-distribution-status) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.status), [ADMS](https://www.w3.org/TR/vocab-adms/#adms-status)  | 
> | Änderungen zur Vorversion | 3.0: Änderung des kontrollierten Vokabulars. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Distribution: Räumliche Auflösung in Meter {#distribution-raumliche-auflosung-in-meter}
> | *URI*                      | [`dcat:spatialResolutionInMeters`](http://www.w3.org/ns/dcat#spatialResolutionInMeters) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) getyped als [`xsd:decimal`](https://www.w3.org/TR/xmlschema11-2/#decimal) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf den kleinsten räumlichen Abstand, der in der Distribution auflösbar ist, gemessen in Metern. |
> | Verwendungshinweis | Kann die räumliche Auflösung nicht in Metern beschrieben werden, können stattdessen die spezielleren Eigenschaften verwendet werden, die [GeoDCAT-AP](https://semiceu.github.io/GeoDCAT-AP/releases/2.0.0/#spatial-resolution-spatial-resolution-of-the-dataset) hierfür zur Verfügung stellt. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.spatialresolution), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:dataset_spatial_resolution)  | 
> | Änderungen zur Vorversion | 3.0: Errata: Eigenschaft aufgeführt, existierte bereits in DCAT-AP 2.0. | 
> | Interoperabilitätslevel    | <abbr title='Eigenes ergänzt.'>E</abbr> |
> | Änderungen durch DCAT-AP.de | Verwendungshinweis hinzugefügt. | 
<br>

###  Distribution: Zeitliche Auflösung {#distribution-zeitliche-auflosung}
> | *URI*                      | [`dcat:temporalResolution`](http://www.w3.org/ns/dcat#temporalResolution) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) getyped als [`xsd:duration`](https://www.w3.org/TR/xmlschema11-2/#duration) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf den kürzesten in der Distribution auflösbaren Zeitraum. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.temporalresolution), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:dataset_spatial_resolution)  | 
> | Änderungen zur Vorversion | 3.0: Errata: Eigenschaft aufgeführt, existierte bereits in DCAT-AP 2.0. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Distribution: Ausliefernder Datenservice {#distribution-ausliefernder-datenservice}
> | *URI*                      | [`dcat:accessService`](http://www.w3.org/ns/dcat#accessService) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcat:DataService`](http://www.w3.org/ns/dcat#DataService) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf den Datenservice, der Zugang zur Distribution ermöglicht. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.accessservice), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:distribution_access_service)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Distribution: Prüfsumme {#distribution-prufsumme}
> | *URI*                      | [`spdx:checksum`](http://spdx.org/rdf/terms#checksum) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`spdx:Checksum`](http://spdx.org/rdf/terms#Checksum) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft stellt einen Mechanismus zur Verfügung, mit dem sichergestellt werden kann, dass die Inhalte der Distribution sich nicht verändert haben. |
> | Verwendungshinweis | Die Prüfsumme bezieht sich auf die Datei, die über `dcat:downloadURL` erreicht wird. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Distribution.checksum), [SPDX](https://spdx.org/rdf/terms/#d4e165)  | 
> | Änderungen zur Vorversion | 3.0: Harmonisierung: Verwendungshinweis hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |
> | Änderungen durch DCAT-AP.de | DCAT-AP.de stellt ein erweitertes kontrolliertes Vokabular zur Verfügung, dass in der [Klasse Prüfsumme](#klasse-prufsumme) von der [Eigenschaft Algorithmus](#prufsumme-algorithmus) verwendet wird. | 
<br>



***


## Klasse: Zeitraum

> | *URI der Klasse* | [`dcterms:PeriodOfTime`](http://purl.org/dc/terms/PeriodOfTime)      |
> |:-----------------|:-----------------------------------------------------|
> | Beschreibung     | Ein Zeitintervall, welches durch Start- und Endzeitpunkt bezeichnet bzw. definiert ist.<br>Das Zeitintervall kann auch offen sein, dann hat es lediglich einen Start- oder Endzeitpunkt.<br>Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/spec/#datensatz-zeitliche-abdeckung) genauer beschrieben.     |
> | eingebunden über | dcterms:temporal (dcat:Dataset)         | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Periodoftime), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Class:Period_of_Time) |

<br>


|                                 | Eigenschaft  | Wertebereich      | <small>Verbind&shy;lichkeit</small> | Mult. | Interop. |
|:--------------------------------|:-------------|:------------------|:------------------------------------|:-----:|:--------:|
| [Startzeitpunkt](#zeitraum-startzeitpunkt) | `dcat:startDate` | [`rdfs:Literal`]() | <small>Empfohlen</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Endzeitpunkt](#zeitraum-endzeitpunkt) | `dcat:endDate` | [`rdfs:Literal`]() | <small>Empfohlen</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Anfang](#zeitraum-anfang) | `time:hasBeginning` | [`time:Instant`](https://www.w3.org/TR/owl-time/#time:Instant) | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Ende](#zeitraum-ende) | `time:hasEnd` | [`time:Instant`](https://www.w3.org/TR/owl-time/#time:Instant) | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |


<br>
<hr>
<br>

###  Zeitraum: Startzeitpunkt {#zeitraum-startzeitpunkt}
> | *URI*                      | [`dcat:startDate`](http://www.w3.org/ns/dcat#startDate) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) getyped als `xsd:gYear`, `xsd:gYearMonth`, `xsd:date` oder `xsd:dateTime` |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft bezeichnet den Beginn des Zeitraumes. |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/spec/#datensatz-zeitliche-abdeckung) genauer beschrieben. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Periodoftime.startdate), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:period_start_date)  | 
> | Änderungen zur Vorversion | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Zeitraum: Endzeitpunkt {#zeitraum-endzeitpunkt}
> | *URI*                      | [`dcat:endDate`](http://www.w3.org/ns/dcat#endDate) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) getyped als `xsd:gYear`, `xsd:gYearMonth`, `xsd:date` oder `xsd:dateTime` |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft bezeichnet das Ende des Zeitraumes. |
> | Verwendungshinweis | Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/spec/#datensatz-zeitliche-abdeckung) genauer beschrieben. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Periodoftime.enddate), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:period_end_date)  | 
> | Änderungen zur Vorversion | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Zeitraum: Anfang {#zeitraum-anfang}
> | *URI*                      | [`time:hasBeginning`](https://www.w3.org/TR/owl-time/#time:hasBeginning) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`time:Instant`](https://www.w3.org/TR/owl-time/#time:Instant) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Anfang eines Zeitraums oder einer Periode. |
> | Verwendungshinweis | Mit der Range `time:Instant` können auch unkonventionelle Zeitangaben gemacht werden. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Periodoftime.beginning), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:period_has_beginning)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Zeitraum: Ende {#zeitraum-ende}
> | *URI*                      | [`time:hasEnd`](https://www.w3.org/TR/owl-time/#time:hasEnd) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`time:Instant`](https://www.w3.org/TR/owl-time/#time:Instant) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Ende eines Zeitraums oder einer Periode. |
> | Verwendungshinweis | Mit der Range `time:Instant` können auch unkonventionelle Zeitangaben gemacht werden. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Periodoftime.end), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:period_has_end)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>



***


## Klasse: Standort

> | *URI der Klasse* | [`dcterms:Location`](http://purl.org/dc/terms/Location)      |
> |:-----------------|:-----------------------------------------------------|
> | Beschreibung     | Ein räumlicher Bereich oder ein bezeichneter Ort. Er kann durch ein kontrolliertes Vokabular oder mit geographischen Koordinaten repräsentiert werden.<br>Die Verwendung wird im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#angaben-zur-geografischen-abdeckung) genauer beschrieben.     |
> | eingebunden über | dcterms:spatial (dcat:Dataset)         | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Location), [DCMI Metadata Terms](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/terms/Location/) |

<br>


|                                 | Eigenschaft  | Wertebereich      | <small>Verbind&shy;lichkeit</small> | Mult. | Interop. |
|:--------------------------------|:-------------|:------------------|:------------------------------------|:-----:|:--------:|
| [Bounding Box](#standort-bounding-box) | `dcat:bbox` | [`rdfs:Resource`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Empfohlen</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Geografischer Mittelpunkt](#standort-geografischer-mittelpunkt) | `dcat:centroid` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Empfohlen</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Geometrie](#standort-geometrie) | `locn:geometry` | [`locn:Geometry`](http://www.w3.org/ns/locn#Geometry) | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |


<br>
<hr>
<br>

###  Standort: Bounding Box {#standort-bounding-box}
> | *URI*                      | [`dcat:bbox`](http://www.w3.org/ns/dcat#bbox) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | Bewusst generisch gehalten als [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) z. B. getyped als `geo:wktLiteral` |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft beschreibt die Bounding Box einer Ressource. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Location.bbox), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:location_bbox)  | 
> | Änderungen zur Vorversion | 3.0: Errata: Korrektur des zu verwendenden Types. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Standort: Geografischer Mittelpunkt {#standort-geografischer-mittelpunkt}
> | *URI*                      | [`dcat:centroid`](http://www.w3.org/ns/dcat#centroid) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | Bewusst generisch gehalten als [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) z. B. getyped als `geo:wktLiteral` |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft beschreibt den geografischen Mittelpunkt einer Ressource. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Location.centroid), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:location_centroid)  | 
> | Änderungen zur Vorversion | 3.0: Errata: Korrektur des zu verwendenden Types. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Standort: Geometrie {#standort-geometrie}
> | *URI*                      | [`locn:geometry`](http://www.w3.org/ns/locn#geometry) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`locn:Geometry`](http://www.w3.org/ns/locn#Geometry) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft beschreibt die Geometrie einer Ressource. |
> | Verwendungshinweis | Der Wertebereich dieser Eigenschaft lässt jede Art von Geometriespezifikation zu.<br>Empfohlen wird z.B. die Angabe als WKT-Literal (`rdfs:Literal` getyped als `geo:wktLiteral`). | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Location.geometry), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:location_geometry), [locn](https://www.w3.org/ns/locn#locn:geometry)  | 
> | Änderungen zur Vorversion | 3.0: Wertebereich auf locn:Geometry geändert.<br>3.0: Verwendungshinweis von DCAT hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>



***


## Klasse: Verantwortliche Stelle

> | *URI der Klasse* | [`foaf:Agent`](http://xmlns.com/foaf/0.1/Agent)      |
> |:-----------------|:-----------------------------------------------------|
> | Beschreibung     | Eine Stelle oder Person, welche mit Katalogen und Datensätzen in unterschiedlichen Rollenausprägungen assoziiert ist.     |
> | eingebunden über | dcterms:publisher (dcat:Catalog), dcterms:publisher (dcat:Dataset), dcterms:creator (dcat:Dataset), ...         | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Agent), [FOAF Vocabulary](http://xmlns.com/foaf/spec/#term_Agent) |

<br>


|                                 | Eigenschaft  | Wertebereich      | <small>Verbind&shy;lichkeit</small> | Mult. | Interop. |
|:--------------------------------|:-------------|:------------------|:------------------------------------|:-----:|:--------:|
| [Name](#verantwortliche-stelle-name) | `foaf:name` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Pflicht</small> | `[1..*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Typ](#verantwortliche-stelle-typ) | `dcterms:type` | [`skos:Concept`](http://www.w3.org/2004/02/skos/core#Concept) | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |


<br>
<hr>
<br>

###  Verantwortliche Stelle: Name {#verantwortliche-stelle-name}
> | *URI*                      | [`foaf:name`](http://xmlns.com/foaf/0.1/name) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1..*]`                   |
> | Beschreibung               | Diese Eigenschaft enthält den Namen der verantwortlichen Stelle.  |
> | Verwendungshinweis | Sie kann für unterschiedliche Ausprägungen des Namens (z.B. der Name in unterschiedlichen Sprachen) wiederholt werden. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Agent.name), [FOAF Vocabulary](http://xmlns.com/foaf/spec/#term_name)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Verantwortliche Stelle: Typ {#verantwortliche-stelle-typ}
> | *URI*                      | [`dcterms:type`](http://purl.org/dc/terms/type) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`skos:Concept`](http://www.w3.org/2004/02/skos/core#Concept) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf den Typ der verantwortlichen Stelle, die die Ressource bereitstellt. |
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-adms-publisher) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Agent.type), [DCMI Metadata Terms](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/#http://purl.org/dc/terms/type)  | 
> | Änderungen zur Vorversion | 3.0: Errata: Link zur zu verwendenden Codeliste hinzugefügt, war zuvor bei `foaf:name` angegeben. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>



***


## Klasse: Identifier

> | *URI der Klasse* | [`adms:Identifier`](http://www.w3.org/ns/adms#Identifier)      |
> |:-----------------|:-----------------------------------------------------|
> | Beschreibung     | Die Klasse "Identifier" besteht je nach spezifischen Kontext aus einem String, welcher<br>- die ID ist, <br>- eine optionale ID für das ID-Schema ist,<br>- eine optionale ID für die Version des ID-Schemas ist oder<br>- eine optionale ID für die das ID-Schema pflegende verantwortliche Stelle ist.     |
> | eingebunden über | adms:identifier (dcat:Dataset)         | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Identifier), [ADMS](https://www.w3.org/TR/vocab-adms/#dt_identifier) |

<br>


|                                 | Eigenschaft  | Wertebereich      | <small>Verbind&shy;lichkeit</small> | Mult. | Interop. |
|:--------------------------------|:-------------|:------------------|:------------------------------------|:-----:|:--------:|
| [Notation des Identifier](#identifier-notation) | `skos:notation` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Pflicht</small> | `[1]` | <abbr title='Unverändert übernommen.'>A</abbr> |


<br>
<hr>
<br>

###  Identifier: Notation des Identifier {#identifier-notation}
> | *URI*                      | [`skos:notation`](http://www.w3.org/2004/02/skos/core#notation) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) getyped mit der URI eines [DataCite Resource Identifier Schemes](https://sparontologies.github.io/datacite/current/datacite.html#d4e643) |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1]`                   |
> | Beschreibung               | Diese Eigenschaft enthält einen datentypreferenzierten ID-String im Kontext des ID-Schemas. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Identifier.notation), [ADMS](https://www.w3.org/TR/vocab-adms/#skos_notation)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>



***


## Klasse: Prüfsumme

> | *URI der Klasse* | [`spdx:Checksum`](http://spdx.org/rdf/terms#Checksum)      |
> |:-----------------|:-----------------------------------------------------|
> | Beschreibung     | Ein Wert, der es ermöglicht, die Inhalte einer Datei zu verifizieren (für korrekt zu erklären). <br>Diese Klasse ermöglicht es, die Ergebnisse einer Vielzahl von Prüfsummen- und Kryptoalgorithmen zu repräsentieren.     |
> | eingebunden über | spdx:checksum (dcat:Distribution)         | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Checksum), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Class:Checksum), [SPDX](https://spdx.org/rdf/terms/#d4e2091) |

<br>

Die folgenden Eigenschaften wurden von DCAT-AP.de hinzugefügt oder verändert: 
[`spdx:algorithm`](#prufsumme-algorithmus).<br>


|                                 | Eigenschaft  | Wertebereich      | <small>Verbind&shy;lichkeit</small> | Mult. | Interop. |
|:--------------------------------|:-------------|:------------------|:------------------------------------|:-----:|:--------:|
| [Algorithmus](#prufsumme-algorithmus) | `spdx:algorithm` | [`spdx:ChecksumAlgorithm`](http://spdx.org/rdf/terms#ChecksumAlgorithm) | <small>Pflicht</small> | `[1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Prüfsummenwert](#prufsumme-prufsummenwert) | `spdx:checksumValue` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Pflicht</small> | `[1]` | <abbr title='Unverändert übernommen.'>A</abbr> |


<br>
<hr>
<br>

###  Prüfsumme: Algorithmus {#prufsumme-algorithmus}
> | *URI*                      | [`spdx:algorithm`](http://spdx.org/rdf/terms#algorithm) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`spdx:ChecksumAlgorithm`](http://spdx.org/rdf/terms#ChecksumAlgorithm) |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1]`                   |
> | Beschreibung               | Diese Eigenschaft identifiziert den verwendeten Algorithmus zur Erzeugung der Prüfsumme. |
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-hash-algorithms) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Checksum.algorithm), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:checksum_algorithm), [SPDX](https://spdx.org/rdf/terms/#d4e46)  | 
> | Änderungen zur Vorversion | 3.0: Range von `rdfs:Resource` auf `spdx:ChecksumAlgorithm` geändert. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |
> | Änderungen durch DCAT-AP.de | dcat-ap.de führt eine eigene Liste an unterstützten Hashalgorithmen. | 
<br>

###  Prüfsumme: Prüfsummenwert {#prufsumme-prufsummenwert}
> | *URI*                      | [`spdx:checksumValue`](http://spdx.org/rdf/terms#checksumValue) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) getyped als `xsd:hexBinary` |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1]`                   |
> | Beschreibung               | Diese Eigenschaft stellt einen hexadezimal kodierten Übersichtswert in Kleinbuchstaben zur Verfügung, welcher mittels eines spezifischen Algorithmus erzeugt wurde. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Checksum.checksumvalue), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:checksum_checksum_value), [SPDX](https://spdx.org/rdf/terms/#d4e1053)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>



***


## Klasse: Katalogeintrag

> | *URI der Klasse* | [`dcat:CatalogRecord`](http://www.w3.org/ns/dcat#CatalogRecord)      |
> |:-----------------|:-----------------------------------------------------|
> | Beschreibung     | Die Beschreibung des Eintrags in einem Katalog.     |
> | eingebunden über | dcat:record (dcat:Catalog), dcterms:source (dcat:CatalogRecord)         | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#CatalogueRecord), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Class:Catalog_Record) |

<br>

Die folgenden Eigenschaften wurden von DCAT-AP.de hinzugefügt oder verändert: 
[`adms:status`](#katalogeintrag-anderungstyp).<br>


|                                 | Eigenschaft  | Wertebereich      | <small>Verbind&shy;lichkeit</small> | Mult. | Interop. |
|:--------------------------------|:-------------|:------------------|:------------------------------------|:-----:|:--------:|
| [Aktualisierungsdatum](#katalogeintrag-aktualisierungsdatum) | `dcterms:modified` | [`rdfs:Literal`]() | <small>Pflicht</small> | `[1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Katalogeintrag](#katalogeintrag-katalogeintrag) | `foaf:primaryTopic` | [`dcat:Resource`]() | <small>Pflicht</small> | `[1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Application Profile der Metadaten](#katalogeintrag-konform-zu) | `dcterms:conformsTo` | [`dcterms:Standard`](http://purl.org/dc/terms/Standard) | <small>Empfohlen</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Änderungstyp](#katalogeintrag-anderungstyp) | `adms:status` | [`skos:Concept`](http://www.w3.org/2004/02/skos/core#Concept) | <small>Empfohlen</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Veröffentlichungsdatum](#katalogeintrag-veroffentlichungsdatum) | `dcterms:issued` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Empfohlen</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Titel](#katalogeintrag-titel) | `dcterms:title` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Beschreibung](#katalogeintrag-beschreibung) | `dcterms:description` | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Sprache](#katalogeintrag-sprache) | `dcterms:language` | [`dcterms:LinguisticSystem`](http://purl.org/dc/terms/LinguisticSystem) | <small>Optional</small> | `[*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Original-Metadaten der Ressource](#katalogeintrag-original-metadaten-der-ressource) | `dcterms:source` | [`dcat:CatalogRecord`]() | <small>Optional</small> | `[0..1]` | <abbr title='Unverändert übernommen.'>A</abbr> |


<br>
<hr>
<br>

###  Katalogeintrag: Aktualisierungsdatum {#katalogeintrag-aktualisierungsdatum}
> | *URI*                      | [`dcterms:modified`](http://purl.org/dc/terms/modified) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) getyped als  `xsd:gYear`, `xsd:gYearMonth`, `xsd:date` oder `xsd:dateTime` |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1]`                   |
> | Beschreibung               | Diese Eigenschaft erfasst das Datum der letzten Aktualisierung bzw. Modifikation des Katalogeintrags. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#CatalogueRecord.modificationdate), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:resource_update_date)  | 
> | Änderungen zur Vorversion | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Katalogeintrag: Katalogeintrag {#katalogeintrag-katalogeintrag}
> | *URI*                      | [`foaf:primaryTopic`](http://xmlns.com/foaf/0.1/primaryTopic) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | `dcat:Dataset`, `dcat:DataService`, `dcat:DatasetSeries` oder `dcat:Catalog` |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1]`                   |
> | Beschreibung               | Diese Eigenschaft verknüpft den Katalogeintrag mit der im Eintrag beschriebenen `dcat:Resource`. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#CatalogueRecord.primarytopic), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:record_primary_topic)  | 
> | Änderungen zur Vorversion | 3.0: Aufnahme der Ressource `dcat:DatasetSeries` | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Katalogeintrag: Application Profile der Metadaten {#katalogeintrag-konform-zu}
> | *URI*                      | [`dcterms:conformsTo`](http://purl.org/dc/terms/conformsTo) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:Standard`](http://purl.org/dc/terms/Standard) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf das Application Profile zu dem die Metadaten im Katalog konform sind. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#CatalogueRecord.applicationprofile), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:record_conforms_to)  | 
> | Änderungen zur Vorversion | 3.0: Kardinalität von `0..1` auf `*` geändert.<br>3.0: Errata: Anzeige des Wertebereichs korrigiert. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Katalogeintrag: Änderungstyp {#katalogeintrag-anderungstyp}
> | *URI*                      | [`adms:status`](http://www.w3.org/ns/adms#status) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`skos:Concept`](http://www.w3.org/2004/02/skos/core#Concept) |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf den Typ der letzten Revision des Datensatzeintrags in den Katalog. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#CatalogueRecord.changetype), [ADMS](https://www.w3.org/TR/vocab-adms/#adms-status)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |
> | Änderungen durch DCAT-AP.de | Diese Eigenschaft wird von DCAT-AP.de nicht unterstützt, unter anderem weil das eigentlich vorgesehene Vokabular nicht vorhanden ist. | 
<br>

###  Katalogeintrag: Veröffentlichungsdatum {#katalogeintrag-veroffentlichungsdatum}
> | *URI*                      | [`dcterms:issued`](http://purl.org/dc/terms/issued) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) getyped als `xsd:gYear`, `xsd:gYearMonth`, `xsd:date` oder `xsd:dateTime` |
> | Verbindlichkeit            | Empfohlen |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft enthält das Datum, an dem die Beschreibung der Ressource aufgenommen wurde. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#CatalogueRecord.listingdate), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:record_listing_date)  | 
> | Änderungen zur Vorversion | 3.0: `xsd:gYear` und `xsd:gYearMonth` zum Wertebereich hinzugefügt. | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Katalogeintrag: Titel {#katalogeintrag-titel}
> | *URI*                      | [`dcterms:title`](http://purl.org/dc/terms/title) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft bezeichnet den Titel eines Katalogeintrags. |
> | Verwendungshinweis | Diese Eigenschaft kann für parallele Sprachversionen des Katalogtitels wiederholt werden. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#CatalogueRecord.title), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:record_title)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Katalogeintrag: Beschreibung {#katalogeintrag-beschreibung}
> | *URI*                      | [`dcterms:description`](http://purl.org/dc/terms/description) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Literal`](http://www.w3.org/2000/01/rdf-schema#Literal) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft enthält eine Freitextbeschreibung des Katalogeintrags. |
> | Verwendungshinweis | Diese Eigenschaft kann für unterschiedliche Sprachversionen wiederholt werden. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#CatalogueRecord.description), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:record_description)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Katalogeintrag: Sprache {#katalogeintrag-sprache}
> | *URI*                      | [`dcterms:language`](http://purl.org/dc/terms/language) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcterms:LinguisticSystem`](http://purl.org/dc/terms/LinguisticSystem) |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[*]`                   |
> | Beschreibung               | Diese Eigenschaft bezieht sich auf die Sprache der Metadatenbeschreibung für die zum Katalogeintrag gehörenden Eigenschaften (z.B. Titel, Beschreibungen usw.). |
> | Verwendungshinweis | Diese Eigenschaft kann wiederholt werden, falls die Metadaten in verschiedenen Sprachen zur Verfügung stehen. | 
> | Codeliste | [DCAT-AP.de macht Vorgaben zur zu verwendenden Codeliste.](#kv-languages) |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#CatalogueRecord.language), [DCMI Metadata Terms](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/#http://purl.org/dc/terms/language)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Katalogeintrag: Original-Metadaten der Ressource {#katalogeintrag-original-metadaten-der-ressource}
> | *URI*                      | [`dcterms:source`](http://purl.org/dc/terms/source) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcat:CatalogRecord`]() |
> | Verbindlichkeit            | Optional |
> | Multiplizität              | `[0..1]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf die ursprünglichen Metadaten, mit Hilfe derer die Metadaten des Katalogeintrags erstellt wurden. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#CatalogueRecord.sourcemetadata), [DCMI Metadata Terms](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/#http://purl.org/dc/terms/source)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>



***


## Klasse: Beziehung

> | *URI der Klasse* | [`dcat:Relationship`](http://www.w3.org/ns/dcat#Relationship)      |
> |:-----------------|:-----------------------------------------------------|
> | Beschreibung     | Eine Klasse, um eine Beziehung zwischen mehreren DCAT Ressourcen genauer zu beschreiben.     |
> | eingebunden über | dcat:qualifiedRelation (dcat:Dataset)         | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Relationship), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Class:Relationship) |

<br>


|                                 | Eigenschaft  | Wertebereich      | <small>Verbind&shy;lichkeit</small> | Mult. | Interop. |
|:--------------------------------|:-------------|:------------------|:------------------------------------|:-----:|:--------:|
| [Hatte Rolle](#beziehung-rolle) | `dcat:hadRole` | [`dcat:Role`](http://www.w3.org/ns/dcat#Role) | <small>Pflicht</small> | `[1..*]` | <abbr title='Unverändert übernommen.'>A</abbr> |
| [Beziehung](#beziehung-beziehung) | `dcterms:relation` | [`rdfs:Resource`](rdfs:Resource) | <small>Pflicht</small> | `[1..*]` | <abbr title='Unverändert übernommen.'>A</abbr> |


<br>
<hr>
<br>

###  Beziehung: Hatte Rolle {#beziehung-rolle}
> | *URI*                      | [`dcat:hadRole`](http://www.w3.org/ns/dcat#hadRole) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcat:Role`](http://www.w3.org/ns/dcat#Role) |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1..*]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf die Funktion einer Ressource in Beziehung zu einer anderen Ressource. |
> | Verwendungshinweis | DCAT-AP.de definiert mehrere spezifische Rollen, die bevorzugt verwendet werden sollten. Die Klasse [`dcat:Role` (siehe DCAT)]([DCAT](https://www.w3.org/TR/vocab-dcat-3/#Class:Role) verfügt über keine empfohlenen, verpflichtenden oder optionalen Eigenschaften. `dcat:hadRole` sollte, wenn es notwendig ist, mit einem kontrollierten Vokabular verwendet werden, für das aber keine Vorgaben gemacht werden. Das W3C nennt jedoch einige mögliche Kandidaten. | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Relationship.hadrole), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:relationship_hadRole)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>

###  Beziehung: Beziehung {#beziehung-beziehung}
> | *URI*                      | [`dcterms:relation`](http://purl.org/dc/terms/relation) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`rdfs:Resource`](rdfs:Resource) |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1..*]`                   |
> | Beschreibung               | Diese Eigenschaft verweist auf die Ressourcen, die miteinander in einer Beziehung stehen. |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Relationship.relation), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:relationship_relation)  | 
> | Interoperabilitätslevel    | <abbr title='Unverändert übernommen.'>A</abbr> |

<br>



***


## Klasse: Rollenzuordnung

> | *URI der Klasse* | [`prov:Attribution`](http://www.w3.org/ns/prov#Attribution)      |
> |:-----------------|:-----------------------------------------------------|
> | Beschreibung     | Diese Klasse verknüft eine Ressource mit Agenten und beschreibt, welche Rolle die Agenten im Bezug auf die Ressource eingenommen haben.<br>Sie ist insbesondere dann relevant, wenn keine Eigenschaften wie `geodcat:originator`, `dcterms:creator` oder `dcterms:publisher` existieren, um die Rolle zu beschreiben.     |
> | eingebunden über | prov:qualifiedAttribution (dcat:Dataset, dcat:DataService)         | 
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#Attribution), [PROV-O](https://www.w3.org/TR/prov-o/#Attribution) |

<br>

Die folgenden Eigenschaften wurden von DCAT-AP.de hinzugefügt oder verändert: 
[`dcat:hadRole`](#rollenzuordnung-rolle), [`prov:agent`](#rollenzuordnung-agent).<br>


|                                 | Eigenschaft  | Wertebereich      | <small>Verbind&shy;lichkeit</small> | Mult. | Interop. |
|:--------------------------------|:-------------|:------------------|:------------------------------------|:-----:|:--------:|
| [Hatte Rolle](#rollenzuordnung-rolle) | `dcat:hadRole` | [`dcat:Role`](http://www.w3.org/ns/dcat#Role) | <small>Pflicht</small> | `[1..*]` | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
| [Agent](#rollenzuordnung-agent) | `prov:agent` | [`prov:Agent`](https://www.w3.org/TR/prov-o/#Agent) | <small>Pflicht</small> | `[1..*]` | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |


<br>
<hr>
<br>

###  Rollenzuordnung: Hatte Rolle {#rollenzuordnung-rolle}
> | *URI*                      | [`dcat:hadRole`](http://www.w3.org/ns/dcat#hadRole) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`dcat:Role`](http://www.w3.org/ns/dcat#Role) |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1..*]`                   |
> | Beschreibung               | Beschreibt die Funktion, die Agenten in Bezug auf eine Ressource hatten. |
> | Weiterführende Dokumentationen | [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Property:relationship_hadRole)  | 
> | Interoperabilitätslevel    | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
> | Änderungen durch DCAT-AP.de | Von DCAT-AP.de eingeführte Eigenschaft. | 
<br>

###  Rollenzuordnung: Agent {#rollenzuordnung-agent}
> | *URI*                      | [`prov:agent`](http://www.w3.org/ns/prov#agent) |
> |:---------------------------|:-------------------------------------------|
> | Wertebereich               | [`prov:Agent`](https://www.w3.org/TR/prov-o/#Agent) |
> | Verbindlichkeit            | Pflicht |
> | Multiplizität              | `[1..*]`                   |
> | Beschreibung               | Die Eigenschaft referenziert auf einen `prov:Agent`, der eine Ressource beeinflusst hat.  |
> | Weiterführende Dokumentationen | [PROV-O](https://www.w3.org/TR/prov-o/#p_agent)  | 
> | Interoperabilitätslevel    | <abbr title='Profilspezifisch hinzugefügt.'>P</abbr> |
> | Änderungen durch DCAT-AP.de | Von DCAT-AP.de eingeführte Eigenschaft. | 
<br>



***


