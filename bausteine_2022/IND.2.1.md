# IND.2.1: Allgemeine ICS-Komponente

## IND.2.1.A1 Einschränkung des Zugriffs auf Konfigurations- und Wartungsschnittstellen [OT-Betrieb (Operational Technology, OT)] (B)

- Standardmäßig eingerichtete bzw. vom Hersteller gesetzte Passwörter MÜSSEN gewechselt werden (siehe ORP.4 Identitäts- und Berechtigungsmanagement).
- Der Wechsel MUSS dokumentiert werden.
- Die Passwörter MÜSSEN sicher hinterlegt werden.
- Es MUSS sichergestellt werden, dass nur berechtigte Mitarbeiter auf Konfigurations- und Wartungsschnittstellen von ICS-Komponenten zugreifen können.
- Die Konfiguration von ICS-Komponenten DARF NUR nach einer Freigabe durch den Verantwortlichen oder nach einer Authentisierung geändert werden.

## IND.2.1.A2 Nutzung sicherer Übertragungs-Protokolle für die Konfiguration und Wartung [Wartungspersonal, OT-Betrieb (Operational Technology, OT)] (B)

- Für die Konfiguration und Wartung von ICS-Komponenten MÜSSEN sichere Protokolle eingesetzt werden.
- Die Informationen MÜSSEN geschützt übertragen werden.

## IND.2.1.A3 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## IND.2.1.A4 Deaktivierung oder Deinstallation nicht genutzter Dienste, Funktionen und Schnittstellen [Wartungspersonal, OT-Betrieb (Operational Technology, OT)] (B)

- Alle nicht genutzten Dienste, Funktionen und Schnittstellen der ICS-Komponenten MÜSSEN deaktiviert oder deinstalliert werden.

## IND.2.1.A5 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## IND.2.1.A6 Netzsegmentierung [OT-Betrieb (Operational Technology, OT), Planer] (B)

- ICS-Komponenten MÜSSEN von der Office-IT getrennt werden.
- Hängen ICS-Komponenten von anderen Diensten im Netz ab, SOLLTE das ausreichend dokumentiert werden.
- ICS-Komponenten SOLLTEN so wenig wie möglich mit anderen ICS-Komponenten kommunizieren.

## IND.2.1.A7 Erstellung von Datensicherungen [OT-Betrieb (Operational Technology, OT)] (S)

- Vor jeder Systemänderung an einer ICS-Komponente MÜSSEN Backups erstellt werden.

## IND.2.1.A8 Schutz vor Schadsoftware [OT-Betrieb (Operational Technology, OT)] (S)

- ICS-Komponenten SOLLTEN durch geeignete Mechanismen vor Schadprogrammen geschützt werden (siehe OPS.1.1.4 Schutz vor Schadprogrammen).
- Wird dafür ein Virenschutzprogramm benutzt, SOLLTEN das Programm und die Virensignaturen nach der Freigabe durch den Hersteller immer auf dem aktuellen Stand sein.
- Wenn die Ressourcen auf der ICS-Komponente nicht ausreichend sind oder die Echtzeitanforderung durch den Einsatz von Virenschutzprogrammen gefährdet werden könnte, SOLLTEN alternative Maßnahmen ergriffen werden, etwa die Abschottung der ICS-Komponente oder des Produktionsnetzes.

## IND.2.1.A9 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## IND.2.1.A10 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## IND.2.1.A11 Wartung der ICS-Komponenten [Mitarbeiter, OT-Betrieb (Operational Technology, OT), Wartungspersonal] (S)

- Bei der Wartung einer ICS-Komponente SOLLTEN immer die aktuellen und freigegebenen Sicherheitsupdates eingespielt werden.
- Updates für das Betriebssystem SOLLTEN erst nach Freigabe durch den Hersteller einer ICS-Komponente installiert werden.
- Alternativ SOLLTE die Aktualisierung in einer Testumgebung erprobt werden, bevor diese in einer produktiven ICS-Komponente eingesetzt wird.
- Für kritische Sicherheitsupdates SOLLTE kurzfristig eine Wartung durchgeführt werden.

## IND.2.1.A12 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## IND.2.1.A13 Geeignete Inbetriebnahme von ICS-Komponenten [OT-Betrieb (Operational Technology, OT)] (S)

- Bevor ICS-Komponenten in Betrieb genommen werden, SOLLTEN sie dem aktuellen, intern freigegebenen Firmware-, Software- und Patch-Stand entsprechen.
- Neue ICS-Komponenten SOLLTEN in die bestehenden Betriebs-, Überwachungs- und Informationssicherheitsmanagement-Prozesse eingebunden werden.

## IND.2.1.A14 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## IND.2.1.A15 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## IND.2.1.A16 Schutz externer Schnittstellen [OT-Betrieb (Operational Technology, OT)] (S)

- Von außen erreichbare Schnittstellen SOLLTEN vor Missbrauch geschützt werden.

## IND.2.1.A17 Nutzung sicherer Protokolle für die Übertragung von Mess- und Steuerdaten [OT-Betrieb (Operational Technology, OT)] (S)

- Mess- oder Steuerdaten SOLLTEN bei der Übertragung vor unberechtigten Zugriffen oder Veränderungen geschützt werden.
- Bei Anwendungen mit Echtzeitanforderungen SOLLTE geprüft werden, ob dies umsetzbar ist.
- Werden Mess- oder Steuerdaten über öffentliche Netze übertragen, SOLLTEN sie angemessen geschützt werden.

## IND.2.1.A18 Kommunikation im Störfall [OT-Betrieb (Operational Technology, OT), Mitarbeiter] (H)

- Es SOLLTE alternative und unabhängige Kommunikationsmöglichkeiten geben, die bei einem Störfall benutzt werden können, um handlungsfähig zu bleiben.

## IND.2.1.A19 Security-Tests [OT-Betrieb (Operational Technology, OT)] (H)

- Mithilfe von regelmäßigen Security-Tests SOLLTE geprüft werden, ob die technischen Sicherheitsmaßnahmen noch effektiv umgesetzt sind.
- Die Security-Tests SOLLTEN nicht im laufenden Anlagenbetrieb erfolgen.
- Die Tests SOLLTEN auf die Wartungszeiten geplant werden.
- Die Ergebnisse SOLLTEN dokumentiert werden.
- Erkannte Risiken SOLLTEN bewertet und behandelt werden.

## IND.2.1.A20 Vertrauenswürdiger Code [OT-Betrieb (Operational Technology, OT)] (H)

- Firmware-Updates oder neue Steuerungsprogramme SOLLTEN NUR eingespielt werden, wenn vorher ihre Integrität überprüft wurde.
- Sie SOLLTEN nur aus vertrauenswürdigen Quellen stammen.


