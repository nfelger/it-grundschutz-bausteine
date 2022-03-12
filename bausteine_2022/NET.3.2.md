# NET.3.2: Firewall

## NET.3.2.A1 Erstellung einer Sicherheitsrichtlinie (B)

- Ausgehend von der allgemeinen Sicherheitsrichtlinie der Institution MUSS eine spezifische Sicherheitsrichtlinie erstellt werden.
- In dieser MÜSSEN nachvollziehbar Anforderungen und Vorgaben beschrieben sein, wie Firewalls sicher betrieben werden können.
- Die Richtlinie MUSS allen im Bereich Firewalls zuständigen Mitarbeitern bekannt und grundlegend für ihre Arbeit sein.
- Wird die Richtlinie verändert oder wird von den Anforderungen abgewichen, MUSS dies mit dem ISB abgestimmt und dokumentiert werden.
- Es MUSS regelmäßig überprüft werden, ob die Richtlinie noch korrekt umgesetzt ist.
- Die Ergebnisse MÜSSEN sinnvoll dokumentiert werden.

## NET.3.2.A2 Festlegen der Firewall-Regeln (B)

- Die gesamte Kommunikation zwischen den beteiligten Netzen MUSS über die Firewall geleitet werden.
- Es MUSS sichergestellt sein, dass von außen keine unerlaubten Verbindungen in das geschützte Netz aufgebaut werden können.
- Ebenso DÜRFEN KEINE unerlaubten Verbindungen aus dem geschützten Netz heraus aufgebaut werden.
- Für die Firewall MÜSSEN eindeutige Regeln definiert werden, die festlegen, welche Kommunikationsverbindungen und Datenströme zugelassen werden.
- Alle anderen Verbindungen MÜSSEN durch die Firewall unterbunden werden (Whitelist-Ansatz).
- Die Kommunikationsbeziehungen mit angeschlossenen Dienst-Servern, die über die Firewall geführt werden, MÜSSEN in den Regeln berücksichtigt sein.
- Es MÜSSEN Verantwortliche benannt werden, die Filterregeln entwerfen, umsetzen und testen.
- Zudem MUSS geklärt werden, wer Filterregeln verändern darf.
- Die getroffenen Entscheidungen sowie die relevanten Informationen und Entscheidungsgründe MÜSSEN dokumentiert werden.

## NET.3.2.A3 Einrichten geeigneter Filterregeln am Paketfilter (B)

- Basierend auf den Firewall-Regeln aus NET.3.2.A2 Festlegen der Firewall-Regeln MÜSSEN geeignete Filterregeln für den Paketfilter definiert und eingerichtet werden.
- Ein Paketfilter MUSS so eingestellt sein, dass er alle ungültigen TCP-Flag-Kombinationen verwirft.
- Grundsätzlich MUSS immer zustandsbehaftet gefiltert werden.
- Auch für die verbindungslosen Protokolle UDP und ICMP MÜSSEN zustandsbehaftete Filterregeln konfiguriert werden.
- Die Firewall MUSS die Protokolle ICMP und ICMPv6 restriktiv filtern.

## NET.3.2.A4 Sichere Konfiguration der Firewall (B)

- Bevor eine Firewall eingesetzt wird, MUSS sie sicher konfiguriert werden.
- Alle Konfigurationsänderungen MÜSSEN nachvollziehbar dokumentiert sein.
- Die Integrität der Konfigurationsdateien MUSS geeignet geschützt werden.
- Bevor Zugangspasswörter abgespeichert werden, MÜSSEN sie mithilfe eines zeitgemäßen kryptografischen Verfahrens abgesichert werden (siehe CON.1 Kryptokonzept).
- Eine Firewall MUSS so konfiguriert sein, dass ausschließlich zwingend erforderliche Dienste verfügbar sind.
- Wenn funktionale Erweiterungen benutzt werden, MÜSSEN die Sicherheitsrichtlinien der Institution weiterhin erfüllt sein.
- Auch MUSS begründet und dokumentiert werden, warum solche Erweiterungen eingesetzt werden.
- Nicht benötigte (Auskunfts-)Dienste sowie nicht benötigte funktionale Erweiterungen MÜSSEN deaktiviert oder ganz deinstalliert werden.
- Informationen über den internen Konfigurations- und Betriebszustand MÜSSEN nach außen bestmöglich verborgen werden.

## NET.3.2.A5 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## NET.3.2.A6 Schutz der Administrationsschnittstellen (B)

