# SYS.2.4: Clients unter macOS

## SYS.2.4.A1 Planung des sicheren Einsatzes von macOS (B)

- Die Einführung von macOS MUSS sorgfältig geplant werden.
- Es MUSS entschieden werden, wo und wie Daten abgelegt werden.
- Es MUSS geplant werden, wie die Datensicherung in das institutionsweite Datensicherungskonzept integriert werden kann.
- Es MUSS geplant werden, wie Sicherheits- und sonstige Aktualisierungen für macOS und Anwendungen systematisch installiert werden können.
- Es MUSS ermittelt werden, welche Anwendungen bei einem Plattformwechsel zu macOS benötigt werden.
- Wird der Mac in einem Datennetz betrieben, MUSS zusätzlich berücksichtigt werden, welche Netzprotokolle eingesetzt werden sollen.

## SYS.2.4.A2 Nutzung der integrierten Sicherheitsfunktionen von macOS (B)

- Die in macOS integrierten Schutzmechanismen „System Integrity Protection“ (SIP), „Xprotect“ und „Gatekeeper“ MÜSSEN aktiviert sein.
- Gatekeeper DARF NUR die Ausführung signierter Programme erlauben, sofern unsignierte Programme nicht zwingend notwendig sind.

## SYS.2.4.A3 Verwendung geeigneter Benutzerkonten [Benutzer] (B)

- Das bei der Erstkonfiguration von macOS angelegte Administrator-Konto DARF NUR zu administrativen Zwecken verwendet werden.
- Für die normale Verwendung des Macs MUSS ein Standard-Benutzerkonto angelegt werden.
- Sollte der Mac von mehreren Benutzern verwendet werden, MUSS für jeden Benutzer ein eigenes Konto angelegt werden.
- Das Gast-Benutzerkonto MUSS deaktiviert werden.

## SYS.2.4.A4 Verwendung einer Festplattenverschlüsselung (S)

- Festplatten SOLLTEN, insbesondere bei mobilen Macs (z. B. MacBooks), verschlüsselt werden.
- Wird dazu die in macOS integrierte Funktion FileVault verwendet, DARF das Schlüsselmaterial NICHT online bei Apple gespeichert werden.
- Der von FileVault erzeugte Wiederherstellungsschlüssel MUSS an einem sicheren Ort aufbewahrt werden.
- Es SOLLTE geprüft werden, ob ein institutioneller Wiederherstellungsschlüssel für FileVault verwendet werden soll.

## SYS.2.4.A5 Deaktivierung sicherheitskritischer Funktionen von macOS (S)

- Die in macOS integrierten Ortungsdienste SOLLTEN deaktiviert werden.
- Heruntergeladene Daten SOLLTEN NICHT automatisch geöffnet werden.
- Inhalte von optischen und anderen Medien SOLLTEN NICHT automatisch ausgeführt werden.

## SYS.2.4.A6 Verwendung aktueller Mac-Hardware (S)

- Werden neue Macs beschafft, SOLLTEN aktuelle Modelle ausgewählt werden.
- Werden bereits vorhandene Macs eingesetzt, SOLLTE regelmäßig überprüft werden, ob diese sowie das darauf installierte Betriebssystem weiterhin von Apple mit Sicherheits-Updates versorgt werden.
- Werden die Macs nicht mehr durch Apple unterstützt, SOLLTEN sie nicht mehr verwendet werden.

## SYS.2.4.A7 Zwei-Faktor-Authentisierung für Apple-ID [Benutzer] (S)

- Die Zwei-Faktor-Authentisierung für die Verwendung des Apple-ID-Kontos SOLLTE aktiviert werden.

## SYS.2.4.A8 Keine Nutzung von iCloud für schützenswerte Daten [Benutzer] (S)

- Es SOLLTE verhindert werden, dass schützenswerte Daten zwischen mehreren Geräten über iCloud-Dienste synchronisiert werden.
- Stattdessen SOLLTEN Daten nur über selbst betriebene Dienste synchronisiert werden.
- Schützenswerte Daten SOLLTEN NICHT in iCloud gespeichert werden.
- Entwürfe, beispielsweise von E-Mails oder Dokumenten, SOLLTEN NICHT automatisch in iCloud gespeichert werden.

## SYS.2.4.A9 Verwendung von zusätzlichen Schutzprogrammen unter macOS (S)

- Bei Bedarf, etwa wenn Macs in einem heterogenen Netz betrieben werden, SOLLTEN neben den integrierten Schutzmechanismen von macOS zusätzlich Virenschutz-Lösungen von Drittanbietern eingesetzt werden.

## SYS.2.4.A10 Aktivierung der Personal Firewall unter macOS (S)

- Die in macOS integrierte Personal Firewall SOLLTE aktiviert und geeignet konfiguriert werden.

## SYS.2.4.A11 Geräteaussonderung von Macs (S)

- Bei einer Aussonderung des Macs SOLLTEN der nichtflüchtige Datenspeicher NVRAM (Non Volatile Random Access Memory) sowie der SMC (System Management Controller) zurückgesetzt werden.

## SYS.2.4.A12 Firmware-Kennwort und Boot-Schutz auf Macs [Benutzer] (H)

- Auf älteren Macs SOLLTE die Abfrage eines sicheren Firmware-Kennworts im sogenannten „Command-Modus“ aktiviert werden, um ein unberechtigtes Booten des Macs von einem anderen Startlaufwerk zu verhindern.
- Es SOLLTE geprüft werden, ob über den „Full-Modus“ ein Kennwort bei jedem Startvorgang abgefragt werden sollte.
- Auf Macs mit T2-Sicherheitschip SOLLTE ein Firmware-Passwort über das Startsicherheitsdienstprogramm gesetzt werden.
- Die Option „Sicheres Starten: Volle Sicherheit“ SOLLTE aktiviert werden.
- Die Option „Starten von externen Medien nicht zulassen“ SOLLTE aktiviert werden.


