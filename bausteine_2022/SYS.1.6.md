# SYS.1.6: Containerisierung

## SYS.1.6.A1 Planung des Container-Einsatzes (B)

- Bevor Container eingesetzt werden, MUSS zunächst das Ziel des Container-Einsatzes (z. B. Skalierung, Verfügbarkeit, Wegwerf-Container zur Sicherheit oder CI/CD) festgelegt werden, damit alle sicherheitsrelevanten Aspekte der Installation, des Betriebs und der Außerbetriebnahme geplant werden können.
- Bei der Planung SOLLTE auch der Betriebsaufwand berücksichtigt werden, der durch Container-Einsatz oder Mischbetrieb entsteht.
- Die Planung MUSS angemessen dokumentiert werden.

## SYS.1.6.A2 Planung der Verwaltung von Containern (B)

- Die Verwaltung der Container DARF NUR nach einer geeigneten Planung erfolgen.
- Diese Planung MUSS den gesamten Lebenszyklus von Inbetrieb- bis Außerbetriebnahme inklusive Betrieb und Updates umfassen.
- Bei der Planung der Verwaltung MUSS berücksichtigt werden, dass der Ersteller eines Containers aufgrund der Auswirkungen auf den Betrieb in Teilen wie ein Administrator zu betrachten ist.
- Start, Stopp und Überwachung der Container MUSS über die eingesetzte Verwaltungssoftware erfolgen.

## SYS.1.6.A3 Sicherer Einsatz containerisierter IT-Systeme (B)

- Bei containerisierten IT-Systemen MUSS berücksichtigt werden, wie sich eine Containerisierung auf die betriebenen IT-Systeme und Anwendungen auswirkt, dies betrifft insbesondere die Verwaltung und Eignung der Anwendungen.
- Es MUSS anhand des Schutzbedarfs der Anwendungen geprüft werden, ob die Anforderungen an die Isolation und Kapselung der containerisierten IT-Systeme und der virtuellen Netze sowie der betriebenen Anwendungen hinreichend erfüllt sind.
- In diese Prüfung SOLLTEN die Betriebssystem-eigenen Mechanismen mit einbezogen werden.
- Für die virtuellen Netze nimmt der Host die Funktion einer Netzkomponente wahr, die Bausteine der Teilschichten NET.1 Netze und NET.3 Netzkomponenten MÜSSEN entsprechend berücksichtigt werden.
- Logische und OverlayNetze MÜSSEN ebenfalls betrachtet und modelliert werden.
- Weiterhin MÜSSEN die eingesetzten containerisierten IT-Systeme den Anforderungen an die Verfügbarkeit und den Datendurchsatz genügen.
- Im laufenden Betrieb SOLLTEN die Performance und der Zustand der containerisierten IT-Systeme überwacht werden (sogenannte Health Checks).

## SYS.1.6.A4 Planung der Bereitstellung und Verteilung von Images (B)

- Der Prozess zur Bereitstellung und Verteilung von Images MUSS geplant und angemessen dokumentiert werden.

## SYS.1.6.A5 Separierung der Administrations- und Zugangsnetze bei Containern (B)

- Die Netze für die Administration des Hosts, die Administration der Container und deren Zugangsnetze MÜSSEN dem Schutzbedarf angemessen separiert werden.
- Grundsätzlich SOLLTE mindestens die Administration des Hosts nur aus dem Administrationsnetz möglich sein.
- Es SOLLTEN nur die für den Betrieb notwendigen Kommunikationsbeziehungen erlaubt werden.

## SYS.1.6.A6 Verwendung sicherer Images (B)

- Es MUSS sichergestellt sein, dass sämtliche verwendete Images nur aus vertrauenswürdigen Quellen stammen.
- Der Ersteller der Images MUSS eindeutig identifizierbar sein.
- Die Quelle MUSS danach ausgewählt werden, dass der Ersteller des Images die enthaltene Software regelmäßig auf Sicherheitsprobleme prüft, diese behebt und dokumentiert sowie dies seinen Kunden zusichert.
- Die verwendete Version von Basis-Images DARF NICHT abgekündigt („deprecated“) sein.
- Es MÜSSEN eindeutige Versionsnummern angegeben sein.
- Wenn ein Image mit einer neueren Versionsnummer verfügbar ist, MUSS im Rahmen des Patch- und Änderungsmanagement geprüft werden, ob und wie dieses ausgerollt werden kann.

## SYS.1.6.A7 Persistenz von Protokollierungsdaten der Container (B)

- Die Speicherung der Protokollierungsdaten der Container MUSS außerhalb des Containers, mindestens auf dem Container-Host, erfolgen.

## SYS.1.6.A8 Sichere Speicherung von Zugangsdaten bei Containern (B)

