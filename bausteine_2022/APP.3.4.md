# APP.3.4: Samba

## APP.3.4.A1 Planung des Einsatzes eines Samba-Servers (B)

- Der IT-Betrieb MUSS die Einführung eines Samba-Servers sorgfältig planen und regeln.
- Sie MUSS abhängig vom Einsatzszenario definieren, welche Aufgaben der Samba-Server zukünftig erfüllen soll und in welcher Betriebsarter betrieben wird.
- Außerdem MUSS festgelegt werden, welche Komponenten von Samba und welche weiteren Komponenten dafür erforderlich sind.
- Soll die Cluster-Lösung CTDB (Cluster Trivia Data Base) eingesetzt werden, MUSS der IT-Betrieb diese Lösung sorgfältig konzeptionieren.
- Falls Samba die Active-Directory-(AD)-Dienste auch für Linux- und Unix-Systeme bereitstellen soll, MÜSSEN diese Diente ebenfalls sorgfältig geplant und getestet werden.
- Des Weiteren MUSS das Authentisierungsverfahren für das AD sorgfältig konzipiert und implementiert werden.
- Die Einführung und die Reihenfolge, in der die Stackable-Virtual-File-System-(VFS)-Module ausgeführt werden, MUSS sorgfältig konzipiert werden.
- Die Umsetzung SOLLTE dokumentiert werden.
- Soll IPv6 unter Samba eingesetzt werden, MUSS auch dies sorgfältig geplant werden Zudem MUSS in einer betriebsnahen Testumgebung überprüft werden, ob die Integration fehlerfrei funktioniert.

## APP.3.4.A2 Sichere Grundkonfiguration eines Samba-Servers (B)

- Der IT-Betrieb MUSS den Samba-Server sicher konfigurieren.
- Hierfür MÜSSEN unter anderem die Einstellungen für die Zugriffskontrollen angepasst werden.
- Das gleiche SOLLTE auch für Einstellungen gelten, welche die Leistungsfähigkeit des Servers beeinflussen.
- Samba MUSS vom IT-Betrieb so konfiguriert werden, dass Verbindungen nur von sicheren Hosts und Netzen entgegengenommen werden.
- Änderungen an der Konfiguration SOLLTEN sorgfältig dokumentiert werden, sodass zu jeder Zeit nachvollzogen werden kann, wer aus welchem Grund was geändert hat.
- Dabei MUSS nach jeder Änderung überprüft werden, ob die Syntax der Konfigurationsdatei noch korrekt ist.
- Zusätzliche Softwaremodule wie SWAT DÜRFEN NICHT installiert werden.

## APP.3.4.A3 Sichere Konfiguration eines Samba-Servers (S)

- Datenbanken im Trivial-Database-(TDB)-Format SOLLTEN NICHT auf einer Partition gespeichert werden, die ReiserFS als Dateisystem benutzt.
- Wird eine netlogon-Freigabe konfiguriert, SOLLTEN unberechtigte Benutzer KEINE Dateien in dieser Freigabe modifizieren können.
- Das Betriebssystem eines Samba-Servers SOLLTE Access Control Lists (ACLs) in Verbindung mit dem eingesetzten Dateisystem unterstützen.
- Zusätzlich SOLLTE sichergestellt werden, dass das Dateisystem mit den passenden Parametern eingebunden wird.
- Die Voreinstellungen von SMB Message Signing SOLLTEN beibehalten werden, sofern sie nicht im Widerspruch zu den existierenden Sicherheitsrichtlinien im Informationsverbund stehen.

## APP.3.4.A4 Vermeidung der NTFS-Eigenschaften auf einem Samba-Server (S)

- Wird eine Version von Samba eingesetzt, die im New Technology File System (NTFS) keine ADS abbilden kann und sollen Dateisystemobjekte über Systemgrenzen hinweg kopiert oder verschoben werden, SOLLTEN Dateisystemobjekte KEINE ADS mit wichtigen Informationen enthalten.

## APP.3.4.A5 Sichere Konfiguration der Zugriffssteuerung bei einem Samba-Server (S)

