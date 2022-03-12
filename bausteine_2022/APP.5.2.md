# APP.5.2: Microsoft Exchange und Outlook

## APP.5.2.A1 Planung des Einsatzes von Exchange und Outlook (B)

- Bevor Exchange und Outlook eingesetzt werden, MUSS die Institution deren Einsatz sorgfältig planen.
- Dabei MUSS sie mindestens folgende Punkte beachten:
    - Aufbau der E-Mail-Infrastruktur,
    - einzubindende Clients beziehungsweise Server,
    - Nutzung von funktionalen Erweiterungen sowie
    - die zu verwendenden Protokolle.

## APP.5.2.A2 Auswahl einer geeigneten Exchange-Infrastruktur (B)

- Der IT-Betrieb MUSS auf Basis der Planung des Einsatzes von Exchange entscheiden, mit welchen Systemen und Anwendungskomponenten sowie in welcher hierarchischen Abstufung die Exchange-Infrastruktur realisiert wird.
- Im Rahmen der Auswahl MUSS auch entschieden werden, ob die Systeme als Cloud- oder lokaler Dienst betrieben werden sollen.

## APP.5.2.A3 Berechtigungsmanagement und Zugriffsrechte (B)

- Zusätzlich zum allgemeinen Berechtigungskonzept MUSS die Institution ein Berichtigungskonzept für die Systeme der Exchange-Infrastruktur erstellen, geeignet dokumentieren und anwenden.
- Der IT-Betrieb MUSS serverseitige Benutzerprofile für einen rechnerunabhängigen Zugriff der Benutzer auf Exchange-Daten verwenden.
- Er MUSS die Standard-NTFS-Berechtigungen für das Exchange-Verzeichnis so anpassen, dass nur autorisierte Administratoren und Systemkonten auf die Daten in diesem Verzeichnis zugreifen können.

## APP.5.2.A4 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.5.2.A5 Datensicherung von Exchange (B)

- Exchange-Server MÜSSEN vor Installationen und Konfigurationsänderungen sowie in zyklischen Abständen gesichert werden.
- Dabei MÜSSEN insbesondere die Exchange-Server-Datenbanken gesichert werden.
- Gelöschte Exchange-Objekte SOLLTEN erst nach einiger Zeit aus der Datenbank entfernt werden.

## APP.5.2.A6 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.5.2.A7 Migration von Exchange-Systemen (S)

- Der IT-Betrieb SOLLTE alle Migrationsschritte gründlich planen und dokumentieren.
- Der IT-Betrieb SOLLTE dabei Postfächer, Objekte, Sicherheitsrichtlinien, Active-Directory-Konzepte sowie die Anbindung an andere E-MailSysteme berücksichtigen.
- Außerdem SOLLTE er Funktionsunterschiede zwischen verschiedenen Versionen von Exchange beachten.
- Das neue System SOLLTE, bevor es installiert wird, in einem separaten Testnetz geprüft werden.

## APP.5.2.A8 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.5.2.A9 Sichere Konfiguration von Exchange-Servern (S)

- Der IT-Betrieb SOLLTE Exchange-Server entsprechend der Vorgaben aus der Sicherheitsrichtlinie installieren und konfigurieren.
- Konnektoren SOLLTEN sicher konfiguriert werden.
- Der IT-Betrieb SOLLTE die Protokollierung des Exchange-Systems aktivieren.
- Für vorhandene benutzerspezifische Anpassungen SOLLTE ein entsprechendes Konzept erstellt werden.
- Bei der Verwendung von funktionalen Erweiterungen SOLLTE sichergestellt sein, dass die definierten Anforderungen an die Schutzziele Vertraulichkeit, Integrität und Verfügbarkeit weiterhin erfüllt sind.

## APP.5.2.A10 Sichere Konfiguration von Outlook (S)

- Der IT-Betrieb SOLLTE für jeden Benutzer ein eigenes Outlook-Profil mit benutzerspezifischen Einstellungen anlegen.
- Der IT-Betrieb SOLLTE Outlook so konfigurieren, dass nur notwendige Informationen an andere Benutzer übermittelt werden.
- Der IT-Betrieb SOLLTE die Benutzer darüber informieren, welche Informationen automatisiert an andere Benutzer übermittelt werden.
- Lesebestätigungen und Informationen, die auf die interne Struktur der Institution schließen lassen, SOLLTEN NICHT an externe Anwender übermittelt werden.

## APP.5.2.A11 Absicherung der Kommunikation zwischen Exchange-Systemen (S)

- Der IT-Betrieb SOLLTE nachvollziehbar entscheiden, mit welchen Schutzmechanismen die Kommunikation zwischen Exchange-Systemen abgesichert wird.
- Insbesondere SOLLTE der IT-Betrieb festlegen, wie die Kommunikation zu folgenden Schnittstellen abgesichert wird:
    - Administrationsschnittstellen,
    - Client-Server-Kommunikation,
    - vorhandene Web-based-Distributed-Authoring-and-Versioning-(WebDAV)-Schnittstellen,
    - Server-Server-Kommunikation und
    - Public-Key-Infrastruktur, auf der die E-Mail-Verschlüsselung von Outlook basiert.

## APP.5.2.A12 Einsatz von Outlook Anywhere, MAPI over HTTP und Outlook im Web (S)

- Der IT-Betrieb SOLLTE Outlook Anywhere, MAPI over HTTP und Outlook im Web entsprechend den Sicherheitsanforderungen der Institution konfigurieren.
- Der Zugriff auf Exchange über das Internet SOLLTE auf die notwendigen Benutzer beschränkt werden.

## APP.5.2.A13 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.5.2.A14 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.5.2.A15 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.5.2.A16 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.5.2.A19 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.5.2.A17 Verschlüsselung von Exchange-Datenbankdateien (H)

- Der IT-Betrieb SOLLTE ein Konzept für die Verschlüsselung von PST-Dateien und Informationsspeicher-Dateien erstellen.
- Die Institution SOLLTE die Benutzer über die Funktionsweise und die Schutzmechanismen bei der Verschlüsselung von PST-Dateien informieren.
- Weitere Aspekte für lokale PST-Dateien, die berücksichtigt werden SOLLTEN, wenn Exchange-Systemdatenbanken verschlüsselt werden, sind:
    - eigene Verschlüsselungsfunktionen,
    - Verschlüsselungsgrade sowie
    - Mechanismen zur Absicherung der Daten in einer PST-Datei.
- Mechanismen wie z. B. Encrypting File System oder Windows BitLocker Laufwerkverschlüsselung SOLLTEN zur Absicherung der PST-Dateien genutzt werden.

## APP.5.2.A18 ENTFALLEN (H)

- Diese Anforderung ist entfallen.