- Zugangsdaten MÜSSEN so gespeichert und verwaltet werden, dass nur berechtigte Personen und Container darauf zugreifen können.
- Insbesondere MUSS sichergestellt sein, dass Zugangsdaten nur an besonders geschützten Orten und nicht in den Images liegen.
- Die von der Verwaltungssoftware des Container-Dienstes bereitgestellten Verwaltungsmechanismen für Zugangsdaten SOLLTEN eingesetzt werden.
- Mindestens die folgenden Zugangsdaten MÜSSEN sicher gespeichert werden:
    - Passwörter jeglicher Accounts,
    - API-Keys für von der Anwendung genutzte Dienste,
    - Schlüssel für symmetrische Verschlüsselungen sowie
    - private Schlüssel bei Public-Key-Authentisierung.

## SYS.1.6.A9 Eignung für Container-Betrieb (S)

- Die Anwendung bzw. der Dienst, der im Container betrieben werden soll, SOLLTE für den Container-Betrieb geeignet sein.
- Dabei SOLLTE berücksichtigt werden, dass Container häufiger für die darin ausgeführte Anwendung unvorhergesehen beendet werden können.
- Die Ergebnisse der Prüfung nach SYS.1.6.A3 Sicherer Einsatz containerisierter IT-Systeme SOLLTE nachvollziehbar dokumentiert werden.

## SYS.1.6.A10 Richtlinie für Images und Container-Betrieb (S)

- Es SOLLTE eine Richtlinie erstellt und angewendet werden, die die Anforderungen an den Betrieb der Container und die erlaubten Images festlegt.
- Die Richtlinie SOLLTE auch Anforderungen an den Betrieb und die Bereitstellung der Images enthalten.

## SYS.1.6.A11 Nur ein Dienst pro Container (S)

- Jeder Container SOLLTE jeweils nur einen Dienst bereitstellen.

## SYS.1.6.A12 Verteilung sicherer Images (S)

- Es SOLLTE angemessen dokumentiert werden, welche Quellen für Images als vertrauenswürdig klassifiziert wurden und warum.
- Zusätzlich SOLLTE der Prozess angemessen dokumentiert werden, wie Images bzw. die im Image enthaltenen Softwarebestandteile aus vertrauenswürdigen Quellen bezogen und schließlich für den produktiven Betrieb bereitgestellt werden.
- Die verwendeten Images SOLLTEN über Metadaten verfügen, die die Funktion und die Historie des Images nachvollziehbar machen.
- Digitale Signaturen SOLLTEN jedes Image gegen Veränderung absichern.

## SYS.1.6.A13 Freigabe von Images (S)

- Alle Images für den produktiven Betrieb SOLLTEN wie Softwareprodukte einen Test- und Freigabeprozess gemäß des Bausteins OPS.1.1.6 Software-Test und Freigaben durchlaufen.

## SYS.1.6.A14 Aktualisierung von Images (S)

- Bei der Erstellung des Konzeptes für das Patch- und Änderungsmanagement gemäß OPS.1.1.3 Patch- und Änderungsmanagement SOLLTE entschieden werden, wann und wie die Updates der Images oder der betriebenen Software bzw. des betriebenen Dienstes ausgerollt werden.
- Bei persistenten Containern SOLLTE geprüft werden, ob in Ausnahmefällen ein Update des jeweiligen Containers geeigneter ist, als den Container vollständig neu zu provisionieren.

## SYS.1.6.A15 Limitierung der Ressourcen pro Container (S)

- Für jeden Container SOLLTEN Ressourcen auf dem Host-System, wie CPU, flüchtiger und persistenter Speicher sowie Netzbandbreite, angemessen reserviert und limitiert werden.
- Es SOLLTE definiert und dokumentiert sein, wie das System im Fall einer Überschreitung dieser Limitierungen reagiert.

## SYS.1.6.A16 Administrativer Fernzugriff auf Container (S)

- Administrative Zugriffe von einem Container auf den Container-Host und umgekehrt SOLLTEN prinzipiell wie administrative Fernzugriffe betrachtet werden.
- Aus einem Container SOLLTEN KEINE administrativen Fernzugriffe aufden Container-Host erfolgen.
- Applikations-Container SOLLTEN keine Fernwartungszugänge enthalten.
- Administrative Zugriffe auf Applikations-Container SOLLTEN immer über die Container-Runtime erfolgen.

## SYS.1.6.A17 Ausführung von Containern ohne Privilegien (S)

