# Kontrollierte Vokabulare 

Durch die Profilbildung und Einbeziehung von DCAT, DCAT-AP und DCAT-AP.de sind obligatorische und optionale Vokabulare auf unterschiedlicher Ebene zu berücksichtigen. Die folgenden Kapitel führen, neben Anforderungen an den Entwurf und Betrieb von Vokabularen, konkrete Wertelisten aus dem Geltungsbereich DCAT (ADMS, Dublin Core), DCAT-AP und DCAT-AP.de auf

__Anforderungen an kontrollierte Vokabulare__

Die nachfolgende Liste beschreibt [Anforderungen](28), die für neue kontrollierte Vokabulare in diesem Application Profile oder bei Erweiterungen auf kommunaler und Landesebene berücksichtigt werden sollten. 
Das kontrollierte Vokabular sollte:
 -	unter einer offenen Lizenz veröffentlicht sein,
 -	von einer Institution der Europäischen Union – „Recognised Standards Organisation“ oder einer anderen vertrauenswürdigen Instanz – gepflegt werden,
 - ausreichend dokumentiert sein,
 - mehrsprachige Beschreibungen haben (idealerweise sollten alle offiziell in der Europäischen Union vertretenen Sprachen prinzipiell unterstützt werden),
 - eine relativ geringe Anzahl von Begriffen beinhalten (10-25), die allgemein genug sind, um eine Vielzahl von Ressourcen zu klassifizieren,
 - verwendete Begriffe durch „URIs“ identifizieren, wobei die jeweilige URI zu einer Dokumentation des verwendeten Begriffs führt, und
 - assoziierte Persistenz- und Versionierungsregeln besitzen.

__Vokabulare zur Nutzung (DCAT-AP.de)__

In den folgenden Unterkapiteln findet sich eine Auflistung von kontrollierten Vokabularen, welche zum Erhalt der DCAT-AP.de-Konformität unterstützt werden müssen.
Ihre Verwendung sichert ein minimales Level an Interoperabilität. Ebenfalls wird aufgeführt, mit welcher Verbindlichkeit das jeweilige Vokabular genutzt werden muss, sofern die entsprechende Eigenschaft (z.B. dcterms:accrualPeriodicity) verwendet wird.


## Liste der GovData Datenbereitsteller {#kv-contributors}
Liste der unmittelbar an GovData anliefernden Systeme. Diese Datenbereitsteller sind im engeren Sinne Metadatenbereitsteller, für den Bezug der eigentlichen Open Data Daten wird auf das „Originalportal“ verwiesen.

