# SYS.1.1: Allgemeiner Server

## SYS.1.1.A1 Geeignete Aufstellung (B)

- Server MÜSSEN an Orten betrieben werden, zu denen nur berechtigte Personen Zutritt haben.
- Server MÜSSEN daher in Rechenzentren, Rechnerräumen oder abschließbaren Serverschränken aufgestellt beziehungsweise eingebaut werden (siehe hierzu die entsprechenden Bausteine der Schicht INF Infrastruktur).
- Server DÜRFEN NICHT als Arbeitsplatzrechner genutzt werden.
- Als Arbeitsplatz genutzte IT-Systeme DÜRFEN NICHT als Server genutzt werden.

## SYS.1.1.A2 Benutzerauthentisierung an Servern (B)

- Für die Anmeldung von Benutzern und Diensten am Server MÜSSEN Authentisierungsverfahren eingesetzt werden, die dem Schutzbedarf der Server angemessen sind.
- Dies SOLLTE in besonderem Maße für administrative Zugänge berücksichtigt werden.
- Soweit möglich, SOLLTE dabei auf zentrale, netzbasierte Authentisierungsdienste zurückgegriffen werden.

## SYS.1.1.A3 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## SYS.1.1.A4 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## SYS.1.1.A5 Schutz von Schnittstellen (B)

- Es MUSS gewährleistet werden, dass nur dafür vorgesehene Wechselspeicher und sonstige Geräte an die Server angeschlossen werden können.
- Alle Schnittstellen, die nicht verwendet werden, MÜSSEN deaktiviert werden.

## SYS.1.1.A6 Deaktivierung nicht benötigter Dienste (B)

- Alle nicht benötigten Dienste und Anwendungen MÜSSEN deaktiviert oder deinstalliert werden, vor allem Netzdienste.
- Auch alle nicht benötigten Funktionen in der Firmware MÜSSEN deaktiviert werden.
- Auf Servern SOLLTE der Speicherplatz für die einzelnen Benutzer, aber auch für Anwendungen, geeignet beschränkt werden.
- Die getroffenen Entscheidungen SOLLTEN so dokumentiert werden, dass nachvollzogen werden kann, welche Konfiguration und Softwareausstattung für die Server gewählt wurden.

## SYS.1.1.A7 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## SYS.1.1.A8 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## SYS.1.1.A9 Einsatz von Virenschutz-Programmen auf Servern (B)

- Abhängig vom installierten Betriebssystem, den bereitgestellten Diensten und von anderen vorhandenen Schutzmechanismen des Servers MUSS geprüft werden, ob Viren-Schutzprogramme eingesetzt werden sollen und können.
- Soweit vorhanden, MÜSSEN konkrete Aussagen, ob ein Virenschutz notwendig ist, aus den betreffenden Betriebssystem-Bausteinen des IT-Grundschutz-Kompendiums berücksichtigt werden.

## SYS.1.1.A10 Protokollierung (B)

- Generell MÜSSEN alle sicherheitsrelevanten Systemereignisse protokolliert werden, dazu gehören mindestens:
    - Systemstarts und Reboots,
    - erfolgreiche und erfolglose Anmeldungen am System (Betriebssystem und Anwendungssoftware),
    - fehlgeschlagene Berechtigungsprüfungen,
    - blockierte Datenströme (Verstöße gegen ACLs oder Firewallregeln),
    - Einrichtung oder Änderungen von Benutzern, Gruppen und Berechtigungen,
    - sicherheitsrelevante Fehlermeldungen (z. B. Hardwaredefekte, Überschreitung von Kapazitätsgrenzen) sowie
    - Warnmeldungen von Sicherheitssystemen (z. B. Virenschutz).

## SYS.1.1.A11 Festlegung einer Sicherheitsrichtlinie für Server (S)

- Ausgehend von der allgemeinen Sicherheitsrichtlinie der Institution SOLLTEN die Anforderungen an Server in einer separaten Sicherheitsrichtlinie konkretisiert werden.
- Diese Richtlinie SOLLTE allen Administratoren und anderen Personen, die an der Beschaffung und dem Betrieb der Server beteiligt sind, bekannt und Grundlage für deren Arbeit sein.
- Die Umsetzung der in der Richtlinie geforderten Inhalte SOLLTE regelmäßig überprüft werden.
- Die Ergebnisse SOLLTEN sinnvoll dokumentiert werden.

