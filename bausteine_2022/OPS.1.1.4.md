# OPS.1.1.4: Schutz vor Schadprogrammen

## OPS.1.1.4.A1 Erstellung eines Konzepts für den Schutz vor Schadprogrammen (B)

- Es MUSS ein Konzept erstellt werden, das beschreibt, welche IT-Systeme vor Schadprogrammen geschützt werden müssen.
- Hierbei MÜSSEN auch IoT-Geräte und Produktionssysteme berücksichtigt werden.
- Außerdem MUSS festgehalten werden, wie der Schutz zu erfolgen hat.
- Ist kein verlässlicher Schutz möglich, so SOLLTEN die identifizierten IT-Systeme NICHT betrieben werden.
- Das Konzept SOLLTE nachvollziehbar dokumentiert und aktuell gehalten werden.

## OPS.1.1.4.A2 Nutzung systemspezifischer Schutzmechanismen (B)

- Es MUSS geprüft werden, welche Schutzmechanismen die verwendeten IT-Systeme sowie die darauf genutzten Betriebssysteme und Anwendungen bieten.
- Diese Mechanismen MÜSSEN genutzt werden, sofern es keinen mindestens gleichwertigen Ersatz gibt oder gute Gründe dagegen sprechen.
- Werden sie nicht genutzt, MUSS dies begründet und dokumentiert werden.

## OPS.1.1.4.A3 Auswahl eines Virenschutzprogrammes (B)

- Abhängig vom verwendeten Betriebssystem, anderen vorhandenen Schutzmechanismen sowie der Verfügbarkeit geeigneter Virenschutzprogramme MUSS für den konkreten Einsatzzweck ein entsprechendes Schutzprogramm ausgewählt und installiert werden.
- Für Gateways und IT-Systeme, die dem Datenaustausch dienen, MUSS ein geeignetes Virenschutzprogramm ausgewählt und installiert werden.
- Es DÜRFEN NUR Produkte für den Enterprise-Bereich mit auf die Institution zugeschnittenen Service- und Supportleistungen eingesetzt werden.
- Produkte für reine Heimanwender oder Produkte ohne Herstellersupport DÜRFEN NICHT im professionellen Wirkbetrieb eingesetzt werden.
- Cloud-Dienste zur Verbesserung der Detektionsleistung der Virenschutzprogramme SOLLTEN genutzt werden.
- Falls Cloud-Funktionen solcher Produkte verwendet werden, MUSS sichergestellt werden, dass dies nicht im Widerspruch zum Daten- oder Geheimschutz steht.
- Neben Echtzeit- und On-Demand-Scans MUSS eine eingesetzte Lösung die Möglichkeit bieten, auch komprimierte Daten nach Schadprogrammen zu durchsuchen.

## OPS.1.1.4.A4 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## OPS.1.1.4.A5 Betrieb und Konfiguration von Virenschutzprogrammen (B)

- Das Virenschutzprogramm MUSS für seine Einsatzumgebung geeignet konfiguriert werden.
- Die Erkennungsleistung SOLLTE dabei im Vordergrund stehen, sofern nicht Datenschutz- oder Leistungsgründe im jeweiligen Einzelfall dagegen sprechen.
- Wenn sicherheitsrelevante Funktionen des Virenschutzprogramms nicht genutzt werden, SOLLTE dies begründet und dokumentiert werden.
- Bei Schutzprogrammen, die speziell für die Desktop-Virtualisierung optimiert sind, SOLLTE nachvollziehbar dokumentiert sein, ob auf bestimmte Detektionsverfahren zugunsten der Leistung verzichtet wird.
- Es MUSS sichergestellt werden, dass die Benutzer keine sicherheitsrelevanten Änderungen an den Einstellungen der Antivirenprogramme vornehmen können.

## OPS.1.1.4.A6 Regelmäßige Aktualisierung der eingesetzten Virenschutzprogramme und Signaturen (B)

