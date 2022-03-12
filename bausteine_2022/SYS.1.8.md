# SYS.1.8: Speicherlösungen

## SYS.1.8.A1 Geeignete Aufstellung von Speichersystemen [Haustechnik] (B)

- Die IT-Komponenten von Speicherlösungen MÜSSEN in verschlossenen Räumen aufgestellt werden.
- Zu diesen Räumen DÜRFEN NUR Berechtigte Zutritt haben.
- Zudem MUSS eine sichere Stromversorgung sichergestellt sein.
- Die Herstellervorgaben zur empfohlenen Umgebungstemperatur und Luftfeuchte MÜSSEN eingehalten werden.

## SYS.1.8.A2 Sichere Grundkonfiguration von Speicherlösungen (B)

- Bevor eine Speicherlösung produktiv eingesetzt wird, MUSS sichergestellt sein, dass alle eingesetzten Softwarekomponenten und die Firmware aktuell sind.
- Danach MUSS eine sichere Grundkonfiguration hergestellt werden.
- Nicht genutzte Schnittstellen des Speichersystems MÜSSEN deaktiviert werden.
- Die Dateien zur Default-Konfiguration, zur vorgenommenen Grundkonfiguration und zur aktuellen Konfiguration SOLLTEN redundant und geschützt aufbewahrt werden.

## SYS.1.8.A3 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## SYS.1.8.A4 Schutz der Administrationsschnittstellen (B)

- Alle Administrations- und Management-Zugänge der Speichersysteme MÜSSEN eingeschränkt werden.
- Es MUSS sichergestellt sein, dass aus nicht-vertrauenswürdigen Netzen heraus nicht auf die Administrationsschnittstellen zugegriffen werden kann.
- Es SOLLTEN als sicher geltende Protokolle eingesetzt werden.
- Sollten dennoch unsichere Protokolle verwendet werden, MUSS für die Administration ein eigenes Administrationsnetz (siehe NET.1.1 Netzarchitektur und -design) genutzt werden.

## SYS.1.8.A5 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## SYS.1.8.A6 Erstellung einer Sicherheitsrichtlinie für Speicherlösungen (S)

- Ausgehend von der allgemeinen Sicherheitsrichtlinie der Institution SOLLTE eine spezifische Sicherheitsrichtlinie für Speicherlösungen erstellt werden.
- Darin SOLLTEN nachvollziehbar Vorgaben beschrieben sein, wie Speicherlösungen sicher geplant, administriert, installiert, konfiguriert und betrieben werden können.
- Die Richtlinie SOLLTE allen für Speicherlösungen zuständigen Administratoren bekannt und grundlegend für ihre Arbeit sein.
- Wird die Richtlinie verändert oder wird von den Vorgaben abgewichen, SOLLTE dies mit dem ISB abgestimmt und dokumentiert werden.
- Es SOLLTE regelmäßig überprüft werden, ob die Richtlinie noch korrekt umgesetzt ist.
- Gegebenenfalls SOLLTE sie aktualisiert werden.
- Die Ergebnisse SOLLTEN sinnvoll dokumentiert werden.

## SYS.1.8.A7 Planung von Speicherlösungen (S)

- Bevor Speicherlösungen in einer Institution eingesetzt werden, SOLLTE eine Anforderungsanalyse durchgeführt werden.
- In der Anforderungsanalyse SOLLTEN unter anderem die Themen Performance und Kapazität betrachtet werden.
- Auf Basis der ermittelten Anforderungen SOLLTE dann eine detaillierte Planung für Speicherlösungen erstellt werden.
- Darin SOLLTEN folgende Punkte berücksichtigt werden:
    - Auswahl von Herstellern und Lieferanten,
    - Entscheidung für oder gegen zentrale Verwaltungssysteme (Management-Systeme),
    - Planung des Netzanschlusses,
    - Planung der Infrastruktur sowie
    - Integration in bestehende Prozesse.

## SYS.1.8.A8 Auswahl einer geeigneten Speicherlösung (S)

- Die technischen Grundlagen unterschiedlicher Speicherlösungen SOLLTEN detailliert beleuchtet werden.
- Die Auswirkungen dieser technischen Grundlagen auf den möglichen Einsatz in der Institution SOLLTEN geprüft werden.
- Die Möglichkeiten und Grenzen der verschiedenen Speichersystemarten SOLLTEN für die Verantwortlichen der Institution transparent dargestellt werden.
- Die Entscheidungskriterien für eine Speicherlösung SOLLTEN nachvollziehbar dokumentiert werden.
- Ebenso SOLLTE die Entscheidung für die Auswahl einer Speicherlösung nachvollziehbar dokumentiert werden.

## SYS.1.8.A9 Auswahl von Lieferanten für eine Speicherlösung (S)

