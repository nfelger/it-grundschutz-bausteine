# APP.3.1: Webanwendungen und Webservices

## APP.3.1.A1 Authentisierung (B)

- Der IT-Betrieb MUSS Webanwendungen und Webservices so konfigurieren, dass sich Benutzer gegenüber der Webanwendung oder dem Webservice authentisieren müssen, wenn diese auf geschützte Ressourcen zugreifen wollen.
- Dafür MUSS eine angemessene Authentisierungsmethode ausgewählt werden.
- Der Auswahlprozess SOLLTE dokumentiert werden.
- Der IT-Betrieb MUSS geeignete Grenzwerte für fehlgeschlagene Anmeldeversuche festlegen.

## APP.3.1.A2 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.3.1.A3 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.3.1.A4 Kontrolliertes Einbinden von Dateien und Inhalten (B)

- Falls eine Webanwendung oder ein Webservice eine Upload-Funktion für Dateien anbietet, MUSS diese Funktion durch den IT-Betrieb so weit wie möglich eingeschränkt werden.
- Insbesondere MÜSSEN die erlaubte Dateigröße, erlaubte Dateitypen und erlaubte Speicherorte festgelegt werden.
- Es MUSS festgelegt werden, welche Benutzer die Funktion verwenden dürfen.
- Auch MÜSSEN Zugriffs- und Ausführungsrechte restriktiv gesetzt werden.
- Zudem MUSS sichergestellt werden, dass ein Benutzer Dateien nur im vorgegebenen erlaubten Speicherort speichern kann.

## APP.3.1.A5 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.3.1.A6 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.3.1.A7 Schutz vor unerlaubter automatisierter Nutzung (B)

- Der IT-Betrieb MUSS sicherstellen, dass Webanwendungen und Webservices vor unberechtigter automatisierter Nutzung geschützt werden.
- Dabei MUSS jedoch berücksichtigt werden, wie sich die Schutzmechanismen auf die Nutzungsmöglichkeiten berechtigter Benutzer auswirken.
- Wenn die Webanwendung RSS-Feeds oder andere Funktionen enthält, die explizit für die automatisierte Nutzung vorgesehen sind, MUSS dies ebenfalls bei der Konfiguration der Schutzmechanismen berücksichtigt werden.

## APP.3.1.A14 Schutz vertraulicher Daten (B)

- Der IT-Betrieb MUSS sicherstellen, dass Zugangsdaten zur Webanwendung oder zum Webservice serverseitig mithilfe von sicheren kryptografischen Algorithmen vor unbefugtem Zugriff geschützt werden.
- Dazu MÜSSEN Salted Hash-Verfahren verwendet werden.
- Die Dateien mit den Quelltexten der Webanwendung oder des Webservices MÜSSEN vor unerlaubten Abrufen geschützt werden.

## APP.3.1.A16 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.3.1.A19 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.3.1.A8 Systemarchitektur [Beschaffungsstelle] (S)

- Sicherheitsaspekte SOLLTEN bereits während der Planung von Webanwendungen und Webservices betrachtet werden.
- Auch SOLLTE darauf geachtet werden, dass die Architektur der Webanwendung oder des Webservice die Geschäftslogik der Institution exakt erfasst und korrekt umsetzt.

## APP.3.1.A9 Beschaffung von Webanwendungen und Webservices (S)

- Zusätzlich zu den allgemeinen Aspekten der Beschaffung von Software SOLLTE die Institution mindestens Folgendes bei der Beschaffung von Webanwendungen und Webservices berücksichtigen:
    - sichere Eingabevalidierung und Ausgabekodierung,
    - sicheres Session-Management,
    - sichere kryptografische Verfahren,
    - sichere Authentisierungsverfahren,
    - sichere Verfahren zum serverseitigen Speichern von Zugangsdaten,
    - geeignetes Berechtigungsmanagement,
    - ausreichende Protokollierungsmöglichkeiten,
    - regelmäßige Sicherheitsupdates durch den Entwickler der Software,
    - Schutzmechanismen vor verbreiteten Angriffen auf Webanwendungen und Webservices sowie
    - Zugriff auf den Quelltext der Webanwendung oder des Webservices.

## APP.3.1.A10 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.3.1.A11 Sichere Anbindung von Hintergrundsystemen (S)

- Der Zugriff auf Hintergrundsysteme, auf denen Funktionen und Daten ausgelagert werden, SOLLTE ausschließlich über definierte Schnittstellen und von definierten IT-Systemen aus möglich sein.
- Bei der Kommunikation über Netzund Standortgrenzen hinweg SOLLTE der Datenverkehr authentisiert und verschlüsselt werden.

## APP.3.1.A12 Sichere Konfiguration (S)

- Webanwendungen und Webservices SOLLTEN so konfiguriert sein, dass auf ihre Ressourcen und Funktionen ausschließlich über die vorgesehenen, abgesicherten Kommunikationspfade zugegriffen werden kann.
- Der Zugriff auf nicht benötigte Ressourcen und Funktionen SOLLTE deaktiviert werden.
- Falls dies nicht möglich ist, SOLLTE der Zugriff soweit wie möglich eingeschränkt werden.
- Folgendes SOLLTE bei der Konfiguration von Webanwendungen und Webservices umgesetzt werden:
    - Deaktivieren nicht benötigter HTTP-Methoden,
    - Konfigurieren der Zeichenkodierung,
    - Vermeiden von sicherheitsrelevanten Informationen in Fehlermeldungen und Antworten,
    - Speichern von Konfigurationsdateien außerhalb des Web-Root-Verzeichnisses sowie
    - Festlegen von Grenzwerten für Zugriffsversuche.

## APP.3.1.A13 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.3.1.A15 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.3.1.A17 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.3.1.A18 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.3.1.A21 Sichere HTTP-Konfiguration bei Webanwendungen (S)

- Zum Schutz vor Clickjacking, Cross-Site-Scripting und anderen Angriffen SOLLTE der IT-Betrieb geeignete HTTPResponse-Header setzen.
- Dazu SOLLTEN mindestens die folgenden HTTP-Header verwendet werden:
    - Content-Security-Policy,
    - Strict-Transport-Security,
    - Content-Type,
    - X-Content-Type-Options sowie
    - Cache-Control.
- Die verwendeten HTTP-Header SOLLTEN so restriktiv wie möglich sein.
- Cookies SOLLTEN grundsätzlich mit den Attributen secure, SameSite und httponly gesetzt werden.

## APP.3.1.A22 Penetrationstest und Revision (S)

- Webanwendungen und Webservices SOLLTEN regelmäßig auf Sicherheitsprobleme hin überprüft werden.
- Insbesondere SOLLTEN regelmäßig Revisionen durchgeführt werden.
- Die Ergebnisse SOLLTEN nachvollziehbar dokumentiert, ausreichend geschützt und vertraulich behandelt werden.
- Abweichungen SOLLTE nachgegangen werden.
- Die Ergebnisse SOLLTEN dem ISB vorgelegt werden.

## APP.3.1.A23 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.3.1.A20 Einsatz von Web Application Firewalls (H)

- Institutionen SOLLTEN Web Application Firewalls (WAF) einsetzen.
- Die Konfiguration der eingesetzten WAF SOLLTE auf die zu schützende Webanwendung oder den Webservice angepasst werden.
- Nach jedem Update der Webanwendung oder des Webservices SOLLTE die Konfiguration der WAF geprüft werden.

## APP.3.1.A24 ENTFALLEN (H)

- Diese Anforderung ist entfallen.

## APP.3.1.A25 ENTFALLEN (H)

- Diese Anforderung ist entfallen.


