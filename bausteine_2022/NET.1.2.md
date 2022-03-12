# NET.1.2: Netzmanagement

## NET.1.2.A1 Planung des Netzmanagements (B)

- Die Netzmanagement-Infrastruktur MUSS geeignet geplant werden.
- Dabei SOLLTEN alle in der Sicherheitsrichtlinie und Anforderungsspezifikation für das Netzmanagement genannten Punkte berücksichtigt werden.
- Es MÜSSEN mindestens folgende Themen berücksichtigt werden:
    - zu trennende Bereiche für das Netzmanagement,
    - Zugriffsmöglichkeiten auf die Management-Server,
    - Kommunikation für den Managementzugriff,
    - eingesetzte Protokolle, z. B. IPv4 und IPv6,
    - Anforderungen an Management-Werkzeuge,
    - Schnittstellen, um erfasste Ereignis- oder Alarmmeldungen weiterzuleiten,
    - Protokollierung, inklusive erforderlicher Schnittstellen zu einer zentralen Protokollierungslösung,
    - Reporting und Schnittstellen zu übergreifenden Lösungen sowie
    - korrespondierende Anforderungen an die einzubindenden Netzkomponenten.

## NET.1.2.A2 Anforderungsspezifikation für das Netzmanagement (B)

- Ausgehend von NET.1.2.A1 Planung des Netzmanagements MÜSSEN Anforderungen an die Netzmanagement-Infrastruktur und -Prozesse spezifiziert werden.
- Dabei MÜSSEN alle wesentlichen Elemente für das Netzmanagement berücksichtigt werden.
- Auch SOLLTE die Richtlinie für das Netzmanagement beachtet werden.

## NET.1.2.A3 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## NET.1.2.A4 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## NET.1.2.A5 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## NET.1.2.A6 Regelmäßige Datensicherung (B)

- Bei der Datensicherung des Netzmanagements MÜSSEN mindestens die Systemdaten für die Einbindung der zu verwaltenden Komponenten bzw. Objekte, Ereignismeldungen, Statistikdaten sowie vorgehaltene Daten für das Konfigurationsmanagement gesichert werden.

## NET.1.2.A7 Grundlegende Protokollierung von Ereignissen (B)

- Mindestens folgende Ereignisse MÜSSEN protokolliert werden:
    - unerlaubte Zugriffe bzw. Zugriffsversuche,
    - Leistungs- oder Verfügbarkeitsschwankungen des Netzes,
    - Fehler in automatischen Prozessen (z. B. bei der Konfigurationsverteilung) sowie
    - eingeschränkte Erreichbarkeit von Netzkomponenten.

## NET.1.2.A8 Zeit-Synchronisation (B)

- Alle Komponenten des Netzmanagements, inklusive der eingebundenen Netzkomponenten, MÜSSEN eine synchrone Uhrzeit nutzen.
- Die Uhrzeit SOLLTE an jedem Standort innerhalb des lokalen Netzes mittels NTP-Service synchronisiert werden.
- Ist ein separates Managementnetz eingerichtet, SOLLTE eine NTP-Instanz in diesem Managementnetz positioniert werden.

## NET.1.2.A9 Absicherung der Netzmanagement-Kommunikation und des Zugriffs auf Netz-ManagementWerkzeuge (B)

- Erfolgt die Netzmanagement-Kommunikation über die produktive Infrastruktur, MÜSSEN dafür sichere Protokolle verwendet werden.
- Ist dies nicht möglich, MUSS ein eigens dafür vorgesehenes Administrationsnetz (Out-of-BandManagement) verwendet werden (siehe NET.1.1 Netzarchitektur und -design).
- Falls von einem Netz außerhalb der Managementnetze auf Netzmanagement-Werkzeuge zugegriffen wird, MÜSSEN als sicher geltende Authentisierungs- und Verschlüsselungsmethoden realisiert werden.

## NET.1.2.A10 Beschränkung der SNMP-Kommunikation (B)

- Grundsätzlich DÜRFEN im Netzmanagement KEINE unsicheren Versionen des Simple Network Management Protocol (SNMP) eingesetzt werden.
- Werden dennoch unsichere Protokolle verwendet und nicht über andere sichere Netzprotokolle (z. B. VPN oder TLS) abgesichert, MUSS ein separates Managementnetz genutzt werden.
- Grundsätzlich SOLLTE über SNMP nur mit den minimal erforderlichen Zugriffsrechten zugegriffen werden.
- Die Zugangsberechtigung SOLLTE auf dedizierte Management-Server eingeschränkt werden.

