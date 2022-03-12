# APP.6: Allgemeine Software

## APP.6.A1 Planung des Software-Einsatzes [Fachverantwortliche] (B)

- Bevor eine Institution eine (neue) Software einführt, MUSS sie entscheiden,
    - wofür die Software genutzt und welche Informationen damit verarbeitet werden sollen,
    - wie die Benutzer bei der Anforderungserhebung beteiligt und bei der Einführung unterstützt werden sollen,
    - wie die Software an weitere Anwendungen und IT-Systeme über welche Schnittstellen angebunden wird,
    - auf welchen IT-Systemen die Software ausgeführt werden soll und welche Ressourcen zur Ausführung der Software erforderlich sind, sowie
    - ob sich die Institution in Abhängigkeit zu einem Hersteller begibt, wenn sie diese Software einsetzt.
- Hierbei MÜSSEN bereits Sicherheitsaspekte berücksichtigt werden.
- Zusätzlich MUSS die Institution die Zuständigkeiten für fachliche Betreuung, Freigabe und betriebliche Administration schon im Vorfeld klären und festlegen.
- Die Zuständigkeiten MÜSSEN dokumentiert und bei Bedarf aktualisiert werden.

## APP.6.A2 Erstellung eines Anforderungskatalogs für Software [Fachverantwortliche] (B)

- Auf Basis der Ergebnisse der Planung MÜSSEN die Anforderungen an die Software in einem Anforderungskatalog erhoben werden.
- Der Anforderungskatalog MUSS dabei die grundlegenden funktionalen Anforderungen umfassen.
- Darüber hinaus MÜSSEN die nichtfunktionalen Anforderungen und hier insbesondere die Sicherheitsanforderungen in den Anforderungskatalog integriert werden.
- Hierbei MÜSSEN sowohl die Anforderungen von den Fachverantwortlichen als auch vom IT-Betrieb berücksichtigt werden.
- Insbesondere MÜSSEN auch die rechtlichen Anforderungen, die sich aus dem Kontext der zu verarbeitenden Daten ergeben, berücksichtigt werden.
- Der fertige Anforderungskatalog SOLLTE mit allen betroffenen Fachabteilungen abgestimmt werden.

## APP.6.A3 Sichere Beschaffung von Software [Beschaffungsstelle] (B)

- Wenn Software beschafft wird, MUSS auf Basis des Anforderungskatalog eine geeignete Software ausgewählt werden.
- Die ausgewählte Software MUSS aus vertrauenswürdigen Quellen beschafft werden.
- Die vertrauenswürdige Quelle SOLLTE eine Möglichkeit bereitstellen, die Software auf Integrität zu überprüfen.
- Darüber hinaus SOLLTE die Software mit einem geeigneten Wartungsvertrag oder einer vergleichbaren Zusage des Herstellers oder Software-Anbieters beschafft werden.
- Diese Verträge oder Zusagen SOLLTEN insbesondere garantieren, dass auftretende Sicherheitslücken und Schwachstellen der Software während des gesamten Nutzungszeitraums zeitnah behoben werden.

## APP.6.A4 Regelung für die Installation und Konfiguration von Software [Fachverantwortliche] (B)

- Die Installation und Konfiguration der Software MUSS durch den IT-Betrieb so geregelt werden, dass
    - die Software nur mit dem geringsten notwendigen Funktionsumfang installiert und ausgeführt wird,
    - die Software mit den geringsten möglichen Berechtigungen ausgeführt wird,
    - die datensparsamsten Einstellungen (in Bezug auf die Verarbeitung von personenbezogenen Daten) konfiguriert werden sowie
    - alle relevanten Sicherheitsupdates und -patches installiert sind, bevor die Software produktiv eingesetzt wird.
