# SYS.1.7: IBM Z

## SYS.1.7.A1 Einsatz restriktiver z/OS-Kennungen (B)

- Berechtigungen mit hoher Autorisierung DÜRFEN NUR an Benutzer vergeben werden, die diese Rechte für ihre Tätigkeiten benötigen.
- Insbesondere die RACF-Attribute SPECIAL, OPERATIONS, AUDITOR und die entsprechenden GROUP-Attribute sowie die User-ID 0 unter den Unix System Services (USS) MÜSSEN restriktiv gehandhabt werden.
- Die Vergabe und der Einsatz dieser Berechtigungen MÜSSEN nachvollziehbar sein.
- Die besondere Kennung IBMUSER DARF NUR bei der Neuinstallation zur Erzeugung von Kennungen mit Attribut SPECIAL benutzt werden.
- Diese Kennung MUSS danach dauerhaft gesperrt werden.
- Um zu vermeiden, dass Administratoren sich dauerhaft aussperren, MUSS ein Notfall-User-Verfahren eingerichtet werden.

## SYS.1.7.A2 Absicherung sicherheitskritischer z/OS-Dienstprogramme (B)

- Sicherheitskritische (Dienst-)Programme und Kommandos sowie deren Alias-Namen MÜSSEN mit Rechten auf entsprechende RACF-Profile so geschützt werden, dass sie nur von den dafür vorgesehenen und autorisierten Mitarbeitern benutzt werden können.
- Es MUSS sichergestellt sein, dass (Fremd-) Programme nicht unerlaubt installiert werden können.
- Außerdem DÜRFEN Programme NUR von gesicherten Quellen und über nachvollziehbare Methoden (z. B. SMP/E) installiert werden.

## SYS.1.7.A3 Wartung von Z-Systemen (B)

- Die Z-Hardware und -Firmware, das Betriebssystem sowie die verschiedenen Programme MÜSSEN regelmäßig und bei Bedarf gepflegt werden.
- Die hierfür notwendigen Wartungsaktivitäten MÜSSEN geplant und in das Änderungsmanagement (siehe OPS.1.1.3 Patch- und Änderungsmanagement) integriert werden.
- Insbesondere DÜRFEN Updates durch den Hersteller NUR unter Kontrolle des Betreibers durchgeführt werden, lokal über SE (Support Elements) bzw. HMC (Hardware Management Console) oder remote über die RSF (Remote Support Facility).

## SYS.1.7.A4 Schulung des z/OS-Bedienungspersonals [Vorgesetzte] (B)

- Administratoren, Bediener und Prüfer im z/OS-Bereich MÜSSEN entsprechend ihren Aufgaben ausgebildet sein.
- Insbesondere MÜSSEN RACF-Administratoren mit dem Sicherheitssystem selbst sowie gegebenenfalls mit den weiteren für sie relevanten Funktionen vertraut sein.

## SYS.1.7.A5 Einsatz und Sicherung systemnaher z/OS-Terminals (B)

- Systemnahe z/OS-Terminals MÜSSEN physisch gegen unbefugten Zutritt und logisch gegen unbefugten Zugang geschützt werden.
- Insbesondere die Support-Elemente sowie die HMC-, MCS-, SMCS-, Extended MCS- und Monitor-Konsolen MÜSSEN dabei berücksichtigt werden.
- Voreingestellte Passwörter MÜSSEN geändert werden.
- Zugänge über Webserver und andere Fernzugänge MÜSSEN durch Verschlüsselung geschützt werden.
- Nicht benötigte Webserver und Fernzugänge MÜSSEN deaktiviert werden, wenn sie nicht benötigt werden.

## SYS.1.7.A6 Einsatz und Sicherung der Remote Support Facility (B)

- Der Leiter des IT-Betriebs MUSS entscheiden, ob und gegebenenfalls wie RSF eingesetzt wird.
- Der Einsatz MUSS im Wartungsvertrag vorgesehen und mit dem Hardware-Support abgestimmt sein.
- Es MUSS sichergestellt werden, dass die RSF-Konfiguration nur von hierzu autorisierten Personen geändert werden kann.
- Wartungszugriffe für Firmware-Modifikationen durch den Hersteller MÜSSEN vom Betreiber explizit freigegeben und nach Beendigungwieder deaktiviert werden.
- Die RSF-Kommunikation MUSS über Proxy-Server und zusätzlich über gesicherte Verbindungen (wie TLS) stattfinden.