## SYS.1.1.A12 Planung des Server-Einsatzes (S)

- Jedes Server-System SOLLTE geeignet geplant werden.
- Dabei SOLLTEN mindestens folgende Punkte berücksichtigt werden:
    - Auswahl der Hardwareplattform, des Betriebssystems und der Anwendungssoftware,
    - Dimensionierung der Hardware (Leistung, Speicher, Bandbreite etc.),
    - Art und Anzahl der Kommunikationsschnittstellen,
    - Leistungsaufnahme, Wärmelast, Platzbedarf und Bauform,
    - administrative Zugänge (siehe SYS.1.1.A5 Schutz von Schnittstellen),
    - Zugriffe von Benutzern,
    - Protokollierung (siehe SYS.1.1.A10 Protokollierung),
    - Aktualisierung von Betriebssystem und Anwendungen sowie
    - Einbindung ins System- und Netzmanagement, in die Datensicherung und die Schutzsysteme (Virenschutz, IDS etc.).
- Alle Entscheidungen, die in der Planungsphase getroffen wurden, SOLLTEN so dokumentiert werden, dass sie zu einem späteren Zeitpunkt nachvollzogen werden können.

## SYS.1.1.A13 Beschaffung von Servern (S)

- Bevor ein oder mehrere Server beschafft werden, SOLLTE eine Anforderungsliste erstellt werden, anhand derer die am Markt erhältlichen Produkte bewertet werden.

## SYS.1.1.A14 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.1.1.A15 Unterbrechungsfreie und stabile Stromversorgung [Haustechnik] (S)

- Jeder Server SOLLTE an eine unterbrechungsfreie Stromversorgung (USV) angeschlossen werden.

## SYS.1.1.A16 Sichere Grundkonfiguration von Servern (S)

- Die Grundeinstellungen von Servern SOLLTEN überprüft und falls erforderlich entsprechend den Vorgaben der Sicherheitsrichtlinie angepasst werden.
- Erst nachdem die Installation und die Konfiguration abgeschlossen sind, SOLLTE der Server mit dem Internet verbunden werden.

## SYS.1.1.A17 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.1.1.A18 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.1.1.A19 Einrichtung lokaler Paketfilter (S)

- Vorhandene lokale Paketfilter SOLLTEN über ein Regelwerk so ausgestaltet werden, dass die eingehende und ausgehende Kommunikation auf die erforderlichen Kommunikationspartner, Kommunikationsprotokolle bzw. Ports und Schnittstellen beschränkt wird.
- Die Identität von Remote-Systemen und die Integrität der Verbindungen mit diesen SOLLTE kryptografisch abgesichert sein.

## SYS.1.1.A20 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.1.1.A21 Betriebsdokumentation für Server (S)

- Betriebliche Aufgaben, die an einem Server durchgeführt werden, SOLLTEN nachvollziehbar dokumentiert werden (Wer?,
- Wann?,
- Was?).
- Aus der Dokumentation SOLLTEN insbesondere Konfigurationsänderungen nachvollziehbar sein.
- Sicherheitsrelevante Aufgaben, z. B. wer befugt ist, neue Festplatten einzubauen, SOLLTEN dokumentiert werden.
- Alles, was automatisch dokumentiert werden kann, SOLLTE auch automatisch dokumentiert werden.
- Die Dokumentation SOLLTE gegen unbefugten Zugriff und Verlust geschützt werden.

## SYS.1.1.A22 Einbindung in die Notfallplanung (S)

- Der Server SOLLTE im Notfallmanagementprozess berücksichtigt werden.
- Dazu SOLLTEN die Notfallanforderungen an das System ermittelt und geeignete Notfallmaßnahmen umgesetzt werden, z. B. indem Wiederanlaufpläne erstellt oder Passwörter und kryptografische Schlüssel sicher hinterlegt werden.

## SYS.1.1.A23 Systemüberwachung und Monitoring von Servern (S)

