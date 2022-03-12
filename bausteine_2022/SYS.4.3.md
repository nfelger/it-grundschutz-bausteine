# SYS.4.3: Eingebettete Systeme

## SYS.4.3.A1 Regelungen zum Umgang mit eingebetteten Systemen (B)

- Um eingebettete Systeme reibungslos zu betreiben, MÜSSEN Zuständige ernannt werden.
- Alle Benutzer und Administratoren MÜSSEN über Verhaltensregeln und Meldewege bei Ausfällen, Fehlfunktionen oder bei Verdacht auf einen Sicherheitsvorfall informiert sein.
- Die eingebetteten Systeme MÜSSEN sicher vorkonfiguriert werden.
- Die vorgenommene Konfiguration SOLLTE dokumentiert sein.
- Weiterhin SOLLTEN Regelungen festgelegt werden, um die Integrität und Funktionsfähigkeit zu testen.

## SYS.4.3.A2 Deaktivieren nicht benutzter Schnittstellen und Dienste bei eingebetteten Systemen [Entwickler] (B)

- Es MUSS sichergestellt werden, dass nur auf benötigte Schnittstellen zugegriffen werden kann.
- Zudem DÜRFEN NUR benötigte Dienste aktiviert sein.
- Der Zugang zu Anwendungsschnittstellen MUSS durch sichere Authentisierung geschützt sein.

## SYS.4.3.A3 Protokollierung sicherheitsrelevanter Ereignisse bei eingebetteten Systemen (B)

- Sicherheitsverstöße MÜSSEN protokolliert werden (siehe OPS.1.1.5 Protokollierung).
- Ist eine elektronische Protokollierung nicht oder nur sehr begrenzt realisierbar, SOLLTEN alternative, organisatorische Regelungen geschaffen und umgesetzt werden.

## SYS.4.3.A4 Erstellung von Beschaffungskriterien für eingebettete Systeme [Beschaffungsstelle] (S)

- Bevor eingebettete Systeme beschafft werden, SOLLTE eine Anforderungsliste erstellt werden, anhand derer die infrage kommenden Systeme oder Komponenten bewertet werden.
- Die Anforderungsliste SOLLTE mindestens folgende sicherheitsrelevante Aspekte umfassen:
    - Aspekte der materiellen Sicherheit,
    - Anforderungen an die Sicherheitseigenschaften der Hardware,
    - Anforderungen an die Sicherheitseigenschaften der Software,
    - Unterstützung eines Trusted Plattform Module (TPM) durch das Betriebssystem,
    - Sicherheitsaspekte der Entwicklungsumgebung sowie
    - organisatorische Sicherheitsaspekte.

## SYS.4.3.A5 Schutz vor schädigenden Umwelteinflüssen bei eingebetteten Systemen [Entwickler, Planer] (S)

- Es SOLLTE sichergestellt werden, dass eingebettete Systeme entsprechend ihrer vorgesehenen Einsatzart und des vorgesehenen Einsatzorts angemessen vor schädigenden Umwelteinflüssen geschützt sind.
- Die Anforderungen hierfür SOLLTEN bereits bei der Planung analysiert werden.
- Zudem SOLLTE sichergestellt werden, dass die Vorkehrungen, um einzelne Komponenten vor Staub und Verschmutzung zu schützen, sich mit den Anforderungen des übergeordneten Systems vertragen.

## SYS.4.3.A6 Verhindern von Debugging-Möglichkeiten bei eingebetteten Systemen [Entwickler] (S)

- Eventuelle Debugging-Möglichkeiten SOLLTEN möglichst vollständig aus eingebetteten Systemen entfernt werden.
- Wird On-Chip-Debugging genutzt, MUSS sichergestellt werden, dass Debugging-Funktionen nicht unberechtigt genutzt oder aktiviert werden können.
- Weiterhin SOLLTE sichergestellt werden, dass keine Eingabeschnittstellen für Testsignale und Messpunkte zum Anschluss von Analysatoren aktiviert bzw. für Unberechtigte nutzbar sind.
- Zudem SOLLTEN alle Hardware-DebuggingSchnittstellen deaktiviert sein.

## SYS.4.3.A7 Hardware-Realisierung von Funktionen eingebetteter Systeme [Entwickler, Planer, Beschaffungsstelle] (S)

- Werden eingebettete Systeme selbst entwickelt, SOLLTEN bei der Designentscheidung zur Hardware- und Software-Realisierung Sicherheitsaspekte berücksichtigt werden.
- Auch bei der Entscheidung, eine bestimmte Hardware-Technik zu implementieren, SOLLTEN Sicherheitsaspekte berücksichtigt werden.

## SYS.4.3.A8 Einsatz eines sicheren Betriebssystem für eingebettete Systeme [Entwickler, Planer, Beschaffungsstelle] (S)

- Das eingesetzte Betriebssystem und die Konfiguration des eingebetteten Systems SOLLTEN für den vorgesehenen Betrieb geeignet sein.
- So SOLLTE das Betriebssystem für die vorgesehene Aufgabe über ausreichende Sicherheitsmechanismen verfügen.
- Die benötigten Dienste und Funktionen SOLLTEN aktiviert sein.
- Das Betriebssystem SOLLTE es unterstützen, ein Trusted Plattform Module (TPM) zu nutzen.