## SYS.1.7.A7 Restriktive Autorisierung unter z/OS (B)

- Im Rahmen der Grundkonfiguration MÜSSEN die Autorisierungsmechanismen so konfiguriert werden, dass alle Personen (definierte User-IDs in Gruppen gemäß Rolle) nur die Zugriffsmöglichkeiten erhalten, die sie für ihre jeweiligen Tätigkeiten benötigen.
- Hierfür MÜSSEN insbesondere APF-Autorisierungen (Authorized Program Facility), SVCs (SuperVisor Calls), Ressourcen des z/OS-Betriebssystems, IPL-Parameter, Parmlib-Definitionen, Started Tasks und JES2/3-Definitionen berücksichtigt werden.

## SYS.1.7.A8 Einsatz des z/OS-Sicherheitssystems RACF (B)

- Der Einsatz von RACF für z/OS MUSS sorgfältig geplant werden, dazu gehören auch die Auswahl des Zeichensatzes, die Festlegung von Regeln für User-ID und Passwort sowie die Aktivierung der KDFAES-Verschlüsselung.
- Falls RACF PassTickets verwendet werden, MUSS der Enhanced PassTicket Algorithmus aktiviert werden.
- Voreingestellte Passwörter für das RVARY-Kommando und für neu angelegte User-IDs MÜSSEN geändert werden.
- Falls RACF-Exits eingesetzt werden sollen, MUSS deren Einsatz begründet, dokumentiert und regelmäßig überwacht werden.
- Für das Anlegen, Sperren, Freischalten und Löschen von RACF-Kennungen MÜSSEN geeignete Vorgehensweisen festgelegt sein.
- Nach einer festgelegten Anzahl fehlgeschlagener Anmeldeversuche MUSS eine RACF-Kennung gesperrt werden (Ausnahme: Notfall-User-Verfahren).
- Kennungen von Benutzern MÜSSEN außerdem nach längerer Inaktivität gesperrt werden, Kennungen von Verfahren hingegen nicht.
- Dateien, Started Tasks und sicherheitskritische Programme MÜSSEN mittels RACF-Profilen geschützt werden.
- Benutzer DÜRFEN darüber NUR die Zugriffsmöglichkeiten erhalten, die sie gemäß ihrer Rolle benötigen.
- Es MUSS außerdem sichergestellt sein, dass Benutzer ihre Zugriffsmöglichkeiten nicht unerlaubt erweitern können.

## SYS.1.7.A9 Mandantenfähigkeit unter z/OS (B)

- Falls ein z/OS-System von Mandanten genutzt werden soll, MUSS ein RACF-Konzept zur Mandantentrennung erstellt werden.
- Die Daten und Anwendungen der Mandanten MÜSSEN durch RACF-Profile getrennt werden.
- Hohe Berechtigungen im RACF (SPECIAL, OPERATIONS, AUDITOR) und ändernden Zugriff auf Dateien des z/OS-Betriebssystems DÜRFEN NUR Mitarbeiter des Betreibers haben.
- Die Wartungsfenster, in denen das z/OS-System nicht zur Verfügung steht, MÜSSEN mit allen Mandanten, die auf dem betroffenen System arbeiten, abgestimmt werden.

## SYS.1.7.A10 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## SYS.1.7.A11 Schutz der Session-Daten (B)

- Session-Daten für die Verbindungen der RACF-Administratoren und möglichst auch der anderen Mitarbeiter MÜSSEN verschlüsselt übertragen werden.

## SYS.1.7.A12 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.1.7.A13 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.1.7.A14 Berichtswesen zum sicheren Betrieb von z/OS (S)

- Zur Überwachung aller sicherheitsrelevanten Tätigkeiten unter z/OS SOLLTE ein Prozess eingerichtet werden.
- In diesem SOLLTE festgelegt sein, welche Sicherheitsreports regelmäßig erstellt werden, welche Tools und Datenquellen dabei herangezogen werden (z. B. System Management Facility) und wie mit Abweichungen von den Vorgaben umgegangen wird.
- Die Sicherheitsreports SOLLTEN bei Überprüfungen als Information verwendet werden.

