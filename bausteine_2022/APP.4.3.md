# APP.4.3: Relationale Datenbanken

## APP.4.3.A1 Erstellung einer Sicherheitsrichtlinie für Datenbanksysteme (B)

- Ausgehend von der allgemeinen Sicherheitsrichtlinie der Institution MUSS eine spezifische Sicherheitsrichtlinie für Datenbanksysteme erstellt werden.
- Darin MÜSSEN nachvollziehbar Anforderungen und Vorgaben beschrieben sein, wie Datenbanksysteme sicher betrieben werden sollen.
- Die Richtlinie MUSS allen im Bereich Datenbanksysteme zuständigen Mitarbeitern bekannt sein.
- Sie MUSS grundlegend für ihre Arbeit sein.
- Wird die Richtlinie verändert oder wird von den Anforderungen abgewichen, MUSS dies mit dem ISB abgestimmt und dokumentiert werden.
- Es MUSS regelmäßig überprüft werden, ob die Richtlinie noch korrekt umgesetzt ist.
- Die Ergebnisse MÜSSEN sinnvoll dokumentiert werden.

## APP.4.3.A2 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.4.3.A3 Basishärtung des Datenbankmanagementsystems (B)

- Das Datenbankmanagementsystem MUSS gehärtet werden.
- Hierfür MUSS eine Checkliste mit den durchzuführenden Schritten zusammengestellt und abgearbeitet werden.
- Passwörter DÜRFEN NICHT im Klartext gespeichert werden.
- Die Basishärtung MUSS regelmäßig überprüft und, falls erforderlich, angepasst werden.

## APP.4.3.A4 Geregeltes Anlegen neuer Datenbanken (B)

- Neue Datenbanken MÜSSEN nach einem definierten Prozess angelegt werden.
- Wenn eine neue Datenbank angelegt wird, MÜSSEN Grundinformationen zur Datenbank nachvollziehbar dokumentiert werden.

## APP.4.3.A5 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.4.3.A6 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.4.3.A7 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.4.3.A8 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.4.3.A9 Datensicherung eines Datenbanksystems (B)

- Es MÜSSEN regelmäßig Systemsicherungen des DBMS und der Daten durchgeführt werden.
- Auch bevor eine Datenbank neu erzeugt wird, MUSS das Datenbanksystem gesichert werden.
- Hierfür SOLLTEN die dafür zulässigen Dienstprogramme benutzt werden.
- Alle Transaktionen SOLLTEN so gesichert werden, dass sie jederzeit wiederherstellbar sind.
- Wenn die Datensicherung die verfügbaren Kapazitäten übersteigt, SOLLTE ein erweitertes Konzept erstellt werden, um die Datenbank zu sichern, z. B. eine inkrementelle Sicherung.
- Abhängig vom Schutzbedarf der Daten SOLLTEN die Wiederherstellungsparameter vorgegeben werden (siehe CON.3 Datensicherungskonzept).

## APP.4.3.A10 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.4.3.A11 Ausreichende Dimensionierung der Hardware [Fachverantwortliche] (S)

- Datenbankmanagementsysteme SOLLTEN auf ausreichend dimensionierter Hardware installiert werden.
- Die Hardware SOLLTE über genügend Reserven verfügen, um auch eventuell steigenden Anforderungen gerecht zu werden.
- Zeichnen sich trotzdem während des Betriebs Ressourcenengpässe ab, SOLLTEN diese frühzeitig behoben werden.
- Wenn die Hardware dimensioniert wird, SOLLTE das erwartete Wachstum für den geplanten Einsatzzeitraum berücksichtigt werden.

## APP.4.3.A12 Einheitlicher Konfigurationsstandard von Datenbankmanagementsystemen (S)