- Alle Administrations- und Managementzugänge der Firewall MÜSSEN auf einzelne Quell-IP-Adressen bzw. -Adressbereiche eingeschränkt werden.
- Es MUSS sichergestellt sein, dass aus nicht vertrauenswürdigen Netzen heraus nicht auf die Administrationsschnittstellen zugegriffen werden kann.
- Um die Firewall zu administrieren bzw. zu überwachen, DÜRFEN NUR sichere Protokolle eingesetzt werden.
- Alternativ MUSS ein eigens dafür vorgesehenes Administrationsnetz (Out-of-Band-Management) verwendet werden.
- Für die Benutzerschnittstellen MÜSSEN geeignete Zeitbeschränkungen vorgegeben werden.

## NET.3.2.A7 Notfallzugriff auf die Firewall (B)

- Es MUSS immer möglich sein, direkt auf die Firewall zugreifen zu können, sodass sie im Notfall auch dann lokal administriert werden kann, wenn das gesamte Netz ausfällt.

## NET.3.2.A8 Unterbindung von dynamischem Routing (B)

- In den Einstellungen der Firewall MUSS das dynamische Routing deaktiviert sein, es sei denn, der Paketfilter wird entsprechend dem Baustein NET.3.1 Router und Switches als Perimeter-Router eingesetzt.

## NET.3.2.A9 Protokollierung (B)

- Die Firewall MUSS so konfiguriert werden, dass sie mindestens folgende sicherheitsrelevante Ereignisse protokolliert:
    - abgewiesene Netzverbindungen (Quell- und Ziel-IP-Adressen, Quell- und Zielport oder ICMP/ICMPv6-Typ, Datum, Uhrzeit),
    - fehlgeschlagene Zugriffe auf System-Ressourcen aufgrund fehlerhafter Authentisierungen, mangelnder Berechtigung oder nicht vorhandener Ressourcen,
    - Fehlermeldungen der Firewall-Dienste,
    - allgemeine Systemfehlermeldungen und
    - Konfigurationsänderungen (möglichst automatisch).
- Werden Sicherheitsproxies eingesetzt, MÜSSEN Sicherheitsverletzungen und Verstöße gegen Access-Control-Listen (ACLs oder auch kurz Access-Listen) in geeigneter Weise protokolliert werden.
- Hierbei MÜSSEN mindestens die Art der Protokollverletzung bzw. des ACL-Verstoßes, Quell- und Ziel-IP-Adresse, Quell- und Zielport, Dienst, Datum und Zeit sowie, falls erforderlich, die Verbindungsdauer protokolliert werden.
- Wenn sich ein Benutzer am Sicherheitsproxy authentisiert, MÜSSEN auch Authentisierungsdaten oder ausschließlich die Information über eine fehlgeschlagene Authentisierung protokolliert werden.

## NET.3.2.A10 Abwehr von Fragmentierungsangriffen am Paketfilter (B)

- Am Paketfilter MÜSSEN Schutzmechanismen aktiviert sein, um IPv4- sowie IPv6 Fragmentierungsangriffe abzuwehren.

## NET.3.2.A11 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## NET.3.2.A12 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## NET.3.2.A13 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## NET.3.2.A14 Betriebsdokumentationen (B)

- Die betrieblichen Aufgaben einer Firewall MÜSSEN nachvollziehbar dokumentiert werden.
- Es MÜSSEN alle Konfigurationsänderungen sowie sicherheitsrelevante Aufgaben dokumentiert werden, insbesondere Änderungen an den Systemdiensten und dem Regelwerk der Firewall.
- Die Dokumentation MUSS vor unbefugten Zugriffen geschützt werden.

## NET.3.2.A15 Beschaffung einer Firewall (B)

- Bevor eine Firewall beschafft wird, MUSS eine Anforderungsliste erstellt werden, anhand derer die am Markt erhältlichen Produkte bewertet werden.
- Es MUSS darauf geachtet werden, dass das von der Institution angestrebte Sicherheitsniveau mit der Firewall erreichbar ist.
- Grundlage für die Beschaffung MÜSSEN daher die Anforderungen aus der Sicherheitsrichtlinie sein.
- Wird IPv6 eingesetzt, MUSS der Paketfilter die IPv6-Erweiterungsheader (Extension Header) überprüfen.
- Zudem MUSS sich IPv6 adäquat zu IPv4 konfigurieren lassen.

## NET.3.2.A16 Aufbau einer „P-A-P“-Struktur (S)

- Eine „Paketfilter – Application-Level-Gateway – Paketfilter“-(P-A-P)-Struktur SOLLTE eingesetzt werden.
- Sie MUSS aus mehreren Komponenten mit jeweils dafür geeigneter Hard- und Software bestehen.
- Für die wichtigsten verwendeten Protokolle SOLLTEN Sicherheitsproxies auf Anwendungsschicht vorhanden sein.
- Für andere Dienste SOLLTEN zumindest generische Sicherheitsproxies für TCP und UDP genutzt werden.
- Die Sicherheitsproxies SOLLTEN zudem innerhalb einer abgesicherten Laufzeitumgebung des Betriebssystems ablaufen.