## SYS.1.7.A15 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.1.7.A16 Überwachung von z/OS-Systemen (S)

- Während des Betriebs SOLLTE das z/OS-System auf wichtige Meldungen, Ereignisse und die Einhaltung von Grenzwerten überwacht werden.
- Insbesondere Fehlermeldungen auf der HMC-Konsole, WTOR- und wichtige WTONachrichten (Write To Operator/with Reply), System Tasks, Sicherheitsverletzungen, Kapazitätsgrenzen sowie die Systemauslastung SOLLTEN berücksichtigt werden.
- Für die Überwachung SOLLTEN außerdem mindestens die MCSKonsole, die System Management Facility, das SYSLOG und die relevanten Protokolldaten der Anwendungen herangezogen werden.
- Es SOLLTE gewährleistet sein, dass alle wichtigen Meldungen zeitnah erkannt werden und, falls notwendig, in geeigneter Weise darauf reagiert wird.
- Systemnachrichten SOLLTEN dabei so gefiltert werden, dass nur die wichtigen Nachrichten dargestellt werden.

## SYS.1.7.A17 Synchronisierung von z/OS-Passwörtern und RACF-Kommandos (S)

- Falls z/OS-Passwörter oder RACF-Kommandos über mehrere z/OS-Systeme automatisch synchronisiert werden sollen, SOLLTEN die jeweiligen Systeme möglichst weitgehend standardisiert sein.
- Die Sperrung von Benutzerkennungen durch Fehleingaben von Passwörtern SOLLTE NICHT synchronisiert werden.
- Das Risiko durch Synchronisation sicherheitskritischer RACF-Kommandos SOLLTE berücksichtigt werden.
- Die Verwaltungsfunktion des Synchronisationsprogramms SOLLTE nur autorisierten Mitarbeitern im Rahmen ihrer Tätigkeit zur Verfügung stehen.

## SYS.1.7.A18 Rollenkonzept für z/OS-Systeme (S)

- Mindestens für die Systemverwaltung von z/OS-Systemen SOLLTE ein Rollenkonzept eingeführt werden.
- Für alle wichtigen Rollen der Systemverwaltung SOLLTEN außerdem Stellvertreter-Regelungen vorhanden sein.
- Die RACFAttribute SPECIAL, OPERATIONS und AUDITOR SOLLTEN verschiedenen Personen zugeordnet werden (Rollentrennung).

## SYS.1.7.A19 Absicherung von z/OS-Transaktionsmonitoren (S)

- Falls Transaktionsmonitore oder Datenbanken unter z/OS eingesetzt werden, wie beispielsweise IMS, CICS oder Db2, SOLLTEN diese mittels RACF abgesichert werden.
- Dies gilt auch für die zugehörigen System-Kommandos und -Dateien.
- Interne Sicherheitsmechanismen der Transaktionsmonitore und Datenbanken SOLLTEN hingegen nur dort angewandt werden, wo es keine entsprechenden RACF-Funktionen gibt.
- Benutzer und Administratoren SOLLTEN nur die Zugriffsrechte erhalten, die sie für ihre jeweilige Tätigkeit benötigen.

## SYS.1.7.A20 Stilllegung von z/OS-Systemen (S)

- Bei der Stilllegung von z/OS-Systemen SOLLTEN andere z/OS-Systeme, Verbünde und Verwaltungssysteme so angepasst werden, dass sie nicht mehr auf das stillgelegte System verweisen.
- Auch die Auswirkungen auf die SoftwareLizenzen SOLLTEN berücksichtigt werden.
- Festplatten, die vertrauliche Daten enthalten, SOLLTEN so gelöscht werden, dass ihr Inhalt nicht mehr reproduziert werden kann.
- Für den Fall, dass defekte Festplatten durch den Hersteller ausgetauscht werden, SOLLTE vertraglich vereinbart sein, dass diese Festplatten sicher vernichtet oder so gelöscht werden, dass ihr Inhalt nicht mehr reproduziert werden kann.

## SYS.1.7.A21 Absicherung des Startvorgangs von z/OS-Systemen (S)