- Anhand der spezifizierten Anforderungen an eine Speicherlösung SOLLTE ein geeigneter Lieferant ausgewählt werden.
- Die Auswahlkriterien und die Entscheidung für einen Lieferanten SOLLTEN nachvollziehbar dokumentiert werden.
- Außerdem SOLLTEN Aspekte der Wartung und Instandhaltung schriftlich in sogenannten Service-Level-Agreements (SLAs) festgehalten werden.
- Die SLAs SOLLTEN eindeutig und quantifizierbar sein.
- Es SOLLTE genau geregelt werden, wann der Vertrag mit dem Lieferanten endet.

## SYS.1.8.A10 Erstellung und Pflege eines Betriebshandbuchs (S)

- Es SOLLTE ein Betriebshandbuch erstellt werden.
- Darin SOLLTEN alle Regelungen, Anforderungen und Einstellungen dokumentiert werden, die erforderlich sind, um Speicherlösungen zu betreiben.
- Das Betriebshandbuch SOLLTE regelmäßig aktualisiert werden.

## SYS.1.8.A11 Sicherer Betrieb einer Speicherlösung (S)

- Das Speichersystem SOLLTE hinsichtlich der Verfügbarkeit der internen Anwendungen, der Systemauslastung sowie kritischer Ereignisse überwacht werden.
- Weiterhin SOLLTEN für Speicherlösungen feste Wartungsfenster definiert werden, in denen Änderungen durchgeführt werden können.
- Insbesondere Firmware- oder Betriebssystemupdates von Speichersystemen oder den Netzkomponenten einer Speicherlösung SOLLTEN ausschließlich innerhalb eines solchen Wartungsfensters durchgeführt werden.

## SYS.1.8.A12 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.1.8.A13 Überwachung und Verwaltung von Speicherlösungen (S)

- Speicherlösungen SOLLTEN überwacht werden.
- Dabei SOLLTEN alle erhobenen Daten (Nachrichten) vorrangig daraufhin geprüft werden, ob die Vorgaben des Betriebshandbuchs eingehalten werden.
- Die wesentlichen Nachrichten SOLLTEN mit Nachrichtenfilter herausgefiltert werden.
- Einzelne Komponenten der Speicherlösung und des Gesamtsystems SOLLTEN zentral verwaltet werden.

## SYS.1.8.A14 Absicherung eines SANs durch Segmentierung (S)

- Ein SAN SOLLTE segmentiert werden.
- Es SOLLTE ein Konzept erarbeitet werden, das die SAN-Ressourcen den jeweiligen Servern zuordnet.
- Hierfür SOLLTE anhand der Sicherheitsanforderungen und des Administrationsaufwands entschieden werden, welche Segmentierung in welcher Implementierung (z. B. FC-SANs oder iSCSI-Speichernetze) eingesetzt werden soll.
- Die aktuelle Ressourcenzuordnung SOLLTE mithilfe von Verwaltungswerkzeugen einfach und übersichtlich erkennbar sein.
- Weiterhin SOLLTE die aktuelle Zoning-Konfiguration dokumentiert werden.
- Die Dokumentation SOLLTE auch in Notfällen verfügbar sein.

## SYS.1.8.A15 Sichere Trennung von Mandanten in Speicherlösungen (S)

- Es SOLLTE definiert und nachvollziehbar dokumentiert werden, welche Anforderungen die Institution an die Mandantenfähigkeit einer Speicherlösung stellt.
- Die eingesetzten Speicherlösungen SOLLTEN diese dokumentierten Anforderungen erfüllen.
- Im Block-Storage-Umfeld SOLLTE LUN Masking eingesetzt werden, um Mandanten voneinander zu trennen.
- In Fileservice-Umgebungen SOLLTE es möglich sein, mit virtuellen Fileservern zu agieren.
- Dabei SOLLTE jedem Mandanten ein eigener Fileservice zugeordnet werden.
- Beim Einsatz von IP oder iSCSI SOLLTEN die Mandanten über eine Segmentierung im Netz voneinander getrennt werden.
- Wird Fibre Channel eingesetzt, SOLLTE mithilfe von VSANs und Soft-Zoning separiert werden.

## SYS.1.8.A16 Sicheres Löschen in SAN-Umgebungen (S)

- In mandantenfähigen Speichersystemen SOLLTE sichergestellt werden, dass Logical Unit Numbers (LUNs), die einem bestimmten Mandanten zugeordnet sind, gelöscht werden.

## SYS.1.8.A17 Dokumentation der Systemeinstellungen von Speichersystemen (S)

- Alle Systemeinstellungen von Speichersystemen SOLLTEN dokumentiert werden.
- Die Dokumentation SOLLTE die technischen und organisatorischen Vorgaben sowie alle spezifischen Konfigurationen der Speichersysteme der Institution enthalten.
- Sofern die Dokumentation der Systemeinstellungen vertrauliche Informationen beinhaltet, SOLLTEN diese vor unberechtigtem Zugriff geschützt werden.
- Die Dokumentation SOLLTE regelmäßig überprüft werden.
- Sie SOLLTE immer aktuell sein.