- Die Container-Runtime und alle instanziierten Container SOLLTEN nur von einem nicht-privilegierten System-Account ausgeführt werden, der über keine erweiterten Rechte für den Container-Dienst bzw. das Betriebssystem des Host-Systems verfügt oder diese Rechte erlangen kann.
- Die Container-Runtime SOLLTE durch zusätzliche Maßnahmen gekapselt werden, etwa durch Verwendung der Virtualisierungs-Erweiterungen von CPUs.
- Sofern Container ausnahmsweise Aufgaben des Host-Systems übernehmen sollen, SOLLTEN die Privilegien auf dem Host-System auf das erforderliche Minimum begrenzt werden.
- Ausnahmen SOLLTEN angemessen dokumentiert werden.

## SYS.1.6.A18 Accounts der Anwendungsdienste (S)

- Die System-Accounts innerhalb eines Containers SOLLTEN keine Berechtigungen auf dem Host-System haben.
- Wo aus betrieblichen Gründen diese Berechtigung notwendig ist, SOLLTE diese nur für unbedingt notwendige Daten und Systemzugriffe gelten.
- Der Account im Container, der für diesen Datenaustausch notwendig ist, SOLLTE im Host-System bekannt sein.

## SYS.1.6.A19 Einbinden von Datenspeichern in Container (S)

- Die Container SOLLTEN NUR auf die für den Betrieb notwendigen Massenspeicher und Verzeichnisse zugreifen können.
- Nur wenn Berechtigungen benötigt werden, SOLLTEN diese explizit vergeben werden.
- Sofern die Container-Runtime für einen Container lokalen Speicher einbindet, SOLLTEN die Zugriffsrechte im Dateisystem auf den Service-Account des Containers eingeschränkt sein.
- Werden Netzspeicher verwendet, so SOLLTEN die Berechtigungen auf dem Netzspeicher selbst gesetzt werden.

## SYS.1.6.A20 Absicherung von Konfigurationsdaten (S)

- Die Beschreibung der Container-Konfigurationsdaten SOLLTE versioniert erfolgen.
- Änderungen SOLLTEN nachvollziehbar dokumentiert sein.

## SYS.1.6.A21 Erweiterte Sicherheitsrichtlinien (H)

- Erweiterte Richtlinien SOLLTEN die Berechtigungen der Container einschränken.
- Mandatory Access Control (MAC) oder eine vergleichbare Technik SOLLTE diese Richtlinien erzwingen.
- Die Richtlinien SOLLTEN mindestens folgende Zugriffe einschränken:
    - eingehende und ausgehende Netzverbindungen,
    - Dateisystem-Zugriffe und
    - Kernel-Anfragen (Syscalls).
- Die Runtime SOLLTE die Container so starten, dass der Kernel des Host-Systems alle nicht von der Richtlinie erlaubten Aktivitäten der Container verhindert (z. B. durch die Einrichtung lokaler Paketfilter oder durch Entzug von Berechtigungen) oder zumindest Verstöße geeignet meldet.

## SYS.1.6.A22 Vorsorge für Untersuchungen (H)

- Um Container im Bedarfsfall für eine spätere Untersuchung verfügbar zu haben, SOLLTE ein Abbild des Zustands nach festgelegten Regeln erstellt werden.

## SYS.1.6.A23 Unveränderlichkeit der Container (H)

- Container SOLLTEN ihr Dateisystem während der Laufzeit nicht verändern können.
- Dateisysteme SOLLTEN nicht mit Schreibrechten eingebunden sein.

## SYS.1.6.A24 Hostbasierte Angriffserkennung (H)

- Das Verhalten der Container und der darin betriebenen Anwendungen bzw. Dienste SOLLTE überwacht werden.
- Abweichungen von einem normalen Verhalten SOLLTEN bemerkt und gemeldet werden.
- Die Meldungen SOLLTEN im zentralen Prozess zur Behandlung von Sicherheitsvorfällen angemessen behandelt werden.
- Das zu überwachenden Verhalten SOLLTE mindestens umfassen:
    - Netzverbindungen,
    - erstellte Prozesse,
    - Dateisystem-Zugriffe und
    - Kernel-Anfragen (Syscalls).

## SYS.1.6.A25 Hochverfügbarkeit von containerisierten Anwendungen (H)

- Bei hohen Verfügbarkeitsanforderungen der containerisierten Anwendungen SOLLTE entschieden werden, auf welcher Ebene die Verfügbarkeit realisiert werden soll (z. B. redundant auf der Ebene des Hosts).

## SYS.1.6.A26 Weitergehende Isolation und Kapselung von Containern (H)

- Wird eine weitergehende Isolation und Kapselung von Containern benötigt, dann SOLLTEN folgende Maßnahmen nach steigender Wirksamkeit geprüft werden:
    - feste Zuordnung von Containern zu Container-Hosts,
    - Ausführung der einzelnen Container und/oder des Container-Hosts mit Hypervisoren,
    - feste Zuordnung eines einzelnen Containers zu einem einzelnen Container-Host.