## NET.1.2.A11 Festlegung einer Sicherheitsrichtlinie für das Netzmanagement (S)

- Für das Netzmanagement SOLLTE eine Sicherheitsrichtlinie erstellt und nachhaltig gepflegt werden.
- Die Sicherheitsrichtlinie SOLLTE allen Personen, die am Netzmanagement beteiligt sind, bekannt sein.
- Die Sicherheitsrichtlinie SOLLTE zudem grundlegend für ihre Arbeit sein.
- Es SOLLTE regelmäßig und nachvollziehbar überprüft werden, dass die in der Sicherheitsrichtlinie geforderten Inhalte umgesetzt werden.
- Die Ergebnisse SOLLTEN sinnvoll dokumentiert werden.
- Die Sicherheitsrichtlinie SOLLTE festlegen, welche Bereiche des Netzmanagements über zentrale ManagementWerkzeuge und -Dienste realisiert werden.
- Auch SOLLTE sie definieren, inwieweit Aufgaben im Netzmanagement der Institution automatisiert realisiert werden sollen.
- Darüber hinaus SOLLTEN Rahmenbedingungen und Vorgaben für die Netztrennung, die Zugriffskontrolle, die Protokollierung sowie für den Schutz der Kommunikation spezifiziert werden.
- Auch für das eingesetzte Netzmanagement-Werkzeug und für die operativen Grundregeln des Netzmanagements SOLLTEN Rahmenbedingungen und Vorgaben spezifiziert werden.

## NET.1.2.A12 Ist-Aufnahme und Dokumentation des Netzmanagements (S)

- Es SOLLTE eine Dokumentation erstellt werden, die beschreibt, wie die Management-Infrastruktur des Netzes aufgebaut ist.
- Darin SOLLTEN die initiale Ist-Aufnahme sowie alle durchgeführten Änderungen im Netzmanagement enthalten sein.
- Insbesondere SOLLTE dokumentiert werden, welche Netzkomponenten mit welchen ManagementWerkzeugen verwaltet werden.
- Außerdem SOLLTEN alle für das Netzmanagement benutzten IT-Arbeitsplätze und -Endgeräte sowie alle Informationsbestände, Management-Daten und Informationen über den Betrieb des Netzmanagements erfasst werden.
- Letztlich SOLLTEN sämtliche Schnittstellen zu Anwendungen und Diensten außerhalb des Netzmanagements dokumentiert werden.
- Der so dokumentierte Ist-Zustand der Management-Infrastruktur SOLLTE mit der Dokumentation der Netz-Infrastruktur abgeglichen werden (siehe Baustein NET.1.1 Netz-Architektur- und Design).
- Die Dokumentation SOLLTE vollständig und immer aktuell sein.

## NET.1.2.A13 Erstellung eines Netzmanagement-Konzepts (S)

- Ausgehend von der Sicherheitsrichtlinie für das Netzmanagement SOLLTE ein Netzmanagement-Konzept erstellt und nachhaltig gepflegt werden.
- Dabei SOLLTEN mindestens folgende Aspekte bedarfsgerecht berücksichtigt werden:
    - Methoden, Techniken und Werkzeuge für das Netzmanagement,
    - Absicherung des Zugangs und der Kommunikation,
    - Netztrennung, insbesondere Zuordnung von Netzmanagement-Komponenten zu Zonen,
    - Umfang des Monitorings und der Alarmierung je Netzkomponente,
    - Protokollierung,
    - Automatisierung, insbesondere zentrale Verteilung von Konfigurationsdateien auf Switches,
    - Meldeketten bei Störungen und Sicherheitsvorfällen,
    - Bereitstellung von Netzmanagement-Informationen für andere Betriebsbereiche sowie
    - Einbindung des Netzmanagements in die Notfallplanung.

## NET.1.2.A14 Fein- und Umsetzungsplanung (S)

- Es SOLLTE eine Fein- und Umsetzungsplanung für die Netzmanagement-Infrastruktur erstellt werden.
- Dabei SOLLTEN alle in der Sicherheitsrichtlinie und im Netzmanagement-Konzept adressierten Punkte berücksichtigt werden.

## NET.1.2.A15 Konzept für den sicheren Betrieb der Netzmanagement-Infrastruktur (S)

