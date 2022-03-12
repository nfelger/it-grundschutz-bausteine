# SYS.2.2.3: Clients unter Windows 10

## SYS.2.2.3.A1 Planung des Einsatzes von Cloud-Diensten unter Windows 10 (B)

- Da Windows 10-basierte Geräte eng mit den Cloud-Diensten des Herstellers Microsoft verzahnt sind, MUSS vor ihrer Verwendung strategisch festgelegt werden, welche enthaltenen Cloud-Dienste in welchem Umfang genutzt werden sollen bzw. dürfen.

## SYS.2.2.3.A2 Auswahl und Beschaffung einer geeigneten Windows 10-Version (B)

- Der Funktionsumfang und die Versorgung mit funktionalen Änderungen einer Windows 10-Version MÜSSEN unter Berücksichtigung des ermittelten Schutzbedarfs und des Einsatzzwecks ausgewählt werden.
- Die Umsetzbarkeit der erforderlichen Absicherungsmaßnahmen MUSS bei der Auswahl berücksichtigt werden.
- Basierend auf dem Ergebnis der Überprüfung MUSS der etablierte Beschaffungsprozess um die Auswahl des entsprechenden Lizenzmodells und „Service Branches“ (CB, CBB oder LTSC) erweitert werden.

## SYS.2.2.3.A3 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## SYS.2.2.3.A4 Telemetrie und Datenschutzeinstellungen unter Windows 10 (B)

- Die Telemetriedienste übertragen Diagnose- und Nutzungsdaten, die der Hersteller zur Erkennung und Lösung von Problemen, zur Verbesserung der Dienste und Produkte und zur Identifizierung mit eindeutigen Merkmalen verknüpft.
- Diese können nur unter Windows 10 Enterprise mit der Einstellung des Telemetrielevels 0 (Security) stark reduziert werden.
- Wenn diese Einstellung nicht wirksam umgesetzt werden kann, dann MUSS durch geeignete Maßnahmen, etwa auf Netzebene, sichergestellt werden, dass diese Daten nicht an den Hersteller übertragen werden.

## SYS.2.2.3.A5 Schutz vor Schadsoftware unter Windows 10 (B)

- Sofern nicht gleich- oder höherwertige Maßnahmen, wie z. B. Ausführungskontrolle, zum Schutz des IT-Systems vor einer Infektion mit Schadsoftware getroffen wurden, MUSS eine spezialisierte Komponente zum Schutz vor Schadsoftware auf Windows 10-Clients eingesetzt werden.

## SYS.2.2.3.A6 Integration von Online-Konten in das Betriebssystem [Benutzer] (B)

- Die Anmeldung am System sowie an der Domäne DARF NUR mit dem Konto eines selbst betriebenen Verzeichnisdienstes möglich sein.
- Anmeldungen mit lokalen Konten SOLLTEN Administratoren vorbehalten sein.
- Online-Konten zur Anmeldung, etwa ein Microsoft-Konto oder Konten anderer Anbieter von Identitätsmanagementsystemen, DÜRFEN NICHT verwendet werden, da hier personenbezogene Daten an die Systeme des Herstellers übertragen werden.

## SYS.2.2.3.A7 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.2.2.3.A8 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.2.2.3.A9 Sichere zentrale Authentisierung in Windows-Netzen (S)

- Für die zentrale Authentisierung SOLLTE ausschließlich Kerberos eingesetzt werden.
- Eine Gruppenrichtlinie SOLLTE die Verwendung älterer Protokolle verhindern.
- Ist dies nicht möglich, MUSS alternativ NTLMv2 eingesetzt werden.
- Die Authentisierung mittels LAN-Manager und NTLMv1 DARF NICHT innerhalb der Institution und in einer produktiven Betriebsumgebung erlaubt werden.
- Die eingesetzten kryptografischen Mechanismen SOLLTEN entsprechend dem ermittelten Schutzbedarf und basierend auf den internen Richtlinien konfiguriert und dokumentiert werden.
- Abweichende Einstellungen SOLLTEN begründet und mit dem Sicherheitsmanagement abgestimmt sein.

## SYS.2.2.3.A10 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.2.2.3.A11 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.2.2.3.A12 Datei- und Freigabeberechtigungen unter Windows 10 (S)

