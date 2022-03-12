# IND.1: Prozessleit- und Automatisierungstechnik

## IND.1.A1 Einbindung in die Sicherheitsorganisation (B)

- Ein Managementsystem für Informationssicherheit (ISMS) für den Betrieb der OT-Infrastruktur MUSS entweder als selbständiges ISMS oder als Teil eines Gesamt-ISMS existieren.
- Ein Gesamtverantwortlicher für die Informationssicherheit im OT-Bereich MUSS benannt werden.
- Er MUSS innerhalb der Institution bekannt gegeben werden.

## IND.1.A2 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## IND.1.A3 Schutz vor Schadprogrammen (B)

- Beim Einsatz von Virenschutz-Software auf OT-Komponenten MUSS berücksichtigt werden, ob und in welcher Konfiguration der Betrieb von Virenschutz-Software vom Hersteller unterstützt wird.
- Ist dies nicht der Fall, MUSS der Bedarf an alternativen Schutzverfahren geprüft werden.
- Die Virensignaturen DÜRFEN NICHT von OT-Systemen direkt aus dem Internet bezogen werden.

## IND.1.A18 Protokollierung [OT-Betrieb (Operational Technology, OT)] (B)

- Jede Änderung an ICS-Komponenten MUSS protokolliert werden.
- Außerdem MÜSSEN alle Zugriffe auf ICS-Komponeten protokolliert werden.

## IND.1.A19 Erstellung von Datensicherungen [Mitarbeiter, OT-Betrieb (Operational Technology, OT)] (B)

- Programme und Daten MÜSSEN regelmäßig gesichert werden.
- Auch nach jeder Systemänderung an OT-Komponenten MUSS eine Sicherung erstellt werden.

## IND.1.A4 Dokumentation der OT-Infrastruktur (S)

- Alle sicherheitsrelevanten Parameter der OT-Infrastruktur SOLLTEN dokumentiert sein.
- In einem Bestandsverzeichnis SOLLTEN alle Software- und Systemkomponenten geführt werden.
- Hieraus SOLLTEN die eingesetzten Produktund Protokollversionen sowie die Zuständigkeiten hervorgehen.
- Zu den eingesetzten Komponenten SOLLTEN eventuelle Restriktionen der Hersteller oder regulatorische Auflagen bestimmt sein.
- Diese Dokumentation und ein Systeminventar SOLLTEN beispielsweise in einem Leitsystem geführt werden.
- Zusätzlich SOLLTE ein aktueller Netzplan Zonen, Zonenübergänge (Conduits), eingesetzte Kommunikationsprotokolle und -verfahren sowie Außenschnittstellen dokumentieren.
- Bei den Schnittstellen SOLLTEN aktive Netzkompo-nenten und manuelle Datentransferverfahren, z. B. durch Wechseldatenträger, berücksichtigt werden.
- Zonen und Conduits schützen die OT-Infrastrukur, indem die Automatisierungslösung in Zellen und Kommunikationskanälen strukturiert werden SOLLTE.

## IND.1.A5 Entwicklung eines geeigneten Zonenkonzepts [Planer] (S)

- Die OT-Infrastruktur SOLLTE auch horizontal in unabhängige Funktionsbereiche, wie etwa Anlagen, segmentiert werden.
- Die einzelnen Zonen SOLLTEN, so weit wie möglich, im Betrieb voneinander unabhängig sein.
- Insbesondere die Zonen, in denen der technische Prozess gesteuert wird, SOLLTEN bei einem Ausfall der anderen Zonen für einen gewissen Zeitraum weiter funktionstüchtig sein.
- Auch SOLLTE die Abkopplung nach einem Angriff weiter funktionieren.
- Dieser Zeitraum SOLLTE geeignet definiert und dokumentiert werden.
- Das Netz SOLLTE manipulations- und fehlerresistent konzipiert werden.

## IND.1.A6 Änderungsmanagement im OT-Betrieb (S)

- Für Änderungen an der OT SOLLTE ein eigener Änderungsprozess definiert, dokumentiert und gelebt werden.

## IND.1.A7 Etablieren einer übergreifenden Berechtigungsverwaltung zwischen der OT und in der Office-IT (S)

- Die Institution SOLLTE einen Prozess zur Verwaltung von Benutzerzugängen und zugeordneten Berechtigungen für den Zugriff auf die OT etablieren.
- Die Berechtigungsverwaltung SOLLTE den Prozess, die Durchführung und die Dokumentation für die Beantragung, Einrichtung und den Entzug von Berechtigungen umfassen.
- Die Berechtigungsverwaltung SOLLTE gewährleisten, dass Berechtigungen nach dem Minimalprinzip vergeben und regelmäßig überprüft werden.
- In der Berechtigungsverwaltung SOLLTEN die Zugriffe auf IT-Systeme für Mitarbeiter, Administratoren und Dritte geregelt sein.
- Jeder Beteiligte SOLLTE regelmäßig zu den einzuhaltenden Regelungen sensibilisiert werden.
- Die Einhaltung SOLLTE überprüft werden.
- Fehlverhalten SOLLTE sanktioniert werden.

