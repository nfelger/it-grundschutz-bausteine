# APP.4.4: Kubernetes

## APP.4.4.A1 Planung der Separierung der Anwendungen (B)

- Vor der Inbetriebnahme MUSS geplant werden, wie die in den Pods betriebenen Anwendungen und deren unterschiedliche Test- und Produktions-Betriebsumgebungen separiert werden.
- Auf Basis des Schutzbedarfs der Anwendungen MUSS die Planung festlegen, welche Architektur der Namespaces, Meta-Tags, Cluster und Netze angemessen auf die Risiken eingeht und ob auch virtualisierte Server und Netze zum Einsatz kommen sollen.
- Die Planung MUSS Regelungen zu Netz-, CPU- und Festspeicherseparierung enthalten.
- Die Separierung SOLLTE auch das Netzzonenkonzept und den Schutzbedarf beachten und auf diese abgestimmt sein.
- Anwendungen SOLLTEN jeweils in einem eigenen Kubernetes-Namespace laufen, der alle Programme der Anwendung umfasst.
- Nur Anwendungen mit ähnlichem Schutzbedarf und ähnlichen möglichen Angriffsvektoren SOLLTEN einen Kubernetes-Cluster teilen.

## APP.4.4.A2 Planung der Automatisierung mit CI/CD (B)

- Wenn eine Automatisierung des Betriebs von Anwendungen in Kubernetes mithilfe von CI/CD stattfindet, DARF diese NUR nach einer geeigneten Planung erfolgen.
- Die Planung MUSS den gesamten Lebenszyklus von Inbetriebbis Außerbetriebnahme inklusive Entwicklung, Tests, Betrieb, Überwachung und Updates umfassen.
- Das Rollenund Rechtekonzept sowie die Absicherung von Kubernetes Secrets MÜSSEN Teil der Planung sein.

## APP.4.4.A3 Identitäts- und Berechtigungsmanagement bei Kubernetes (B)

- Kubernetes und alle anderen Anwendungen der Control Plane MÜSSEN jede Aktion eines Benutzers oder, im automatisierten Betrieb, einer entsprechenden Software authentifizieren und autorisieren, unabhängig davon, ob die Aktionen über einen Client, eine Weboberfläche oder über eine entsprechende Schnittstelle (API) erfolgt.
- Administrative Handlungen DÜRFEN NICHT anonym erfolgen.
- Jeder Benutzer DARF NUR die unbedingt notwendigen Rechte erhalten.
- Berechtigungen ohne Einschränkungen MÜSSEN sehr restriktiv vergeben werden.
- Nur ein kleiner Kreis von Personen SOLLTE berechtigt sein, Prozesse der Automatisierung zu definieren.
- Nur ausgewählte Administratoren SOLLTEN in Kubernetes das Recht erhalten, Freigaben für Festspeicher (Persistent Volumes) anzulegen oder zu ändern.

## APP.4.4.A4 Separierung von Pods (B)

- Der Betriebssystem-Kernel der Nodes MUSS über Isolationsmechanismen zur Beschränkung von Sichtbarkeit und Ressourcennutzung der Pods untereinander verfügen (vgl. Linux Namespaces und cgroups).
- Die Trennung MUSS dabei mindestens Prozess-IDs, Inter-Prozess-Kommunikation, Benutzer-IDs, Dateisystem und Netz inklusive Hostname umfassen.

## APP.4.4.A5 Datensicherung im Cluster (B)

- Es MUSS eine Datensicherung des Clusters erfolgen.
- Die Datensicherung MUSS umfassen:
    - Festspeicher (Persistent Volumes),
    - Konfigurationsdateien von Kubernetes und den weiteren Programmen der Control Plane,
    - den aktuellen Zustand des Kubernetes-Clusters inklusive der Erweiterungen,
    - Datenbanken der Konfiguration, namentlich hier etcd,
    - alle Infrastrukturanwendungen, die zum Betrieb des Clusters und der darin befindlichen Dienste notwendig sind und
    - die Datenhaltung der Code und Image Registries.
- Es SOLLTEN auch Snapshots für den Betrieb der Anwendungen betrachtet werden.
- Snapshots DÜRFEN die Datensicherung NICHT ersetzen.

## APP.4.4.A6 Initialisierung von Pods (S)

- Sofern im Pod zum Start eine Initialisierung z.B. einer Anwendung erfolgt, SOLLTE diese in einem eigenen Init-Container stattfinden.
- Es SOLLTE sichergestellt sein, dass die Initialisierung alle bereits laufenden Prozesse beendet.
- Kubernetes SOLLTE NUR bei erfolgreicher Initialisierung die weiteren Container starten.

