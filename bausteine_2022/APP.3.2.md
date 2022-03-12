# APP.3.2: Webserver

## APP.3.2.A1 Sichere Konfiguration eines Webservers (B)

- Nachdem der IT-Betrieb einen Webserver installiert hat, MUSS er eine sichere Grundkonfiguration vornehmen.
- Dazu MUSS er insbesondere den Webserver-Prozess einem Benutzerkonto mit minimalen Rechten zuweisen.
- Der Webserver MUSS in einer gekapselten Umgebung ausgeführt werden, sofern dies vom Betriebssystem unterstützt wird.
- Ist dies nicht möglich, SOLLTE jeder Webserver auf einem eigenen physischen oder virtuellen Server ausgeführt werden.
- Dem Webserver-Dienst MÜSSEN alle nicht notwendige Schreibberechtigungen entzogen werden.
- Nicht benötigte Module und Funktionen des Webservers MÜSSEN deaktiviert werden.

## APP.3.2.A2 Schutz der Webserver-Dateien (B)

- Der IT-Betrieb MUSS alle Dateien auf dem Webserver, insbesondere Skripte und Konfigurationsdateien, so schützen, dass sie nicht unbefugt gelesen und geändert werden können.
- Es MUSS sichergestellt werden, dass Webanwendungen nur auf einen definierten Verzeichnisbaum zugreifen können (WWW-Wurzelverzeichnis).
- Der Webserver MUSS so konfiguriert sein, dass er nur Dateien ausliefert, die sich innerhalb des WWW-Wurzelverzeichnisses befinden.
- Der IT-Betrieb MUSS alle nicht benötigten Funktionen, die Verzeichnisse auflisten, deaktivieren.
- Vertrauliche Daten MÜSSEN vor unberechtigtem Zugriff geschützt werden.
- Insbesondere MUSS der IT-Betrieb sicherstellen, dass vertrauliche Dateien nicht in öffentlichen Verzeichnissen des Webservers liegen.
- Der IT-Betrieb MUSS regelmäßig überprüfen, ob vertrauliche Dateien in öffentlichen Verzeichnissen gespeichert wurden.

## APP.3.2.A3 Absicherung von Datei-Uploads und -Downloads (B)

- Alle mithilfe des Webservers veröffentlichten Dateien MÜSSEN vorher auf Schadprogramme geprüft werden.
- Es MUSS eine Maximalgröße für Datei-Uploads spezifiziert sein.
- Für Uploads MUSS genügend Speicherplatz reserviert werden.

## APP.3.2.A4 Protokollierung von Ereignissen (B)

- Der Webserver MUSS mindestens folgende Ereignisse protokollieren:
    - erfolgreiche Zugriffe auf Ressourcen,
    - fehlgeschlagene Zugriffe auf Ressourcen aufgrund von mangelnder Berechtigung, nicht vorhandenen Ressourcen und Server-Fehlern sowie
    - allgemeine Fehlermeldungen.
- Die Protokollierungsdaten SOLLTEN regelmäßig ausgewertet werden.

## APP.3.2.A5 Authentisierung (B)

- Wenn sich Clients mit Hilfe von Passwörtern am Webserver authentisieren, MÜSSEN diese kryptografisch gesichert und vor unbefugtem Zugriff geschützt gespeichert werden.

## APP.3.2.A6 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.3.2.A7 Rechtliche Rahmenbedingungen für Webangebote [Fachverantwortliche, Zentrale Verwaltung, Anforderungsmanager (Compliance Manager)] (B)

- Werden über den Webserver Inhalte für Dritte publiziert oder Dienste angeboten, MÜSSEN dabei die relevanten rechtlichen Rahmenbedingungen beachtet werden.
- Die Institution MUSS die jeweiligen Telemedien- und Datenschutzgesetze sowie das Urheberrecht einhalten.

## APP.3.2.A11 Verschlüsselung über TLS (B)

- Der Webserver MUSS für alle Verbindungen durch nicht vertrauenswürdige Netze eine sichere Verschlüsselung über TLS anbieten (HTTPS).
- Falls es aus Kompatibilitätsgründen erforderlich ist, veraltete Verfahren zu verwenden, SOLLTEN diese auf so wenige Fälle wie möglich beschränkt werden.
- Wenn eine HTTPS-Verbindung genutzt wird, MÜSSEN alle Inhalte über HTTPS ausgeliefert werden.
- Sogenannter Mixed Content DARF NICHT verwendet werden.

## APP.3.2.A8 Planung des Einsatzes eines Webservers (S)

- Es SOLLTE geplant und dokumentiert werden, für welchen Zweck der Webserver eingesetzt und welche Inhalte er bereitstellen soll.
- In der Dokumentation SOLLTEN auch die Informationen oder Dienstleistungen des Webangebots und die jeweiligen Zielgruppen beschrieben werden.
- Für den technischen Betrieb und die Webinhalte SOLLTEN geeignete Verantwortliche festgelegt werden.

## APP.3.2.A9 Festlegung einer Sicherheitsrichtlinie für den Webserver (S)