- Das Server-System SOLLTE in ein geeignetes Systemüberwachungs- bzw. Monitoringkonzept eingebunden werden.
- Hierbei SOLLTEN der Systemzustand und die Funktionsfähigkeit des Systems und der darauf betriebenen Dienste laufend überwacht werden.
- Fehlerzustände sowie die Überschreitung definierter Grenzwerte SOLLTEN hierüber an das Betriebspersonal meldet werden.

## SYS.1.1.A24 Sicherheitsprüfungen für Server (S)

- Server SOLLTEN regelmäßigen Sicherheitstests unterzogen werden, die überprüfen, ob alle Sicherheitsvorgaben eingehalten werden und ggf. vorhandene Schwachstellen identifizieren.
- Diese Sicherheitsprüfungen SOLLTEN insbesondere auf Servern mit externen Schnittstellen durchgeführt werden.
- Um mittelbare Angriffe über infizierte Sys-teme im eigenen Netz zu vermeiden, SOLLTEN jedoch auch interne Server in festgelegten Zyklen entsprechend überprüft werden.
- Es SOLLTE geprüft werden, ob die Sicherheitsprüfungen automatisiert, z. B. mittels geeigneter Skripte, realisiert werden können.

## SYS.1.1.A25 Geregelte Außerbetriebnahme eines Servers (S)

- Bei der Außerbetriebnahme eines Servers SOLLTE sichergestellt werden, dass keine wichtigen Daten, die eventuell auf den verbauten Datenträgern gespeichert sind, verloren gehen und dass keine schutzbedürftigen Daten zurückbleiben.
- Es SOLLTE einen Überblick darüber geben, welche Daten wo auf dem Server gespeichert sind.
- Es SOLLTE außerdem sichergestellt sein, dass vom Server angebotene Dienste durch einen anderen Server übernommen werden, wenn dies erforderlich ist.
- Es SOLLTE eine Checkliste erstellt werden, die bei der Außerbetriebnahme eines Servers abgearbeitet werden kann.
- Diese Checkliste SOLLTE mindestens Aspekte zur Datensicherung, Migration von Diensten und dem anschließenden sicheren Löschen aller Daten umfassen.

## SYS.1.1.A35 Erstellung und Pflege eines Betriebshandbuchs (S)

- Es SOLLTE ein Betriebshandbuch erstellt werden.
- Darin SOLLTEN alle erforderlichen Regelungen, Anforderungen und Einstellungen dokumentiert werden, die erforderlich sind, um Server zu betreiben.
- Für jede Art von Server SOLLTE es ein spezifisches Betriebshandbuch geben.
- Das Betriebshandbuch SOLLTE regelmäßig aktualisiert werden.
- Das Betriebshandbuch SOLLTE vor unberechtigtem Zugriff geschützt werden.
- Das Betriebshandbuch SOLLTE in Notfällen zur Verfügung stehen.

## SYS.1.1.A37 Kapselung von sicherheitskritischen Anwendungen und Betriebssystemkomponenten (S)

- Um sowohl den Zugriff eines Angreifers auf das Betriebssystem oder andere Anwendungen als auch den Zugriff vom Betriebssystem auf besonders schützenswerte Dateien zu verhindern, SOLLTEN Anwendungen und Betriebssystemkomponenten (wie beispielsweise Authentisierung oder Zertifikatsüberprüfung) ihrem Schutzbedarf entsprechend besonders gekapselt bzw. anderen Anwendungen und Betriebssystemkomponenten gegenüber isoliert werden.
- Dabei SOLLTEN insbesondere sicherheitskritische Anwendungen berücksichtigt werden, die mit Daten aus unsicheren Quellen arbeiten (z.B. Webbrowser und Bürokommunikations-Anwendungen).

## SYS.1.1.A26 ENTFALLEN (H)

- Diese Anforderung ist entfallen.

## SYS.1.1.A27 Hostbasierte Angriffserkennung (H)