- Für alle eingesetzten Datenbankmanagementsysteme SOLLTE ein einheitlicher Konfigurationsstandard definiert werden.
- Alle Datenbankmanagementsysteme SOLLTEN nach diesem Standard konfiguriert und einheitlich betrieben werden.
- Falls es bei einer Installation notwendig ist, vom Konfigurationsstandard abzuweichen, SOLLTEN alle Schritte vom ISB freigegeben und nachvollziehbar dokumentiert werden.
- Der Konfigurationsstandard SOLLTE regelmäßig überprüft und, falls erforderlich, angepasst werden.

## APP.4.3.A13 Restriktive Handhabung von Datenbank-Links (S)

- Es SOLLTE sichergestellt sein, dass nur Verantwortliche dazu berechtigt sind, Datenbank-Links (DB-Links) anzulegen.
- Werden solche Links angelegt, MÜSSEN so genannte Private DB-Links vor Public DB-Links bevorzugt angelegt werden.
- Alle von den Verantwortlichen angelegten DB-Links SOLLTEN dokumentiert und regelmäßig überprüft werden.
- Zudem SOLLTEN DB-Links mitberücksichtigt werden, wenn das Datenbanksystem gesichert wird (siehe APP.4.3.A9 Datensicherung eines Datenbanksystems).

## APP.4.3.A14 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.4.3.A15 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.4.3.A16 Verschlüsselung der Datenbankanbindung (S)

- Das Datenbankmanagementsystem SOLLTE so konfiguriert werden, dass Datenbankverbindungen immer verschlüsselt werden.
- Die dazu eingesetzten kryptografischen Verfahren und Protokolle SOLLTEN den internen Vorgaben der Institution entsprechen (siehe CON.1 Kryptokonzept).

## APP.4.3.A17 Datenübernahme oder Migration [Fachverantwortliche] (S)

- Es SOLLTE vorab definiert werden, wie initial oder regelmäßig Daten in eine Datenbank übernommen werden sollen.
- Nachdem Daten übernommen wurden, SOLLTE geprüft werden, ob sie vollständig und unverändert sind.

## APP.4.3.A18 Überwachung des Datenbankmanagementsystems (S)

- Die für den sicheren Betrieb kritischen Parameter, Ereignisse und Betriebszustände des Datenbankmanagementsystems SOLLTEN definiert werden.
- Diese SOLLTEN mithilfe eines Monitoring-Systems überwacht werden.
- Für alle kritischen Parameter, Ereignisse und Betriebszustände SOLLTEN Schwellwerte festgelegt werden.
- Wenn diese Werte überschritten werden, MUSS geeignet reagiert werden.
- Hierbei SOLLTEN die zuständigen Mitarbeiter alarmiert werden.
- Anwendungsspezifische Parameter, Ereignisse, Betriebszustände und deren Schwellwerte SOLLTEN mit den Verantwortlichen für die Fachanwendungen abgestimmt werden.

## APP.4.3.A19 Schutz vor schädlichen Datenbank-Skripten [Entwickler] (S)

- Werden Datenbank-Skripte entwickelt, SOLLTEN dafür verpflichtende Qualitätskriterien definiert werden (siehe CON.8 Software-Entwicklung).
- Datenbank-Skripte SOLLTEN ausführlichen Funktionstests auf gesonderten Testsystemen unterzogen werden, bevor sie produktiv eingesetzt werden.
- Die Ergebnisse SOLLTEN dokumentiert werden.

## APP.4.3.A20 Regelmäßige Audits (S)

- Bei allen Komponenten des Datenbanksystems SOLLTE regelmäßig überprüft werden, ob alle festgelegten Sicherheitsmaßnahmen umgesetzt und diese korrekt konfiguriert sind.
- Dabei SOLLTE geprüft werden, ob der dokumentierte Stand dem Ist-Zustand entspricht und ob die Konfiguration des Datenbankmanagementsystems der dokumentierten Standardkonfiguration entspricht.
- Zudem SOLLTE geprüft werden, ob alle Datenbank-Skripte benötigt werden.
- Auch SOLLTE geprüft werden, ob sie dem Qualitätsstandard der Institution genügen.
- Zusätzlich SOLLTEN die Protokolldateien des Datenbanksystems und des Betriebssystems nach Auffälligkeiten untersucht werden (siehe DER.1 Detektion von sicherheitsrelevanten Ereignissen).
- Die Auditergebnisse SOLLTEN nachvollziehbar dokumentiert sein.
- Sie SOLLTEN mit dem Soll-Zustand abgeglichen werden.
- Abweichungen SOLLTE nachgegangen werden.

