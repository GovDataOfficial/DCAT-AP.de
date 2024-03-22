## Klasse: Ressource
Die Klasse [`dcat:Resource`](https://www.w3.org/TR/vocab-dcat-2/#Class:Resource), die in der Version 2.0 von DCAT eingeführt wurde, ist die Super-Klasse von [`dcat:Dataset`](#klasse-datensatz) und [`dcat:DataService`](#klasse-datenservice).
Dadurch, dass [`dcat:Catalog`](#klasse-katalog) zudem eine Sub-Klasse von [`dcat:Dataset`](#klasse-datensatz) ist, vererbt `dcat:Resource` seine Eigenschaften auch auf den [`dcat:Catalog`](#klasse-katalog).


DCAT-AP.de 1.1 erweiterte das `dcat:Dataset` um die Eigenschaften [`dcatde:contributorID`](#datensatz-datenbereitsteller-id), [`dcatde:qualityProcessURI`](#datensatz-qualitatssicherungsprozess), [`dcatde:originator`](#datensatz-urheber), [`dcatde:maintainer`](#datensatz-verwalter), [`dcatde:politicalGeocodingLevelURI`](#datensatz-ebene-geopolitischen-abdeckung), [`dcatde:politicalGeocodingURI`](#datensatz-geopolitischen-abdeckung), [`dcatde:geocodingDescription`](#datensatz-beschreibung-abdeckung), [`dcatde:legalBasis`](#datensatz-rechtsgrundlage-zugangseroffnung) und [`dct:contributor`](#datensatz-bearbeiter).​
<br>Für die Version 2.0 wurde entschieden, diese Eigenschaften künftig der `dcat:Resource` zuzuordnen.


Abweichend von DCAT-AP wurde entschieden, die Eigenschaft [`dcatap:availability`](#datensatz-verfugbarkeit) der `dcat:Resource` zuzuordnen.
Darüber hinaus wurde die Eigenschaft [`dct:references`](#datensatz-referenziert) in DCAT-AP.de 2.0 neu hinzugefügt.


Daraus ergibt sich die folgende Übersicht:

<small>

| Eigenschaften vom W3C-DCAT |                             | Eigenschaften von DCAT-AP.de        |
| -------------------------- | --------------------------- | ----------------------------------- |
| `dcat:contactPoint`        | `dct:issued`                | `dcatap:availability`               |
| `dcat:keyword`             | `dct:language`              | `dcatde:contributorID`              |
| `dcat:landingPage`         | `dct:license`               | `dcatde:geocodingDescription`       |
| `dcat:qualifiedRelation`   | `dct:modified`              | `dcatde:legalBasis`                 |
| `dcat:theme`               | `dct:publisher`             | `dcatde:maintainer`                 |
| `dct:accessRights`         | `dct:relation`              | `dcatde:originator`                 |
| `dct:conformsTo`           | `dct:rights`                | `dcatde:politicalGeocodingLevelURI` |
| `dct:creator`              | `dct:title`                 | `dcatde:politicalGeocodingURI`      |
| `dct:description`          | `dct:type`                  | `dcatde:qualityProcessURI`          |
| `dct:identifier`           | `odrl:hasPolicy`            | `dct:contributor`                   |
| `dct:isReferencedBy`       | `prov:qualifiedAttribution` | `dct:references`                    |

</small>