- Auf den damit ausgestatteten IT-Systemen MÜSSEN die Scan-Engine des Virenschutzprogramms sowie die Signaturen für die Schadprogramme regelmäßig und zeitnah aktualisiert werden.

## OPS.1.1.4.A7 Sensibilisierung und Verpflichtung der Benutzer [Benutzer] (B)

- Benutzer MÜSSEN regelmäßig über die Bedrohung durch Schadprogramme aufgeklärt werden.
- Sie MÜSSEN die grundlegenden Verhaltensregeln einhalten, um die Gefahr eines Befalls durch Schadprogramme zu reduzieren.
- Dateien, E-Mails, Webseiten usw. aus nicht vertrauenswürdigen Quellen SOLLTEN NICHT geöffnet werden.
- Benutzern MÜSSEN entsprechende Ansprechpartner für den Fall eines Verdacht auf eine Infektion mit einem Schadprogramm bekannt sein.
- Benutzer MÜSSEN sich an die ihnen benannten Ansprechpartner wenden, wenn der Verdacht auf eine Infektion mit einem Schadprogramm besteht.

## OPS.1.1.4.A8 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## OPS.1.1.4.A9 Meldung von Infektionen mit Schadprogrammen [Benutzer] (S)

- Das eingesetzte Virenschutzprogramm SOLLTE eine Infektion mit einem Schadprogramm automatisch blockieren und melden.
- Die automatische Meldung SOLLTE an einer zentralen Stelle angenommen werden.
- Dabei SOLLTEN die zuständigen Mitarbeiter je nach Sachlage über das weitere Vorgehen entscheiden.
- Das Vorgehen bei Meldungen und Alarmen der Virenschutzprogramme SOLLTE geplant, dokumentiert und getestet werden.
- Es SOLLTE insbesondere geregelt sein, was im Falle einer bestätigten Infektion geschehen soll.

## OPS.1.1.4.A10 Nutzung spezieller Analyseumgebungen (H)

- Automatisierte Analysen in einer speziellen Testumgebung (basierend auf Sandboxen bzw. separaten virtuellen oder physischen Systemen) SOLLTEN für eine Bewertung von verdächtigen Dateien ergänzend herangezogen werden.

## OPS.1.1.4.A11 Einsatz mehrerer Scan-Engines (H)

- Zur Verbesserung der Erkennungsleistung SOLLTEN für besonders schutzwürdige IT-Systeme, wie Gateways und ITSysteme zum Datenaustausch, Virenschutzprogramme mit mehreren alternativen Scan-Engines eingesetzt werden.

## OPS.1.1.4.A12 Einsatz von Datenträgerschleusen (H)

- Bevor insbesondere Datenträger von Dritten mit den IT-Systemen der Institution verbunden werden, SOLLTEN diese durch eine Datenträgerschleuse geprüft werden.

## OPS.1.1.4.A13 Umgang mit nicht vertrauenswürdigen Dateien (H)

- Ist es notwendig, nicht vertrauenswürdige Dateien zu öffnen, SOLLTE dies nur auf einem isolierten IT-System geschehen.
- Die betroffenen Dateien SOLLTEN dort z. B. in ein ungefährliches Format umgewandelt oder ausgedruckt werden, wenn sich hierdurch das Risiko einer Infektion durch Schadsoftware verringert.

## OPS.1.1.4.A14 Auswahl und Einsatz von Cyber-Sicherheitsprodukten gegen gezielte Angriffe (H)

- Der Einsatz sowie der Mehrwert von Produkten und Services, die im Vergleich zu herkömmlichen Virenschutzprogrammen einen erweiterten Schutzumfang bieten, SOLLTE geprüft werden.
- Solche Sicherheitsprodukte gegen gezielte Angriffe SOLLTEN z. B. bei der Ausführung von Dateien in speziellen Analyseumgebungen, bei der Härtung von Clients oder bei der Kapselung von Prozessen eingesetzt werden.
- Vor einer Kaufentscheidung für ein Sicherheitsprodukt SOLLTEN Schutzwirkung und Kompatibilität zur eigenen IT-Umgebung getestet werden.


