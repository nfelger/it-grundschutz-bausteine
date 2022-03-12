# IND.3.2: Fernwartung im industriellen Umfeld

## IND.3.2.A1 Planung des Einsatzes der Fernwartung in der OT (B) [Planer]

- Im industriellen Umfeld MUSS für sämtliche Einrichtungen zur Fernwartung ein einheitliches, zentrales Fernwartungskonzept für die gesamte OT der Institution erstellt werden.
- In dem OT-Fernwartungskonzept MÜSSEN folgende Aspekte berücksichtigt werden:
    - spezifische Vorgaben durch Anlagenhersteller,
    - spezifische Anforderungen durch dezentrale Infrastrukturen,
    - spezifische Anforderungen an die Anbindungen für die Fernwartung,
    - spezifische Anforderungen an die Verfügbarkeit der Fernwartung,
    - spezifische Anforderungen durch Umgebungsbedingungen sowie
    - spezifische Anforderungen durch Bestandsanlagen.
- Alle diese Aspekte MÜSSEN mit sämtlichen beteiligten internen und externen Stellen abgestimmt werden.
- Sämtliche Fernwartungszugänge, über die Zugriffe auf ein ICS der Institution möglich sind, MÜSSEN in einer zentralen Dokumentation erfasst werden.
- Für neu anzuschaffende fernwartbare Maschinen MÜSSEN die Anforderungen an die Informationssicherheit mit dem Lieferanten abgestimmt werden.
- Das Ziel SOLLTE eine Standardisierung der verwendeten Fernwartungslösungen sein.
- Sobald standardisierte Lösungen für die Fernwartung geplant werden, MÜSSEN sich die OT und die Büro- und Gebäude-IT gemeinsam abstimmen.

## IND.3.2.A2 Konsistente Dokumentation der Fernwartung durch OT sowie Büro- und Gebäude-IT (B) [ITBetrieb, Wartungspersonal]

- Im industriellen Umfeld MÜSSEN die OT und die Büro- und Gebäude-IT sämtliche OT-Fernwartungszugänge gemeinsam erfassen und dokumentieren.
- Insbesondere bei Fernwartungskomponenten, die in Package Units integriert sind, MÜSSEN auch alle deaktivierten Zugänge dokumentiert werden.

## IND.3.2.A3 Regelmäßige Prüfungen sowie Ausnahmegenehmigungen bestehender OTFernwartungszugänge (B) [IT-Betrieb]

- Sämtliche Anlagen MÜSSEN regelmäßig geprüft werden, ob alle ihre Fernwartungszugänge dem Soll-Zustand, d. h. dem aktuellen Fernwartungskonzept für die OT entsprechen.
- Für notwendige Abweichungen vom Konzept SOLLTE innerhalb der OT ein Genehmigungsprozess etabliert werden.

## IND.3.2.A4 Verbindliche Regelung der OT-Fernwartung durch Dritte (B)

- Mit sämtlichen externen Benutzern, d. h. Herstellern, Integratoren und Wartungsdienstleistern MÜSSEN angemessen restriktive Regelungen für die OT-Fernwartung vertraglich vereinbart werden.
- Diese vertraglichen Regelungen MÜSSEN zu jedem Zeitpunkt gewährleisten, dass externe Benutzer jegliche OT-Fernwartungszugänge ausschließlich kontrolliert und abgestimmt nutzen.
- Intern MUSS festgelegt werden, über welche Fernwartungszugänge welche Tätigkeiten durch welche externen Benutzer zulässig sind.
- Darüber hinaus MUSS festgelegt werden, welche internen Mitarbeiter Fernwartungszugriffe und -tätigkeiten von Externen autorisieren, beobachten und gegebenenfalls unterstützen.
- Insbesondere bei Safety-Maschinen MUSS der interne OT-Mitarbeiter sowohl organisatorisch als auch technisch die Hoheit über den Zeitpunkt der Fernwartung haben.
- Vertraglich MUSS ausgeschlossen werden, dass der VPN-Tunnel von innen nach außen aufgebaut werden kann.

## IND.3.2.A5 Interne Abstimmung für die OT-Fernwartung mit der Büro- und Gebäude-IT (B) [Planer]