- Es SOLLTE eine Sicherheitsrichtlinie erstellt werden, in der die erforderlichen Maßnahmen und Verantwortlichkeiten benannt sind.
- Weiterhin SOLLTE geregelt werden, wie Informationen zu aktuellen Sicherheitslücken besorgt werden.
- Auch SOLLTE geregelt werden, wie Sicherheitsmaßnahmen umgesetzt werden und wie vorgegangen werden soll, wenn Sicherheitsvorfälle eintreten.

## APP.3.2.A10 Auswahl eines geeigneten Webhosters (S)

- Betreibt die Institution den Webserver nicht selbst, sondern nutzt Angebote externer Dienstleister im Rahmen von Webhosting, SOLLTE die Institution bei der Auswahl eines geeigneten Webhosters auf folgende Punkte achten:
    - Es SOLLTE vertraglich geregelt werden, wie die Dienste zu erbringen sind. Dabei SOLLTEN Sicherheitsaspekte innerhalb des Vertrags schriftlich in einem Service Level Agreement (SLA) festgehalten werden.
    - Die eingesetzten IT-Systeme SOLLTEN vom Dienstleister regelmäßig kontrolliert und gewartet werden. Er SOLLTE dazu verpflichtet werden, bei technischen Problemen oder einer Kompromittierung von Kundensystemen zeitnah zu reagieren.
    - Der Dienstleister SOLLTE grundlegende technische und organisatorische Maßnahmen umsetzen, um seinen Informationsverbund zu schützen.

## APP.3.2.A12 Geeigneter Umgang mit Fehlern und Fehlermeldungen (S)

- Aus den HTTP-Informationen und den angezeigten Fehlermeldungen SOLLTEN weder der Produktname noch die verwendete Version des Webservers ersichtlich sein.
- Fehlermeldungen SOLLTEN keine Details zu Systeminformationen oder Konfigurationen ausgeben.
- Der IT-Betrieb SOLLTE sicherstellen, dass der Webserver ausschließlich allgemeine Fehlermeldungen ausgibt, die den Benutzer darauf hinweisen, dass ein Fehler aufgetreten ist.
- Die Fehlermeldung SOLLTE ein eindeutiges Merkmal enthalten, das es Administratoren ermöglicht, den Fehler nachzuvollziehen.
- Bei unerwarteten Fehlern SOLLTE sichergestellt sein, dass der Webserver nicht in einem Zustand verbleibt, in dem er anfällig für Angriffe ist.

## APP.3.2.A13 Zugriffskontrolle für Webcrawler (S)

- Der Zugriff von Webcrawlern SOLLTE nach dem Robots-Exclusion-Standard geregelt werden.
- Inhalte SOLLTEN mit einem Zugriffsschutz versehen werden, um sie vor Webcrawlern zu schützen, die sich nicht an diesen Standard halten.

## APP.3.2.A14 Integritätsprüfungen und Schutz vor Schadsoftware (S)

- Der IT-Betrieb SOLLTE regelmäßig prüfen, ob die Konfigurationen des Webservers und die von ihm bereitgestellten Dateien noch integer sind und nicht durch Angreifer verändert wurden.
- Die zur Veröffentlichung vorgesehenen Dateien SOLLTEN regelmäßig auf Schadsoftware geprüft werden.

## APP.3.2.A16 Penetrationstest und Revision (S)

- Webserver SOLLTEN regelmäßig auf Sicherheitsprobleme hin überprüft werden.
- Auch SOLLTEN regelmäßig Revisionen durchgeführt werden.
- Die Ergebnisse SOLLTEN nachvollziehbar dokumentiert, ausreichend geschützt und vertraulich behandelt werden.
- Abweichungen SOLLTE nachgegangen werden.
- Die Ergebnisse SOLLTEN dem ISB vorgelegt werden.

## APP.3.2.A20 Benennung von Ansprechpartnern [Zentrale Verwaltung] (S)

- Bei umfangreichen Webangeboten SOLLTE die Institution einen Ansprechpartner für die Webangebote bestimmen.
- Es SOLLTEN Prozesse, Vorgehensweisen und Verantwortliche für Probleme oder Sicherheitsvorfälle benannt werden.
- Die Institution SOLLTE eine Kontaktmöglichkeit auf ihrer Webseite veröffentlichen, über die Externe Sicherheitsprobleme an die Institution melden können.
- Für die Behandlung von externen Sicherheitsmeldungen SOLLTE die Institution Prozesse definieren.

## APP.3.2.A15 Redundanz (H)

- Webserver SOLLTEN redundant ausgelegt werden.
- Auch die Internetanbindung des Webservers und weiterer ITSysteme, wie etwa der Webanwendungsserver, SOLLTEN redundant ausgelegt sein.

## APP.3.2.A17 ENTFALLEN (H)

- Diese Anforderung ist entfallen.

## APP.3.2.A18 Schutz vor Denial-of-Service-Angriffen (H)

- Der Webserver SOLLTE ständig überwacht werden.
- Des Weiteren SOLLTEN Maßnahmen definiert und umgesetzt werden, die DDoS-Angriffe verhindern oder zumindest abschwächen.

## APP.3.2.A19 ENTFALLEN (H)

- Diese Anforderung ist entfallen.


