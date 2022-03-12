# APP.3.3: Fileserver

## APP.3.3.A1 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.3.3.A2 Einsatz von RAID-Systemen (B)

- Der IT-Betrieb MUSS festlegen, ob im Fileserver ein RAID-System eingesetzt werden soll.
- Eine Entscheidung gegen ein solches System MUSS nachvollziehbar dokumentiert werden.
- Falls ein RAID-System eingesetzt werden soll, MUSS der IT-Betrieb entscheiden:
    - welches RAID-Level benutzt werden soll,
    - wie lang die Zeitspanne für einen RAID-Rebuild-Prozess sein darf und
    - ob ein Software- oder ein Hardware-RAID eingesetzt werden soll.
- In einem RAID SOLLTEN Hotspare-Festplatten vorgehalten werden.

## APP.3.3.A3 Einsatz von Viren-Schutzprogrammen (B)

- Alle Daten MÜSSEN durch ein Viren-Schutzprogramm auf Schadsoftware untersucht werden, bevor sie auf dem Fileserver abgelegt werden.

## APP.3.3.A4 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.3.3.A5 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.3.3.A15 Planung von Fileservern (B)

- Bevor eine Institution einen oder mehrere Fileserver einführt, SOLLTE sie entscheiden, wofür die Fileserver genutzt und welche Informationen darauf verarbeitet werden.
- Die Institution SOLLTE jede benutzte Funktion eines Fileservers einschließlich deren Sicherheitsaspekte planen.
- Arbeitsplatzrechner DÜRFEN NICHT als Fileserver eingesetzt werden.
- Der Speicherplatz des Fileservers MUSS ausreichend dimensioniert sein.
- Auch ausreichende Speicherreserven SOLLTEN vorgehalten werden.
- Es SOLLTE ausschließlich Massenspeicher verwendet werden, der für einen Dauerbetriebausgelegt ist.
- Die Geschwindigkeit und die Anbindung der Massenspeicher MUSS für den Einsatzzweck angemessen sein.

## APP.3.3.A6 Beschaffung eines Fileservers und Auswahl eines Dienstes (S)

- Die Fileserver-Software SOLLTE geeignet ausgewählt werden.
- Der Fileserver-Dienst SOLLTE den Einsatzzweck des Fileservers unterstützen, z. B. Einbindung von Netzlaufwerken in den Clients, Streaming von Multimedia-Inhalten, Übertragung von Boot-Images von festplattenlosen IT-Systemen oder ausschließliche Dateiübertragung über FTP.
- Die Leistung, die Speicherkapazität, die Bandbreite sowie die Anzahl der Benutzer, die den Fileserver nutzen, SOLLTEN bei der Beschaffung des Fileservers berücksichtigt werden.

## APP.3.3.A7 Auswahl eines Dateisystems (S)

- Der IT-Betrieb SOLLTE eine Anforderungsliste erstellen, nach der die Dateisysteme des Fileservers bewertet werden.
- Das Dateisystem SOLLTE den Anforderungen der Institution entsprechen.
- Das Dateisystem SOLLTE eine JournalingFunktion bieten.
- Auch SOLLTE es über einen Schutzmechanismus verfügen, der verhindert, dass mehrere Benutzer oder Anwendungen gleichzeitig schreibend auf eine Datei zugreifen.

## APP.3.3.A8 Strukturierte Datenhaltung [Benutzer] (S)

- Es SOLLTE eine Struktur festgelegt werden, nach der Daten abzulegen sind.
- Die Benutzer SOLLTEN regelmäßig über die geforderte strukturierte Datenhaltung informiert werden.
- Die Dateien SOLLTEN ausschließlich strukturiert auf den Fileserver abgelegt werden.
- Es SOLLTE schriftlich festgelegt werden, welche Daten lokal und welche auf dem Fileserver gespeichert werden dürfen.
- Programm- und Arbeitsdaten SOLLTEN in getrennten Verzeichnissen gespeichert werden.
- Die Institution SOLLTE regelmäßig überprüfen, ob die Vorgaben zur strukturierten Datenhaltung eingehalten werden.

## APP.3.3.A9 Sicheres Speichermanagement (S)

- Der IT-Betrieb SOLLTE regelmäßig überprüfen, ob die Massenspeicher des Fileservers noch wie vorgesehen funktionieren.
- Es SOLLTEN geeignete Ersatzspeicher vorgehalten werden.
- Wurde eine Speicherhierarchie (Primär-, Sekundär- bzw. Tertiärspeicher) aufgebaut, SOLLTE ein (teil-)automatisiertes Speichermanagement verwendet werden.
- Werden Daten automatisiert verteilt, SOLLTE regelmäßig manuell überprüft werden, ob dies korrekt funktioniert.
- Es SOLLTEN mindestens nicht-autorisierte Zugriffsversuche auf Dateien und Änderungen von Zugriffsrechten protokolliert werden.

## APP.3.3.A10 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.3.3.A11 Einsatz von Speicherbeschränkungen (S)

- Der IT-Betrieb SOLLTE bei mehreren Benutzern auf dem Fileserver prüfen, Beschränkungen des Speicherplatzes für einzelne Benutzer (Quotas) einzurichten.
- Alternativ SOLLTEN Mechanismen des verwendeten Datei- oder Betriebssystems genutzt werden, um die Benutzer bei einem bestimmten Füllstand der Festplatte zu warnen oder in diesem Fall nur noch dem Systemadministrator Schreibrechte einzuräumen.

## APP.3.3.A14 Einsatz von Error-Correction-Codes (S)

- Der IT-Betrieb SOLLTE ein fehlererkennendes bzw. fehlerkorrigierendes Dateisystem einsetzen.
- Hierfür SOLLTE genügend Speicherplatz vorgehalten werden.
- Der IT-Betrieb SOLLTE beachten, dass, je nach eingesetztem Verfahren, Fehler nur mit einer gewissen Wahrscheinlichkeit erkannt und auch nur in begrenzter Größenordnung behoben werden können.

## APP.3.3.A12 Verschlüsselung des Datenbestandes (H)

- Die Massenspeicher des Fileservers SOLLTEN auf Dateisystem- oder Hardwareebene verschlüsselt werden.
- Falls Hardwareverschlüsselung eingesetzt wird, SOLLTEN Produkte verwendet werden, deren Verschlüsselungsfunktion zertifiziert wurde.
- Es SOLLTE sichergestellt werden, dass der Virenschutz die verschlüsselten Daten auf Schadsoftware prüfen kann.

## APP.3.3.A13 Replikation zwischen Standorten (H)

- Für hochverfügbare Fileserver SOLLTE eine angemessene Replikation der Daten auf mehreren Massenspeichern stattfinden.
- Daten SOLLTEN zudem zwischen unabhängigen Fileservern repliziert werden, die sich an unabhängigen Standorten befinden.
- Dafür SOLLTE vom IT-Betrieb ein geeigneter Replikationsmechanismus ausgewählt werden.
- Damit die Replikation wie vorgesehen funktionieren kann, SOLLTEN hinreichend genaue Zeitdienste genutzt und betrieben werden.


