## Klasse: Ressource

> | *URI der Klasse*   | [`dcat:Resource`](https://www.w3.org/ns/dcat#Resource)                           |
> |:-------------------|:---------------------------------------------------------------------------------|
> | Beschreibung       | Ressource, die von einem einzelnen Akteur veröffentlicht oder kuratiert wurde.   |
> | Verwendungshinweis | In DCAT-AP und DCAT-AP.de ist dies eine abstrakte Klasse. Sie sollte nicht direkt verwendet werden, sondern ihre Sub-Klassen.   |
> | Weiterführende Dokumentationen | [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#CataloguedResource), [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Class:Resource) |

<br>

DCAT-AP.de 1.1 erweiterte das `dcat:Dataset` um die Eigenschaften [`dcatde:contributorID`](#datensatz-datenbereitsteller-id), [`dcatde:qualityProcessURI`](#datensatz-qualitatssicherungsprozess), [`dcatde:originator`](#datensatz-urheber), [`dcatde:maintainer`](#datensatz-verwalter), [`dcatde:politicalGeocodingLevelURI`](#datensatz-ebene-geopolitischen-abdeckung), [`dcatde:politicalGeocodingURI`](#datensatz-geopolitischen-abdeckung), [`dcatde:geocodingDescription`](#datensatz-beschreibung-abdeckung), [`dcatde:legalBasis`](#datensatz-rechtsgrundlage-zugangseroffnung) und [`dcterms:contributor`](#datensatz-bearbeiter). Für die Version 2.0 wurde entschieden, diese Eigenschaften künftig der `dcat:Resource` zuzuordnen.

Abweichend von DCAT-AP wurde entschieden, die Eigenschaft [`dcatap:availability`](#datensatz-verfugbarkeit) der `dcat:Resource` zuzuordnen.
Darüber hinaus wurde die Eigenschaft [`dcterms:references`](#datensatz-referenziert) in DCAT-AP.de 2.0 neu hinzugefügt.

Daraus ergibt sich die folgende Übersicht an Eigenschaften für die Super-Klasse `dcat:Resource`:

<small>

| Eigenschaften                   | vom W3C-DCAT              |                              | Eigenschaften von DCAT-AP.de          |
| ------------------------------- | ------------------------- | ---------------------------- | ------------------------------------- |
| `adms:status`&nbsp;+            | `dcat:qualifiedRelation`  | `dcterms:language`           | `dcatap:availability`                 |
| `adms:versionNotes`&nbsp;+      | `dcat:theme`              | `dcterms:license`            | `dcatde:contributorID`                |
| `dcat:contactPoint`             | `dcat:version`&nbsp;+     | `dcterms:modified`           | `dcatde:geocodingDescription`&nbsp;-  |
| `dcat:first`&nbsp;+             | `dcterms:accessRights`    | `dcterms:publisher`          | `dcatde:legalBasis`&nbsp;-            |
| `dcat:hasCurrentVersion`&nbsp;+ | `dcterms:conformsTo`      | `dcterms:relation`           | `dcatde:maintainer`&nbsp;-            |
| `dcat:hasVersion`&nbsp;+        | `dcterms:creator`         | `dcterms:replaces`&nbsp;+    | `dcatde:originator`&nbsp;-            |
| `dcat:keyword`                  | `dcterms:description`     | `dcterms:rights`             | `dcatde:politicalGeocodingLevelURI`   |
| `dcat:landingPage`              | `dcterms:hasPart`&nbsp;+  | `dcterms:title`              | `dcatde:politicalGeocodingURI`&nbsp;- |
| `dcat:last`&nbsp;+              | `dcterms:identifier`      | `dcterms:type`               | `dcatde:qualityProcessURI`&nbsp;-     |
| `dcat:prev`&nbsp;+              | `dcterms:isReferencedBy`  | `odrl:hasPolicy`             | `dcterms:contributor`                 |
| `dcat:previousVersion`&nbsp;+   | `dcterms:issued`          | `prov:qualifiedAttribution`  | `dcterms:references`                  |
|                                 |                           |                              | `geodcat:custodian`&nbsp;+            |
|                                 |                           |                              | `geodcat:originator`&nbsp;+           |

*(+ = Wurde in DCAT-AP.de 3.0 hinzugefügt; - = Wurde in DCAT-AP.de 3.0 deprecated.)*

</small>