## APP.4.4.A7 Separierung der Netze bei Kubernetes (S)

- Die Netze für die Administration der Nodes, der Control Plane sowie die einzelnen Netze der Anwendungsdienste SOLLTEN separiert werden.
- Es SOLLTEN NUR die für den Betrieb notwendigen Netzports der Pods in die dafür vorgesehenen Netze freigegeben werden.
- Bei mehreren Anwendungen auf einem Kubernetes-Cluster SOLLTEN zunächst alle Netzverbindungen zwischen den Kubernetes-Namespaces untersagt und nur benötigte Netzverbindungen gestattet sein (Whitelisting).
- Die zur Administration der Nodes, der Runtime und von Kubernetes inklusive seiner Erweiterungen notwendigen Netzports SOLLTEN NUR aus dem Administrationsnetz und von Pods, die diese benötigen, erreichbar sein.
- Nur ausgewählte Administratoren SOLLTEN in Kubernetes berechtigt sein, das CNI zu verwalten und Regeln für das Netz anzulegen oder zu ändern.

## APP.4.4.A8 Absicherung von Konfigurationsdateien bei Kubernetes (S)

- Die Konfigurationsdateien des Kubernetes-Cluster, inklusive aller Erweiterungen und Anwendungen SOLLTEN versioniert und annotiert werden.
- Zugangsrechte auf die Verwaltungssoftware der Konfigurationsdateien SOLLTEN minimal vergeben werden.
- Zugriffsrechte für lesenden und schreibenden Zugriff auf die Konfigurationsdateien der Control Plane SOLLTEN besonders sorgfältig vergeben und eingeschränkt sein.

## APP.4.4.A9 Nutzung von Kubernetes Service-Accounts (S)

- Pods SOLLTEN NICHT den „default“-Service-Account nutzen.
- Dem „default“-Service-Account SOLLTEN keine Rechte eingeräumt werden.
- Pods für unterschiedliche Anwendungen SOLLTEN jeweils unter eigenen Service-Accounts laufen.
- Berechtigungen für die Service-Accounts der Pods der Anwendungen SOLLTEN auf die unbedingt notwendigen Rechte beschränkt werden.
- Pods, die keinen Service-Account benötigen, SOLLTEN diesen nicht einsehen können und keinen Zugriff auf entsprechende Token haben.
- Nur Pods der Control Plane und Pods, die diese unbedingt benötigen, SOLLTEN privilegierte Service-Accounts nutzen.
- Programme der Automatisierung SOLLTEN jeweils eigene Token erhalten, auch wenn sie aufgrund ähnlicher Aufgaben einen gemeinsamen Service-Account nutzen.

## APP.4.4.A10 Absicherung von Prozessen der Automatisierung (S)

- Alle Prozesse der Automatisierungssoftware, wie CI/CD und deren Pipelines, SOLLTEN nur mit unbedingt notwendigen Rechten arbeiten.
- Wenn unterschiedliche Benutzergruppen über die Automatisierungssoftware die Konfiguration verändern oder Pods starten können, SOLLTE dies für jede Gruppe durch eigene Prozesse durchgeführt werden, die nur die für die jeweilige Benutzergruppe notwendigen Rechte besitzen.

## APP.4.4.A11 Überwachung der Container (S)

- In Pods SOLLTE jeder Container einen Health Check für den Start und den Betrieb („readiness“ und „liveness“) definieren.
- Diese Checks SOLLTEN Auskunft über die Verfügbarkeit der im Pod ausgeführten Software geben.
- Die Checks SOLLTEN fehlschlagen, wenn die überwachte Software ihre Aufgaben nicht ordnungsgemäß wahrnehmen kann.
- Für jede dieser Kontrollen SOLLTE eine dem im Pod betriebenen Dienst angemessene Zeitspanne definieren.
- Auf Basis dieser Checks SOLLTE Kubernetes die Pods löschen oder neu starten.

## APP.4.4.A12 Absicherung der Infrastruktur-Anwendungen (S)

- Sofern eine eigene Registry für Images oder eine Software zur Automatisierung, zur Verwaltung des Festspeichers, zur Speicherung von Konfigurationsdateien oder ähnliches im Einsatz ist, SOLLTE deren Absicherung mindestens betrachten:
    - Verwendung von personenbezogenen und Service-Accounts für den Zugang,
    - verschlüsselte Kommunikation auf allen Netzports,
    - minimale Vergabe der Berechtigungen an Benutzer und Service Accounts,
    - Protokollierung der Veränderungen und
    - regelmäßige Datensicherung.

## APP.4.4.A13 Automatisierte Auditierung der Konfiguration (H)