- Hierbei MÜSSEN auch abhängige Komponenten (u. a. Laufzeitumgebungen, Bibliotheken, Schnittstellen sowie weitere Programme) mitbetrachtet werden.
- Der IT-Betrieb MUSS in Abstimmung mit dem Fachverantwortlichen festlegen, wer die Software wie installieren darf.
- Idealerweise SOLLTE Software immer zentral durch den IT-Betrieb installiert werden.
- Ist es erforderlich, dass die Software (teilweise) manuell installiert wird, dann MUSS der IT-Betrieb eine Installationsanweisung erstellen, in der klar geregelt wird, welche Zwischenschritte zur Installation durchzuführen und welche Konfigurationen vorzunehmen sind.
- Darüber hinaus MUSS der IT-Betrieb regeln, wie die Integrität der Installationsdateien überprüft wird.
- Falls zu einem Installationspaket digitale Signaturen oder Prüfsummen verfügbar sind, MUSS mit diesen die Integrität überprüft werden.
- Sofern erforderlich, SOLLTE der IT-Betrieb eine sichere Standardkonfiguration der Software festlegen, mit der die Software konfiguriert wird.
- Die Standardkonfiguration SOLLTE dokumentiert werden.

## APP.6.A5 Sichere Installation von Software (B)

- Software MUSS entsprechend der Regelung für die Installation auf den IT-Systemen installiert werden.
- Dabei MÜSSEN ausschließlich unveränderte Versionen der freigegebenen Software verwendet werden.
- Wird von diesen Anweisungen abgewichen, MUSS dies durch den Vorgesetzten und den IT-Betrieb genehmigt werden und entsprechend dokumentiert werden.

## APP.6.A6 Berücksichtigung empfohlener Sicherheitsanforderungen (S)

- Die Institution SOLLTE die nachfolgenden Sicherheitsanforderungen im Anforderungskatalog für die Software berücksichtigen:
    - Die Software SOLLTE generelle Sicherheitsfunktionen wie Protokollierung und Authentifizierung umfassen, die im Anwendungskontext erforderlich sind.
    - Die Software SOLLTE es ermöglichen, die Härtungsfunktionen der Einsatzumgebung zu nutzen. Hierbei SOLLTEN insbesondere die Härtungsfunktionen des geplanten Betriebssystems und der geplanten Ausführungsumgebung berücksichtigt werden.
    - Wenn durch die Software Informationen über ungesicherte, öffentliche Netze übertragen werden, dann SOLLTE die Software sichere Verschlüsselungsfunktionen einsetzen, die dem Stand der Technik entsprechen. Darüber hinaus SOLLTEN die übertragenen Daten auf Integrität überprüft werden, indem Prüfsummen oder digitale Signaturen eingesetzt werden.
    - Verwendet die Software Zertifikate, dann SOLLTE sie die Möglichkeit bieten, die Zertifikate transparent darzustellen. Zudem SOLLTE es möglich sein, Zertifikate zu sperren, ihnen das Vertrauen zu entziehen oder eigene Zertifikate zu ergänzen.
- Die sich aus den Sicherheitsanforderungen ergebenden Funktionen der Software SOLLTEN im Betrieb verwendet werden.

## APP.6.A7 Auswahl und Bewertung potentieller Software [Fachverantwortliche, Beschaffungsstelle] (S)

- Anhand des Anforderungskatalogs SOLLTEN die am Markt erhältlichen Produkte gesichtet werden.
- Sie SOLLTEN mithilfe einer Bewertungsskala miteinander verglichen werden.
- Danach SOLLTE untersucht werden, ob die Produkte aus der engeren Wahl die Anforderungen der Institution erfüllen.
- Gibt es mehrere Alternativen für Produkte, SOLLTEN auch die Nutzerakzeptanz und der zusätzliche Aufwand für z. B. Schulungen oder die Migration berücksichtigt werden.
- Die Fachverantwortlichen SOLLTEN gemeinsam mit dem IT-Betrieb anhand der Bewertungen und Testergebnisse ein geeignetes Softwareprodukt auswählen.

## APP.6.A8 Regelung zur Verfügbarkeit der Installationsdateien (S)

- Der IT-Betrieb SOLLTE die Verfügbarkeit der Installationsdateien sicherstellen, um die Installation reproduzieren zu können.
- Hierzu SOLLTE der IT-Betrieb
    - die Installationsdateien geeignet sichern oder
    - die Verfügbarkeit der Installationsdateien durch die Bezugsquelle (z. B. App-Store) sicherstellen.
- Zusätzlich SOLLTE sichergestellt werden, dass Software reproduzierbar konfiguriert werden kann.
- Hierzu SOLLTEN die Konfigurationsdateien gesichert werden.
- Alternativ SOLLTE geeignet dokumentiert werden, wie die Software konfiguriert wird.
- Diese Regelung SOLLTE in das Datensicherungskonzept der Institution integriert werden.