- Die für den Startvorgang eines z/OS-Systems notwendigen Parameter SOLLTEN dokumentiert und dem OperatingPersonal bekannt sein.
- Außerdem SOLLTEN die erforderlichen Hardware-Konfigurationen vorliegen, wie die IOCDSDatei (Input/Output Configuration Data Set) und die LPARs (Logical Partitions).
- Eine z/OS-Master-Konsole und eine Backup-Konsole SOLLTEN definiert sein, um Nachrichten kontrollieren zu können.
- Nach dem Startvorgang SOLLTE anhand einer Prüfliste kontrolliert werden, ob der Systemstatus den Soll-Vorgaben entspricht.
- Darüber hinaus SOLLTE eine Fallback-Konfiguration vorgehalten werden, mit der das System vor der letzten Änderung erfolgreich gestartet worden ist.

## SYS.1.7.A22 Absicherung der Betriebsfunktionen von z/OS (S)

- Alle die Produktion beeinflussenden Wartungsarbeiten sowie dynamische und sonstige Änderungen SOLLTEN nur im Rahmen des Änderungsmanagements durchgeführt werden (siehe OPS.1.1.3 Patch- und Änderungsmanagement).
- SDSF (System Display and Search Facility) und ähnliche Funktionen sowie die Prioritäten-Steuerung für Jobs SOLLTEN mittels RACF vor unberechtigtem Zugriff geschützt werden.
- z/OS-System-Kommandos und besonders sicherheitsrelevante Befehle für dynamische Änderungen SOLLTEN über RACF geschützt werden.
- Bei der dynamischen Definition von Hardware SOLLTE sichergestellt werden, dass eine Ressource im Wirkbetrieb nicht mehreren Einzelsystemen außerhalb eines Parallel Sysplex zugeordnet wird.

## SYS.1.7.A23 Absicherung von z/VM (S)

- Falls z/VM eingesetzt wird, SOLLTE das Produkt in das Patch-Management integriert werden.
- Alle voreingestellten Passwörter SOLLTEN geändert werden.
- Die Rolle des z/VM-Systemadministrators SOLLTE nur an Personen vergeben werden, die diese Berechtigungen benötigen.
- Die Sicherheitsadministration von z/VM SOLLTE über RACF für z/VM erfolgen.
- Passwörter von realen Usern und Guest-Usern SOLLTEN mittels RACF für z/VM verschlüsselt werden.
- Die sicherheitskritischen Systemkommandos von z/VM SOLLTEN über RACF geschützt werden.
- Unter z/VM definierte virtuelle Maschinen SOLLTEN nur die für die jeweiligen Aufgaben notwendigen Ressourcen erhalten und strikt voneinander getrennt sein.
- Unter z/VM SOLLTEN nur die benötigten Dienste gestartet werden.
- Wenn Überprüfungen durchgeführt werden, SOLLTEN die Journaling-Funktion von z/VM und die Audit-Funktionen von RACF eingesetzt werden.

## SYS.1.7.A24 Datenträgerverwaltung unter z/OS-Systemen (S)

- Dateien, Programme und Funktionen zur Verwaltung von Datenträgern sowie die Datenträger selbst (Festplatten und Bänder) einschließlich Master-Katalog SOLLTEN mittels RACF-Profilen geschützt werden.
- Es SOLLTEN Sicherungskopien aller wichtigen Dateien zur Verfügung stehen, die in einer Notfallsituation zurückgespielt werden können.
- Die Zuordnung von Datenträgern zu den Z-Systemen SOLLTE nachvollziehbar sein.
- Es SOLLTE gewährleistet werden, dass je nach Volumen und Zeitfenster genügend Bandstationen zur Verfügung stehen.
- Beim Einsatz des HSM (Hierarchical Storage Manager) SOLLTE festgelegt werden, welche Festplatten gesichert werden sollen und wie die Sicherung erfolgen soll.
- Bänder, die vom HSM verwaltet werden, SOLLTEN NICHT anderweitig bearbeitet werden.

## SYS.1.7.A25 Festlegung der Systemdimensionierung von z/OS (S)

