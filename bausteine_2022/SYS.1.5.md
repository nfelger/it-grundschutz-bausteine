# SYS.1.5: Virtualisierung

## SYS.1.5.A1 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## SYS.1.5.A2 Sicherer Einsatz virtueller IT-Systeme (B)

- Jeder Administrator von virtuellen IT-Systemen MUSS wissen, wie sich eine Virtualisierung auf die betriebenen ITSysteme und Anwendungen auswirkt.
- Die Zugriffsrechte für Administratoren auf virtuelle IT-Systeme MÜSSEN auf das tatsächlich notwendige Maß reduziert sein.
- Es MUSS gewährleistet sein, dass die für die virtuellen IT-Systeme notwendigen Netzverbindungen in der virtuellen Infrastruktur verfügbar sind.
- Auch MUSS geprüft werden, ob die Anforderungen an die Isolation und Kapselung der virtuellen IT-Systeme sowie der darauf betriebenen Anwendungen hinreichend erfüllt sind.
- Weiterhin MÜSSEN die eingesetzten virtuellen IT-Systeme den Anforderungen an die Verfügbarkeit und den Datendurchsatz genügen.
- Im laufenden Betrieb MUSS die Performance der virtuellen IT-Systeme überwacht werden.

## SYS.1.5.A3 Sichere Konfiguration virtueller IT-Systeme (B)

- Gast-Systeme DÜRFEN NICHT auf Geräte und Schnittstellen des Virtualisierungsservers zugreifen.
- Ist eine solche Verbindung jedoch notwendig, MUSS diese exklusiv zugeteilt werden.
- Sie DARF NUR für die notwendige Dauer vom Administrator des Host-Systems hergestellt werden.
- Dafür MÜSSEN verbindliche Regelungen festgelegt werden.
- Virtuelle IT-Systeme SOLLTEN nach den Sicherheitsrichtlinien der Institution konfiguriert und geschützt werden.

## SYS.1.5.A4 Sichere Konfiguration eines Netzes für virtuelle Infrastrukturen (B)

- Es MUSS sichergestellt werden, dass bestehende Sicherheitsmechanismen (z. B. Firewalls) und Monitoring-Systeme nicht über virtuelle Netze umgangen werden können.
- Auch MUSS ausgeschlossen sein, dass über virtuelle IT-Systeme, die mit mehreren Netzen verbunden sind, unerwünschte Netzverbindungen aufgebaut werden können.
- Netzverbindungen zwischen virtuellen IT-Systemen und physischen IT-Systemen sowie für virtuelle Firewalls SOLLTEN gemäß den Sicherheitsrichtlinien der Institution konfiguriert werden.

## SYS.1.5.A5 Schutz der Administrationsschnittstellen (B)

- Alle Administrations- und Management-Zugänge zum Managementsystem und zu den Host-Systemen MÜSSEN eingeschränkt werden.
- Es MUSS sichergestellt sein, dass aus nicht-vertrauenswürdigen Netzen heraus nicht auf die Administrationsschnittstellen zugegriffen werden kann.
- Um die Virtualisierungsserver oder die Managementsysteme zu administrieren bzw. zu überwachen, SOLLTEN als sicher geltende Protokolle eingesetzt werden.
- Sollte dennoch auf unsichere Protokolle zurückgegriffen werden, MUSS für die Administration ein eigenes Administrationsnetz genutzt werden.

## SYS.1.5.A6 Protokollierung in der virtuellen Infrastruktur (B)

- Betriebszustand, Auslastung und Netzanbindungen der virtuellen Infrastruktur MÜSSEN laufend protokolliert werden.
- Werden Kapazitätsgrenzen erreicht, SOLLTEN virtuelle Maschinen verschoben werden.
- Zudem SOLLTE eventuell die Hardware erweitert werden.
- Auch MUSS überwacht werden, ob die virtuellen Netze den jeweiligen virtuellen IT-Systemen korrekt zugeordnet sind.

## SYS.1.5.A7 Zeitsynchronisation in virtuellen IT-Systemen (B)

- Die Systemzeit aller produktiv eingesetzten virtuellen IT-Systeme MUSS immer synchron sein.

## SYS.1.5.A8 Planung einer virtuellen Infrastruktur [Planer] (S)

- Der Aufbau der virtuellen Infrastruktur SOLLTE detailliert geplant werden.
- Dabei SOLLTEN die geltenden Regelungen und Richtlinien für den Betrieb von IT-Systemen, Anwendungen und Netzen (inklusive Speichernetzen) berücksichtigt werden.
- Wenn mehrere virtuelle IT-Systeme auf einem Virtualisierungsserver betrieben werden, SOLLTEN KEINE Konflikte hinsichtlich des Schutzbedarfs der IT-Systeme auftreten.
- Weiterhin SOLLTEN die Aufgaben der einzelnen Administratorengruppen festgelegt und klar voneinander abgegrenzt werden.
- Es SOLLTE auch geregelt werden, welcher Mitarbeiter für den Betrieb welcher Komponente verantwortlich ist.