- Ausgehend von der Sicherheitsrichtlinie für das Netzmanagement und dem Netzmanagement-Konzept SOLLTE ein Konzept für den sicheren Betrieb der Netzmanagement-Infrastruktur erstellt werden.
- Darin SOLLTE der Anwendungs- und Systembetrieb für die Netzmanagement-Werkzeuge berücksichtigt werden.
- Auch SOLLTE geprüft werden, wie sich die Leistungen anderer operativer Einheiten einbinden und steuern lassen.

## NET.1.2.A16 Einrichtung und Konfiguration von Netzmanagement-Lösungen (S)

- Lösungen für das Netzmanagement SOLLTEN anhand der Sicherheitsrichtlinie, der spezifizierten Anforderungen (siehe NET1.2.A2 Anforderungsspezifikation für das Netzmanagement) und der Fein- und Umsetzungsplanung aufgebaut, sicher konfiguriert und in Betrieb genommen werden.
- Danach SOLLTEN die spezifischen Prozesse für das Netzmanagement eingerichtet werden.

## NET.1.2.A17 Regelmäßiger Soll-Ist-Vergleich im Rahmen des Netzmanagements (S)

- Es SOLLTE regelmäßig und nachvollziehbar geprüft werden, inwieweit die Netzmanagement-Lösung dem Sollzustand entspricht.
- Dabei SOLLTE geprüft werden, ob die bestehende Lösung noch die Sicherheitsrichtlinie und Anforderungsspezifikation erfüllt.
- Auch SOLLTE geprüft werden, inwieweit die umgesetzte Management-Struktur und die genutzten Prozesse dem aktuellen Stand entsprechen.
- Weiter SOLLTE verglichen werden, ob die Management-Infrastruktur aktuell ist.

## NET.1.2.A18 Schulungen für Management-Lösungen [Vorgesetzte] (S)

- Für die eingesetzten Netzmanagement-Lösungen SOLLTEN Schulungs- und Trainingsmaßnahmen konzipiert und durchgeführt werden.
- Die Maßnahmen SOLLTEN die individuellen Gegebenheiten im Configuration-, Availabilityund Capacity-Management sowie typische Situationen im Fehlermanagement abdecken.
- Die Schulungen und Trainings SOLLTEN regelmäßig wiederholt werden, mindestens jedoch, wenn sich größere technische oder organisatorische Änderungen innerhalb der Netzmanagement-Lösung ergeben.

## NET.1.2.A19 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## NET.1.2.A20 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## NET.1.2.A21 Entkopplung der Netzmanagement-Kommunikation (S)

- Direkte Management-Zugriffe eines Administrators von einem IT-System außerhalb der Managementnetze auf eine Netzkomponente SOLLTEN vermieden werden.
- Ist ein solcher Zugriff ohne zentrales Management-Werkzeug notwendig, SOLLTE die Kommunikation entkoppelt werden.
- Solche Sprungserver SOLLTEN im Management-Netz integriert und in einem getrennten Zugangssegment positioniert sein.

## NET.1.2.A22 Beschränkung der Management-Funktionen (S)

- Es SOLLTEN NUR die benötigten Management-Funktionen aktiviert werden.

## NET.1.2.A23 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## NET.1.2.A24 Zentrale Konfigurationsverwaltung für Netzkomponenten (S)

- Software bzw. Firmware und Konfigurationsdaten für Netzkomponenten SOLLTEN automatisch über das Netz verteilt und ohne Betriebsunterbrechung installiert und aktiviert werden können.
- Die dafür benötigten Informationen SOLLTEN an zentraler Stelle sicher verfügbar sein sowie in die Versionsverwaltung und die Datensicherung eingebunden werden.
- Die zentrale Konfigurationsverwaltung SOLLTE nachhaltig gepflegt und regelmäßig auditiert werden.

## NET.1.2.A25 Statusüberwachung der Netzkomponenten (S)

- Die grundlegenden Performance- und Verfügbarkeitsparameter der zentralen Netzkomponenten SOLLTEN kontinuierlich überwacht werden.
- Dafür SOLLTEN vorab die jeweiligen Schwellwerte ermittelt werden (Baselining).

## NET.1.2.A26 Alarming und Logging (S)

- Wichtige Ereignisse auf Netzkomponenten und auf den Netzmanagement-Werkzeugen SOLLTEN automatisch an ein zentrales Management-System übermittelt und dort protokolliert werden (siehe OPS.1.1.5 Protokollierung).
- Das zuständige Personal SOLLTE zusätzlich automatisch benachrichtigt werden.
- Das Alarming und Logging SOLLTE mindestens folgende Punkte beinhalten:
    - Ausfall bzw. Nichterreichbarkeit von Netz- oder Management-Komponenten,
    - Hardware-Fehlfunktionen,
    - fehlerhafte Anmeldeversuche sowie
    - kritische Zustände oder Überlastung von IT-Systemen.
