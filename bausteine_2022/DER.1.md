# DER.1: Detektion von sicherheitsrelevanten Ereignissen

## DER.1.A1 Erstellung einer Sicherheitsrichtlinie für die Detektion von sicherheitsrelevanten Ereignissen (B)

- Ausgehend von der allgemeinen Sicherheitsrichtlinie der Institution MUSS eine spezifische Sicherheitsrichtlinie für die Detektion von sicherheitsrelevanten Ereignissen erstellt werden.
- In der spezifischen Sicherheitsrichtlinie MÜSSEN nachvollziehbar Anforderungen und Vorgaben beschrieben werden, wie die Detektion von sicherheitsrelevanten Ereignissen geplant, aufgebaut und sicher betrieben werden kann.
- Die spezifische Sicherheitsrichtlinie MUSS allen im Bereich Detektion zuständigen Mitarbeitern bekannt und grundlegend für ihre Arbeit sein.
- Falls die spezifische Sicherheitsrichtlinie verändert wird oder von den Anforderungen abgewichen wird, dann MUSS dies mit dem verantwortlichen ISB abgestimmt und dokumentiert werden.
- Es MUSS regelmäßig überprüft werden, ob die spezifische Sicherheitsrichtlinie noch korrekt umgesetzt ist.
- Die Ergebnisse der Überprüfung MÜSSEN sinnvoll dokumentiert werden.

## DER.1.A2 Einhaltung rechtlicher Bedingungen bei der Auswertung von Protokollierungsdaten (B)

- Wenn Protokollierungsdaten ausgewertet werden, dann MÜSSEN dabei die Bestimmungen aus den aktuellen Gesetzen zum Bundes- und Landesdatenschutz eingehalten werden.
- Wenn Detektionssysteme eingesetzt werden, dann MÜSSEN die Persönlichkeitsrechte bzw. Mitbestimmungsrechte der Mitarbeitervertretungen gewahrt werden.
- Ebenso MUSS sichergestellt sein, dass alle weiteren relevanten gesetzlichen Bestimmungen beachtet werden, z. B. das Telemediengesetz (TMG), das Betriebsverfassungsgesetz und das Telekommunikationsgesetz.

## DER.1.A3 Festlegung von Meldewegen für sicherheitsrelevante Ereignisse (B)

- Für sicherheitsrelevante Ereignisse MÜSSEN geeignete Melde- und Alarmierungswege festgelegt und dokumentiert werden.
- Es MUSS bestimmt werden, welche Stellen wann zu informieren sind.
- Es MUSS aufgeführt sein, wie die jeweiligen Personen erreicht werden können.
- Je nach Dringlichkeit MUSS ein sicherheitsrelevantes Ereignis über verschiedene Kommunikationswege gemeldet werden.
- Alle Personen, die für die Meldung bzw. Alarmierung relevant sind, MÜSSEN über ihre Aufgaben informiert sein.
- Alle Schritte des Melde- und Alarmierungsprozesses MÜSSEN ausführlich beschrieben sein.
- Die eingerichteten Melde- und Alarmierungswege SOLLTEN regelmäßig geprüft, erprobt und aktualisiert werden, falls erforderlich.

## DER.1.A4 Sensibilisierung der Mitarbeiter [Vorgesetzte, Benutzer, Mitarbeiter] (B)

- Jeder Benutzer MUSS dahingehend sensibilisiert werden, dass er Ereignismeldungen seines Clients nicht einfach ignoriert oder schließt.
- Jeder Benutzer MUSS die Meldungen entsprechend der Alarmierungswege an das verantwortliche Incident Management weitergeben (siehe DER.2.1 Behandlung von Sicherheitsvorfällen).
- Jeder Mitarbeiter MUSS einen von ihm erkannten Sicherheitsvorfall unverzüglich dem Incident Management melden.

## DER.1.A5 Einsatz von mitgelieferten Systemfunktionen zur Detektion [Fachverantwortliche] (B)

- Falls eingesetzte IT-Systeme oder Anwendungen über Funktionen verfügen, mit denen sich sicherheitsrelevante Ereignisse detektieren lassen, dann MÜSSEN diese aktiviert und benutzt werden.
- Falls ein sicherheitsrelevanter Vorfall vorliegt, dann MÜSSEN die Meldungen der betroffenen IT-Systeme ausgewertet werden.
- Zusätzlich MÜSSEN die protokollierten Ereignisse anderer IT-Systeme überprüft werden.
- Auch SOLLTEN die gesammelten Meldungen in verbindlich festgelegten Zeiträumen stichpunktartig kontrolliert werden.
- Es MUSS geprüft werden, ob zusätzliche Schadcodescanner auf zentralen IT-Systemen installiert werden sollen.
- Falls zusätzliche Schadcodescanner eingesetzt werden, dann MÜSSEN diese es über einen zentralen Zugriff ermöglichen, ihre Meldungen und Protokolle auszuwerten.
- Es MUSS sichergestellt sein, dass die Schadcodescanner sicherheitsrelevante Ereignisse automatisch an die Zuständigen melden.
- Die Zuständigen MÜSSEN die Meldungen auswerten und untersuchen.