## APP.4.3.A21 Einsatz von Datenbank Security Tools (H)

- Es SOLLTEN Informationssicherheitsprodukte für Datenbanken eingesetzt werden.
- Die eingesetzten Produkte SOLLTEN folgende Funktionen bereitstellen:
    - Erstellung einer Übersicht über alle Datenbanksysteme,
    - erweiterte Konfigurationsmöglichkeiten und Rechtemanagement der Datenbanken,
    - Erkennung und Unterbindung von möglichen Angriffen (z. B. Brute Force Angriffe auf ein Benutzerkonto, SQLInjection) und
    - Auditfunktionen (z. B. Überprüfung von Konfigurationsvorgaben).

## APP.4.3.A22 Notfallvorsorge (H)

- Für das Datenbankmanagementsystem SOLLTE ein Notfallplan erstellt werden, der festlegt, wie ein Notbetrieb realisiert werden kann.
- Die für den Notfallplan notwendigen Ressourcen SOLLTEN ermittelt werden.
- Zusätzlich SOLLTE der Notfallplan definieren, wie aus dem Notbetrieb der Regelbetrieb wiederhergestellt werden kann.
- Der Notfallplan SOLLTE die nötigen Meldewege, Reaktionswege, Ressourcen und Reaktionszeiten der Fachverantwortlichenfestlegen.
- Auf Basis eines Koordinationsplans zum Wiederanlauf SOLLTEN alle von der Datenbank abhängigen ITSysteme vorab ermittelt und berücksichtigt werden.

## APP.4.3.A23 Archivierung (H)

- Ist es erforderlich, Daten eines Datenbanksystems zu archivieren, SOLLTE ein entsprechendes Archivierungskonzept erstellt werden.
- Es SOLLTE sichergestellt sein, dass die Datenbestände zu einem späteren Zeitpunkt wieder vollständig und konsistent verfügbar sind.
- Im Archivierungskonzept SOLLTEN sowohl die Intervalle der Archivierung als auch die Vorhaltefristen der archivierten Daten festgelegt werden.
- Zusätzlich SOLLTE dokumentiert werden, mit welcher Technik die Datenbanken archiviert wurden.
- Mit den archivierten Daten SOLLTEN regelmäßig Wiederherstellungstests durchgeführt werden.
- Die Ergebnisse SOLLTEN dokumentiert werden.

## APP.4.3.A24 Datenverschlüsselung in der Datenbank (H)

- Die Daten in den Datenbanken SOLLTEN verschlüsselt werden.
- Dabei SOLLTEN vorher unter anderem folgende Faktoren betrachtet werden:
    - Einfluss auf die Performance,
    - Schlüsselverwaltungsprozesse und -verfahren, einschließlich separater Schlüsselaufbewahrung und -sicherung,
    - Einfluss auf Backup-Recovery-Konzepte,
    - funktionale Auswirkungen auf die Datenbank, beispielsweise Sortiermöglichkeiten.

## APP.4.3.A25 Sicherheitsprüfungen von Datenbanksystemen (H)

- Datenbanksysteme SOLLTEN regelmäßig mithilfe von Sicherheitsprüfungen kontrolliert werden.
- Bei den Sicherheitsprüfungen SOLLTEN die systemischen und herstellerspezifischen Aspekte der eingesetzten Datenbank-Infrastruktur (z. B. Verzeichnisdienste) sowie des eingesetzten Datenbankmanagementsystems betrachtet werden.