## SYS.4.3.A9 Einsatz kryptografischer Prozessoren bzw. Koprozessoren bei eingebetteten Systemen [Entwickler, Planer, Beschaffungsstelle] (S)

- Wird ein zusätzlicher Mikrocontroller für die kryptografischen Berechnungen verwendet, SOLLTE dessen Kommunikation mit dem System-Mikrocontroller ausreichend abgesichert sein.
- Für das eingebettete System SOLLTEN die nötigen Vertrauensanker realisiert werden.
- Auch SOLLTE eine Vertrauenskette (Chain of Trust) implementiert sein.

## SYS.4.3.A10 Wiederherstellung von eingebetteten Systemen (S)

- Eingebettete Systeme SOLLTEN über Rollback-Fähigkeiten verfügen.

## SYS.4.3.A11 Sichere Aussonderung eines eingebetteten Systems (S)

- Bevor eingebettete Systeme ausgesondert werden, SOLLTEN sämtliche Daten auf dem System sicher gelöscht werden.
- Die Löschung oder Vernichtung SOLLTE dokumentiert werden.

## SYS.4.3.A12 Auswahl einer vertrauenswürdigen Lieferanten- und Logistikkette sowie qualifizierter Hersteller für eingebettete Systeme [Beschaffungsstelle] (H)

- Es SOLLTEN in der Logistikkette wirksame Kontrollen durchgeführt werden, sodass sichergestellt ist,
    - dass eingebettete Systeme keine manipulierten, gefälschten oder getauschten Komponenten enthalten,
    - die Systeme der Spezifikation entsprechen und keine verdeckten Funktionen bei der Herstellung implementiert wurden sowie
    - Unbefugte nicht an vertrauliche Informationen über das eingebettete System gelangen können.
- Die beteiligten Unternehmen SOLLTEN nachweisbar qualifiziert sein.

## SYS.4.3.A13 Einsatz eines zertifizierten Betriebssystems [Entwickler, Planer, Beschaffungsstelle] (H)

- Das Betriebssystem SOLLTE nach einem anerkannten Standard auf einer angemessenen Stufe evaluiert sein.

## SYS.4.3.A14 Abgesicherter und authentisierter Bootprozess bei eingebetteten Systemen [Entwickler, Planer, Beschaffungsstelle] (H)

- Der Bootprozess eines eingebetteten Systems SOLLTE abgesichert sein, indem der Bootloader die Integrität des Betriebssystems überprüft und es nur dann lädt, wenn es als korrekt eingestuft wurde.
- Umgekehrt SOLLTE auch das Betriebssystem die Integrität des Bootloaders prüfen.
- Es SOLLTE ein mehrstufiges Boot-Konzept mit kryptografisch sicherer Überprüfung der Einzelschritte realisiert werden.
- Sichere Hardware-Vertrauensanker SOLLTEN verwendet werden.
- Bei einem ARM-basierten eingebetteten System SOLLTE ARM Secure Boot genutzt werden.
- Bei einem Unified Extensible Firmware Interface (UEFI) SOLLTE Secure Boot genutzt werden.

## SYS.4.3.A15 Speicherschutz bei eingebetteten Systemen [Entwickler, Planer, Beschaffungsstelle] (H)

- Bereits beim Entwurf eingebetteter Systeme SOLLTEN Speicherschutzmechanismen berücksichtigt werden.
- Die Art des Speicherschutzes sowie Anzahl und Größe der Schutzräume SOLLTEN für den Einsatzzweck angemessen sein.

## SYS.4.3.A16 Tamper-Schutz bei eingebetteten Systemen [Planer] (H)

- Für eingebettete Systeme SOLLTE ein Tamper-Schutz-Konzept entwickelt werden.
- Es SOLLTEN angemessene Mechanismen etabliert werden, die Tamper-Angriffe erkennen, aufzeichnen und verhindern.
- Schließlich SOLLTEN angemessene Vorgaben etabliert werden, wie auf einen Tamper-Angriff zu reagieren ist.

## SYS.4.3.A17 Automatische Überwachung der Baugruppenfunktion [Planer, Beschaffungsstelle] (H)

- Sämtliche Baugruppen eines eingebetteten Systems mit erhöhten Anforderungen an die Verfügbarkeit und Integrität SOLLTEN integrierte Selbsttesteinrichtungen (Built-in Self-Test, BIST) besitzen.
- Tests SOLLTEN während des Einschaltvorgangs sowie in angemessenen zeitlichen Intervallen während des Betriebs die Integrität des Systems prüfen.
- Soweit möglich, SOLLTEN die Selbsttestfunktionen auch Sicherheitsfunktionen bzw. Sicherheitseigenschaften der Baugruppe überprüfen.
- Regelmäßig SOLLTE die Integrität der Speicher und I/O-Komponenten im Rahmen des BIST geprüft werden.
- Bestehende BIST-Funktionen SOLLTEN, falls möglich, um die erforderlichen Funktionen ergänzt werden.

## SYS.4.3.A18 Widerstandsfähigkeit eingebetteter Systeme gegen Seitenkanalangriffe [Entwickler, Beschaffungsstelle] (H)

- Um eingebettete Systeme widerstandsfähig gegen Seitenkanalangriffe zu machen, SOLLTEN angemessene Vorkehrungen gegen nicht-invasive und (semi-)invasive Seitenkanalangriffe getroffen werden.