- Die Grenzen für die maximale Belastung der Ressourcen (Anzahl der CPUs, Speicher, Bandbreite etc.) SOLLTEN den Hardware-Voraussetzungen entsprechend festgelegt und den zuständigen Administratoren und Anwendungseignern bekannt sein.
- Die Anzahl der zur Verfügung stehenden Magnetband-Stationen, die Zeiten, zu denen Anwendungen auf Magnetband-Stationen zugreifen und die benötigten Festplattenkapazitäten SOLLTEN mit den Anwendungseignern abgestimmt sein.
- Die Festplattenkapazitäten SOLLTEN außerdem vom Space-Management überwacht werden.

## SYS.1.7.A26 WorkLoad Management für z/OS-Systeme (S)

- Die Programme, Dateien und Kommandos des WorkLoad Managers (WLM) sowie die dafür notwendigen Couple Data Sets SOLLTEN mittels RACF geschützt werden.
- Dabei SOLLTE sichergestellt sein, dass die Berechtigungen zum Ändern des WLM über z/OS-Kommandos und über die SDSF-Schnittstelle gleich sind.

## SYS.1.7.A27 Zeichensatzkonvertierung bei z/OS-Systemen (S)

- Wenn Textdateien zwischen z/OS-Systemen und anderen Systemen übertragen werden, SOLLTE darauf geachtet werden, dass eventuell eine Zeichensatzkonvertierung erforderlich ist.
- Dabei SOLLTE die korrekte Umsetzungstabelle verwendet werden.
- Bei der Übertragung von Programm-Quellcode SOLLTE geprüft werden, ob alle Zeichen richtig übersetzt wurden.
- Bei der Übertragung von Binärdaten SOLLTE hingegen sichergestellt sein, dass keine Zeichensatzkonvertierung stattfindet.

## SYS.1.7.A28 Lizenzschlüssel-Management für z/OS-Software (S)

- Für Lizenzschlüssel, deren Gültigkeit zeitlich begrenzt ist, SOLLTE ein Verfahren zur rechtzeitigen Erneuerung eingerichtet sein.
- Die Laufzeiten der Lizenzschlüssel SOLLTEN dokumentiert werden.
- Die Dokumentation SOLLTE allen betroffenen Administratoren zur Verfügung stehen.

## SYS.1.7.A29 Absicherung von Unix System Services bei z/OS-Systemen (S)

- Die Parameter der Unix System Services (USS) SOLLTEN entsprechend der funktionalen und sicherheitstechnischen Vorgaben sowie unter Berücksichtigung der verfügbaren Ressourcen eingestellt werden.
- HFS- und zFS-Dateien, die USS-Dateisysteme enthalten, SOLLTEN über RACF-Profile abgesichert und in das Datensicherungskonzept einbezogen werden.
- Außerdem SOLLTE das Root-Dateisystem mit der Option Read-Only gemounted werden.
- Es SOLLTE im USS-Dateisystem KEINE APF-Autorisierung (Authorized Program Facility) über das File Security Packet (FSP) geben.
- Stattdessen SOLLTEN die Module von APF-Dateien des z/OS-Betriebssystems geladen werden.
- Zwischen USS-UserIDs und z/OS-User-IDs SOLLTE es eine eindeutige Zuordnung geben.
- Berechtigungen unter USS SOLLTEN über die RACF-Klasse UNIXPRIV vergeben werden und NICHT durch Vergabe der UID 0. Für Überprüfungen und das Monitoring der USS SOLLTEN die gleichen Mechanismen wie für z/OS genutzt werden.

## SYS.1.7.A30 Absicherung der z/OS-Trace-Funktionen (S)

- Die Trace-Funktionen von z/OS wie GTF (Generalized Trace Facility), NetView oder ACF/TAP (Advanced Communication Function/Trace Analysis Program) und die entsprechenden Dateien SOLLTEN so geschützt werden, dass nur die zuständigen und autorisierten Mitarbeiter darauf Zugriff haben.
- Die Trace-Funktion von NetView SOLLTE deaktiviert sein und nur im Bedarfsfall aktiviert werden.

## SYS.1.7.A31 Notfallvorsorge für z/OS-Systeme (S)

- Es SOLLTE ein Verfahren zur Wiederherstellung einer funktionierenden RACF-Datenbank vorgesehen sein.
- Weiterhin SOLLTEN eine Kopie des z/OS-Betriebssystems als z/OS-Backup-System und, unabhängig von Produktivsystem, ein z/OS-Notfallsystem vorgehalten werden.