## IND.1.A8 Sichere Administration [IT-Betrieb] (S)

- Für die Erstkonfiguration, Verwaltung und Fernwartung in der OT SOLLTEN entweder sichere Protokolle oder abgetrennte Administrationsnetze mit entsprechendem Schutzbedarf genutzt werden.
- Der Zugang zu diesen Schnittstellen SOLLTE auf die Berechtigten eingeschränkt sein.
- Es SOLLTE nur der Zugriff auf die Systeme und Funktionen gewährt sein, die für die jeweilige Administrationsaufgabe benötigt werden.
- Die Systeme und Kommunikationskanäle, mit denen die Administration oder Fernwartung durchgeführt wird, SOLLTEN das gleiche Schutzniveau aufweisen wie die verwaltete OT-Komponente.

## IND.1.A9 Restriktiver Einsatz von Wechseldatenträgern und mobilen Endgeräten in ICS-Umgebungen (S)

- Für die Nutzung von Wechseldatenträgern und mobilen Endgeräten SOLLTEN Regelungen aufgestellt und bekannt gegeben werden.
- Der Einsatz von Wechseldatenträgern und mobilen Endgeräten in ICS-Umgebungen SOLLTE beschränkt werden.
- Für Medien und Geräte von Dienstleistern SOLLTEN ein Genehmigungsprozess und eine Anforderungsliste existieren.
- Die Vorgaben SOLLTEN jedem Dienstleister bekannt sein und von diesen schriftlich bestätigt werden.
- Auf den OT-Komponenten SOLLTEN alle nicht benötigten Schnittstellen deaktiviert werden.
- An den aktiven Schnittstellen SOLLTE die Nutzung auf bestimmte Geräte oder Medien eingeschränkt werden.

## IND.1.A10 Monitoring, Protokollierung und Detektion [OT-Betrieb (Operational Technology, OT)] (S)

- Betriebs- und sicherheitsrelevante Ereignisse SOLLTEN zeitnah identifiziert werden.
- Hierzu SOLLTE ein geeignetes Log- und Event-Management entwickelt und umgesetzt werden.
- Das Log- und Event-Management SOLLTE angemessene Maßnahmen umfassen, um sicherheitsrelevante Ereignisse zu erkennen und zu erheben.
- Es SOLLTE zudem einen Reaktionsplan (Security Incident Response) enthalten.
- Der Reaktionsplan SOLLTE Verfahren zur Behandlung von Sicherheitsvorfällen festlegen.
- Darin abgedeckt sein SOLLTEN die Klassifizierung von Ereignissen, Meldewege und Festlegung der einzubeziehenden Organisationseinheiten, Reaktionspläne zur Schadensbegrenzung, Analyse und Wiederherstellung von Systemen und Diensten sowie die Dokumentation und Nachbereitung von Vorfällen.

## IND.1.A11 Sichere Beschaffung und Systementwicklung (S)

- Sollen OT-Systeme beschafft, geplant oder entwickelt werden, SOLLTEN Regelungen zur Informationssicherheit getroffen und dokumentiert werden.
- Die Unterlagen SOLLTEN Teil der Ausschreibung sein.
- Bei Beschaffungen, Planungen oder Entwicklungen SOLLTE die Informationssicherheit in dem gesamten Lebenszyklus berücksichtigt werden.
- Voraussetzungen und Umsetzungshinweise für einen sicheren Betrieb von ICS-Komponenten von Herstellern SOLLTEN frühzeitig eingeplant und umgesetzt werden.
- Für ICS-Komponenten SOLLTEN einheitliche und dem Schutzbedarf angemessene Anforderungen an die Informationssicherheit definiert werden.
- Diese SOLLTEN berücksichtigt werden, wenn neue ICS-Komponenten beschafft werden.
- Die Einhaltung und Umsetzung SOLLTE dokumentiert werden.
- Die Institution SOLLTE dokumentieren, wie sich das System in die Konzepte für die Zoneneinteilung, das Berechtigungs- und Schwachstellen-Management sowie für den Virenschutz einfügt und diese gegebenenfalls anpassen.
- Es SOLLTE geregelt sein, wie der Betrieb aufrechterhalten werden kann, falls einer der Kooperationspartner keine Dienstleistungen mehr anbietet.

## IND.1.A12 Etablieren eines Schwachstellen-Managements (S)

- Für den sicheren Betrieb einer OT-Umgebung SOLLTE die Institution ein Schwachstellen-Management etablieren.
- Das Schwachstellen-Management SOLLTE Lücken in Software, Komponenten, Protokollen und Außenschnittstellen der Umgebung identifizieren.
- Außerdem SOLLTEN sich daraus erforderliche Handlungen ableiten, bewerten und umsetzen lassen.
- Grundlage dafür SOLLTEN Schwachstellenmeldungen von Herstellern oder öffentlich verfügbare CERT-Meldungen sein.
- Ergänzend hierzu SOLLTEN organisatorische und technische Audits zur Schwachstellenanalyse durchgeführt werden.

