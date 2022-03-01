# Konventionen zur `dcat:Distribution`

Laut Definition müssen alle Distributionen eines Datasets weitestgehend die selben Daten beinhalten. Diese können in unterschiedlichen Formaten vorliegen. Weiter gilt:
- Zeitreihen sollen generell nicht als unterschiedliche Distributionen innerhalb eines Datensatzes dargestellt werden. 
- In Ausnahmefällen kann dct:title für die Erläuterung der Inhalte der Distributionen genutzt werden
- Datasets, die über Distributionen mit einem DataService verfügen, können Distributionen mit einem Auszug an Daten haben.
- Gemäß dem [Leitfaden zur Berücksichtigung von Dokumenten im Metadatenkatalog von „GovData – das Datenportal für Deutschland“](https://www.govdata.de/documents/10156/18448/2020-07-29-Dokumente+im+GovData+Portal_Leitfaden_nach_Fachgruppensitzung.pdf/8c8be2ca-bd07-4f26-acb5-72a90d24a120) dürfen zusätzlich auch Dokumente mit Erläuterungen zu den maschinenlesbaren Distributionen angefügt werden. Diese könnte z.B. eine PDF-Datei mit Erläuterungen und Vorbemerkungen zum Haushaltsplan sein, der in maschinenlesbarer Form in einer anderen Distribution vorliegt.

Werden, wie im letzten Punkt beschrieben, Dokumente mit Erläuterungen als Distribution mit veröffentlicht, sollten diese Dokumentation auch zusätzlich vom [Datasatz aus über `foaf:page`](https://www.dcat-ap.de/def/dcatde/2.0/spec/#datensatz-dokumentation) eingebunden werden.


## Angaben zu Dateiformaten (insb. `dct:format`) {#angaben-zu-dateiformaten}

DCAT-AP sieht zur Kennzeichnung des Dateiformats vor, dass für `dct:format` das [EU Vokabular "File Type" des Publications Office](https://op.europa.eu/en/web/eu-vocabularies/concept-scheme/-/resource?uri=http://publications.europa.eu/resource/authority/file-type) zu verwenden ist.

<figure id="konvention-31" class="konvention"><figcaption>
Hat die Datei, die die Daten einer Distribution beinhaltet, ein im <a href="https://op.europa.eu/en/web/eu-vocabularies/concept-scheme/-/resource?uri=http://publications.europa.eu/resource/authority/file-type" target="_blank">EU Vokabular "File Type"</a> geführtes Format, so MUSS auf dieses mittels `dct:format` verwiesen werden. Andernfalls MUSS über das <a href="https://op.europa.eu/en/web/eu-vocabularies/concept-scheme/-/resource?uri=http://publications.europa.eu/resource/authority/file-type" target="_blank">Webformular</a> mittels "CONTRIBUTE" bzw. "BEITRAGEN" eine Aufnahme des Formats beantragt werden.
</figcaption></figure>

Befinden sich die Dateien, die die eigentlichen Informationen enthalten, innerhalb eines Containers, sollte zusätzlich noch das Kompressionsformat (`dcat:compressFormat`) bzw. das Paketformat (`dcat:packageFormat`) angegeben werden. Ist das `dcat:compressFormat` zugleich das `dcat:packageFormat`, kann auf die Angabe von `dcat:packageFormat` verzichtet werden.

Die bisherige Regelung, Containerformaten über eine URI die z.B. `+zip` beinhaltet anzugeben, entfällt mit der Einführung der neuen Eigenschafen.

Die Eigenschaft `dct:format` ist gegenüber `dcat:mediaType` vorrangig zu benutzten. Alle drei Eigenschaften aus dem dcat-Namensraum (`dcat:mediaType`, `dcat:compressFormat` und `dcat:packageFormat`) verwenden das [IANA Vokabular "Media Types"](https://www.iana.org/assignments/media-types/media-types.xhtml).

<pre class="example HTML" title="Angabe zu Dateiformaten, reine CSV-Datei">
&lt;https://example.org/distr-just-csv&gt; a dcat:Distribution ;
  dcat:downloadURL &lt;https://example.org/download/distr.csv&gt; ;
  dct:format &lt;http://publications.europa.eu/resource/authority/file-type/CSV&gt; ;
</pre>

<pre class="example HTML" title="Angabe zu Dateiformaten, CSV in GZ">
&lt;https://example.org/distr-csv-gz&gt; a dcat:Distribution ;
  dcat:downloadURL &lt;https://example.org/download/distr.csv.gz&gt; ;
  dct:format &lt;http://publications.europa.eu/resource/authority/file-type/CSV&gt; ;
  dcat:compressFormat &lt;http://www.iana.org/assignments/media-types/application/gzip&gt; .
</pre>

<pre class="example HTML" title="Angabe zu Dateiformaten, CSV in ZIP">
&lt;https://example.org/distr-csv-zip&gt; a dcat:Distribution ;
  dcat:downloadURL &lt;https://example.org/download/distr.zip&gt; ;
  dct:format &lt;http://publications.europa.eu/resource/authority/file-type/CSV&gt; ;
  dcat:compressFormat &lt;http://www.iana.org/assignments/media-types/application/zip&gt; .
</pre>


## Angaben zur Lizenz und zu Rechten (insb. `dct:license`) {#angaben-zur-lizenz-und-zu-rechten}

### Vorgaben und Abgrenzung

DCAT-AP bietet verschiedener Felder für die Abbildung von Nutzungsrechten und weiteren Einschränkungen ab. Die Fachgruppe GovData hat beschlossen, für die Datenbereitstellung an GovData eine abschließende Lizenzliste innerhalb des DCAT-AP.de-Namensraums beizubehalten. Sie kann sich auch außerhalb des DCAT-AP.de Releasezyklus ändern. 

Die abschließende Liste der verpflichtend zu verwendenden Lizenzen-URIs finden Sie im Kapitel zu [kontrollierten Vokabularen](#kontrollierte-vokabulare).

Ergänzend zur verpflichtenden Angabe einer Lizenz (`dct:license`) können optional Aussagen über Grad der Zugänglichkeit (`dct:accessRights`), über  Nutzungsbestimmungen (`dct:rights`) und zu einem Regelwerk (`odrl:hasPolicy`) gemacht werden. Für GovData ist jedoch die Angabe der Lizenz entscheidend.

<pre class="example HTML" title="Angabe einer Lizenz und zusätzlicher Nutzungsbestimmungen">
&lt;https://example.org/distr-1234&gt; a dcat:Distribution ;
  dct:license &lt;http://dcat-ap.de/def/licenses/dl-by-de/2.0&gt; ;
  dct:rights &lt;https://www.govdata.de/web/guest/lizenzen&gt; .
</pre>

<figure id="konvention-32" class="konvention"><figcaption>
Distributionen von Datensätzen MÜSSEN mit einer Lizenz ausgewiesen werden. Für die Kennzeichnung der Lizenzen MÜSSEN die unter http://dcat-ap.de/def/licenses/ genannten URIs verwendet werden. Zusätzlich MUSS auch ein `dcat:DataServices` mit einer Lizenz versehen werden, wenn die Daten die er ausspielt, eine Lizenz haben. 
</figcaption></figure>

Mit DCAT-AP 2.0 wurde `dct:license` auch auf Ebene der `dcat:Resource` und damit beim `dcat:Dataset` eingeführt. Für GovData bleibt aber die Angabe auf Ebene der Distribution ausschlaggebend.

<figure id="konvention-33" class="konvention"><figcaption>
ENTFÄLLT
</figcaption></figure>

<figure id="konvention-34" class="konvention"><figcaption>
Die URIs der Lizenzen außerhalb der GovData Lizenzliste MÜSSEN zum Erhalt der DCAT-AP Konformität unverändert weitergegeben werden.
</figcaption></figure>

Mit diesen Konventionen soll die Anforderung nach einer geschlossenen Lizenzliste umgesetzt und gleichzeitig DCAT-AP-Konformität von DCAT-AP.de eingehalten werden.
Es bestehen weiterhin Konventionen zur Namensbildung der URIs, welche bei Neuanlage von URIs zu berücksichtigen sind und welche zu einer harmonisierenden Anpassung der ehemaligen OGD-Lizenzcodes führt.

### Angabe von By-Texten

Das Feld `dcatde:licenseAttributionByText` speichert Angaben (insbes. für Share-Alike Lizenzen), bei denen der By-Text exakt wiedergegeben werden muss. Alternative Namensnennungen aus Autoren oder Herausgebernamen sind hier im Textfeld explizit so anzugeben, wie es der Lizenzgeber vorgesehen hat. Dieses Vorgehen ist temporär notwendig, bis DCAT-AP ein entsprechendes Feld zur Unterstützung der Lizenzangabe einführt.

<figure id="konvention-35" class="konvention"><figcaption>
Wird bei der Verwendung der Lizenz die Angabe des Herausgebers gefordert, so MUSS der Namensnennungstext im Feld `dcatde:licenseAttributionByText` hinterlegt werden.
</figcaption></figure>


## Status und erwartete Verfügbarkeit (`adms:status`, `dcatap:availability`) {#status-und-erwartete-verfugbarkeit}

### Status der Distribution (`adms:status`)

Für den Status einer Distribution wird die Eigenschaft `status` des Asset Description Metadata Schemas `adms` verwendet. Für das kontrollierte Vokabular stehen PURL-URIs zur Verfügung. Für den Portalverbund GovData wird vereinbart, die Ausprägung „in Entwicklung“ für Distributionen nicht zu verwenden.

| Deutsche Übersetzung | Wert                                         | unterstützt durch DCAT-AP | unterstützt durch GovData |
| :------------------- | -------------------------------------------- | :-----------------------: | :-----------------------: |
| in Entwicklung       | http://purl.org/adms/status/UnderDevelopment |             +             |             -             |
| Vollständig          | http://purl.org/adms/status/Completed        |             +             |             +             |
| Nicht mehr empfohlen | http://purl.org/adms/status/Deprecated       |             +             |             +             |
| Zurückgezogen        | http://purl.org/adms/status/Withdrawn        |             +             |             +             |

Zu einem Datensatz wird kein eigener Status geführt; vielmehr leitet sich sein Status logisch aus dem Status seiner Distributionen ab. Ein Datensatz wird als „Completed“ betrachtet, wenn mindestens eine seiner Distributionen diesen Status hat. Ein Datensatz wird als „Deprecated“ betrachtet, wenn mindestens eine seiner Distributionen diesen Status und keine den Status „Completed“ hat. Ein Datensatz wird nur als „Withdrawn“ betrachtet, wenn alle ihre Distributionen diesen Status haben.

<figure id="konvention-22" class="konvention"><figcaption>
Es MÜSSEN Metadaten zu Datensätzen mit Distributionen im `adms:status` „Completed“, „Deprecated“ oder „Withdrawn“ transportiert werden.
</figcaption></figure>

Beim Entwurf der Metadaten haben Distributionen oft ungeklärte Lizenzverhältnisse, Ansprechpartner, oder sind in der Kategorisierung noch nicht trennscharf. Während die Erfassung von Datensätzen in diesem Status in einem Katalog durchaus Sinn machen kann, ist es in der Regel nicht erwünscht, die Metadaten bereits zu publizieren. Daher werden mit DCAT-AP.de die Status „Completed“, „Withdrawn“ und „Deprecated“ verwendet.

<figure id="konvention-23" class="konvention"><figcaption>
Es MÜSSEN Metadaten zu Datensätzen mit Distributionen im `adms:status` „Completed“, „Deprecated“ in DCAT-AP.de konformen Portalen angezeigt werden.
</figcaption></figure>

Bevor Elemente mit „Withdrawn“ längerfristig als „zurückgezogen“ markiert werden, SOLLEN sie zuvor für die Dauer von 30 Tagen mit dem adms:status „Deprecated“ als „Nicht mehr empfohlen“ ausgewiesen werden.

<figure id="konvention-24" class="konvention"><figcaption>
Es SOLLEN Datensätzen mit Distributionen im `adms:status` „Withdrawn“ zunächst mit „Deprecated“ ausgewiesen werden.
</figcaption></figure>

### Abgrenzung zu `dcatap:availability`

Der Status der Distribution ist von der Verfügbarkeit (`dcatap:availability`) zu unterscheiden. Der Staus gibt an, ob eine Distribution z.B. vollständig ist oder aber nicht mehr zur Nutzung empfohlen wird. Die Verfügbarkeit gibt hingegen an, wie lange die Informationen voraussichtlich zur Verfügung stehen werden. Sie betrachtet insbesondere die Stabilität der `dcat:accessURL` als zentrales Merkmal einer Distribution. 

So kann ein z.B. eine Distribution aufgrund eines neueren Dateiformats nicht mehr zur Nutzung empfohlen werden zugleich aber dennoch weiterhin zur Verfügung gestellt werden:

<pre class="example HTML" title="Distribution deprecated aber stabil">
&lt;https://example.org/distr-100&gt; a dcat:Distribution ;
  dcatap:avaliability &lt;http://data.europa.eu/r5r/availability/stable&gt; ;
  adms:status &lt;http://purl.org/adms/status/Deprecated&gt; .
</pre>

Ein anderer Fall liegt vor, wenn eine Distribution zur Nutzung empfohlen wird, aber z.B. aufgrund einer besonderen Lage oder im Rahmen eines Projektes nur temporär bereitgestellt wird:

<pre class="example HTML" title="Distribution vollständig aber experimentell">
&lt;https://example.org/distr-200&gt; a dcat:Distribution ;
  dcatap:avaliability &lt;http://data.europa.eu/r5r/availability/experimental&gt; ;
  adms:status &lt;http://purl.org/adms/status/Completed&gt; .
</pre>


## Zugriff auf eine herunterladbare Datei (`dcat:downloadURL`) {#zugriff-auf-eine-herunterladbare-datei}

Die Eigenschaft `dcat:downloadURL` verweist auf den URL der herunterladbaren Datei, die die Daten im angegebenen Format enthält. Dahingehend kann der URL, der mit der Eigenschaft `dcat:accessURL` übertragen wird, auch lediglich auf eine Seite verweisen, die darüber informiert, wie auf die Daten zugegriffen werden kann.

<figure id="konvention-39" class="konvention"><figcaption>
Werden die Daten nur als direkter Download veröffentlicht, so wird der URL der Datei sowohl als `dcat:downloadURL` als auch als `dcat:accessURL` angegeben.
</figcaption></figure>


## Angabe des abgedeckten Zeitraums (`dcat:startDate`, `dcat:endDate`)

Der abgedeckte Zeitraum (`dct:temporal`) wird mittels dessen „Startzeitpunkt“ und „Endzeitpunkt“ angegeben. Eine von beiden MUSS (obwohl beide optional sind) für jede Instanz der Klasse `dct:PeriodOfTime` vorhanden sein.

<figure id="konvention-38" class="konvention"><figcaption>
Bei Zeitangaben mittels „Zeitraum“ MUSS eine der Angaben Beginn (`dcat:startDate`) oder Ende (`dcat:endDate`) angegeben sein.
</figcaption></figure>


## Konformität zu bestehenden Standards (`dct:conformsTo`) {#konformitat-zu-bestehenden-standards}

Konformität zu bestehende Standards (für Datensätze oder Distributionen) oder Application Profiles (für Katalogeinträge) kann unter Verwendung der Eigenschaft `dct:conformsTo` angezeigt werden.

<figure id="konvention-29" class="konvention"><figcaption>
Verweise auf bestehende andere Verschlagwortungssysteme oder Ontologien KÖNNEN mit `dct:conformsTo` ausgedrückt werden. angezeigt werden.
</figcaption></figure>

Wird in einer Distributionen ein maschinenlesbares Format zum Download angeboten, ist ein Verweis darauf, wie die Inhaltsdaten zu verstehen sind, besonders wertvoll für die weitere Verarbeitung der Daten.

| Datentyp   | Konformitätsangabe (Beispiel)                                                    |
| :--------- | :--------------------------------------------------------------------------------|
| RDF-Daten  | Ontologie im [OWL-Format](https://de.wikipedia.org/wiki/Web_Ontology_Language).  |
| XML-Daten  | XML-Schema-Definition im [XSD-Format](https://de.wikipedia.org/wiki/XML_Schema). |
| JSON-Daten | JSON-Schema-Definition im [JSON-Schema-Format](https://json-schema.org/).        |
| CSV-Daten  | Beschreibung des Aufbaus mit [Hilfe von CSVW](https://w3c.github.io/csvw/).      |


**Beispiel für RDF-Daten**
<aside class="example html" data-format="text" title="Daten einer Distribution sind konform zu einer Ontologie">

```
_:distr-1 a dcat:Distribution ;
  dct:title "Angebote im Online-Shop";
  dcat:downloadURL <https://example.com/angebote.rdf> ;
  dct:conformsTo <http://purl.org/goodrelations/v1> .
```

</aside>

**Beispiel für XML-Daten**
<aside class="example html" data-format="text" title="Daten einer Distribution sind konform zu einem XML-Schema">

```
_:distr-2 a dcat:Distribution ;
  dct:title "Sammlung von virtuellen Visitenkarten";
  dcat:downloadURL <https://example.com/visitenkarten.xml> ;
  dct:conformsTo <https://www.iana.org/assignments/xml-registry/schema/vcard-4.0.xsd> .
```

</aside>

**Beispiel für JSON-Daten**
<aside class="example html" data-format="text" title="Daten einer Distribution sind konform zu einem JSON-Schema">

```
_:distr-2 a dcat:Distribution ;
  dct:title "Sammlung von Punkten auf einer Karte";
  dcat:downloadURL <https://example.com/points-on-map.json> ;
  dct:conformsTo <https://geojson.org/schema/Point.json> .
```

</aside>

**Beispiel für CSV-Daten**
<aside class="example html" data-format="text" title="Beschreibung einer CSV-Datei mittels CSVW">

```
@prefix csvw: <http://www.w3.org/ns/csvw#> .
@prefix dcat: <http://www.w3.org/ns/dcat#> .
@prefix dct:  <http://purl.org/dc/terms/> .

_:distr-3 a dcat:Distribution ;
  dct:title "Städte in Deutschland";
  dcat:downloadURL <https://example.com/staedte.csv> ;
  dct:conformsTo _:staedteTabelle .

_:staedteTabelle csvw:table [
  csvw:url <https://example.com/staedte.csv> ;
  csvw:dialect [
    csvw:delimiter ";" ;
    csvw:quoteChar "'" ;
    csvw:header true ;
  ] ;
  csvw:tableSchema [
    csvw:column (
      [
        csvw:title "Stadtname"@de ;
        csvw:title "City Name"@en ;
        csvw:name "stadtname" ;
        csvw:datatype xsd:string ;
        csvw:maxLength 42 ;
      ][
        csvw:title "Bundesland (Code)"@de ;
        csvw:title "State (Code)"@en ;
        csvw:name "bundesland_XY" ;
        csvw:datatype xsd:string ;
        csvw:minLength 2 ;
        csvw:maxLength 2 ;
      ][
        csvw:title "Einwohner"@de ;
        csvw:title "Population"@en ;
        csvw:name "einwohner" ;
        csvw:datatype xsd:integer ;
        csvw:minInclusive 1 ;
      ]
    )
  ] ;
] .
```

</aside>

Die Beschreibung des Schemas und Dialekts hilft Nutzern, insbesondere Programmen, die unten angegebene Beispiel-CSV-Datei korrekt zu interpretieren.
Dabei helfen insbesondere die [Informationen, die über `csvw:dialect`](https://www.w3.org/TR/2015/REC-tabular-metadata-20151217/#dfn-dialect-description) eingebunden werden. 
Aber auch die Angaben zur jeweiligen Spalte in `csvw:column`, insbesondere der `csvw:datatype`, unterstützt beim Verständnis der Tabelle.

<aside class="example html" data-format="text" title="Beispiel-CSV-Datei die durch CSVW beschrieben wurde">

```
stadtname;bundesland_XY;einwohner
'Berlin';BE;3664088
'Freie und Hansestadt Hamburg';HH;1851430
'München';BY;1488202 
```

</aside>

| Stadtname                    | Bundesland (Code) | Einwohner |
| ---------------------------- | ----------------- | --------- |
| Berlin                       | BE                | 3664088   |
| Freie und Hansestadt Hamburg | HH                | 1851430   |
| München                      | BY                | 1488202   |


Dieses [englischsprachige Tutorial](https://medium.swirrl.com/how-to-publish-csv-on-the-web-csvw-4ea6cbb603b4) geht auf die Verwendung von CSVW mit JSON-LD und weitere Aspekte ein.