- Der Zugriff auf Dateien und Ordner auf dem lokalen System sowie auf Netzfreigaben SOLLTE gemäß einem Berechtigungs- und Zugriffskonzept konfiguriert werden.
- Auch die standardmäßig vorhandenen administrativen Freigaben auf dem System SOLLTEN hierbei berücksichtigt werden.
- Die Schreibrechte für Benutzer SOLLTEN auf einen definierten Bereich im Dateisystem beschränkt werden.
- Insbesondere SOLLTEN Benutzer keine Schreibrechte für Ordner des Betriebssystems oder installierte Anwendungen erhalten.

## SYS.2.2.3.A13 Einsatz der SmartScreen-Funktion (S)

- Die SmartScreen-Funktion, die aus dem Internet heruntergeladene Dateien und Webinhalte auf mögliche Schadsoftware untersucht und dazu unter Umständen personenbezogene Daten an Microsoft überträgt, SOLLTE deaktiviert werden.

## SYS.2.2.3.A14 Einsatz des Sprachassistenten Cortana [Benutzer] (S)

- Cortana SOLLTE deaktiviert werden.

## SYS.2.2.3.A15 Einsatz der Synchronisationsmechanismen unter Windows 10 (S)

- Die Synchronisierung von Nutzerdaten mit Microsoft Cloud-Diensten und das Sharing von WLAN-Passwörtern SOLLTEN vollständig deaktiviert werden.

## SYS.2.2.3.A16 Anbindung von Windows 10 an den Microsoft-Store (S)

- Die Verwendung des Microsoft-Stores SOLLTE auf die Verträglichkeit mit den Datenschutz- und Sicherheitsvorgaben der Institution überprüft und bewertet werden.
- Die generelle Installation von Apps auf Windows 10 ist nicht von der Anbindung an den Microsoft-Store abhängig, daher SOLLTE sie, sofern sie nicht benötigt wird, deaktiviert werden.

## SYS.2.2.3.A17 Keine Speicherung von Daten zur automatischen Anmeldung (S)

- Die Speicherung von Kennwörtern, Zertifikaten und anderen Informationen zur automatischen Anmeldung an Webseiten und IT-Systemen SOLLTE NICHT erlaubt werden.

## SYS.2.2.3.A18 Einsatz der Windows-Remoteunterstützung (S)

- Die Auswirkungen auf die Konfiguration der lokalen Firewall SOLLTEN bei der Planung der Windows-Remoteunterstützung (hiermit ist nicht RDP gemeint) berücksichtigt werden.
- Eine Remoteunterstützung SOLLTE nur nach einer expliziten Einladung erfolgen.
- Bei der Speicherung einer Einladung in einer Datei SOLLTE diese ein Kennwort besitzen.
- Der aktuell angemeldete Benutzer SOLLTE dem Aufbau einer Sitzung immer explizit zustimmen.
- Die maximale Gültigkeit der Einladung für eine Unterstützung aus der Ferne SOLLTE in der Dauer angemessen sein.
- Sofern dieser Service nicht verwendet wird, SOLLTE er vollständig deaktiviert werden.

## SYS.2.2.3.A19 Sicherheit beim Fernzugriff über RDP [Benutzer] (S)

- Die Auswirkungen auf die Konfiguration der lokalen Firewall SOLLTEN bei der Planung des Fernzugriffs berücksichtigt werden.
- Die Gruppe der berechtigten Benutzer für den Remote-Desktopzugriff (RDP) SOLLTE durch die Zuweisung entsprechender Benutzerrechte festgelegt werden.
- In komplexen Infrastrukturen SOLLTE das RDP-Zielsystem nur durch ein dazwischengeschaltetes RDP-Gateway erreicht werden können.
- Für die Verwendung von RDP SOLLTE eine Prüfung und deren Umsetzung sicherstellen, dass die nachfolgend aufgeführten Komfortfunktionen im Einklang mit dem Schutzbedarf des Zielsystems stehen:
    - die Verwendung der Zwischenablage,
    - die Einbindung von Druckern,
    - die Einbindung von Wechselmedien und Netzlaufwerken sowie
    - die Nutzung der Dateiablagen und von Smartcard-Anschlüssen.