> | Betroffene Eigenschaften       | [`dcatde:contributorID`](#datensatz-datenbereitsteller-id) |
> |:-------------------------------|:-----------------------|
> | Verbindlichkeit Vokabular      | Optional               |
> | Verwendung in Klassen          | [`dcat:Dataset`](#datensatz-datenbereitsteller-id) |
> | Menschenlesbare Ansicht        | http://dcat-ap.de/def/contributors/   |
> | Basis-URI                      | `http://dcat-ap.de/def/contributors/` |
> | Beispiel                       | `<http://dcat-ap.de/def/contributors/tranzparenzportalHamburg>` |


## Liste der Lizenzen {#kv-licenses}
Liste der Lizenzen, die im Feld dcterms:license einer DCAT-AP.de-konformen dcat:distribution für die Zulieferung an GovData erlaubt sind. GovData empfiehlt die Verwendung der Datenlizenz Deutschland 2.0 (Zero oder Namensnennung) sowie der Creative Commons Namensnennung – 4.0 International. Soweit dies nicht möglich sein sollte, wird die Verwendung einer der übrigen zur „freien Nutzung“ ausgewiesenen Lizenzen in der jeweils neuesten Version empfohlen.

Kontaktieren Sie zur Aufnahme neuer Lizenzen bitte die Geschäfts- und Koordinierungsstelle GovData: info@govdata.de.

> | Betroffene Eigenschaften       | [`dcterms:license`](#distribution-lizenz) |
> |:-------------------------------|:----------------------------------|
> | Verbindlichkeit Vokabular      | Empfohlen                         |
> | Verwendung in Klassen          | [`dcat:Distribution`](#distribution-lizenz), [`dcat:Catalog`](#katalog-lizenz)   |
> | Menschenlesbare Ansicht        | http://dcat-ap.de/def/licenses/   |
> | Basis-URI                      | `http://dcat-ap.de/def/licenses/` |
> | Beispiel                       | `<http://dcat-ap.de/def/licenses/dl-by-de/2.0/>` |


## Liste der Ebene für die geopolitische Kodierung {#kv-political-geocoding-level}
Zur kodierten Angabe der jeweiligen prinzipiellen Verwaltungsebene, von der der Datensatz erhoben und eingestellt wurde.

> | Betroffene Eigenschaften       | [`dcatde:politicalGeocodingLevel`](#datensatz-ebene-geopolitischen-abdeckung) |
> |:-------------------------------|:---------------------------------|
> | Verbindlichkeit Vokabular      | Empfohlen                        |
> | Verwendung in Klassen          | [`dcat:Dataset`](#datensatz-ebene-geopolitischen-abdeckung) |
> | Menschenlesbare Ansicht        | http://dcat-ap.de/def/politicalGeocoding/Level/            |
> | Basis-URI                      | `http://dcat-ap.de/def/politicalGeocoding/Level/`          |
> | Beispiel                       | `<http://dcat-ap.de/def/politicalGeocoding/Level/federal>` |


## Listen für Gemeindeschlüssel, Regionalschlüssel, Gemeindeverband, Kreis, Bezirk und Bundesland {#kv-political-geocoding-uri}
Die einzelnen Listen basieren auf offiziellen Listen, die im [XRepository](https://www.xrepository.de/) veröffentlicht werden. Für die Referenzierung des verwaltungspolitischen Geobezugs kann auf folgende Wertelisten zurückgegriffen werden:

1. Gemeindeschlüssel
2. Regionalschlüssel
3. Gemeindeverband
4. Kreis
5. Bezirk
6. Bundesland

Gemeinden können mit dem Gemeindeschlüssel oder dem Regionalschlüssel referenziert werden. Gemeindeverbände, Kreise, Bezirke und Bundesländer mit Schlüsseln aus ihrer jeweiligen Liste. Welche Liste den Geobezug eines Datensatzes am besten abbildet, ist eine fachliche Entscheidung des Datenbereitstellers. 


> | Betroffene Eigenschaften       | [`dcatde:politicalGeocodingURI`](#datensatz-geopolitischen-abdeckung) |
> |:-------------------------------|:-------------------------------|
> | Verbindlichkeit Vokabular      | Empfohlen                      |
> | Verwendung in Klassen          | [`dcat:Dataset`](#datensatz-geopolitischen-abdeckung) |
> | Menschenlesbare Ansichten      | http://dcat-ap.de/def/politicalGeocoding/municipalityKey/ <br> http://dcat-ap.de/def/politicalGeocoding/regionalKey/ <br> http://dcat-ap.de/def/politicalGeocoding/municipalAssociationKey/ <br> http://dcat-ap.de/def/politicalGeocoding/districtKey/ <br> http://dcat-ap.de/def/politicalGeocoding/governmentDistrictKey/ <br> http://dcat-ap.de/def/politicalGeocoding/stateKey/ |
> | Basis-URIs                     | `http://dcat-ap.de/def/politicalGeocoding/municipalityKey/` <br> `http://dcat-ap.de/def/politicalGeocoding/regionalKey/` <br> `http://dcat-ap.de/def/politicalGeocoding/municipalAssociationKey/` <br> `http://dcat-ap.de/def/politicalGeocoding/districtKey/` <br> `http://dcat-ap.de/def/politicalGeocoding/governmentDistrictKey/` <br> `http://dcat-ap.de/def/politicalGeocoding/stateKey/` |
> | Beispiele                      | Borgsum: `<http://dcat-ap.de/def/politicalGeocoding/municipalityKey/01054015>` <br> Halle (Saale): `<http://dcat-ap.de/def/politicalGeocoding/regionalKey/15002000000>` <br> Bornhöved: `<http://dcat-ap.de/def/politicalGeocoding/municipalAssociationKey/010605024>` <br> Main-Tauber-Kreis: `<http://dcat-ap.de/def/politicalGeocoding/districtKey/08128>` <br> Mittelfranken: `<http://dcat-ap.de/def/politicalGeocoding/governmentDistrictKey/095>` <br> Hamburg: `<http://dcat-ap.de/def/politicalGeocoding/stateKey/02>` |


## SPDX-Liste der Algorithmen {#kv-hash-algorithms}
Mit DCAT-AP.de 3.0 wird empfohlen, den verwendeten Algorithmus mittels der URI anzugeben, die von SPDX vorgegeben wird.

> | Betroffene Eigenschaften       | [`spdx:algorithm`](#prufsumme-algorithmus) |
> |:-------------------------------|:-------------------------|
> | Verbindlichkeit Vokabular      | Optional                 |
> | Verwendung in Klassen          | [`spdx:Checksum`](#prufsumme-algorithmus)           |
> | Menschenlesbare Ansicht        | https://spdx.org/rdf/terms/#d4e2129                 |
> | Basis-URI                      | `http://spdx.org/rdf/terms#checksumAlgorithm_`      |
> | Beispiel                       | `<http://spdx.org/rdf/terms#checksumAlgorithm_md5>` |


## Liste der Algorithmen (DEPRECATED) {#kv-hash-algorithms-deprecated}
Diese Liste ist eine Erweiterung von Algorithmen, die durch SPDX veröffentlich werden.

> | Betroffene Eigenschaften       | [`spdx:algorithm`](#prufsumme-algorithmus) |
> |:-------------------------------|:-------------------------|
> | Verbindlichkeit Vokabular      | Optional                 |
> | Verwendung in Klassen          | [`spdx:Checksum`](#prufsumme-algorithmus)      |
> | Menschenlesbare Ansicht        | http://dcat-ap.de/def/hashAlgorithms/          |
> | Basis-URI                      | `http://dcat-ap.de/def/hashAlgorithms/`        |
> | Beispiel                       | `<http://dcat-ap.de/def/hashAlgorithms/md/5/>` |


## Liste der zugesicherten Verfügbarkeiten {#kv-availability}
Diese Verfügbarkeitsgrade geben an, wie lange geplant ist, das Dokument verfügbar zu halten.

> | Betroffene Eigenschaften       | [`dcatap:availability`](#distribution-verfugbarkeit) |
> |:-------------------------------|:-----------------------------|
> | Verbindlichkeit Vokabular      | Pflicht                      |
> | Verwendung in Klassen          | [`dcat:Distribution`](#distribution-verfugbarkeit), [`dcat:Dataset`](#datensatz-verfugbarkeit), [`dcat:DataService`](#datenservice-verfugbarkeit), [`dcat:Catalog`](#katalog-verfugbarkeit) |
> | Menschenlesbare Ansicht        | https://op.europa.eu/en/web/eu-vocabularies/dataset/-/resource?uri=http://publications.europa.eu/resource/dataset/planned-availability|
> | Basis-URI                      | `http://publications.europa.eu/resource/authority/planned-availability/` |
> | Beispiel                       | `<http://publications.europa.eu/resource/authority/planned-availability/AVAILABLE>` |


## EU Vokabular "Frequency" {#kv-frequency}
Diese Tabelle enthält die mögliche Aktualisierungsfrequenzen (-häufigkeiten) in den 24 Amtssprachen der Europäischen Union.

> | Betroffene Eigenschaften       | [`dcterms:accrualPeriodicity`](#datensatz-aktualisierungsfrequenz) |
> |:-------------------------------|:----------------------------------|
> | Verbindlichkeit Vokabular      | Pflicht                           |
> | Verwendung in Klassen          | [`dcat:Dataset`](#datensatz-aktualisierungsfrequenz) |
> | Menschenlesbare Ansicht        | [EU Vocabularies: frequency](https://op.europa.eu/de/web/eu-vocabularies/dataset/-/resource?uri=http://publications.europa.eu/resource/dataset/frequency) |
> | Basis-URI                      | `http://publications.europa.eu/resource/authority/frequency/`            |
> | Beispiel                       | `<http://publications.europa.eu/resource/authority/frequency/BIMONTHLY>` |


## EU Vokabular "Languages" {#kv-languages}
> | Betroffene Eigenschaften       | [`dcterms:language`](#datensatz-sprache)                  |
> |:-------------------------------|:--------------------------------|
> | Verbindlichkeit Vokabular      | Pflicht                         |
> | Verwendung in Klassen          | [`dcat:Dataset`](#datensatz-sprache), [`dcat:Catalog`](#katalog-sprache), [`dcat:CatalogRecord`](#katalogeintrag-sprache), [`dcat:Distribution`](#distribution-sprache) |
> | Menschenlesbare Ansicht        | [EU Vocabularies: languages](https://op.europa.eu/de/web/eu-vocabularies/concept-scheme/-/resource?uri=http://publications.europa.eu/resource/authority/language) |
> | Basis-URI                      | `http://publications.europa.eu/resource/authority/language/`      |
> | Beispiel                       | `<http://publications.europa.eu/resource/authority/language/DEU>` |


## EU Vokabulare "Continents", "Countries", "Places" & Geonames {#kv-spatial}
Die "EU Name Authority Tables" müssen für Kontinente, Länder oder Plätze verwendet werden, die explizit in einer der Listen aufgeführt sind. Wenn ein Ort nicht namentlich in einer der "EU Name Authority Tables" benannt ist, müssen Geonames URIs verwendet werden.

Wenn das abgedeckte Gebiet stattdessen durch eine Geometrie repräsentiert werden soll, so ist dies mittels des Core Location Vocabularies entspreched dem Vorgehen in GeoDCAT (https://joinup.ec.europa.eu/sites/default/files/distribution/2016-08/geodcat-ap_v1.0.1.pdf) zu lösen.

Weitere Details und Beispiele finden Sie im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#angaben-zur-geografischen-abdeckung).

> | Betroffene Eigenschaften       | [`dcterms:spatial`](#datensatz-raumliche-abdeckung)                   |
> |:-------------------------------|:--------------------------------|
> | Verbindlichkeiten Vokabular    | Pflicht                         |
> | Verwendung in Klassen          | [`dcat:Dataset`](#datensatz-raumliche-abdeckung), [`dcat:Catalog`](#katalog-raumliche-abdeckung), tbd |
> | Menschenlesbare Ansichten      | [EU Vocabularies: continent](https://op.europa.eu/de/web/eu-vocabularies/concept-scheme/-/resource?uri=http://publications.europa.eu/resource/authority/continent) <br> [EU Vocabularies: country](https://op.europa.eu/de/web/eu-vocabularies/concept-scheme/-/resource?uri=http://publications.europa.eu/resource/authority/country) <br> [EU Vocabularies: place](https://op.europa.eu/de/web/eu-vocabularies/concept-scheme/-/resource?uri=http://publications.europa.eu/resource/authority/place) <br> https://sws.geonames.org/ |
> | Basis-URIs                     | `http://publications.europa.eu/resource/authority/continent/` <br> `http://publications.europa.eu/resource/authority/country/` <br> `http://publications.europa.eu/resource/authority/place/` <br> `http://sws.geonames.org/` |
> | Beispiele                      | Europa: `<http://publications.europa.eu/resource/authority/continent/EUROPE>` <br> Finnland: `<http://publications.europa.eu/resource/authority/country/FIN>` <br> Würzburg: `<http://publications.europa.eu/resource/authority/place/DEU_WUE>` <br> Deutschland: `<http://sws.geonames.org/2921044/>` |


## EU Vokabular "Dataset Type" {#kv-dataset-type}
> | Betroffene Eigenschaften       | [`dcterms:type`](#datensatz-typ) |
> |:-------------------------------|:-------------------------|
> | Verbindlichkeit Vokabular      | Optional                 |
> | Verwendung in Klassen          | [`dcat:Dataset`](#datensatz-typ) |
> | Menschenlesbare Ansicht        | [EU Vocabularies: dataset-type](https://op.europa.eu/de/web/eu-vocabularies/concept-scheme/-/resource?uri=http://publications.europa.eu/resource/authority/dataset-type) |
> | Basis-URI                      | `http://publications.europa.eu/resource/authority/dataset-type/` |
> | Beispiel                       | Statistische Daten: `<http://publications.europa.eu/resource/authority/dataset-type/STATISTICAL>` |


## EU Vokabular "Data Theme" {#kv-data-theme}
> | Betroffene Eigenschaften       | [`dcat:theme`](#datensatz-kategorie) |
> |:-------------------------------|:-------------------------|
> | Verbindlichkeit Vokabular      | Pflicht                  |
> | Verwendung in Klassen          | [`dcat:Dataset`](#datensatz-kategorie) |
> | Menschenlesbare Ansicht        | [EU Vocabularies: data-theme](https://op.europa.eu/de/web/eu-vocabularies/concept-scheme/-/resource?uri=http://publications.europa.eu/resource/authority/data-theme) |
> | Basis-URI                      | `http://publications.europa.eu/resource/authority/data-theme/`                   |
> | Beispiel                       | Gesundheit: `<http://publications.europa.eu/resource/authority/data-theme/HEAL>` |


## EU Vokabular "Access Right" {#kv-access-right}
Die Access right authority table ist ein kontrolliertes Vokabular, in dem die Zugriffsrechte oder -beschränkungen auf Ressourcen aufgeführt sind. Sie ist für DCAT-Beschreibungen von Datensätzen gedacht, aber nicht auf diese beschränkt.

> | Betroffene Eigenschaften       | [`dcterms:accessRights`](#datensatz-grad-zuganglichkeit) |
> |:-------------------------------|:-------------------------|
> | Verbindlichkeit Vokabular      | Pflicht                  |
> | Verwendung in Klassen          | [dcat:Dataset](#datensatz-grad-zuganglichkeit),  [dcat:DataService](#datenservice-grad-zuganglichkeit) |
> | Menschenlesbare Ansicht        | [EU Vocabularies: access-right](https://op.europa.eu/de/web/eu-vocabularies/dataset/-/resource?uri=http://publications.europa.eu/resource/dataset/access-right) |
> | Basis-URI                      | `http://publications.europa.eu/resource/authority/access-right/`                    |
> | Beispiel                       | Öffentlich:  `http://publications.europa.eu/resource/authority/access-right/PUBLIC` |
> | Verwendungsnotiz               | Folgende Werte sollen verwendet werden: <br> `PUBLIC` <br> `RESTRICTED` <br> `NON_PUBLIC` |

## EU Vokabular "File Type" {#kv-file-type}
Die File type authority table ist ein kontrolliertes Vokabular, in dem die verschiedenen Arten von (digitalen) Dateien (z. B. PDF, XML, DOC, ...) aufgeführt sind. Die File type authority table wird vom Interinstitutional Metadata Maintenance Committee (IMMC) verwaltet und vom Amt für Veröffentlichungen der Europäischen Union auf der Website EU Vocabularies gepflegt. 
Fehlende Dateitypen können und müssen über die Funktion ["BEITRAGEN" ("CONTRIBUTE")](https://op.europa.eu/de/web/eu-vocabularies/concept-scheme/-/resource?uri=http://publications.europa.eu/resource/authority/file-type) der Liste hinzugefügt werden.
Weitere Details und Beispiele finden Sie im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#angaben-zu-dateiformaten)

> | Betroffene Eigenschaften       | [`dcterms:format`](#distribution-format) |
> |:-------------------------------|:-------------------------|
> | Verbindlichkeit Vokabular      | Pflicht                  |
> | Verwendung in Klassen          | [dcat:Distribution](#distribution-format) |
> | Menschenlesbare Ansicht        | [EU Vocabularies: file-type](https://op.europa.eu/de/web/eu-vocabularies/concept-scheme/-/resource?uri=http://publications.europa.eu/resource/authority/file-type) |
> | Basis-URI                      | `http://publications.europa.eu/resource/authority/file-type/`            |
> | Beispiel                       | CSV:  `http://publications.europa.eu/resource/authority/file-type/CSV` |


## IANA Vokabular "Media Types" {#kv-iana-media-types}
Die von DCAT eingeführten Eigenschaften zur Angabe des Fomats im weiteren Sinne, verwenden die IANA-Liste als kontrolliertes Vokabular.
Auch hier können fehlende Einträge bei Bedarf eingetragen werden: https://www.iana.org/form/media-types

> | Betroffene Eigenschaften       | [`dcat:mediaType`](#distribution-medientyp) <br> [`dcat:compressFormat`](#distribution-kompressionsformat) <br> [`dcat:packageFormat`](#distribution-paketformat) |
> |:-------------------------------|:-------------------------|
> | Verbindlichkeit Vokabular      | Pflicht                  |
> | Verwendung in Klassen          | [`dcat:Distribution`](#distribution-medientyp) |
> | Menschenlesbare Ansicht        | https://www.iana.org/assignments/media-types/media-types.xhtml        |
> | Basis-URI                      | `https://www.iana.org/assignments/media-types/`                       |
> | Beispiel                       | ZIP: `<https://www.iana.org/assignments/media-types/application/pdf>` |


## EU Vokabular "Distribution Status" {#kv-distribution-status}
Die Liste der möglichen Status wurde aus der ADMS-Spezifikation herausgelöste und ins Publication Office überführte.

> | Betroffene Eigenschaften       | [`adms:status` ](#distribution-status) |
> |:-------------------------------|:---------------------------------------|
> | Verbindlichkeit Vokabular      | Pflicht                                |
> | Verwendung in Klassen          | [`dcat:Distribution`](#distribution-status) |
> | Menschenlesbare Ansicht        | [EU Vocabularies: distribution-status](https://op.europa.eu/de/web/eu-vocabularies/concept-scheme/-/resource?uri=http://publications.europa.eu/resource/authority/distribution-status) |
> | Basis-URI                      | `http://publications.europa.eu/resource/authority/distribution-status/` |
> | Beispiel                       | Vollständig:  `http://publications.europa.eu/resource/authority/distribution-status/COMPLETED` |


## ADMS Vokabular "Status Type" (DEPRECATED) {#kv-adms-status}
Die ADMS-Spezifikation enthält die Liste von Begriffen im ADMS „Status“-Vokabular.

> | Betroffene Eigenschaften       | [`adms:status` ](#distribution-status) |
> |:-------------------------------|:-------------------------------|
> | Verbindlichkeit Vokabular      | Pflicht                        |
> | Verwendung in Klassen          | [`dcat:Distribution`](#distribution-status) |
> | Menschenlesbare Ansicht        | -                              |
> | Basis-URI                      | `http://purl.org/adms/status/` |
> | Verwendungsnotiz               | Folgende Werte werden unterstützt: <br> `<http://purl.org/adms/status/Completed>` <br> `<http://purl.org/adms/status/Deprecated>` <br> `<http://purl.org/adms/status/Withdrawn>` |


## ADMS Vokabular "Publisher Type" {#kv-adms-publisher}
Die ADMS Spezifikation enthält die Liste von Begriffen im ADMS „Publisher Type“-Vokabular. Eine Auswahl (local = Kommunalebene, regional = Landesebene, national = Bundesebene und supranational) ist im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#angaben-zum-herausgeber) angegeben.

> | Betroffene Eigenschaften       | [`dcterms:type`](#verantwortliche-stelle-typ) |
> |:-------------------------------|:-----------------------------|
> | Verbindlichkeit Vokabular      | Pflicht                      |
> | Verwendung in Klassen          | [`foaf:Agent`](#verantwortliche-stelle-typ) |
> | Menschenlesbare Ansicht        | -                            |
> | Basis-URI                      | `http://purl.org/adms/publishertype/` |


## ADMS Vokabular "Licence Type" {#kv-adms-licencetype}
Die Liste von Begriffen des ADMS „Licence Type“-Vokabulars ist in der ADMS Spezifikation angegeben. 
DCAT-AP.de Anwendungshinweis: Die ADMS-Taxonomie wird für volle dcat-ap Konformität unterstützt. Für die Kommunikation im GovData Verbund dürfen jedoch keine selbst modellierten Lizenzen verwendet werden. Stattdessen ist [das entsprechende kontrollierte Vokabular](#kv-licenses) zu verwenden. 

Weitere Details und Beispiele finden Sie im [Konventionenhandbuch](https://www.dcat-ap.de/def/dcatde/2.0/implRules/#angaben-zur-lizenz-und-zu-rechten-insb-dct-license).

> | Betroffene Eigenschaften       | [`dcterms:type`](http://purl.org/dc/terms/type) |
> |:-------------------------------|:-----------------------|
> | Verbindlichkeit Vokabular      | Optional               |
> | Verwendung in Klassen          | [`dcterms:LicenseDocument`](https://dublincore.org/specifications/dublin-core/dcmi-terms/#LicenseDocument) |
> | Menschenlesbare Ansicht        | -                      |
> | Basis-URI                      | `http://purl.org/adms/licencetype/` |