## SYS.1.7.A32 Festlegung von Standards für z/OS-Systemdefinitionen (H)

- Es SOLLTEN Standards und Namenskonventionen für z/OS-Systemdefinitionen festgelegt und dokumentiert werden.
- Die Dokumentationen SOLLTEN den Administratoren zur Verfügung stehen.
- Die Einhaltung der Standards SOLLTE regelmäßig überprüft werden.
- Standards SOLLTEN insbesondere für Datei-, Datenbank-, Job- und VolumeNamen sowie für Application-, System- und User-IDs definiert werden.

## SYS.1.7.A33 Trennung von Test- und Produktionssystemen unter z/OS (H)

- Es SOLLTEN technische Maßnahmen ergriffen werden, um Entwicklungs- und Testsysteme von Produktionssystemen unter z/OS zu trennen.
- Dabei SOLLTEN eventuelle Zugriffsmöglichkeiten über gemeinsame Festplatten und den Parallel Sysplex beachtet werden.

## SYS.1.7.A34 Batch-Job-Planung für z/OS-Systeme (H)

- Wenn ein z/OS-System eine größere Anzahl von Batch-Jobs verarbeitet, SOLLTE für die Ablaufsteuerung der BatchJobs ein Job-Scheduler eingesetzt werden.
- Der Job-Scheduler sowie die zugehörigen Dateien und Tools SOLLTEN mittels RACF geeignet geschützt werden.

## SYS.1.7.A35 Einsatz von RACF-Exits (H)

- Falls RACF-Exits eingesetzt werden, SOLLTEN die sicherheitstechnischen und betrieblichen Auswirkungen analysiert werden.
- Die RACF-Exits SOLLTEN außerdem über das SMP/E (System Modification Program/Enhanced) als USERMOD installiert und überwacht werden.

## SYS.1.7.A36 Interne Kommunikation von Betriebssystemen (H)

- Die Kommunikation von Betriebssystemen, z/OS oder Linux, die entweder im LPAR-Mode oder unter z/VM auf derselben Z-Hardware installiert sind, SOLLTE über interne Kanäle erfolgen, d. h. über HiperSockets oder virtuelle CTCVerbindungen (Channel-to-Channel).

## SYS.1.7.A37 Parallel Sysplex unter z/OS (H)

- Anhand der Verfügbarkeits- und Skalierbarkeitsanforderungen SOLLTE entschieden werden, ob ein Parallel Sysplex (Cluster von z/OS-Systemen) eingesetzt wird und gegebenenfalls welche Redundanzen dabei vorgesehen werden.
- Bei der Dimensionierung der Ressourcen SOLLTEN die Anforderungen der Anwendungen berücksichtigt werden.
- Die Software und die Definitionen der LPARs des Sysplex, einschließlich RACF, SOLLTEN synchronisiert oder als gemeinsam benutzte Dateien bereitgestellt sein.
- Es SOLLTE sichergestellt sein, dass alle LPARs des Sysplex auf die Couple Data Sets zugreifen können.
- Die Couple Data Sets sowie alle sicherheitskritischen Programme und Kommandos zur Verwaltung des Sysplex SOLLTEN mittels RACF geschützt werden.
- Außerdem SOLLTE ein GRS-Verbund (Global Resource Serialization) eingerichtet werden.
- Die Festplatten des Sysplexes SOLLTEN strikt von den Festplatten anderer Systeme getrennt werden.
- Der System Logger SOLLTE mit Staging Data Set eingesetzt werden.

## SYS.1.7.A38 Einsatz des VTAM Session Management Exit unter z/OS (H)

- Falls ein VTAM Session Management Exit eingesetzt werden soll, SOLLTE gewährleistet werden, dass dadurch der sichere und performante Betrieb nicht beeinträchtigt wird.
- Der Exit SOLLTE mindestens eine nachträgliche Kontrolle der abgewiesenen Login-Versuche ermöglichen.
- Außerdem SOLLTE sich der Exit dynamisch konfigurieren lassen und das Regelwerk von einer externen Datei nachladen.
- Funktionen, Kommandos und Dateien im Zusammenhang mit dem Exit SOLLTEN durch RACF geschützt werden.