- Ereignismeldungen bzw. Logging-Daten SOLLTEN einem zentralen Management-System entweder kontinuierlich oder gebündelt übermittelt werden.
- Alarmmeldungen SOLLTEN sofort wenn sie auftreten übermittelt werden.

## NET.1.2.A27 Einbindung des Netzmanagements in die Notfallplanung (S)

- Die Netzmanagement-Lösungen SOLLTEN in die Notfallplanung der Institution eingebunden werden.
- Dazu SOLLTEN die Netzmanagement-Werkzeuge und die Konfigurationen der Netzkomponenten gesichert und in die Wiederanlaufpläne integriert sein.

## NET.1.2.A28 Platzierung der Management-Clients für das In-Band-Management (S)

- Für die Administration sowohl der internen als auch der externen IT-Systeme SOLLTEN dedizierte ManagementClients eingesetzt werden.
- Dafür SOLLTE mindestens ein Management-Client am äußeren Netzbereich (für die Administration am Internet anliegender IT-Systeme) und ein weiterer im internen Bereich (für die Administration interner IT-Systeme) platziert werden.

## NET.1.2.A29 Einsatz von VLANs im Management-Netz (S)

- Werden Managementnetze durch VLANs getrennt, SOLLTE darauf geachtet werden, dass der äußere Paketfilter sowie die daran angeschlossenen Geräte in einem eigenen Teilnetz stehen.
- Zudem SOLLTE sichergestellt werden, dass das ALG dabei nicht umgangen wird.

## NET.1.2.A30 Hochverfügbare Realisierung der Management-Lösung (H)

- Zentrale Management-Lösungen SOLLTEN hochverfügbar betrieben werden.
- Dazu SOLLTEN die Server bzw. Werkzeuge inklusive der Netzanbindungen redundant ausgelegt sein.
- Auch die einzelnen Komponenten SOLLTEN hochverfügbar bereitgestellt werden.

## NET.1.2.A31 Grundsätzliche Nutzung von sicheren Protokollen (H)

- Für das Netzmanagement SOLLTEN ausschließlich sichere Protokolle benutzt werden.
- Es SOLLTEN alle Sicherheitsfunktionen dieser Protokolle verwendet werden.

## NET.1.2.A32 Physische Trennung des Managementnetzes [Planer] (H)

- Das Managementnetz SOLLTE physisch von den produktiven Netzen getrennt werden.

## NET.1.2.A33 Physische Trennung von Management-Segmenten [Planer] (H)

- Es SOLLTEN physisch getrennte Zonen mindestens für das Management von LAN-Komponenten, Sicherheitskomponenten und Komponenten zur Außenanbindung eingerichtet werden.

## NET.1.2.A34 ENTFALLEN (H)

- Diese Anforderung ist entfallen.

## NET.1.2.A35 Festlegungen zur Beweissicherung (H)

- Die erhobenen Protokollierungsdaten SOLLTEN für forensische Analysen gesetzeskonform und revisionssicher archiviert werden (siehe auch DER.2.2 Vorsorge für die IT-Forensik).

## NET.1.2.A36 Einbindung der Protokollierung des Netzmanagements in eine SIEM-Lösung (H)

- Die Protokollierung des Netzmanagements SOLLTE in eine Security-Information-and-Event-Management (SIEM)Lösung eingebunden werden.
- Dazu SOLLTEN die Anforderungskataloge zur Auswahl von Netzmanagement-Lösungen hinsichtlich der erforderlichen Unterstützung von Schnittstellen und Übergabeformaten angepasst werden (siehe NET.1.2.A2 Anforderungsspezifikation für das Netzmanagement).

## NET.1.2.A37 Standort übergreifende Zeitsynchronisation (H)

- Die Zeitsynchronisation SOLLTE über alle Standorte der Institution sichergestellt werden.
- Dafür SOLLTE eine gemeinsame Referenzzeit benutzt werden.

## NET.1.2.A38 Festlegung von Notbetriebsformen für die Netzmanagement-Infrastruktur (H)

- Für eine schnelle Wiederherstellung der Sollzustände von Software bzw. Firmware sowie der Konfiguration der Komponenten in der Netzmanagement-Infrastruktur SOLLTEN hinreichend gute Ersatzlösungen festgelegt werden.


