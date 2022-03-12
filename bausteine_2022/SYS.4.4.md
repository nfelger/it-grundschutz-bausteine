# SYS.4.4: Allgemeines IoT-Gerät

## SYS.4.4.A1 Einsatzkriterien für IoT-Geräte (B)

- IoT-Geräte MÜSSEN Update-Funktionen besitzen.
- Der Hersteller MUSS einen Update-Prozess anbieten.
- Die Geräte MÜSSEN eine angemessene Authentisierung ermöglichen.
- Es DÜRFEN KEINE fest codierten Zugangsdaten in den Geräten existieren.

## SYS.4.4.A2 Authentisierung (B)

- Eine angemessene Authentisierung MUSS aktiviert sein.
- IoT-Gerate MÜSSEN in das Identitäts- und Berechtigungsmanagement der Institution integriert werden.

## SYS.4.4.A3 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## SYS.4.4.A4 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## SYS.4.4.A5 Einschränkung des Netzzugriffs (B)

- Der Netzzugriff von IoT-Geräten MUSS auf das erforderliche Minimum eingeschränkt werden.
- Dies SOLLTE regelmäßig kontrolliert werden.
- Dazu SOLLTEN folgende Punkte beachtet werden:
    - Bei Verkehrskontrollen an Netzübergängen, z. B. durch Regelwerke auf Firewalls und Access Control Lists (ACLs) auf Routern, DÜRFEN NUR zuvor definierte ein- und ausgehende Verbindungen erlaubt werden.
    - Die Routings auf IoT-Geräten und Sensoren, insbesondere die Unterdrückung von Default-Routen, SOLLTE restriktiv konfiguriert werden.
    - Die IoT-Geräte und Sensoren SOLLTEN in einem eigenen Netzsegment betrieben werden, das ausschließlich mit dem Netzsegment für das Management kommunizieren darf.
    - Virtual Private Networks (VPNs) zwischen den Netzen mit IoT-Geräten und Sensor-Netzen und den Management-Netzen SOLLTE restriktiv konfiguriert werden.
    - Die UPnP-Funktion MUSS an allen Routern deaktiviert sein.

## SYS.4.4.A6 Aufnahme von IoT-Geräten in die Sicherheitsrichtlinie der Institution (S)

- In der allgemeinen Sicherheitsrichtlinie der Institution SOLLTEN die Anforderungen an IoT-Geräte konkretisiert werden.
- Die Richtlinie SOLLTE allen Personen, die IoT-Geräte beschaffen und betreiben, bekannt und Grundlage fürderen Arbeit sein.
- Die Umsetzung der in der Richtlinie geforderten Inhalte SOLLTE regelmäßig überprüft und die Ergebnisse sinnvoll dokumentiert werden.

## SYS.4.4.A7 Planung des Einsatzes von IoT-Geräten (S)

- Um einen sicheren Betrieb von IoT-Geräten zu gewährleisten, SOLLTE im Vorfeld geplant werden, wo und wie diese eingesetzt werden sollen.
- Die Planung SOLLTE dabei nicht nur Aspekte betreffen, die klassischerweise mit dem Begriff Informationssicherheit verknüpft werden, sondern auch normale, betriebliche Aspekte, die Anforderungen im Bereich der Sicherheit nach sich ziehen.
- Alle Entscheidungen, die in der Planungsphase getroffen wurden, SOLLTEN geeignet dokumentiert werden.

## SYS.4.4.A8 Beschaffungskriterien für IoT-Geräte [Beschaffungsstelle] (S)

- Der ISB SOLLTE auch bei Beschaffungen von IoT-Geräten mit einbezogen werden, die keine offensichtlichen ITFunktionen haben.
- Bevor IoT-Geräte beschafft werden, SOLLTE festgelegt werden, welche Sicherheitsanforderungen diese erfüllen müssen.
- Bei der Beschaffung von IoT-Geräten SOLLTEN Aspekte der materiellen Sicherheit ebenso wie Anforderungen an die Sicherheitseigenschaften der Software ausreichend berücksichtigt werden.
- Eine Anforderungsliste SOLLTE erstellt werden, anhand derer die am Markt erhältlichen Produkte bewertet werden.