## SYS.1.8.A18 Sicherheitsaudits und Berichtswesen bei Speichersystemen (S)

- Alle eingesetzten Speichersysteme SOLLTEN regelmäßig auditiert werden.
- Dafür SOLLTE ein entsprechender Prozess eingerichtet werden.
- Es SOLLTE geregelt werden, welche Sicherheitsreports mit welchen Inhalten regelmäßig zu erstellen sind.
- Zudem SOLLTE auch geregelt werden, wie mit Abweichungen von Vorgaben umgegangen wird und wie oft und in welcher Tiefe Audits durchgeführt werden.

## SYS.1.8.A19 Aussonderung von Speicherlösungen (S)

- Werden ganze Speicherlösungen oder einzelne Komponenten einer Speicherlösung nicht mehr benötigt, SOLLTEN alle darauf vorhandenen Daten auf andere Speicherlösungen übertragen werden.
- Hierfür SOLLTE eine Übergangsphase eingeplant werden.
- Anschließend SOLLTEN alle Nutzdaten und Konfigurationsdaten sicher gelöscht werden.
- Aus allen relevanten Dokumenten SOLLTEN alle Verweise auf die außer Betrieb genommene Speicherlösung entfernt werden.

## SYS.1.8.A20 Notfallvorsorge und Notfallreaktion für Speicherlösungen (S)

- Es SOLLTE ein Notfallplan für die eingesetzte Speicherlösung erstellt werden.
- Der Notfallplan SOLLTE genau beschreiben, wie in bestimmten Notfallsituationen vorzugehen ist.
- Auch SOLLTEN Handlungsanweisungen in Form von Maßnahmen und Kommandos enthalten sein, die die Fehleranalyse und Fehlerkorrektur unterstützen.
- Um Fehler zu beheben, SOLLTEN geeignete Werkzeuge eingesetzt werden.
- Regelmäßige Übungen und Tests SOLLTEN anhand des Notfallplans durchgeführt werden.
- Nach den Übungen und Tests sowie nach einem tatsächlichen Notfall SOLLTEN die dabei erzeugten Daten sicher gelöscht werden.

## SYS.1.8.A21 Einsatz von Speicherpools zur Mandantentrennung (H)

- Mandanten SOLLTEN Speicherressourcen aus unterschiedlichen sogenannten Speicherpools zugewiesen werden.
- Dabei SOLLTE ein Speichermedium immer nur einem einzigen Pool zugewiesen werden.
- Die logischen Festplatten (LUNs), die aus einem solchen Pool generiert werden, SOLLTEN nur einem einzigen Mandanten zugeordnet werden.

## SYS.1.8.A22 Einsatz einer hochverfügbaren SAN-Lösung (H)

- Eine hochverfügbare SAN-Lösung SOLLTE eingesetzt werden.
- Die eingesetzten Replikationsmechanismen SOLLTEN den Verfügbarkeitsanforderungen der Institution an die Speicherlösung entsprechen.
- Auch die Konfiguration der Speicherlösung SOLLTE den Verfügbarkeitsanforderungen gerecht werden.
- Außerdem SOLLTE ein Test- und Konsolidierungssystem vorhanden sein.

## SYS.1.8.A23 Einsatz von Verschlüsselung für Speicherlösungen (H)

- Alle in Speicherlösungen abgelegten Daten SOLLTEN verschlüsselt werden.
- Es SOLLTE festgelegt werden, auf welchen Ebenen (Data-in-Motion und Data-at-Rest) verschlüsselt wird.
- Dabei SOLLTE beachtet werden, dass die Verschlüsselung auf dem Transportweg auch bei Replikationen und Backup-Traffic relevant ist.

## SYS.1.8.A24 Sicherstellung der Integrität der SAN-Fabric (H)

- Um die Integrität der SAN-Fabric sicherzustellen, SOLLTEN Protokolle mit zusätzlichen Sicherheitsmerkmalen eingesetzt werden.
- Bei den folgenden Protokollen SOLLTEN deren Sicherheitseigenschaften berücksichtigt und entsprechende Konfigurationen verwendet werden:
    - Diffie Hellman Challenge Handshake Authentication Protocol (DH-CHAP),
    - Fibre Channel Authentication Protocol (FCAP) und
    - Fibre Channel Password Authentication Protocol (FCPAP).

## SYS.1.8.A25 Mehrfaches Überschreiben der Daten einer LUN (H)

- In SAN-Umgebungen SOLLTEN Daten gelöscht werden, indem die zugehörigen Speichersegmente einer LUN mehrfach überschrieben werden.

## SYS.1.8.A26 Absicherung eines SANs durch Hard-Zoning (H)

- Um SANs zu segmentieren, SOLLTE Hard-Zoning eingesetzt werden.


