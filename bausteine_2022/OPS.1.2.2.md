# OPS.1.2.2: Archivierung

## OPS.1.2.2.A1 Ermittlung von Einflussfaktoren für die elektronische Archivierung (B)

- Bevor entschieden wird, welche Verfahren und Produkte für die elektronische Archivierung eingesetzt werden, MÜSSEN die technischen, rechtlichen und organisatorischen Einflussfaktoren ermittelt und dokumentiert werden.
- Die Ergebnisse MÜSSEN in das Archivierungskonzept einfließen.

## OPS.1.2.2.A2 Entwicklung eines Archivierungskonzepts (B)

- Es MUSS definiert werden, welche Ziele mit der Archivierung erreicht werden sollen.
- Hierbei MUSS insbesondere berücksichtigt werden, welche Regularien einzuhalten sind, welche Mitarbeiter verantwortlich sind und welcher Funktions- und Leistungsumfang angestrebt wird.
- Die Ergebnisse MÜSSEN in einem Archivierungskonzept erfasst werden.
- Die Institutionsleitung MUSS in diesen Prozess einbezogen werden.
- Das Archivierungskonzept MUSS regelmäßig an die aktuellen Gegebenheiten der Institution angepasst werden.

## OPS.1.2.2.A3 Geeignete Aufstellung von Archivsystemen und Lagerung von Archivmedien [IT-Betrieb] (B)

- Die IT-Komponenten eines Archivsystems MÜSSEN in gesicherten Räumen aufgestellt werden.
- Es MUSS sichergestellt sein, dass nur berechtigte Personen die Räume betreten dürfen.
- Archivspeichermedien MÜSSEN geeignet gelagert werden.

## OPS.1.2.2.A4 Konsistente Indizierung von Daten bei der Archivierung [IT-Betrieb, Benutzer] (B)

- Alle in einem Archiv abgelegten Daten, Dokumente und Datensätze MÜSSEN eindeutig indiziert werden.
- Dazu MUSS bereits während der Konzeption festgelegt werden, welche Struktur und welchen Umfang die Indexangaben für ein Archiv haben sollen.

## OPS.1.2.2.A5 Regelmäßige Aufbereitung von archivierten Datenbeständen [IT-Betrieb] (B)

- Über den gesamten Archivierungszeitraum hinweg MUSS sichergestellt werden, dass
    - das verwendete Datenformat von den benutzten Anwendungen verarbeitet werden kann,
    - die gespeicherten Daten auch zukünftig lesbar und so reproduzierbar sind, dass Semantik und Beweiskraft beibehalten werden,
    - das benutzte Dateisystem auf dem Speichermedium von allen beteiligten Komponenten verarbeitet werden kann,
    - die Speichermedien jederzeit technisch einwandfrei gelesen werden können sowie
    - die verwendeten kryptografischen Verfahren zur Verschlüsselung und zum Beweiswerterhalt mittels digitaler Signatur, Siegel, Zeitstempel oder technischen Beweisdaten (Evidence Records) dem Stand der Technik entsprechen.

## OPS.1.2.2.A6 Schutz der Integrität der Indexdatenbank von Archivsystemen [IT-Betrieb] (B)

- Die Integrität der Indexdatenbank MUSS sichergestellt und überprüfbar sein.
- Außerdem MUSS die Indexdatenbank regelmäßig gesichert werden.
- Die Datensicherungen MÜSSEN wiederherstellbar sein.
- Mittlere und große Archive SOLLTEN über redundante Indexdatenbanken verfügen.

## OPS.1.2.2.A7 Regelmäßige Datensicherung der System- und Archivdaten [IT-Betrieb] (B)

- Alle Archivdaten, die zugehörigen Indexdatenbanken sowie die Systemdaten MÜSSEN regelmäßig gesichert werden (siehe CON.3 Datensicherungskonzept).

## OPS.1.2.2.A8 Protokollierung der Archivzugriffe [IT-Betrieb] (B)

- Alle Zugriffe auf elektronische Archive MÜSSEN protokolliert werden.
- Dafür SOLLTEN Datum, Uhrzeit, Benutzer, Client und die ausgeführten Aktionen sowie Fehlermeldungen aufgezeichnet werden.
- Im Archivierungskonzept SOLLTE festgelegt werden, wie lange die Protokolldaten aufbewahrt werden.
- Die Protokolldaten der Archivzugriffe SOLLTEN regelmäßig ausgewertet werden.
- Dabei SOLLTEN die institutionsinternen Vorgaben beachtet werden.
- Auch SOLLTE definiert sein, welche Ereignisse welchen Mitarbeitern angezeigt werden, wie z. B. Systemfehler, Timeouts oder wenn Datensätze kopiert werden.
- Kritische Ereignisse SOLLTEN sofort nach der Erkennung geprüft und, falls nötig, weiter eskaliert werden.