## NET.3.2.A17 Deaktivierung von IPv4 oder IPv6 (S)

- Wenn das IPv4- oder IPv6-Protokoll in einem Netzsegment nicht benötigt wird, SOLLTE es am jeweiligen FirewallNetzzugangspunkt (z. B. am entsprechenden Firewall-Interface) deaktiviert werden.
- Falls das IPv4- oder IPv6-Protokoll nicht benötigt bzw. eingesetzt wird, SOLLTE es auf der Firewall komplett deaktiviert werden.

## NET.3.2.A18 Administration über ein gesondertes Managementnetz (S)

- Firewalls SOLLTEN ausschließlich über ein separates Managementnetz (Out-of-Band-Management) administriert werden.
- Eine eventuell vorhandene Administrationsschnittstelle über das eigentliche Datennetz (In-Band) SOLLTE deaktiviert werden.
- Die Kommunikation im Managementnetz SOLLTE über Management-Firewalls (siehe NET.1.1 Netz-Architektur und -design) auf wenige Managementprotokolle mit genau festgelegten Ursprüngen und Zielen beschränkt werden.
- Die verfügbaren Sicherheitsmechanismen der eingesetzten Managementprotokolle zur Authentisierung, Integritätssicherung und Verschlüsselung SOLLTEN aktiviert sein.
- Alle unsicheren Managementprotokolle SOLLTEN deaktiviert werden (siehe NET.1.2 Netz-Management).

## NET.3.2.A19 Schutz vor TCP SYN Flooding, UDP Paket Storm und Sequence Number Guessing am Paketfilter (S)

- Am Paketfilter, der Server-Dienste schützt, die aus nicht vertrauenswürdigen Netzen erreichbar sind, SOLLTE ein geeignetes Limit für halboffene und offene Verbindungen gesetzt werden.
- Am Paketfilter, der Server-Dienste schützt, die aus weniger oder nicht vertrauenswürdigen Netzen erreichbar sind, SOLLTEN die sogenannten Rate Limits für UDP-Datenströme gesetzt werden.
- Am äußeren Paketfilter SOLLTE bei ausgehenden Verbindungen für TCP eine zufällige Generierung von Initial Sequence Numbers (ISN) aktiviert werden, sofern dieses nicht bereits durch Sicherheitsproxies realisiert wird.

## NET.3.2.A20 Absicherung von grundlegenden Internetprotokollen (S)

- Die Protokolle HTTP, SMTP und DNS inklusive ihrer verschlüsselten Versionen SOLLTEN über protokollspezifische Sicherheitsproxies geleitet werden.

## NET.3.2.A21 Temporäre Entschlüsselung des Datenverkehrs (S)

- Verschlüsselte Verbindungen in nicht vertrauenswürdige Netze SOLLTEN temporär entschlüsselt werden, um das Protokoll zu verifizieren und die Daten auf Schadsoftware zu prüfen.
- Hierbei SOLLTEN die rechtlichen Rahmenbedingungen beachtet werden.
- Die Komponente, die den Datenverkehr temporär entschlüsselt, SOLLTE unterbinden, dass veraltete Verschlüsselungsoptionen und kryptografische Algorithmenbenutzt werden.
- Der eingesetzte TLS-Proxy SOLLTE prüfen können, ob Zertifikate vertrauenswürdig sind.
- Ist ein Zertifikat nicht vertrauenswürdig, SOLLTE es möglich sein, die Verbindung abzuweisen.
- Eigene Zertifikate SOLLTEN nachrüstbar sein, um auch „interne“ Root-Zertifikate konfigurieren und prüfen zu können.
- Vorkonfigurierte Zertifikate SOLLTEN überprüft und entfernt werden, wenn sie nicht benötigt werden.

## NET.3.2.A22 Sichere Zeitsynchronisation (S)

- Die Uhrzeit der Firewall SOLLTE mit einem Network-Time-Protocol (NTP)-Server synchronisiert werden.
- Die Firewall SOLLTE keine externe Zeitsynchronisation zulassen.

## NET.3.2.A23 Systemüberwachung und -Auswertung (S)

- Firewalls SOLLTEN in ein geeignetes Systemüberwachungs- bzw. Monitoringkonzept eingebunden werden.
- Es SOLLTE ständig überwacht werden, ob die Firewall selbst sowie die darauf betriebenen Dienste korrekt funktionieren.
- Bei Fehlern oder wenn Grenzwerte überschritten werden, SOLLTE das Betriebspersonal alarmiert werden.
- Zudem SOLLTEN automatische Alarmmeldungen generiert werden, die bei festgelegten Ereignissen ausgelöst werden.
- Protokolldaten oder Statusmeldungen SOLLTEN NUR über sichere Kommunikationswege übertragen werden.