- Die OT, die Büro- und Gebäude-IT sowie alle weiteren beteiligten Organisationseinheiten MÜSSEN angemessen restriktive Regelungen für sämtliche Komponenten und Schnittstellen festlegen, die direkt oder indirekt OT-Fernwartung in der Institution ermöglichen.
- Diese internen Regelungen MÜSSEN zu jedem Zeitpunkt eine kontrollierte und abgestimmte Nutzung der jeweiligen OT-Fernwartungszugänge gewährleisten.
- Folgende Aspekte MÜSSEN geregelt werden:
    - Prozesse,
    - Zuständigkeiten,
    - Berechtigungen.

## IND.3.2.A6 Absicherung jedes Fernwartungszugriffs auf die OT (B) [IT-Betrieb]

- Im industriellen Umfeld MUSS die OT jeden Zugriff auf ein IT-System, das einen Fernwartungsdienst für die OT bereitstellt, selbst steuern können.
- Hierfür MUSS der Zugriff durch mindestens eine Sicherheitskomponente in der Zuständigkeit der OT abgesichert werden.
- Der Zugang zur Fernwartung SOLLTE für alle Zugriffe vereinheitlicht werden.
- Jeder Zugriff SOLLTE mithilfe zentraler Authentisierungskomponenten kontrolliert und explizit zugelassen werden.
- Falls OT-Fernwartungszugänge dezentrale Infrastrukturen oder in Package Units integrierte Komponenten beinhalten, dann MÜSSEN die Zugänge durch eine zusätzliche Sicherheitskomponente abgesichert werden, die ihrerseits weder integriert noch Teil der dezentralen Infrastruktur ist.

## IND.3.2.A7 Technische Entkopplung von Zugriffen (S) [Planer]

- Jeder Fernzugriff auf jegliche Komponenten in einer OT-Zone SOLLTE entkoppelt erfolgen.
- In jedem Fernwartungszugang in die OT SOLLTE ein IT-System positioniert sein, das die Verbindung vor dem Übergang in die OT-Zielzone terminiert und zum Fernwartungsdienst eine neue, reglementierte Kommunikation mit einem entsprechend anderen Protokoll aufbaut.
- Alle für die Fernwartung benötigten Werkzeuge und Programme SOLLTEN auf dem IT-System des Fernwartungszugangs installiert und lauffähig sein sowie einen Mehrbenutzerbetrieb unterstützen.
- Das IT-System SOLLTE einSprungserver oder ein Application Layer Gateway (ALG) sein, das in einem dedizierten Sicherheitssegment, z. B. in einer demilitarisierten Zone (DMZ) positioniert ist.
- Für das IT-System zur Entkopplung der Zugriffe SOLLTE die OT zuständig sein, d. h. es liegt idealerweise in einer OT-DMZ.

## IND.3.2.A8 Explizite Freigabe jeder OT-Fernwartungssitzung (S) [Mitarbeiter]

- Jede Fernwartungssitzung SOLLTE vorab durch einen OT-Mitarbeiter der Betreiber-Institution, der für das Zielsystem der Sitzung zuständig ist, genehmigt werden.
- Erst danach SOLLTE dieser zuständige OT-Mitarbeiter den Fernwartungszugang freischalten.
- Die explizite Freigabe SOLLTE sowohl im Bedarfsfall als auch während abgestimmter Wartungsfenster eingehalten werden.
- Die Freigabe SOLLTE grundsätzlich nur für einen begrenzten Zeitraum gültig sein, d. h. der zuständige OT-Mitarbeiter behält die Hoheit über den Zeitpunkt der Fernwartung (siehe Anforderung IND.3.2.A3 Regelmäßige Prüfungen sowie Ausnahmegenehmigungen bestehender OT-Fernwartungszugänge).
- Darüber hinaus SOLLTEN externe Fernwartungszugriffe ausschließlich von innen nach außen, d. h. aus dem OTNetz heraus, aufgebaut werden.
- Insbesondere DÜRFEN offene Ports zur Fernwartung NICHT von außen, d. h. von nicht vertrauenswürdigen Netzen aus, erreichbar sein.