## SYS.4.4.A9 Regelung des Einsatzes von IoT-Geräten (S)

- Für jedes IoT-Gerät SOLLTE ein Zuständiger für dessen Betrieb benannt werden.
- Die Zuständigen SOLLTEN ausreichend über den Umgang mit dem IoT-Gerät informiert werden.

## SYS.4.4.A10 Sichere Installation und Konfiguration von IoT-Geräten (S)

- Es SOLLTE festgelegt werden, unter welchen Rahmenbedingungen IoT-Geräte installiert und konfiguriert werden.
- Die IoT-Geräte SOLLTE nur von autorisierten Personen (Zuständige für IoT-Geräte, Administratoren oder vertraglich gebundene Dienstleister) nach einem definierten Prozess installiert und konfiguriert werden.
- Alle Installations- und Konfigurationsschritte SOLLTEN so dokumentiert werden, dass die Installation und Konfiguration durch einen sachkundigen Dritten anhand der Dokumentation nachvollzogen und wiederholt werden kann.
- Die Grundeinstellungen von IoT-Geräten SOLLTEN überprüft und nötigenfalls entsprechend den Vorgaben der Sicherheitsrichtlinie angepasst werden.
- Falls möglich, SOLLTEN IoT-Geräte erst mit Datennetzen verbunden werden, nachdem die Installation und die Konfiguration abgeschlossen sind.

## SYS.4.4.A11 Verwendung von verschlüsselter Datenübertragung (S)

- IoT-Geräte SOLLTEN Daten nur verschlüsselt übertragen.

## SYS.4.4.A12 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.4.4.A13 Deaktivierung und Deinstallation nicht benötigter Komponenten (S)

- Nach der Installation SOLLTE überprüft werden, welche Protokolle, Anwendungen und weiteren Tools auf den IoTGeräten installiert und aktiviert sind.
- Nicht benötigte Protokolle, Dienste, Benutzerkennungen und Schnittstellen SOLLTEN deaktiviert oder ganz deinstalliert werden.
- Die Verwendung von nicht benötigten Funkschnittstellen SOLLTE unterbunden werden.
- Wenn dies nicht am Gerät selber möglich ist, SOLLTEN nicht benötigte Dienste über die Firewall eingeschränkt werden.
- Die getroffenen Entscheidungen SOLLTEN so dokumentiert werden, dass nachvollzogen werden kann, welche Konfiguration für die IoT-Geräte gewählt wurden.

## SYS.4.4.A14 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.4.4.A15 Restriktive Rechtevergabe (S)

- Die Zugriffsberechtigungen auf IoT-Geräte SOLLTEN möglichst restriktiv vergeben werden.
- Wenn dies über die IoTGeräte selber nicht möglich ist, SOLLTE überlegt werden, dies netzseitig zu regeln.

## SYS.4.4.A16 Beseitigung von Schadprogrammen auf IoT-Geräten (S)

- Der IT-Betrieb SOLLTE sich regelmäßig informieren, ob sich die eingesetzten IoT-Geräte mit Schadprogrammen infizieren könnten und wie diese beseitigt werden können.
- Schadprogramme SOLLTEN unverzüglich beseitigt werden.
- Kann die Ursache für die Infektion nicht behoben bzw. eine Neuinfektion nicht wirksam verhindert werden, SOLLTEN die betroffenen IoT-Geräte nicht mehr verwendet werden.

## SYS.4.4.A17 Überwachung des Netzverkehrs von IoT-Geräten (S)

- Es SOLLTE überwacht werden, ob die IoT-Geräte oder Sensor-Systeme nur mit IT-Systemen kommunizieren, die für den Betrieb der IoT-Geräte notwendig sind.

## SYS.4.4.A18 Protokollierung sicherheitsrelevanter Ereignisse bei IoT-Geräten (S)

- Sicherheitsrelevante Ereignisse SOLLTEN automatisch protokolliert werden.
- Falls dies durch die IoT-Geräte selber nicht möglich ist, SOLLTEN hierfür Router oder Protokollmechanismen anderer IT-Systeme genutzt werden.
- Die Protokolle SOLLTEN geeignet ausgewertet werden.

