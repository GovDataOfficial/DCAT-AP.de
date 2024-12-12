# Konformität zu DCAT-AP

Der Anwendungsbereich von DCAT-AP ist grenz- und domänenüberschreitend. Nationale oder domänenspezifische Anwendungen unterliegen verschiedenen Anforderungen und definieren Erweiterungen zum DCAT-AP-Basisprofil. 
Die folgenden Regeln erlauben es dem Erweiterungsprofil DCAT-AP.de, die gegebenen deutschlandspezifischen Anforderungen umzusetzen und dabei gleichzeitig Interoperabilität im europaweiten Kontext sicherzustellen.

Die wichtigste Regel für Erweiterungen von DCAT-AP lautet:
- Jede Erweiterung von DCAT-AP muss die minimalen Konformitätskriterien erfüllen, welche in [Kapitel 4 von DCAT-AP 3.0](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#conformance) definiert sind.


Des Weiteren gelten folgende Regeln:
 - Erweiterungen dürfen die DCAT-AP 3.0 Nutzungsbestimmungen nicht erweitern, sondern nur einschränken, sodass alle Informationen, die in Bezug auf die Erweiterung valide sind, auch weiterhin in Bezug auf DCAT-AP 3.0 Validität besitzen.
 - Erweiterungen können Klassen beinhalten, die nicht in DCAT-AP 3.0 spezifiziert sind, jedoch sollten solche Klassen keine Ähnlichkeit zu ursprünglichen DCAT-AP-Klassen aufweisen.
-  Erweiterungen können Eigenschaften beinhalten, die nicht in DCAT-AP 3.0 spezifiziert sind, jedoch sollten solche Eigenschaften keine Ähnlichkeit zu ursprünglichen DCAT-AP-Eigenschaften aufweisen.
 - Erweiterungen können Kardinalitäten von Eigenschaften beinhalten, die von den Kardinalitäten der Eigenschaften in DCAT-AP 3.0 abweichen, sofern die folgenden Regeln berücksichtigt werden:
   - Obligatorische Eigenschaften aus DCAT-AP 3.0 müssen auch in der Erweiterung obligatorisch sein.
   - Empfohlene Eigenschaften aus DCAT-AP 3.0 können in der Erweiterung als optional, empfohlen oder obligatorisch deklariert werden.
   - Optionale Eigenschaften aus DCAT-AP 3.0 können in der Erweiterung als optional, empfohlen oder obligatorisch deklariert werden.
  - Empfohlene und optionale Eigenschaften aus DCAT-AP 3.0 können in der Erweiterung entfernt werden.
 - Erweiterungen müssen alle obligatorischen kontrollierten Vokabulare enthalten, die in [Kapitel 10 von DCAT-AP 3.0](https://semiceu.github.io/DCAT-AP/releases/3.0.0/#controlled-vocs) aufgelistet sind.
 - Erweiterungen können zusätzliche obligatorische kontrollierte Vokabulare beinhalten.

Das in dieser Spezifikation vorgestellte Erweiterungsprofil DCAT-AP.de in der Version 3.0 folgt diesen Regeln und damit sind sind alle DCAT-AP.de 3.0 Kataloge auch mit DCAT-AP 3.0 kompatibel.