- Es SOLLTE ein automatisches Audit der Einstellungen der Nodes, von Kubernetes und der Pods der Anwendungen gegen eine definierte Liste der erlaubten Einstellungen und gegen standardisierte Benchmarks erfolgen.
- Kubernetes SOLLTE die aufgestellten Regeln im Cluster durch Anbindung geeigneter Werkzeuge durchsetzen.

## APP.4.4.A14 Verwendung dedizierter Nodes (H)

- In einem Kubernetes-Cluster SOLLTEN die Nodes dedizierte Aufgaben zugewiesen bekommen und jeweils nur Pods betreiben, welche der jeweiligen Aufgabe zugeordnet sind.
- Bastion Nodes SOLLTEN alle ein- und ausgehenden Datenverbindungen der Anwendungen zu anderen Netzen übernehmen.
- Management Nodes SOLLTEN die Pods der Control Plane betreiben und sie SOLLTEN nur die Datenverbindungen der Control Plane übernehmen.
- Sofern eingesetzt, SOLLTEN Speicher-Nodes nur die Pods der Festspeicherdienste im Cluster betreiben.

## APP.4.4.A15 Trennung von Anwendungen auf Node- und Cluster-Ebene (H)

- Anwendungen mit einem sehr hohen Schutzbedarf SOLLTEN jeweils eigene Kubernetes-Cluster oder dedizierte Nodes nutzen, die nicht für andere Anwendungen bereitstehen.

## APP.4.4.A16 Verwendung von Operatoren (H)

- Die Automatisierung von Betriebsaufgaben in Operatoren SOLLTE bei besonders kritischen Anwendungen und den Programmen der Control Plane zum Einsatz kommen.

## APP.4.4.A17 Attestierung von Nodes (H)

- Nodes SOLLTEN eine kryptografisch und möglichst mit einem TPM verifizierte gesicherte Zustandsmeldung an die Control Plane senden.
- Die Control Plane SOLLTE NUR Nodes in den Cluster aufnehmen, die erfolgreich ihre Unversehrtheit nachweisen konnten.

## APP.4.4.A18 Verwendung von Mikro-Segmentierung (H)

- Die Pods SOLLTEN auch innerhalb eines Kubernetes-Namespace nur über die notwendigen Netzports miteinander kommunizieren können.
- Es SOLLTEN Regeln innerhalb des CNI existieren, die alle bis auf die für den Betrieb notwendigen Netzverbindungen innerhalb des Kubernetes-Namespace unterbinden.
- Diese Regeln SOLLTEN Quelle und Ziel der Verbindungen genau definieren und dafür mindestens eines der folgenden Kriterien nutzen: ServiceName, Metadaten („Labels“), die Kubernetes Service Accounts oder zertifikatsbasierte Authentifizierung.
- Alle Kriterien, die als Bezeichnung für diese Verbindung dienen, SOLLTEN so abgesichert sein, dass sie nur von berechtigten Personen und Verwaltungs-Diensten verändert werden können.

## APP.4.4.A19 Hochverfügbarkeit von Kubernetes (H)

- Der Betrieb SOLLTE so aufgebaut sein, dass bei Ausfall eines Standortes die Cluster und damit die Anwendungen in den Pods entweder ohne Unterbrechung weiterlaufen oder in kurzer Zeit an einem anderen Standort neu anlaufen können.
- Für den Wiederanlauf SOLLTEN alle notwendigen Konfigurationsdateien, Images, Nutzdaten, Netzverbindungen und sonstige für den Betrieb benötigten Ressourcen inklusive der zum Betrieb nötigen Hardware bereits an diesem Standort verfügbar sein.
- Für den unterbrechungsfreien Betrieb des Clusters SOLLTEN die Control Plane von Kubernetes, die InfrastrukturAnwendungen der Cluster sowie die Pods der Anwendungen anhand von Standort-Daten der Nodes über mehrere Brandabschnitte so verteilt werden, dass der Ausfall eines Brandabschnitts nicht zum Ausfall der Anwendung führt.

## APP.4.4.A20 Verschlüsselte Datenhaltung bei Pods (H)

- Die Dateisysteme mit den persistenten Daten der Control Plane (hier besonders etcd) und der Anwendungsdienste SOLLTEN verschlüsselt werden.

## APP.4.4.A21 Regelmäßiger Restart von Pods (H)

- Bei einem erhöhten Risiko für Fremdeinwirkung und einem sehr hohen Schutzbedarf SOLLTEN Pods regelmäßig gestoppt und neu gestartet werden.
- Kein Pod SOLLTE länger als 24 Stunden laufen.
- Dabei SOLLTE die Verfügbarkeit der Anwendungen im Pod sichergestellt sein.