## APP.6.A9 Inventarisierung von Software (S)

- Software SOLLTE inventarisiert werden.
- In einem Bestandsverzeichnis SOLLTE dokumentiert werden, auf welchen Systemen die Software unter welcher Lizenz eingesetzt wird.
- Bei Bedarf SOLLTEN zusätzlich die sicherheitsrelevanten Einstellungen mit erfasst werden.
- Software SOLLTE nur mit Lizenzen eingesetzt werden, die dem Einsatzzweck und den vertraglichen Bestimmungen entsprechen.
- Die Lizenz SOLLTE den gesamten vorgesehenen Nutzungszeitraum der Software abdecken.
- Wird von einer Standardkonfiguration abgewichen, SOLLTE dies dokumentiert werden.
- Das Bestandsverzeichnis SOLLTE anlassbezogen durch den IT-Betrieb aktualisiert werden, insbesondere wenn Software installiert wird.
- Das Bestandsverzeichnis SOLLTE so aufgebaut sein, dass bei Sicherheitsvorfällen eine schnelle Gesamtübersicht mit den notwendigen Details ermöglicht wird.

## APP.6.A10 Erstellung einer Sicherheitsrichtlinie für den Einsatz der Software (S)

- Die Institution SOLLTE die Regelungen, die festlegen, wie die Software eingesetzt und betrieben wird, in einer Sicherheitsrichtlinie zusammenfassen.
- Die Richtlinie SOLLTE allen relevanten Verantwortlichen, Zuständigen und Mitarbeitern der Institution bekannt sein und die Grundlage für ihre Arbeit und ihr Handeln bilden.
- Inhaltlich SOLLTE die Richtlinie auch ein Benutzer-Handbuch umfassen, dass erläutert, wie die Software zu benutzen und zu administrieren ist.
- Es SOLLTE regelmäßig und stichprobenartig überprüft werden, ob die Mitarbeiter sich an die Richtlinie halten.
- Die Richtlinie SOLLTE regelmäßig aktualisiert werden.

## APP.6.A11 Verwendung von Plug-ins und Erweiterungen (S)

- Es SOLLTEN nur unbedingt notwendige Plug-ins und Erweiterungen installiert werden.
- Werden Erweiterungen eingesetzt, SOLLTE die Software die Möglichkeit bieten, Erweiterungen zu konfigurieren und abzuschalten.

## APP.6.A12 Geregelte Außerbetriebnahme von Software [Fachverantwortliche] (S)

- Wenn Software außer Betrieb genommen wird, SOLLTE der IT-Betrieb mit den Fachverantwortlichen regeln, wie dies im Detail durchzuführen ist.
- Ebenfalls SOLLTE geregelt werden, wie die Benutzer hierüber zu informieren sind.
- Hierbei SOLLTE geklärt werden, ob die funktionalen Anforderungen fortbestehen (z. B. zur Bearbeitung von Fachaufgaben).
- Ist dies der Fall, dann SOLLTE geregelt werden, wie die benötigten Funktionen der betroffenen Software weiter verfügbar sein werden.

## APP.6.A13 Deinstallation von Software (S)

- Wird Software deinstalliert, SOLLTEN alle angelegten und nicht mehr benötigten Dateien entfernt werden.
- Alle Einträge in Systemdateien, die für das Produkt vorgenommen wurden und nicht länger benötigt werden, SOLLTEN rückgängig gemacht werden.

## APP.6.A14 Nutzung zertifizierter Software (H)

- Bei der Beschaffung von Software SOLLTE festgelegt werden, ob Zusicherungen des Herstellers, Vertreibers und Anbieters über implementierte Sicherheitsfunktionen als ausreichend vertrauenswürdig anerkannt werden können.
- Ist dies nicht der Fall, SOLLTE eine Zertifizierung der Anwendung z. B. nach Common Criteria als Entscheidungskriterium herangezogen werden.
- Stehen mehrere Produkte zur Auswahl, SOLLTEN insbesondere dann Sicherheitszertifikate berücksichtigt werden, wenn der evaluierte Funktionsumfang die Mindestfunktionalität (weitestgehend) umfasst und die Mechanismenstärke dem Schutzbedarf entspricht.