## OPS.1.2.2.A9 Auswahl geeigneter Datenformate für die Archivierung von Dokumenten [IT-Betrieb] (B)

- Für die Archivierung MUSS ein geeignetes Datenformat ausgewählt werden.
- Es MUSS gewährleisten, dass sich Archivdaten sowie ausgewählte Merkmale des ursprünglichen Dokumentmediums langfristig und originalgetreu reproduzieren lassen.
- Die Dokumentstruktur des ausgewählten Datenformats MUSS eindeutig interpretierbar und elektronisch verarbeitbar sein.
- Die Syntax und Semantik der verwendeten Datenformate SOLLTE dokumentiert und von einer Standardisierungsorganisation veröffentlicht sein.
- Es SOLLTE für eine beweis- und revisionssichere Archivierung ein verlustfreies Bildkompressionsverfahren benutzt werden.

## OPS.1.2.2.A10 Erstellung einer Richtlinie für die Nutzung von Archivsystemen [IT-Betrieb] (S)

- Es SOLLTE sichergestellt werden, dass Mitarbeiter das Archivsystem so benutzen, wie es im Archivierungskonzept vorgesehen ist.
- Dazu SOLLTE eine Administrations- und eine Benutzerrichtlinie erstellt werden.
- Die Administrationsrichtlinie SOLLTE folgende Punkte enthalten:
    - Festlegung der Verantwortung für Betrieb und Administration,
    - Vereinbarungen über Leistungsparameter beim Betrieb (u. a. Service Level Agreements),
    - Modalitäten der Vergabe von Zutritts- und Zugriffsrechten,
    - Modalitäten der Vergabe von Zugangsrechten zu den vom Archiv bereitgestellten Diensten,
    - Regelungen zum Umgang mit archivierten Daten und Archivmedien,
    - Überwachung des Archivsystems und der Umgebungsbedingungen,
    - Regelungen zur Datensicherung,
    - Regelungen zur Protokollierung sowie
    - Trennung von Produzenten und Konsumenten (OAIS-Modell).

## OPS.1.2.2.A11 Einweisung in die Administration und Bedienung des Archivsystems [IT-Betrieb, Benutzer] (S)

- Die verantwortlichen Mitarbeiter des IT-Betriebs und die Benutzer SOLLTEN für ihren Aufgabenbereich geschult werden.
- Die Schulung der Mitarbeiter des IT-Betriebs SOLLTE folgende Themen umfassen:
    - Systemarchitektur und Sicherheitsmechanismen des verwendeten Archivsystems und des darunterliegenden Betriebssystems,
    - Installation und Bedienung des Archivsystems und Umgang mit Archivmedien,
    - Dokumentation der Administrationstätigkeiten sowie
    - Eskalationsprozeduren.
- Die Schulung der Benutzer SOLLTE folgende Themen umfassen:
    - Umgang mit dem Archivsystem,
    - Bedienung des Archivsystems sowie
    - rechtliche Rahmenbedingungen der Archivierung.
- Die Durchführung der Schulungen sowie die Teilnahme SOLLTEN dokumentiert werden.

## OPS.1.2.2.A12 Überwachung der Speicherressourcen von Archivmedien [IT-Betrieb] (S)

- Die auf den Archivmedien vorhandene freie Speicherkapazität SOLLTE kontinuierlich überwacht werden.
- Sobald ein definierter Grenzwert unterschritten wird, MUSS ein zuständiger Mitarbeiter automatisch alarmiert werden.
- Die Alarmierung SOLLTE rollenbezogen erfolgen.
- Es MÜSSEN immer ausreichend leere Archivmedien verfügbar sein, um Speicherengpässen schnell vorbeugen zu können.

## OPS.1.2.2.A13 Regelmäßige Revision der Archivierungsprozesse (S)

- Es SOLLTE regelmäßig überprüft werden, ob die Archivierungsprozesse noch korrekt und ordnungsgemäß funktionieren.
- Dazu SOLLTE eine Checkliste erstellt werden, die Fragen zu Verantwortlichkeiten, Organisationsprozessen, zum Einsatz der Archivierung, zur Redundanz der Archivdaten, zur Administration und zur technischen Beurteilung des Archivsystems enthält.
- Die Auditergebnisse SOLLTEN nachvollziehbar dokumentiert und mit dem Soll-Zustand abgeglichen werden.
- Abweichungen SOLLTE nachgegangen werden.

## OPS.1.2.2.A14 Regelmäßige Beobachtung des Marktes für Archivsysteme [IT-Betrieb] (S)