## IND.3.2.A9 Sicherer Austausch von Dateien begleitend zur OT-Fernwartung (S) [Planer, IT-Betrieb]

- Für einen Dateiaustausch im Rahmen der OT-Fernwartung, z. B. von Konfigurationsdateien, Updates oder Handbüchern, SOLLTE ein sicheres Vorgehen etabliert werden.
- Dies MUSS mindestens eine Überprüfung auf Schadsoftware beinhalten.
- Der Verbindungsaufbau zwischen einem Datenaustauschsystem und Dateiquelle SOLLTE nicht automatisiert erfolgen, sondern vor jedem Dateiaustausch von der OT der Institution initiiert und authentisiert werden.
- Ein Dateiaustausch SOLLTE grundsätzlich protokolliert werden.

## IND.3.2.A10 Beobachtung und Kontrolle von OT-Fernwartungssitzungen (S) [Mitarbeiter]

- Im industriellen Umfeld MUSS sichergestellt werden, dass Personen an oder in Anlagen und Maschinen weder direkt noch indirekt durch eine aktive Fernwartung gefährdet werden können.
- Darüber hinaus MUSS sichergestellt werden, dass eine aktive Fernwartung den Produktionsprozess nicht beeinträchtigt.
- Falls Personen- oder Sachschäden möglich sind, MUSS sichergestellt sein, dass ein OT-Mitarbeiter die Fernwartungstätigkeiten vor Ort mitverfolgen kann (Vier-Augen-Prinzip).
- Der OT-Mitarbeiter SOLLTE bei Bedarf eingreifen können sowie eine Fernwartungssitzung unterbrechen können.

## IND.3.2.A11 Zentrale Verwaltung aller Benutzerkonten für die OT-Fernwartung (S) [IT-Betrieb]

- Für den Fernwartungszugriff in der OT SOLLTEN ausschließlich Benutzerkonten verwendet werden, die in einem zentralen Verzeichnisdienst der OT oder der Institution verwaltet werden.

## IND.3.2.A12 Dedizierte Fernwartungslösung in der OT (H) [Planer]

- Für die Fernwartung im industriellen Umfeld SOLLTE eine dedizierte OT-Fernwartungslösung eingesetzt werden, die unabhängig von der Büro- und Gebäude-IT ist.
- Alle weiteren Funktionen auf den IT-Systemen zur OT-Fernwartung, insbesondere auch Funktionen zur Administration von IT-Systemen und Netzen außerhalb der OT, SOLLTEN deaktiviert bzw. unterbunden werden.
- Falls eine maximale Unabhängigkeit realisiert werden soll, SOLLTE auch ein dedizierter Internet-Zugang für die OTFernwartung genutzt werden.

## IND.3.2.A13 Protokollierung der Inhalte von Fernwartungszugriffen in der OT (H) [Planer, Datenschutzbeauftragter]

- Für die Fernwartung von OT-Anwendungen oder -Systemen SOLLTE die Protokollierung so ausgeweitet werden, dass sämtliche Tätigkeiten lückenlos und umgehend nachvollziehbar sind.
- Hierzu SOLLTEN ergänzend zur Protokollierung von Ereignissen und Sitzungsdaten auch die Inhalte von Fernwartungszugriffen protokolliert werden.

## IND.3.2.A14 Technische Kontrolle von Fernwartungssitzungen (H) [Planer, Datenschutzbeauftragter]

- OT-Fernwartungssitzungen SOLLTEN ergänzend zu IND.3.2.A10 Beobachtung und Kontrolle von OT-Fernwartungssitzungen kontinuierlich durch eine technische Lösung reglementiert werden.
- Dabei SOLLTEN die Aktivitäten auf Befehlsebene, d. h. manuelle und automatisierte Befehle, technisch überwacht und gegebenenfalls automatisch unterbunden werden.
- Zusätzlich SOLLTEN Sitzungen komponentenübergreifend überwacht werden.
- Falls technisch überwacht wird, dann SOLLTE nicht nur bei konkreten Regelverstößen, sondern auch bei Anomalien im Nutzerverhalten ein Alarm ausgelöst werden, z. B. sobald ein plötzlich erhöhtes Kommunikationsvolumen erkannt wird.


