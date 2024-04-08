### Deprecated Elemente entfernen

Die folgenden Eigenschaften sind in Version 2.0 als _deprecated_ gekennzeichnet gewesen und werden daher entfernt:

**dcat:Distribution**
 - [dcatde:plannedAvailability](https://www.dcat-ap.de/def/dcatde/2.0/spec/#distribution-verfugbarkeit-deprecated)

**dct:PeriodOfTime**
 - [schema:startDate](https://www.dcat-ap.de/def/dcatde/2.0/spec/#zeitraum-startzeitpunkt)
 - [schema:endDate](https://www.dcat-ap.de/def/dcatde/2.0/spec/#zeitraum-endzeitpunkt)

**dcat:Dataset**
 - [dcat:granularity](https://www.dcat-ap.de/def/dcatde/2.0/spec/#datensatz-abgedeckte-zeitliche-granularitat-deprecated)
 - [dct:hasVersion](https://www.dcat-ap.de/def/dcatde/2.0/spec/#datensatz-weitere-version); bleibt als Eigenschaft zwar erhalten, wird aber nicht mehr für Collections verwendet.
 - [dct:type](https://www.dcat-ap.de/def/dcatde/2.0/spec/#datensatz-typ) (mit datasetTypes/collection); bleibt als Eigenschaft zwar erhalten, wird aber nicht mehr für Collections verwendet.

**Codelisten**
Die folgenden Codelisten sind in Version 2.0 als _deprecated_ gekennzeichnet gewesen und werden daher entfernt:

 - [Liste der zugesicherten Verfügbarkeiten](https://www.dcat-ap.de/def/dcatde/2.0/spec/#kv-planned-availability)
 - [Liste der Datenstrukturtypen](https://www.dcat-ap.de/def/dcatde/2.0/spec/#kv-dataset-type)

### Kontrolliertes Vokabular für Prüfsummen

SPDX stellt inzwischen eine umfangreiche Liste an möglichen Hash-Algorithmen zur Verfügung. Diese Liste soll künftig statt der selbst veröffentlichen Liste verwendet werden.

Die von GovData gepflegte [Liste der Algorithmen](#kv-hash-algorithms-deprecated) wurde daher als _deprecated_ gekennzeichnet und die [SPDX-Liste der Algorithmen](#kv-hash-algorithms) wurde aufgenommen.

### Kontrolliertes Vokabular für Zugriffsrechte

Das [EU Vokabular "Access Right"](#kv-access-right) wurde zum Standard hinzugefügt. Es wird für die Eigenschaft `dct:accessRights` in [dcat:Dataset](#datensatz-grad-zuganglichkeit) und [dcat:DataService](#datenservice-grad-zuganglichkeit) verwendet.

---