- Die von Samba standardmäßig verwendeten Parameter, mit denen DOS-Attribute auf das Unix-Dateisystem abgebildet werden, SOLLTEN NICHT verwendet werden.
- Stattdessen SOLLTE Samba so konfiguriert werden, dass es DOS-Attribute und die Statusindikatoren zur Vererbung (Flag) in Extended Attributes speichert.
- Die Freigaben SOLLTEN ausschließlich über die Samba-Registry verwaltet werden.
- Ferner SOLLTEN die effektiven Zugriffsberechtigungen auf die Freigaben des Samba-Servers regelmäßig überprüft werden.

## APP.3.4.A6 Sichere Konfiguration von Winbind unter Samba (S)

- Für jeden Windows-Domänenbenutzer SOLLTE im Betriebssystem des Servers ein Benutzerkonto mit allen notwendigen Gruppenmitgliedschaften vorhanden sein.
- Falls das nicht möglich ist, SOLLTE Winbind eingesetzt werden.
- Dabei SOLLTE Winbind Domänen-Benutzernamen in eindeutige Unix-Benutzernamen umsetzen.
- Beim Einsatz von Winbind SOLLTE sichergestellt werden, dass Kollisionen zwischen lokalen Unix-Benutzern und Domänen-Benutzern verhindert werden.
- Des Weiteren SOLLTEN die PAM (Pluggable Authentication Modules) eingebunden werden.

## APP.3.4.A7 Sichere Konfiguration von DNS unter Samba (S)

- Wenn Samba als DNS-Server eingesetzt wird, SOLLTE die Einführung sorgfältig geplant und die Umsetzung vorab getestet werden.
- Da Samba verschiedene AD-Integrationsmodi unterstützt, SOLLTE der IT-Betrieb die DNS-Einstellungen entsprechend dem Verwendungsszenario von Samba vornehmen.

## APP.3.4.A8 Sichere Konfiguration von LDAP unter Samba (S)

- Werden die Benutzer unter Samba mit LDAP verwaltet, SOLLTE die Konfiguration sorgfältig vom IT-Betrieb geplant und dokumentiert werden.
- Die Zugriffsberechtigungen auf das LDAP SOLLTEN mittels ACLs geregelt werden.

## APP.3.4.A9 Sichere Konfiguration von Kerberos unter Samba (S)

- Zur Authentisierung SOLLTE das von Samba implementierte Heimdal Kerberos Key Distribution Center (KDC) verwendet werden.
- Es SOLLTE darauf geachtet werden, dass die von Samba vorgegebene Kerberos-Konfigurationsdatei verwendet wird.
- Es SOLLTEN nur sichere Verschlüsselungsverfahren für Kerberos-Tickets benutzt werden.
- Wird mit Kerberos authentisiert, SOLLTE der zentrale Zeitserver lokal auf dem Samba-Server installiert werden.
- Der NTP-Dienst SOLLTE so konfiguriert werden, dass nur autorisierte Clients die Zeit abfragen können.

## APP.3.4.A10 Sicherer Einsatz externer Programme auf einem Samba-Server (S)

- Vom IT-Betrieb SOLLTE sichergestellt werden, dass Samba nur auf schadhafte Funktionen überprüfte und vertrauenswürdige externe Programme aufruft.

## APP.3.4.A11 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.3.4.A12 Schulung der Administratoren eines Samba-Servers (S)

- Administratoren SOLLTEN zu den genutzten spezifischen Bereichen von Samba wie z. B. Benutzerauthentisierung, Windows- und Unix-Rechtemodelle, aber auch zu NTFS ACLs und NTFS ADS geschult werden.

## APP.3.4.A13 Regelmäßige Sicherung wichtiger Systemkomponenten eines Samba-Servers (S)

- Es SOLLTEN alle Systemkomponenten in das institutionsweite Datensicherungskonzept eingebunden werden, die erforderlich sind, um einen Samba-Server wiederherzustellen.
- Auch die Kontoinformationen aus allen eingesetzten Backends SOLLTEN berücksichtigt werden.
- Ebenso SOLLTEN alle TDB-Dateien gesichert werden.
- Des Weiteren SOLLTE die Samba-Registry mit gesichert werden, falls sie für Freigaben eingesetzt wurde.

## APP.3.4.A14 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.3.4.A15 Verschlüsselung der Datenpakete unter Samba (H)

- Um die Sicherheit der Datenpakete auf dem Transportweg zu gewährleisten, SOLLTEN die Datenpakete mit den ab SMB Version 3 integrierten Verschlüsselungsverfahren verschlüsselt werden.