## IND.1.A20 Systemdokumentation [Mitarbeiter, OT-Betrieb (Operational Technology, OT)] (S)

- Es SOLLTE eine erweiterte Systemdokumentation erstellt werden.
- Darin SOLLTEN Besonderheiten im Betrieb und die Möglichkeiten zur Systemverwaltung festgehalten werden.
- Außerdem SOLLTE dokumentiert werden, wenn ICS-Komponenten verändert werden.

## IND.1.A21 Dokumentation der Kommunikationsbeziehungen [OT-Betrieb (Operational Technology, OT)] (S)

- Es SOLLTE dokumentiert werden, mit welchen Systemen eine ICS-Kompnente welche Daten austauscht.
- Außerdem SOLLTEN die Kommunikationsverbindungen neu integrierter ICS-Komponenten dokumentiert werden.

## IND.1.A22 Zentrale Systemprotokollierung und -überwachung [OT-Betrieb (Operational Technology, OT)] (S)

- Die Protokollierungsdaten von ICS-Komponenten SOLLTEN zentral gespeichert werden.
- Bei sicherheitskritischen Ereignissen SOLLTE automatisch alarmiert werden.

## IND.1.A23 Aussonderung von ICS-Komponenten [OT-Betrieb (Operational Technology, OT)] (S)

- Wenn alte oder defekte ICS-Komponenten ausgesondert werden, SOLLTEN alle schützenswerten Daten sicher gelöscht werden.
- Es SOLLTE insbesondere sichergestellt sein, dass alle Zugangsdaten nachhaltig entfernt wurden.

## IND.1.A13 Notfallplanung für OT (H)

- Notfallpläne für den Ausfall und für die Kompromittierung jeder Zone SOLLTEN definiert, dokumentiert, nach jeder größeren Änderung getestet und regelmäßig geübt sein.
- Zudem SOLLTE ein wirksames Ersatzverfahren für den Ausfall der (Fern-) Administrationsmöglichkeit definiert, dokumentiert und getestet sein.

## IND.1.A14 Starke Authentisierung an OT-Komponenten (H)

- Zur sicheren Authentisierung von privilegierten Benutzern in Steuerungssystemen SOLLTE ein zentraler Verzeichnisdienst eingerichtet werden (siehe Baustein ORP.4 Identitäts- und Berechtigungsmanagement).
- Die Authentisierung SOLLTE durch den Einsatz mehrerer Faktoren wie Wissen, Besitz oder Biometrie zusätzlich abgesichert werden.
- Bei der Planung SOLLTE darauf geachtet werden, dass daraus entstehende Abhängigkeiten in der Benutzerauthentisierung bekannt sind und bei der Umsetzung der Lösung berücksichtigt werden.
- Es SOLLTE sichergestellt werden, dass die Authentisierung von betrieblich erforderlichen technischen Konten auch in Notfällen durchgeführt werden kann.

## IND.1.A15 Überwachung von weitreichenden Berechtigungen (H)

- Die Institution SOLLTE ein Bestandsverzeichnis führen, das alle vergebenen Zutritts-, Zugangs und Zugriffsrechte auf kritische Systeme enthält.
- Das Verzeichnis SOLLTE beinhalten, welche Rechte ein bestimmter Benutzer effektiv hat und wer an einem bestimmten System über welche Rechte verfügt.
- Alle kritischen administrativen Tätigkeiten SOLLTEN protokolliert werden.
- Der IT-Betrieb SOLLTE NICHT die Protokolle löschen oder manipulieren können.

## IND.1.A16 Stärkere Abschottung der Zonen (H)

- Bei hoch schutzbedürftigen oder schlecht absicherbaren ICS-Umgebungen SOLLTEN vorbeugend Schnittstellensysteme mit Sicherheitsprüffunktionen eingesetzt werden.
- Durch Realisierung einer oder mehrerer Anbindungszonen (DMZ) in P-A-P-Struktur SOLLTEN durchgängige Außenverbindungen terminiert werden.
- Erforderliche Sicherheitsprüfungen SOLLTEN so erfolgen, dass die ICS-Anlage nicht angepasst werden muss.

## IND.1.A17 Regelmäßige Sicherheitsüberprüfung (H)

- Die Sicherheitskonfiguration von OT-Komponenten SOLLTE regelmäßig und bedarfsorientiert bei plötzlich auftretenden neuen, bisher unbekannten Gefährdungen überprüft werden.
- Die Sicherheitsüberprüfung SOLLTE zumindest die exponierten Systeme mit Außenschnittstellen oder Benutzerinteraktion umfassen.
- Auch das realisierte Sicherheitskonzept SOLLTE regelmäßig überprüft werden.
- Die Sicherheitsüberprüfung SOLLTE als Konfigurationsprüfung oder auch durch automatisierte Konformitätsprüfungen erfolgen.

## IND.1.A24 Kommunikation im Störfall [Mitarbeiter, OT-Betrieb (Operational Technology, OT)] (H)

- Alternative und unabhängige Kommunikationsmöglichkeiten SOLLTEN aufgebaut und betrieben werden.