- Sofern der Einsatz von Remote-Desktopzugriffen nicht vorgesehen ist, SOLLTEN diese vollständig deaktiviert werden.
- Die eingesetzten kryptografischen Protokolle und Algorithmen SOLLTEN den internen Vorgaben der Institution entsprechen.

## SYS.2.2.3.A20 Einsatz der Benutzerkontensteuerung UAC für privilegierte Konten (S)

- Die Konfigurationsparameter der Benutzerkontensteuerung (User Account Control, UAC) SOLLTEN für die privilegierten Konten zwischen Bedienbarkeit und Sicherheitsniveau abgewogen eingesetzt werden.
- Die Entscheidungen für die zu verwendenden Konfigurationsparameter SOLLTEN dokumentiert werden.
- Darüber hinaus SOLLTE die Dokumentation alle Konten mit Administratorrechten enthalten sowie regelmäßig geprüft werden, ob es notwendig ist, die Rechte erweitern zu können.

## SYS.2.2.3.A21 Einsatz des Encrypting File Systems (H)

- Da das Encrypting File System (EFS) die verwendeten Schlüssel mit dem Passwort des Benutzerkontos schützt, SOLLTE ein sicheres Passwort verwendet werden.
- Zusätzlich SOLLTEN restriktive Zugriffsrechte die mit EFS verschlüsselten Dateien schützen.
- Der Wiederherstellungsagent SOLLTE ein dediziertes Konto und nicht der Administrator sein.
- In diesem Zusammenhang SOLLTE der private Schlüssel des Agenten gesichert und aus dem System entfernt werden.
- Es SOLLTEN von allen privaten Schlüsseln Datensicherungen erstellt werden.
- Beim Einsatz von EFS mit lokalen Benutzerkonten SOLLTEN die lokalen Passwortspeicher mittels Syskey verschlüsselt werden.
- Alternativ kann der Windows Defender Credential Guard genutzt werden.
- Die Benutzer SOLLTEN im korrekten Umgang mit EFS geschult werden.

## SYS.2.2.3.A22 Verwendung der Windows PowerShell (H)

- Die PowerShell und die WPS-Dateien SOLLTEN NUR von Administratoren ausgeführt werden können.
- Die PowerShell-Ausführung selbst SOLLTE zentral protokolliert und die Protokolle überwacht werden.
- Die Ausführung von PowerShell-Skripten SOLLTE mit dem Befehl Set-ExecutionPolicy AllSigned eingeschränkt werden, um zu verhindern, dass unsignierte Skripte versehentlich ausgeführt werden.

## SYS.2.2.3.A23 Erweiterter Schutz der Anmeldeinformationen unter Windows 10 (H)

- Auf UEFI-basierten Systemen SOLLTE SecureBoot verwendet und der Status des geschützten Modus für den Local Credential Store LSA beim Systemstart überwacht werden (vgl. hierzu SYS.2.2.3.A11 Schutz der Anmeldeinformationen unter Windows 10).
- Ist eine Fernwartung der Clients mittels RDP vorgesehen, SOLLTE beim Einsatz von Windows 10 in einer Domäne ab dem Funktionslevel 2012 R2 von der Option „restrictedAdmin“ für RDP Gebrauch gemacht werden.

## SYS.2.2.3.A24 Aktivierung des Last-Access-Zeitstempels (H)

- Wird ein Sicherheitskonzept für ein IT-System mit Windows 10 erstellt, SOLLTE dabei geprüft werden, ob der LastAccess-Zeitstempel im Dateisystem aktiviert werden kann, um die Analyse eines Systemmissbrauchs zu erleichtern.
- Bei der Prüfung SOLLTEN mögliche Auswirkungen dieser Einstellung, wie Performance-Aspekte oder resultierende Einschränkungen bei inkrementellen Backups, berücksichtigt werden.

## SYS.2.2.3.A25 Umgang mit Fernzugriffsfunktionen der „Connected User Experience and Telemetry“ (H)

- Es SOLLTE berücksichtigt werden, dass die Komponente „Connected User Experience and Telemetry“ (CUET) bei Windows 10 fester Bestandteil des Betriebssystems ist und neben der Telemetriefunktion auch eine Fernzugriffsmöglichkeit für den Betriebssystemhersteller auf das lokale System erlaubt.
- Ein solcher Fernzugriff auf den Windows 10-Client SOLLTE netzseitig geloggt und falls erforderlich geblockt werden.