## SYS.4.4.A19 Schutz der Administrationsschnittstellen (S)

- Abhängig davon, ob IoT-Geräte lokal, direkt über das Netz oder über zentrale netzbasierte Tools administriert werden, SOLLTEN geeignete Sicherheitsvorkehrungen getroffen werden.
- Der Zugriff auf die Administrationsschnittstellen von IoT-Geräten SOLLTE wie folgt eingeschränkt werden:
    - Netzbasierte Administrationsschnittstellen SOLLTEN auf berechtigte IT-Systeme bzw. Netzsegmente beschränkt werden.
    - Es SOLLTEN bevorzugt lokale Administrationsschnittstellen am IoT-Gerät oder Administrationsschnittstellen über lokale Netze verwendet werden.
- Die zur Administration verwendeten Methoden SOLLTEN in der Sicherheitsrichtlinie festgelegt werden.
- Die IoTGeräte SOLLTEN entsprechend der Sicherheitsrichtlinie administriert werden.

## SYS.4.4.A20 Geregelte Außerbetriebnahme von IoT-Geräten (S)

- Es SOLLTE eine Übersicht darüber geben, welche Daten wo auf IoT-Geräten gespeichert sind.
- Es SOLLTE eine Checkliste erstellt werden, die bei der Außerbetriebnahme von IoT-Geräten abgearbeitet werden kann.
- Diese Checkliste SOLLTE mindestens Aspekte zur Datensicherung weiterhin benötigter Daten und dem anschließenden sicheren Löschen aller Daten umfassen.

## SYS.4.4.A21 Einsatzumgebung und Stromversorgung [Haustechnik] (H)

- Es SOLLTE geklärt werden, ob IoT-Geräte in der angedachten Einsatzumgebung betrieben werden dürfen (Schutzbedarf anderer IT-Systeme, Datenschutz).
- IoT-Geräte SOLLTEN in der Einsatzumgebung vor Diebstahl, Zerstörung und Manipulation geschützt werden.
- Es SOLLTE geklärt sein, ob ein IoT-Gerät bestimmte Anforderungen an die physische Einsatzumgebung hat, wie z. B. Luftfeuchtigkeit, Temperatur oder Energieversorgung.
- Falls erforderlich, SOLLTEN dafür ergänzende Maßnahmen bei der Infrastruktur umgesetzt werden.
- Wenn IoT-Geräte mit Batterien betrieben werden, SOLLTE der regelmäßige Funktionstest und Austausch der Batterien geregelt werden.
- IoT-Geräte SOLLTEN entsprechend ihrer vorgesehenen Einsatzart und dem vorgesehenen Einsatzort vor Staub und Verschmutzungen geschützt werden.

## SYS.4.4.A22 Systemüberwachung (H)

- Die IoT-Geräte SOLLTEN in ein geeignetes Systemüberwachungs- bzw. Monitoringkonzept eingebunden werden.
- Dieses SOLLTE den Systemzustand und die Funktionsfähigkeit der IoT-Geräte laufend überwachen und Fehlerzustände sowie die Überschreitung definierter Grenzwerte an das Betriebspersonal melden.
- Es SOLLTE geprüft werden, ob die verwendeten Geräte die Anforderung an die Verfügbarkeit erfüllen.
- Alternativ SOLLTE geprüft werden, ob weitere Maßnahmen, wie das Einrichten eines Clusters oder die Beschaffung von Standby-Geräten, erforderlich sind.

## SYS.4.4.A23 Auditierung von IoT-Geräten (H)

- Alle eingesetzten IoT-Geräte SOLLTEN regelmäßig überprüft werden.

## SYS.4.4.A24 Sichere Konfiguration und Nutzung eines eingebetteten Webservers (H)

- In IoT-Geräten integrierte Webserver SOLLTEN möglichst restriktiv konfiguriert sein.
- Der Webserver SOLLTE, soweit möglich, NICHT unter einem privilegierten Konto betrieben werden.


