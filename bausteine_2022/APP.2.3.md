# APP.2.3: OpenLDAP

## APP.2.3.A1 Planung und Auswahl von Backends und Overlays für OpenLDAP (B)

- Der Einsatz von OpenLDAP in einer Institution MUSS sorgfältig geplant werden.
- Soll OpenLDAP gemeinsam mit anderen Anwendungen verwendet werden, so MÜSSEN die Planung, Konfiguration und Installation der Anwendungen mit OpenLDAP aufeinander abgestimmt werden.
- Für die zur Datenhaltung verwendete Datenbank MUSS sichergestellt werden, dass die verwendete Version kompatibel ist.
- Backends und Overlays für OpenLDAP MÜSSEN restriktiv selektiert werden.
- Dazu MUSS sichergestellt werden, dass die OpenLDAP-Overlays in der korrekten Reihenfolge eingesetzt werden.
- Bei der Planung von OpenLDAP MÜSSEN die auszuwählenden und unterstützten Client-Anwendungen berücksichtigt werden.

## APP.2.3.A2 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.2.3.A3 Sichere Konfiguration von OpenLDAP (B)

- Für die sichere Konfiguration von OpenLDAP MUSS der slapd-Server korrekt konfiguriert werden.
- Es MÜSSEN auch die verwendeten Client-Anwendungen sicher konfiguriert werden.
- Bei der Konfiguration von OpenLDAP MUSS darauf geachtet werden, dass im Betriebssystem die Berechtigungen korrekt gesetzt sind.
- Die Vorgabewerte aller relevanten Konfigurationsdirektiven von OpenLDAP MÜSSEN geprüft und gegebenenfalls angepasst werden.
- Die Backends und Overlays von OpenLDAP MÜSSEN in die Konfiguration einbezogen werden.
- Für die Suche innerhalb von OpenLDAP MÜSSEN angemessene Zeit- und Größenbeschränkungen festgelegt werden.
- Die Konfiguration am slapd-Server MUSS nach jeder Änderung geprüft werden.

## APP.2.3.A4 Konfiguration der durch OpenLDAP verwendeten Datenbank (B)

- Die Zugriffsrechte für neu angelegte Datenbankdateien MÜSSEN auf die Benutzerkennung beschränkt werden, in deren Kontext der slapd-Server betrieben wird.
- Die Standard-Einstellungen der von OpenLDAP genutzten Datenbank MÜSSEN angepasst werden.

## APP.2.3.A5 Sichere Vergabe von Zugriffsrechten auf dem OpenLDAP (B)

- Die in OpenLDAP geführten globalen und datenbankspezifischen Zugriffskontrolllisten (Access Control Lists) MÜSSEN beim Einsatz von OpenLDAP korrekt berücksichtigt werden.
- Datenbank-Direktiven MÜSSEN Vorrang vor globalen Direktiven haben.

## APP.2.3.A6 Sichere Authentisierung gegenüber OpenLDAP (B)

- Wenn der Verzeichnisdienst zwischen verschiedenen Benutzern unterscheiden soll, MÜSSEN sich diese geeignet authentisieren.
- Die Authentisierung zwischen dem slapd-Server und den Kommunikationspartnern MUSS verschlüsselt werden.
- Es DÜRFEN NUR die Hashwerte von Passwörtern auf den Clients und Servern abgespeichert werden.
- Es MUSS ein geeigneter Hashing-Algorithmus verwendet werden.

## APP.2.3.A7 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.2.3.A8 Einschränkungen von Attributen bei OpenLDAP (S)

- Anhand von Overlays SOLLTEN die Attribute in OpenLDAP eingeschränkt werden.
- OpenLDAP SOLLTE so angepasst werden, dass Werte im Verzeichnisdienst nur einem bestimmten regulären Ausdruck entsprechen.
- Zudem SOLLTE mit Hilfe von Overlays sichergestellt werden, das ausgesuchte Werte nur einmal im Verzeichnisbaum vorhanden sind.
- Solche Restriktionen SOLLTEN ausschließlich auf Nutzerdaten angewendet werden.

## APP.2.3.A9 Partitionierung und Replikation bei OpenLDAP (S)

- OpenLDAP SOLLTE in Teilbäume auf verschiedene Server aufgeteilt (partitioniert) werden.
- Dabei SOLLTEN Veränderungen an den Daten durch Replikation zwischen den Servern ausgetauscht werden.
- Der Replikationsmodus SOLLTE in Abhängigkeit von Netzverbindungen und Verfügbarkeitsanforderungen gewählt werden.

## APP.2.3.A10 Sichere Aktualisierung von OpenLDAP (S)

- Bei Updates SOLLTE darauf geachtet werden, ob die Änderungen eingesetzte Backends oder Overlays sowie Softwareabhängigkeiten betreffen.
- Setzen Administratoren eigene Skripte ein, SOLLTEN sie daraufhin überprüft werden, ob sie mit der aktualisierten Version von OpenLDAP problemlos zusammenarbeiten.
- Die Konfiguration und die Zugriffsrechte SOLLTEN nach einer Aktualisierung sorgfältig geprüft werden.

## APP.2.3.A11 Einschränkung der OpenLDAP-Laufzeitumgebung (S)

- Der slapd-Server SOLLTE auf ein Laufzeitverzeichnis eingeschränkt werden.
- Hierfür SOLLTE dieses Verzeichnis alle Konfigurationsdateien und Datenbanken beinhalten.

## APP.2.3.A12 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.2.3.A13 ENTFALLEN (S)

- Diese Anforderung ist entfallen.