## SYS.1.5.A9 Netzplanung für virtuelle Infrastrukturen [Planer] (S)

- Der Aufbau des Netzes für virtuelle Infrastrukturen SOLLTE detailliert geplant werden.
- Auch SOLLTE geprüft werden, ob für bestimmte Virtualisierungsfunktionen (wie z. B. die Live-Migration) ein eigenes Netz aufgebaut und genutzt werden muss.
- Es SOLLTE geplant werden, welche Netzsegmente aufgebaut werden müssen (z. B. Managementnetz, Speichernetz).
- Es SOLLTE festgelegt werden, wie die Netzsegmente sich sicher voneinander trennen und schützen lassen.
- Dabei SOLLTE sichergestellt werden, dass das produktive Netz vom Managementnetz getrennt ist (siehe SYS.1.5.A11 Administration der Virtualisierungsinfrastruktur über ein gesondertes Managementnetz).
- Auch die Verfügbarkeitsanforderungen an das Netz SOLLTEN erfüllt werden.

## SYS.1.5.A10 Einführung von Verwaltungsprozessen für virtuelle IT-Systeme (S)

- Für Virtualisierungsserver und virtuelle IT-Systeme SOLLTEN Prozesse für die Inbetriebnahme, die Inventarisierung, den Betrieb und die Außerbetriebnahme definiert und etabliert werden.
- Die Prozesse SOLLTEN dokumentiert und regelmäßig aktualisiert werden.
- Wenn der Einsatz von virtuellen IT-Systemen geplant wird, SOLLTE festgelegt werden, welche Virtualisierungsfunktionen die virtuellen IT-Systeme benutzen dürfen.
- Test- und Entwicklungsumgebungen SOLLTEN NICHT auf demselben Virtualisierungsserver betrieben werden wie produktive virtuelle IT-Systeme.

## SYS.1.5.A11 Administration der Virtualisierungsinfrastruktur über ein gesondertes Managementnetz (S)

- Die Virtualisierungsinfrastruktur SOLLTE ausschließlich über ein separates Managementnetz administriert werden (siehe NET.1.1 Netzarchitektur und -design).
- Die verfügbaren Sicherheitsmechanismen der eingesetzten Managementprotokolle zur Authentisierung, Integritätssicherung und Verschlüsselung SOLLTEN aktiviert werden.
- Alle unsicheren Managementprotokolle SOLLTEN deaktiviert werden (siehe NET.1.2 Netzmanagement).

## SYS.1.5.A12 Rechte- und Rollenkonzept für die Administration einer virtuellen Infrastruktur (S)

- Anhand der in der Planung definierten Aufgaben und Rollen (siehe SYS.1.5.A8 Planung einer virtuellen Infrastruktur) SOLLTE für die Administration der virtuellen IT-Systeme und Netze sowie der Virtualisierungsserver und der Managementumgebung ein Rechte- und Rollenkonzept erstellt und umgesetzt werden.
- Alle Komponenten der virtuellen Infrastruktur SOLLTEN in ein zentrales Identitäts- und Berechtigungsmanagement eingebunden werden.
- Administratoren von virtuellen Maschinen und Administratoren der Virtualisierungsumgebung SOLLTEN unterschieden werden.
- Sie SOLLTEN mit unterschiedlichen Zugriffsrechten ausgestattet werden.
- Weiterhin SOLLTE die Managementumgebung virtuelle Maschinen zur geeigneten Strukturierung gruppieren können.
- Die Rollen der Administratoren SOLLTEN entsprechend zugeteilt werden.

## SYS.1.5.A13 Auswahl geeigneter Hardware für Virtualisierungsumgebungen (S)

- Die verwendete Hardware SOLLTE kompatibel mit der eingesetzten Virtualisierungslösung sein.
- Dabei SOLLTE darauf geachtet werden, dass der Hersteller der Virtualisierungslösung über den geplanten Einsatzzeitraum auch Support für die betriebene Hardware anbietet.

## SYS.1.5.A14 Einheitliche Konfigurationsstandards für virtuelle IT-Systeme (S)

- Für die eingesetzten virtuellen IT-Systeme SOLLTEN einheitliche Konfigurationsstandards definiert werden.
- Die virtuellen IT-Systeme SOLLTEN nach diesen Standards konfiguriert werden.
- Die Konfigurationsstandards SOLLTEN regelmäßig überprüft werden.
- Sie SOLLTEN, falls erforderlich, angepasst werden.

## SYS.1.5.A15 Betrieb von Gast-Betriebssystemen mit unterschiedlichem Schutzbedarf (S)