- Hostbasierte Angriffserkennungssysteme (Host-based Intrusion Detection Systems, IDS bzw. Intrusion Prevention Systems, IPS) SOLLTEN eingesetzt werden, um das Systemverhalten auf Anomalien und Missbrauch hin zu überwachen.
- Die eingesetzten IDS/IPS-Mechanismen SOLLTEN geeignet ausgewählt, konfiguriert und ausführlich getestet werden.
- Im Falle einer Angriffserkennung SOLLTE das Betriebspersonal in geeigneter Weise alarmiert werden.
- Über Betriebssystem-Mechanismen oder geeignete Zusatzprodukte SOLLTEN Veränderungen an Systemdateien und Konfigurationseinstellungen überprüft, eingeschränkt und gemeldet werden.

## SYS.1.1.A28 Steigerung der Verfügbarkeit durch Redundanz (H)

- Server mit hohen Verfügbarkeitsanforderungen SOLLTEN gegen Ausfälle in geeigneter Weise geschützt sein.
- Hierzu SOLLTEN mindestens geeignete Redundanzen verfügbar sein sowie Wartungsverträge mit den Lieferanten abgeschlossen werden.
- Es SOLLTE geprüft werden, ob bei sehr hohen Anforderungen Hochverfügbarkeitsarchitekturen mit automatischem Failover, gegebenenfalls über verschiedene Standorte hinweg, erforderlich sind.

## SYS.1.1.A29 ENTFALLEN (H)

- Diese Anforderung ist entfallen.

## SYS.1.1.A30 Ein Dienst pro Server (H)

- Abhängig von der Bedrohungslage und dem Schutzbedarf der Dienste SOLLTE auf jedem Server jeweils nur ein Dienst betrieben werden.

## SYS.1.1.A31 Einsatz von Ausführungskontrolle (H)

- Es SOLLTE über eine Ausführungskontrolle sichergestellt werden, dass nur explizit erlaubte Programme und Skripte ausgeführt werden können.
- Die Regeln SOLLTEN so eng wie möglich gefasst werden.
- Falls Pfade und Hashes nicht explizit angegeben werden können, SOLLTEN alternativ auch zertifikatsbasierte oder Pfad-Regeln genutzt werden.

## SYS.1.1.A32 ENTFALLEN (H)

- Diese Anforderung ist entfallen.

## SYS.1.1.A33 Aktive Verwaltung der Wurzelzertifikate (H)

- Im Zuge der Beschaffung und Installation des Servers SOLLTE dokumentiert werden, welche Wurzelzertifikate für den Betrieb des Servers notwendig sind.
- Auf dem Server SOLLTEN lediglich die für den Betrieb notwendigen und vorab dokumentierten Wurzelzertifikate enthalten sein.
- Es SOLLTE regelmäßig überprüft werden, ob die vorhandenen Wurzelzertifikate noch den Vorgaben der Institution entsprechen.
- Es SOLLTEN alle auf dem IT-System vorhandenen Zertifikatsspeicher in die Prüfung einbezogen werden.

## SYS.1.1.A34 Festplattenverschlüsselung (H)

- Bei erhöhtem Schutzbedarf sollten die Datenträger des Servers mit einem als sicher geltenden Produkt bzw. Verfahren verschlüsselt werden.
- Dies SOLLTE auch für virtuelle Maschinen mit produktiven Daten gelten.
- Es SOLLTE nicht nur ein TPM allein als Schlüsselschutz dienen.
- Das Wiederherstellungspasswort SOLLTE an einem geeigneten sicheren Ort gespeichert werden.
- Bei sehr hohen Anforderungen z. B. an die Vertraulichkeit SOLLTE eine Full Volume oder Full Disk Encryption erfolgen.

## SYS.1.1.A36 Absicherung des Bootvorgangs (H)

- Bootloader und Betriebssystem-Kern SOLLTEN durch selbstkontrolliertes Schlüsselmaterial signiert beim Systemstart in einer vertrauenswürdigen Kette geprüft werden (Secure Boot).
- Nicht benötigtes Schlüsselmaterial SOLLTE entfernt werden.

## SYS.1.1.A38 Härtung des Host-Systems mittels Read-Only-Dateisystem (H)

- Die Integrität des Host-Systems sollte durch ein Read-Only-Dateisystem sichergestellt werden (Immutable OS).