- Der Markt für Archivsysteme SOLLTE regelmäßig und systematisch beobachtet werden.
- Dabei SOLLTEN unter anderem folgende Kriterien beobachtet werden:
    - Veränderungen bei Standards,
    - Wechsel der Technik bei Herstellern von Hard- und Software,
    - veröffentlichte Sicherheitslücken oder Schwachstellen sowie
    - der Verlust der Sicherheitseignung bei kryptografischen Algorithmen.

## OPS.1.2.2.A15 Regelmäßige Aufbereitung von kryptografisch gesicherten Daten bei der Archivierung [ITBetrieb] (S)

- Es SOLLTE kontinuierlich beobachtet werden, wie sich das Gebiet der Kryptografie entwickelt, um beurteilen zu können, ob ein Algorithmus weiterhin zuverlässig und ausreichend sicher ist (siehe auch OPS.1.2.2.A20 Geeigneter Einsatz kryptografischer Verfahren bei der Archivierung).
- Archivdaten, die mit kryptografischen Verfahren gesichert wurden, die sich in absehbarer Zeit nicht mehr zur Sicherung eignen werden, SOLLTEN rechtzeitig mit geeigneten Verfahren neu gesichert werden.

## OPS.1.2.2.A16 Regelmäßige Erneuerung technischer Archivsystem-Komponenten [IT-Betrieb] (S)

- Archivsysteme SOLLTEN über lange Zeiträume auf dem aktuellen technischen Stand gehalten werden.
- Neue Hardund Software SOLLTE vor der Installation in einem laufenden Archivsystem ausführlich getestet werden.
- Wenn neue Komponenten in Betrieb genommen oder neue Dateiformate eingeführt werden, SOLLTE ein Migrationskon-zept erstellt werden.
- Darin SOLLTEN alle Änderungen, Tests und erwarteten Testergebnisse beschrieben sein.
- Die Konvertierung der einzelnen Daten SOLLTE dokumentiert werden (Transfervermerk).
- Wenn Archivdaten in neue Formate konvertiert werden, SOLLTE geprüft werden, ob die Daten aufgrund rechtlicher Anforderungen zusätzlich in ihren ursprünglichen Formaten zu archivieren sind.

## OPS.1.2.2.A17 Auswahl eines geeigneten Archivsystems [IT-Betrieb] (S)

- Ein neues Archivsystem SOLLTE immer auf Basis der im Archivierungskonzept beschriebenen Vorgaben ausgewählt werden.
- Es SOLLTE die dort formulierten Anforderungen erfüllen.

## OPS.1.2.2.A18 Verwendung geeigneter Archivmedien [IT-Betrieb] (S)

- Für die Archivierung SOLLTEN geeignete Medien ausgewählt und benutzt werden.
- Dabei SOLLTEN folgende Aspekte berücksichtigt werden:
    - das zu archivierende Datenvolumen,
    - die mittleren Zugriffszeiten sowie
    - die mittleren gleichzeitigen Zugriffe auf das Archivsystem.
- Ebenfalls SOLLTEN die Archivmedien die Anforderungen an eine Langzeitarchivierung hinsichtlich Revisionssicherheit und Lebensdauer erfüllen.

## OPS.1.2.2.A19 Regelmäßige Funktions- und Recoverytests bei der Archivierung [IT-Betrieb] (S)

- Für die Archivierung SOLLTEN regelmäßige Funktions- und Recoverytests durchgeführt werden.
- Die Archivierungsdatenträger SOLLTEN mindestens einmal jährlich daraufhin überprüft werden, ob sie noch lesbar und integer sind.
- Für die Fehlerbehebung SOLLTEN geeignete Prozesse definiert werden.
- Weiterhin SOLLTEN die Hardwarekomponenten des Archivsystems regelmäßig auf ihre einwandfreie Funktion hin geprüft werden.
- Es SOLLTE regelmäßig geprüft werden, ob alle Archivierungsprozesse fehlerfrei funktionieren.

## OPS.1.2.2.A20 Geeigneter Einsatz kryptografischer Verfahren bei der Archivierung [IT-Betrieb] (H)

- Um lange Aufbewahrungsfristen abdecken zu können, SOLLTEN Archivdaten nur mit kryptografischen Verfahren auf Basis aktueller Standards und Normen gesichert werden.

## OPS.1.2.2.A21 Übertragung von Papierdaten in elektronische Archive (H)

- Werden z. B. Dokumente auf Papier digitalisiert und in ein elektronisches Archiv überführt, SOLLTE sichergestellt werden, dass die digitale Kopie mit dem Originaldokument bildlich und inhaltlich übereinstimmt.