## DER.1.A6 Kontinuierliche Überwachung und Auswertung von Protokollierungsdaten (S)

- Alle Protokollierungsdaten SOLLTEN möglichst permanent aktiv überwacht und ausgewertet werden.
- Es SOLLTEN Mitarbeiter benannt werden, die dafür zuständig sind.
- Falls die zuständigen Mitarbeiter aktiv nach sicherheitsrelevanten Ereignissen suchen müssen, z. B. wenn sie IT-Systeme kontrollieren oder testen, dann SOLLTEN solche Aufgaben in entsprechenden Verfahrensanleitungen dokumentiert sein.
- Für die Detektion von sicherheitsrelevanten Ereignissen SOLLTEN genügend personelle Ressourcen bereitgestellt werden.

## DER.1.A7 Schulung von Zuständigen [Vorgesetzte] (S)

- Alle Zuständigen, die Ereignismeldungen kontrollieren, SOLLTEN weiterführende Schulungen und Qualifikationen erhalten.
- Wenn neue IT-Komponenten beschafft werden, SOLLTE ein Budget für Schulungen eingeplant werden.
- Bevor die zuständigen Mitarbeiter Schulungen für neue IT-Komponenten bekommen, SOLLTE ein Schulungskonzept erstellt werden.

## DER.1.A8 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## DER.1.A9 Einsatz zusätzlicher Detektionssysteme [Fachverantwortliche] (S)

- Anhand des Netzplans SOLLTE festgelegt werden, welche Netzsegmente durch zusätzliche Detektionssysteme geschützt werden müssen.
- Der Informationsverbund SOLLTE um zusätzliche Detektionssysteme und Sensoren ergänzt werden.
- Schadcodedetektionssysteme SOLLTEN eingesetzt und zentral verwaltet werden.
- Auch die im Netzplan definierten Übergange zwischen internen und externen Netzen SOLLTEN um netzbasierte Intrusion Detection Systeme (NIDS) ergänzt werden.

## DER.1.A10 Einsatz von TLS-/SSH-Proxies [Fachverantwortliche] (S)

- An den Übergängen zu externen Netzen SOLLTEN TLS-/SSH-Proxies eingesetzt werden, welche die verschlüsselte Verbindung unterbrechen und es so ermöglichen, die übertragenen Daten auf Malware zu prüfen.
- Alle TLS-/SSHProxies SOLLTEN vor unbefugten Zugriffen geschützt werden.
- Auf den TLS-/SSH-Proxies SOLLTEN sicherheitsrele-vante Ereignisse automatisch detektiert werden.
- Es SOLLTE eine organisatorische Regelung erstellt werden, unter welchen datenschutzrechtlichen Voraussetzungen die Logdaten manuell ausgewertet werden dürfen.

## DER.1.A11 Nutzung einer zentralen Protokollierungsinfrastruktur für die Auswertung sicherheitsrelevanter Ereignisse [Fachverantwortliche] (S)

- Die auf einer zentralen Protokollinfrastruktur gespeicherten Ereignismeldungen der IT-Systeme und Anwendungen (siehe OPS.1.1.5 Protokollierung) SOLLTEN mithilfe eines Tools abgerufen werden können.
- Mit dem auswählten Tool SOLLTEN die Meldungen ausgewertet werden können.
- Die gesammelten Ereignismeldungen SOLLTEN regelmäßig auf Auffälligkeiten kontrolliert werden.
- Die Signaturen der Detektionssysteme SOLLTEN immer aktuell und auf dem gleichen Stand sein, damit sicherheitsrelevante Ereignisse auch nachträglich erkannt werden können.

## DER.1.A12 Auswertung von Informationen aus externen Quellen [Fachverantwortliche] (S)

- Um neue Erkenntnisse über sicherheitsrelevante Ereignisse für den eigenen Informationsverbund zu gewinnen, SOLLTEN externe Quellen herangezogen werden.
- Meldungen über unterschiedliche Kanäle SOLLTEN von den Mitarbeitern auch als relevant erkannt und an die richtige Stelle weitergeleitet werden.
- Informationen aus zuverlässigen Quellen SOLLTEN grundsätzlich ausgewertet werden.
- Alle gelieferten Informationen SOLLTEN danach bewertet werden, ob sie relevant für den eigenen Informationsverbund sind.
- Ist dies der Fall, SOLLTEN die Informationen entsprechend der Sicherheitsvorfallbehandlung eskaliert werden.

