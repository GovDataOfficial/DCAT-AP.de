### Deprecated Elemente entfernen

Die folgenden Eigenschaften sind in Version 2.0 als _deprecated_ gekennzeichnet gewesen und werden daher entfernt:

**dcat:Distribution**
 - [dcatde:plannedAvailability](https://www.dcat-ap.de/def/dcatde/2.0/spec/#distribution-verfugbarkeit-deprecated)

**dcterms:PeriodOfTime**
 - [schema:startDate](https://www.dcat-ap.de/def/dcatde/2.0/spec/#zeitraum-startzeitpunkt)
 - [schema:endDate](https://www.dcat-ap.de/def/dcatde/2.0/spec/#zeitraum-endzeitpunkt)

**dcat:Dataset**
 - [dcat:granularity](https://www.dcat-ap.de/def/dcatde/2.0/spec/#datensatz-abgedeckte-zeitliche-granularitat-deprecated)
 - [dcterms:hasVersion](https://www.dcat-ap.de/def/dcatde/2.0/spec/#datensatz-weitere-version); bleibt als Eigenschaft zwar erhalten, wird aber nicht mehr für Collections verwendet.
 - [dcterms:type](https://www.dcat-ap.de/def/dcatde/2.0/spec/#datensatz-typ) (mit datasetTypes/collection); bleibt als Eigenschaft zwar erhalten, wird aber nicht mehr für Collections verwendet.

**Codelisten**
Die folgenden Codelisten sind in Version 2.0 als _deprecated_ gekennzeichnet gewesen und werden daher entfernt:

 - [Liste der zugesicherten Verfügbarkeiten](https://www.dcat-ap.de/def/dcatde/2.0/spec/#kv-planned-availability)
 - [Liste der Datenstrukturtypen](https://www.dcat-ap.de/def/dcatde/2.0/spec/#kv-dataset-type)

### Kontrolliertes Vokabular für Prüfsummen

SPDX stellt inzwischen eine umfangreiche Liste an möglichen Hash-Algorithmen zur Verfügung. Diese Liste soll künftig statt der selbst veröffentlichen Liste verwendet werden.

Die von GovData gepflegte [Liste der Algorithmen](#kv-hash-algorithms-deprecated) wurde daher als _deprecated_ gekennzeichnet und die [SPDX-Liste der Algorithmen](#kv-hash-algorithms) wurde aufgenommen.

### Kontrolliertes Vokabular für Zugriffsrechte

Das [EU Vokabular "Access Right"](#kv-access-right) wurde zum Standard hinzugefügt. Es wird für die Eigenschaft `dcterms:accessRights` in [dcat:Dataset](#datensatz-grad-zuganglichkeit) und [dcat:DataService](#datenservice-grad-zuganglichkeit) verwendet.

### Kontrolliertes Vokabular für den Status einer Distribution

Das [EU Vokabular "Distribution Status"](#kv-distribution-status) wurde zum Standard hinzugefügt. Es ersetzt für die Eigenschaft `adms:status` in [dcat:Distribution](#distribution-status) die nun als _deprecated_ gekennzeichnete [Liste aus der ADMS-Spezifikation](#kv-adms-status).

### Namespaces

Das Namespace-Prefix von DC Terms wurde von `dct` auf `dcterms` geändert.

### Strukturelle Anpassungen an DCAT-AP 3.0

DCAT-AP 3.0 beschreibt Eigenschaften über "Definition" und "Usage". DCAT-AP.de folgt diesem Vorgehen und splittet die bisherigen "Beschreibung" in "Beschreibung" und "Verwendungshinweis" auf.

Darüber hinaus wird für jede Eigenschaft nun ein "Interoperabilitätslevel" angegeben.

### Ausblenden von Klassen

Die Klassen "Kategorie" (`skos:Concept`) und "Kategorienschema" (`skos:ConceptScheme`) werden nicht mehr beschrieben, da sie exklusiv mit einem EU Vokabular verwendet werden sollen. Zudem ist die Nutzung von (`skos:Concept`) nur als "Kategorie" verwirrend/falsch, da auch andere Eigenschaften als Wertebereich `skos:Concept` haben.

Auch die Klasse "Lizenzdokument" (`dcterms:LicenceType`) soll immer mit einem kontrollierten Vokabular verwendet werden und wird daher nicht weiter beschrieben.

Details beschreibt das Kapitel [Überblick über das DCAT-AP.de Modell](#ueberblick-datenmodell).

---