## NET.3.2.A24 Revision und Penetrationstests (S)

- Die Firewall-Struktur SOLLTE regelmäßig auf bekannte Sicherheitsprobleme hin überprüft werden.
- Es SOLLTEN regelmäßige Penetrationstests und Revisionen durchgeführt werden.

## NET.3.2.A32 Notfallvorsorge für die Firewall (S)

- Diagnose und Fehlerbehebungen SOLLTEN bereits im Vorfeld geplant und vorbereitet werden.
- Für typische Ausfallszenarien SOLLTEN entsprechende Handlungsanweisungen definiert und in regelmäßigen Abständen aktualisiert werden.
- Die Notfallplanungen für die Firewall SOLLTEN mit der übergreifenden Störungs- und Notfallvorsorge abgestimmt sein.
- Sie SOLLTEN sich am allgemeinen Notfallvorsorgekonzept orientieren (siehe DER.4 Notfallmanagement).
- Es SOLLTE sichergestellt sein, dass die Dokumentationen zur Notfallvorsorge und die darin enthaltenen Handlungsanweisungen in Papierform vorliegen.
- Das im Rahmen der Notfallvorsorge beschriebene Vorgehen SOLLTE regelmäßig geprobt werden.

## NET.3.2.A25 Erweiterter Integritätsschutz für die Konfigurationsdateien (H)

- Um eine abgestürzte Firewall wieder herzustellen, SOLLTE sichergestellt werden, dass keine alten oder fehlerhaften Konfigurationen (unter anderem Access-Listen) benutzt werden.
- Dies SOLLTE auch gelten, wenn es einem Angreifer gelingt, die Firewall neu zu starten.

## NET.3.2.A26 Auslagerung von funktionalen Erweiterungen auf dedizierte Hardware (H)

- Funktionale Erweiterungen der Firewall SOLLTEN auf dedizierte Hard- und Software ausgelagert werden.

## NET.3.2.A27 Einsatz verschiedener Firewall-Betriebssysteme und -Produkte in einer mehrstufigen FirewallArchitektur (H)

- In einer mehrstufigen Firewall-Architektur SOLLTEN unterschiedliche Betriebssysteme und -Produkte für die äußeren und inneren Firewalls eingesetzt werden.

## NET.3.2.A28 Zentrale Filterung von aktiven Inhalten (H)

- Aktive Inhalte SOLLTEN gemäß den Sicherheitszielen der Institution zentral gefiltert werden.
- Dafür SOLLTE auch der verschlüsselte Datenverkehr entschlüsselt werden.
- Die erforderlichen Sicherheitsproxies SOLLTEN es unterstützen, aktive Inhalte zu filtern.

## NET.3.2.A29 Einsatz von Hochverfügbarkeitslösungen (H)

- Paketfilter und Application-Level-Gateway SOLLTEN hochverfügbar ausgelegt werden.
- Zudem SOLLTEN zwei voneinander unabhängige Zugangsmöglichkeiten zum externen Netz bestehen, z. B. zwei Internetzugänge von unterschiedlichen Providern.
- Interne und externe Router sowie alle weiteren beteiligten aktiven Komponenten (z. B. Switches) SOLLTEN ebenfalls hochverfügbar ausgelegt sein.
- Auch nach einem automatischen Failover SOLLTE die Firewall-Struktur die Anforderungen der Sicherheitsrichtlinie erfüllen (Fail safe bzw. Fail secure).
- Die Funktion SOLLTE anhand von zahlreichen Parametern überwacht werden.
- Die Funktionsüberwachung SOLLTE sich nicht auf ein einzelnes Kriterium stützen.
- Protokolldateien und Warnmeldungen der Hochverfügbarkeitslösung SOLLTEN regelmäßig kontrolliert werden.

## NET.3.2.A30 Bandbreitenmanagement für kritische Anwendungen und Dienste (H)

- Um Bandbreitenmanagement für kritische Anwendungen und Dienste zu gewährleisten, SOLLTEN Paketfilter mit entsprechender Bandbreitenmanagementfunktion an Netzübergängen und am Übergang zwischen verschiedenen Sicherheitszonen eingesetzt werden.

## NET.3.2.A31 Einsatz von zertifizierten Produkten (H)

- Firewalls mit einer Sicherheitsevaluierung nach Common Criteria SOLLTEN eingesetzt werden, mindestens mit der Stufe EAL4.


