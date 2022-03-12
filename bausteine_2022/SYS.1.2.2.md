# SYS.1.2.2: Windows Server 2012

## SYS.1.2.2.A1 Planung von Windows Server 2012 (B)

- Der Einsatz von Windows Server 2012 MUSS vor der Installation sorgfältig geplant werden.
- Die Anforderungen an die Hardware MÜSSEN vor der Beschaffung geprüft werden.
- Es MUSS eine begründete und dokumentierte Entscheidung für eine geeignete Edition des Windows Server 2012 getroffen werden.
- Der Einsatzzweck des Servers sowie die Einbindung ins Active Directory MÜSSEN dabei spezifiziert werden.
- Die Nutzung von ins Betriebssystem integrierten Cloud-Diensten MUSS grundsätzlich abgewogen und geplant werden.
- Wenn nicht benötigt, MUSS die Einrichtung von Microsoft-Konten auf dem Server blockiert werden.

## SYS.1.2.2.A2 Sichere Installation von Windows Server 2012 (B)

- Es DÜRFEN KEINE anderen als die benötigten Serverrollen und Features bzw. Funktionen installiert werden.
- Wenn es vom Funktionsumfang her ausreichend ist, MUSS die Server-Core-Variante installiert werden.
- Andernfalls MUSS begründet werden, warum die Server-Core-Variante nicht genügt.
- Der Server MUSS bereits während der Installation auf einen aktuellen Patch-Stand gebracht werden.

## SYS.1.2.2.A3 Sichere Administration von Windows Server 2012 (B)

- Alle Administratoren, die für das Server-System zuständig sind, MÜSSEN in den sicherheitsrelevanten Aspekten der Administration von Windows Server 2012 geschult sein.
- Webbrowser auf dem Server DÜRFEN NICHT zum Surfen im Web verwendet werden.

## SYS.1.2.2.A4 Sichere Konfiguration von Windows Server 2012 (S)

- Mehrere wesentliche Funktionen bzw. Rollen SOLLTEN NICHT durch einen einzigen Server erfüllt, sondern geeignet aufgeteilt werden.
- Vor Inbetriebnahme SOLLTE das System grundlegend gehärtet werden.
- Dafür SOLLTEN funktionsspezifische und institutionsweite Sicherheitsvorlagen erstellt und gepflegt werden, die auf die Server ausgerollt werden.
- Der Internet Explorer SOLLTE auf dem Server nur in der Enhanced Security Configuration und im Enhanced Protected Mode genutzt werden.

## SYS.1.2.2.A5 Schutz vor Schadsoftware auf Windows Server 2012 (S)

- Außer bei IT-Systemen mit Windows Server 2012, die als Stand-alone-Gerät ohne Netzanschluss und Wechselmedien betrieben werden, SOLLTE vor dem ersten Verbinden mit dem Netz oder Wechselmedien ein Virenschutzprogramm installiert werden.
- Im Konzept zum Schutz vor Schadsoftware SOLLTE vorgesehen werden, dass regelmäßig alle Festplatten vollständig gescannt werden.
- Es SOLLTEN Alarme für die zuständigen Administratoren bei Virenfunden konfiguriert sein.

## SYS.1.2.2.A6 Sichere Authentisierung und Autorisierung in Windows Server 2012 (S)

- In Windows Server 2012 R2 SOLLTEN alle Benutzer Mitglieder der Sicherheitsgruppe „Geschützte Nutzer“ sein.
- Konten für Dienste und Computer SOLLTEN NICHT Mitglied von „Geschützte Nutzer“ sein.
- Dienste-Konten in Windows Server 2012 SOLLTEN Mitglieder der Gruppe „Managed Service Account“ sein.
- Der PPL-Schutz des Local Credential Store LSA SOLLTE aktiviert werden.
- Der Einsatz dynamischer Zugriffsregeln auf Ressourcen SOLLTE bevorzugt werden.

## SYS.1.2.2.A7 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.1.2.2.A8 Schutz der Systemintegrität (S)

- AppLocker SOLLTE aktiviert und möglichst strikt konfiguriert sein.

## SYS.1.2.2.A9 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.1.2.2.A10 ENTFALLEN (H)

- Diese Anforderung ist entfallen.

## SYS.1.2.2.A11 Angriffserkennung bei Windows Server 2012 (H)

- Sicherheitsrelevante Ereignisse in Windows Server 2012 SOLLTEN an einem zentralen Punkt gesammelt und ausgewertet werden.
- Verschlüsselte Partitionen SOLLTEN nach einer definierten Anzahl von Entschlüsselungsversuchen gesperrt werden.

## SYS.1.2.2.A12 Redundanz und Hochverfügbarkeit bei Windows Server 2012 (H)

- Es SOLLTE geprüft werden, welche Verfügbarkeitsanforderungen durch Betriebssystemfunktionen wie Distributed File System (DFS), ReFS, Failover Cluster und Network Load Balancing bzw. NIC-Teaming (LBFO) erfüllt oder unterstützt werden können.
- Für Außenstellen SOLLTE BranchCache aktiviert werden.

## SYS.1.2.2.A13 ENTFALLEN (H)

- Diese Anforderung ist entfallen.

## SYS.1.2.2.A14 Herunterfahren verschlüsselter Server und virtueller Maschinen (H)

- Um verschlüsselten Daten zu schützen, SOLLTEN nicht benötigte Server (inkl. virtuelle Maschinen) immer heruntergefahren werden.
- Dies SOLLTE möglichst automatisiert erfolgen.
- Die Entschlüsselung der Daten SOLLTE einen interaktiven Schritt erfordern oder zumindest im Sicherheitsprotokoll festgehalten werden.


