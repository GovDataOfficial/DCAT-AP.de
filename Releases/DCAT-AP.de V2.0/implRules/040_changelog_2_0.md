## Änderungen in der Version 2.0
https://github.com/GovDataOfficial/DCAT-AP.de/issues/60

In Version 2.0 ist die größte und offensichtlichste Änderung, die Verwendung von ReSpec, um Spezifikation und Konventionenhandbuch als moderne Web-Version zu veröffentlichen. Dieses Vorgehen ist transparenter, einfacher zu handhaben und einfacher konsistent zu halten.​ Zusätzlich wird aber auch ein PDF-Export angeboten.​

Mit der Umstellung ging eine redaktionelle Überarbeitung der meisten Texten einher. Beispiele, die zuvor als Bild eingefügt waren, wurden in Text überführt. Tabellen wurden zum Teil in eine andere, web-kompatiblere, Darstellungsform überführt. Die Aufteilung des Dokuments wurde ebenfalls leicht angepasst.


### Einführung von dcat:DataService​
https://github.com/GovDataOfficial/DCAT-AP.de/issues/53

Der dcat:DataService wird generell so eingeführt, wie er auch in DCAT-AP 2.0 eingeführt wurde. Damit stehen Datenbereitstellern neue und exaktere Möglichkeiten zur Verfügung, Webservices zu beschreiben. Es besteht aber kein Zwang, diese zu nutzen.​
Im Konventionenhandbuch werden Beispiele gegeben, wie ein `dcat:DataService` modelliert werden kann.

### Aufnahme neuer Eigenschaften
https://github.com/GovDataOfficial/DCAT-AP.de/issues/59

Im Konventionenhandbuch erfolgt eine Erläuterung zur Abgrenzung zwischen `dct:license`, `odrl:hasPolice` und `dct:rights`.
Diese Eigenschaften wurden zum Teil neu eingeführt.

### Neue Verweise auf Dateiformate
https://github.com/GovDataOfficial/DCAT-AP.de/issues/56

Durch die Einführung der Eigenschaften `dcat:packageFormat` und `dcat:compressFormat` konnte Konvention 31, die relativ kompliziert und fehleranfällig war, vereinfacht werden.

### Abgrenzung `plannedAvailability` und `adms:status` deutlich machen
https://github.com/GovDataOfficial/DCAT-AP.de/issues/50

Die Eigenschaft `dcatap:availability` betrachtet insbesondere die Stabilität der `dcat:accessURL` als zentrales Merkmal einer Distribution. Ihr Unterschied zu `adms:status` wird im Konventionenhandbuch beschrieben.

### Relationen zw. Datensätzen `dct:relation` und `dct:hasVersion` klären​
https://github.com/GovDataOfficial/DCAT-AP.de/issues/49

Setzen des Collections-Features auf `DEPRECATED` und abwarten auf die `dcat:DatasetSeries` Lösung von DCAT3 und DCAT-AP. ​

Verbesserung bzw. Fehlerkorrektur der Beschreibung im Konventionenhandbuch.

### Kennzeichnung für Markdown
https://github.com/GovDataOfficial/DCAT-AP.de/issues/46

Erläuterung, welche HTML-Tags von GovData interpretiert werden und wie andere Portale mit Markdown umgehen können.

### Klare Aussagen zu Distribution
https://github.com/GovDataOfficial/DCAT-AP.de/issues/44

Alle Distributionen eines Datasets müssen weitestgehend die selben Daten beinhalten. Zeitreihen sollen nicht als mehrere Distributionen innerhalb eines Datasets dargestellt werden. 

### Bei RDF Daten: sneak peek in den Inhalt
https://github.com/GovDataOfficial/DCAT-AP.de/issues/39

Beispiel, wie man einen "sneak peak" mittels `adms:sample` umsetzen kann.

### Angaben zu Spalten einer CSV-Datei​
https://github.com/GovDataOfficial/DCAT-AP.de/issues/32

Beispiel, wie man mittels `dct:conformsTo` und CSVW beschreiben kann, wie eine CSV-Datei aufgebaut ist.

### Weitere Kategorien für Datasets
https://github.com/GovDataOfficial/DCAT-AP.de/issues/33

Verweis auf die Kategorien des Musterdatenkatalogs mittels `dcat:keyword` und `dct:references`.

### `dct:license` auch für `dcat:Dataset`
https://github.com/GovDataOfficial/DCAT-AP.de/issues/25

Zwar kann `dcat:Dataset` mit einer Lizenz versehen werden, für die Anbindung an GovData müssen die Lizenzen aber weiterhin verpflichtend auf Ebene der Distributionen angegeben werden. ​
Konvention 32 bleibt weiter bestehen und wird erweitert, dass ein `dcat:DataService` ebenfalls über `dct:license` verfügen MUSS, wenn die Daten die er ausspielt, eine Lizenz haben. 

### Geodaten: Änderungen und Erhebungsmethoden
https://github.com/GovDataOfficial/DCAT-AP.de/issues/37

Wie `adms:versionNote`, auch Änderungen der Erhebungsmethoden, genutzt werden kann, wurde besser beschrieben.

### Konv. 1 dcat:contactPoint - Pflichtangaben
https://github.com/GovDataOfficial/DCAT-AP.de/issues/47

Konvention 1 war zu streng und der umgebende Text widersprüchlich. Die Konvention wurde so abgeändert, dass entweder `vcard:hasEmail` oder `vcard:hasURL` (Link zum Kontaktformular) angegeben werden muss.​

### Kennzeichnung High Value Datasets (HVD) in DCAT-AP.de​
https://github.com/GovDataOfficial/DCAT-AP.de/issues/29

Verwendung der Eigenschaft `dct:references`, um auf Referenzdatensätze wie ein HVD oder einen Musterdatensatz des Musterdatenkatalogs zu verweisen.​

### Weitere Errata
 - [#59](https://github.com/GovDataOfficial/DCAT-AP.de/issues/59) Kardinalität von adms:versionNotes im UML-Diagramm​ angepasst.
 - [#51](https://github.com/GovDataOfficial/DCAT-AP.de/issues/51) Begriff "Koordinatenreferenzsystem" statt "Koordinatensystem" verwendet und Beispiele vereinfacht.
 - [#48](https://github.com/GovDataOfficial/DCAT-AP.de/issues/48) dcatde:contributorID - Formulierung klargestellt und Beispiel geändert.
 - [#23](https://github.com/GovDataOfficial/DCAT-AP.de/issues/23) Konvention 27/28 - Nicht alle Identifier können als URI übernommen werden, daher Streichung.