## DER.1.A13 Regelmäßige Audits der Detektionssysteme (S)

- Die vorhandenen Detektionssysteme und getroffenen Maßnahmen SOLLTEN in regelmäßigen Audits daraufhin überprüft werden, ob sie noch aktuell und wirksam sind.
- Es SOLLTEN die Messgrößen ausgewertet werden, die beispielsweise anfallen, wenn sicherheitsrelevante Ereignisse aufgenommen, gemeldet und eskaliert werden.
- Die Ergebnisse der Audits SOLLTEN nachvollziehbar dokumentiert und mit dem Soll-Zustand abgeglichen werden.
- Abweichungen SOLLTE nachgegangen werden.

## DER.1.A14 Auswertung der Protokollierungsdaten durch spezialisiertes Personal (H)

- Es SOLLTEN Mitarbeiter speziell damit beauftragt werden, alle Protokollierungsdaten zu überwachen.
- Die Überwachung der Protokollierungsdaten SOLLTE die überwiegende Aufgabe der beauftragten Mitarbeiter sein.
- Die beauftragten Mitarbeiter SOLLTEN spezialisierte weiterführende Schulungen und Qualifikationen erhalten.
- Ein Personenkreis SOLLTE benannt werden, der ausschließlich für das Thema Auswertung von Protokollierungsdaten verantwortlich ist.

## DER.1.A15 Zentrale Detektion und Echtzeitüberprüfung von Ereignismeldungen (H)

- Zentrale Komponenten SOLLTEN eingesetzt werden, um sicherheitsrelevante Ereignisse zu erkennen und auszuwerten.
- Zentrale, automatisierte Analysen mit Softwaremitteln SOLLTEN eingesetzt werden.
- Mit diesen zentrale, automatisierten Analysen mit Softwaremitteln SOLLTEN alle in der Systemumgebung anfallenden Ereignisse aufgezeichnet und in Bezug zueinander gesetzt werden.
- Die sicherheitsrelevante Vorgänge SOLLTEN sichtbar gemacht werden.
- Alle eingelieferten Daten SOLLTEN lückenlos in der Protokollverwaltung einsehbar und auswertbar sein.
- Die Daten SOLLTEN möglichst permanent ausgewertet werden.
- Werden definierte Schwellwerte überschritten, SOLLTE automatisch alarmiert werden.
- Das Personal SOLLTE sicherstellen, dass bei einem Alarm unverzüglich eine qualifizierte und dem Bedarf entsprechende Reaktion eingeleitet wird.
- In diesem Zusammenhang SOLLTE auch der betroffene Mitarbeiter sofort informiert werden.
- Die Systemverantwortlichen SOLLTEN regelmäßig die Analyseparameter auditieren und anpassen, falls dies erforderlich ist.
- Zusätzlich SOLLTEN bereits überprüfte Daten regelmäßig hinsichtlich sicherheitsrelevanter Ereignisse automatisch untersucht werden.

## DER.1.A16 Einsatz von Detektionssystemen nach Schutzbedarfsanforderungen (H)

- Anwendungen mit erhöhtem Schutzbedarf SOLLTEN durch zusätzliche Detektionsmaßnahmen geschützt werden.
- Dafür SOLLTEN z. B. solche Detektionssysteme eingesetzt werden, mit denen sich der erhöhte Schutzbedarf technisch auch sicherstellen lässt.

## DER.1.A17 Automatische Reaktion auf sicherheitsrelevante Ereignisse (H)

- Bei einem sicherheitsrelevanten Ereignis SOLLTEN die eingesetzten Detektionssysteme das Ereignis automatisch melden und mit geeigneten Schutzmaßnahmen reagieren.
- Hierbei SOLLTEN Verfahren eingesetzt werden, die automatisch mögliche Angriffe, Missbrauchsversuche oder Sicherheitsverletzungen erkennen.
- Es SOLLTE möglich sein, automatisch in den Datenstrom einzugreifen, um einen möglichen Sicherheitsvorfall zu unterbinden.

## DER.1.A18 Durchführung regelmäßiger Integritätskontrollen (H)

- Alle Detektionssysteme SOLLTEN regelmäßig daraufhin überprüft werden, ob sie noch integer sind.
- Auch SOLLTEN die Benutzerrechte kontrolliert werden.
- Zusätzlich SOLLTEN die Sensoren eine Integritätskontrolle von Dateien durchführen.
- Bei sich ändernden Werten SOLLTE eine automatische Alarmierung ausgelöst werden.