- Falls virtuelle IT-Systeme mit unterschiedlichem Schutzbedarf gemeinsam auf einem Virtualisierungsserver betrieben werden, SOLLTE dabei sichergestellt sein, dass die virtuellen IT-Systeme ausreichend gekapselt und voneinander isoliert sind.
- Auch SOLLTE dann die Netztrennung in der eingesetzten Virtualisierungslösung ausreichend sicher sein.
- Ist das nicht der Fall, SOLLTEN weitergehende Sicherheitsmaßnahmen identifiziert und umgesetzt werden.

## SYS.1.5.A16 Kapselung der virtuellen Maschinen (S)

- Die Funktionen „Kopieren“ und „Einfügen“ von Informationen zwischen virtuellen Maschinen SOLLTEN deaktiviert sein.

## SYS.1.5.A17 Überwachung des Betriebszustands und der Konfiguration der virtuellen Infrastruktur (S)

- Der Betriebszustand der virtuellen Infrastruktur SOLLTE überwacht werden.
- Dabei SOLLTE unter anderem geprüft werden, ob noch ausreichend Ressourcen verfügbar sind.
- Es SOLLTE auch geprüft werden, ob es eventuell Konflikte bei gemeinsam genutzten Ressourcen eines Virtualisierungsservers gibt.
- Weiterhin SOLLTEN die Konfigurationsdateien der virtuellen IT-Systeme regelmäßig auf unautorisierte Änderungen überprüft werden.
- Wird die Konfiguration der Virtualisierungsinfrastruktur geändert, SOLLTEN die Änderungen geprüft und getestet werden, bevor sie umgesetzt werden.

## SYS.1.5.A18 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.1.5.A19 Regelmäßige Audits der Virtualisierungsinfrastruktur (S)

- Es SOLLTE regelmäßig auditiert werden, ob der Ist-Zustand der virtuellen Infrastruktur dem in der Planung festgelegten Zustand entspricht.
- Auch SOLLTE regelmäßig auditiert werden, ob die Konfiguration der virtuellen Komponenten die vorgegebene Standardkonfiguration einhält.
- Die Auditergebnisse SOLLTEN nachvollziehbar dokumentiert werden.
- Abweichungen SOLLTEN behoben werden.

## SYS.1.5.A20 Verwendung von hochverfügbaren Architekturen [Planer] (H)

- Die virtuelle Infrastruktur SOLLTE hochverfügbar ausgelegt werden.
- Alle Virtualisierungsserver SOLLTEN in Clustern zusammengeschlossen werden.

## SYS.1.5.A21 Sichere Konfiguration virtueller IT-Systeme bei erhöhtem Schutzbedarf (H)

- Für virtuelle IT-Systeme SOLLTEN Überbuchungsfunktionen für Ressourcen deaktiviert werden.

## SYS.1.5.A22 Härtung des Virtualisierungsservers (H)

- Der Virtualisierungsserver SOLLTE gehärtet werden.
- Um virtuelle IT-Systeme voreinander und gegenüber dem Virtualisierungsserver zusätzlich zu isolieren und zu kapseln, SOLLTEN Mandatory Access Controls (MACs) eingesetzt werden.
- Ebenso SOLLTE das IT-System, auf dem die Management-Software installiert ist, gehärtet werden.

## SYS.1.5.A23 Rechte-Einschränkung der virtuellen Maschinen (H)

- Alle Schnittstellen und Kommunikationskanäle, die es einem virtuellen IT-System erlauben, Informationen über das Host-System auszulesen und abzufragen, SOLLTEN deaktiviert sein oder unterbunden werden.
- Weiterhin SOLLTE ausschließlich der Virtualisierungsserver auf seine Ressourcen zugreifen können.
- Virtuelle IT-Systeme SOLLTEN NICHT die sogenannten Pages des Arbeitsspeichers teilen.

## SYS.1.5.A24 Deaktivierung von Snapshots virtueller IT-Systeme (H)

- Für alle virtuellen IT-Systeme SOLLTE die Snapshot-Funktion deaktiviert werden.

## SYS.1.5.A25 Minimale Nutzung von Konsolenzugriffen auf virtuelle IT-Systeme (H)

- Direkte Zugriffe auf die emulierten Konsolen virtueller IT-Systeme SOLLTEN auf ein Mindestmaß reduziert werden.
- Die virtuellen IT-Systeme SOLLTEN möglichst über das Netz gesteuert werden.

## SYS.1.5.A26 Einsatz einer PKI [Planer] (H)

- Für die mit Zertifikaten geschützte Kommunikation zwischen den Komponenten der IT-Infrastruktur SOLLTE eine Public-Key-Infrastruktur (PKI) eingesetzt werden.

## SYS.1.5.A27 Einsatz zertifizierter Virtualisierungssoftware (H)

- Es SOLLTE zertifizierte Virtualisierungssoftware der Stufe EAL 4 oder höher eingesetzt werden.

## SYS.1.5.A28 Verschlüsselung von virtuellen IT-Systemen (H)

- Alle virtuellen IT-Systeme SOLLTEN verschlüsselt werden.


