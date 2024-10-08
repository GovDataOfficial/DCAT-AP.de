# Überblick über das DCAT-AP.de Modell {#ueberblick-datenmodell}

Als Austauschstandard für allgemeine offene Verwaltungsdaten ist der Hauptanwendungsfall von DCAT-AP.de der Austausch von Metadaten zwischen Datenportalen. Dabei wird in der Regel ein Katalog (`dcat:Catalog`) bereitstellt, der Datensätze (`dcat:Dataset`), Datenservices (`dcat:DataService`) und/oder Datensatzserien (`dcat:DatasetSeries`) beinhaltet. Die Zugang zu den eigentlichen Daten wird zudem in Distributionen (`dcat:Distribution`) beschrieben, die daher auch eine zentrale Bedeutung haben. Diese fünf Klassen (und die Superklasse `dcat:Resource` werden im UML-Diagramm rot hervorgehoben.)

W3C-DCAT und DCAT-AP teilen beide die Klassen in Haupt- und Unterstützungsklassen ein, verwenden dafür allerdings unterschiedliche Definitionen (bzw. keine klaren Definitionen). DCAT-AP.de definiert Hauptklassen wie folgt:

<p class="note" title="Definition von Hauptklasse">
Hauptklassen sind alle Klassen, die entweder im DCAT-Namensraum definiert werden oder der Wertebereich einer verpflichtenden Eigenschaft sind.
</p>

Darüber hinaus beschreiben wir nur solche Klassen, die (im W3C-DCAT oder DCAT-AP) über mindestens eine Eigenschaft verfügen und zudem in DCAT-AP.de nicht durch ein kontrolliertes Vokabular abgedeckt werden. Daraus ergibt sich folgende Klassenübersicht:

| Hauptklassen                             |                                                          | Unterstützungsklassen            |
| ---------------------------------------- | -------------------------------------------------------- | -------------------------------- |
| [Ressource](#klasse-ressource)           | [Distribution](#klasse-distribution)                     | [Zeitraum](#klasse-zeitraum)     |
| [Katalog](#klasse-katalog)               | [Katalogeintrag](#klasse-katalogeintrag)                 | [Standort](#klasse-standort)     |
| [Datensatz](#klasse-datensatz)           | [Rollenzuordnung](#klasse-rollenzuordnung)               | [Identifier](#klasse-identifier) |
| [Datenservice](#klasse-datenservice)     | [Kontaktinformationen](#klasse-kontaktinformationen)     | [Prüfsumme](#klasse-prufsumme)   |
| [Datensatzserie](#klasse-datensatzserie) | [Verantwortliche Stelle](#klasse-verantwortliche-stelle) | [Beziehung](#klasse-beziehung)   |


## UML-Diagramm

<figure id="pic-id-5">
  <a href="../uml/dcat-ap-de.svg" target="_blank"><img src="../uml/dcat-ap-de.svg" alt="UML-Diagramm aller DCAT-AP-Klassen einschließlich der DCAT-AP.de Erweiterungen "></a>
  <figcaption>UML-Diagramm aller DCAT-AP-Klassen einschließlich der DCAT-AP.de Erweiterungen</figcaption>
</figure>