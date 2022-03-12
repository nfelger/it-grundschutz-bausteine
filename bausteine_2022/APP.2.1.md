# APP.2.1: Allgemeiner Verzeichnisdienst

## APP.2.1.A1 Erstellung einer Sicherheitsrichtlinie für Verzeichnisdienste (B)

- Es MUSS eine Sicherheitsrichtlinie für den Verzeichnisdienst erstellt werden.
- Diese SOLLTE mit dem übergreifenden Sicherheitskonzept der gesamten Institution abgestimmt sein.

## APP.2.1.A2 Planung des Einsatzes von Verzeichnisdiensten [Datenschutzbeauftragter, Fachverantwortliche] (B)

- Der Einsatz von Verzeichnisdiensten MUSS sorgfältig geplant werden.
- Die konkrete Nutzung des Verzeichnisdienstes MUSS festgelegt werden.
- Es MUSS sichergestellt sein, dass der Verzeichnisdienst und alle ihn verwendenden Anwendungen kompatibel sind.
- Zudem MUSS ein Modell aus Objektklassen und Attributtypen entwickelt werden,das den Ansprüchen der vorgesehenen Nutzungsarten genügt.
- Bei der Planung des Verzeichnisdienstes MÜSSEN Personalvertretung und Datenschutzbeauftragter beteiligt werden.
- Es MUSS ein bedarfsgerechtes Berechtigungskonzept zum Verzeichnisdienst entworfen werden.
- Generell SOLLTE die geplante Verzeichnisdienststruktur vollständig dokumentiert werden.
- Maßnahmen SOLLTEN geplant werden, die es unterbinden, aus dem Verzeichnisdienst unbefugt Daten sammeln zu können.

## APP.2.1.A3 Einrichtung von Zugriffsberechtigungen auf Verzeichnisdienste [Fachverantwortliche] (B)

- Die administrativen Aufgaben für die Administration des Verzeichnisdienstes selbst sowie für die eigentliche Verwaltung der Daten MÜSSEN strikt getrennt werden.
- Die administrativen Tätigkeiten SOLLTEN so delegiert werden, dass sie sich möglichst nicht überschneiden.
- Alle administrativen Aufgabenbereiche und Berechtigungen SOLLTEN ausreichend dokumentiert werden.
- Die Zugriffsrechte der Benutzer- und Administratorengruppen MÜSSEN anhand der erstellten Sicherheitsrichtlinie konfiguriert und umgesetzt werden.
- Bei einer eventuellen Zusammenführung mehrerer Verzeichnisdienstbäume MÜSSEN die daraus resultierenden effektiven Rechte kontrolliert werden.

## APP.2.1.A4 Sichere Installation von Verzeichnisdiensten (B)

- Es MUSS ein Konzept für die Installation erstellt werden, nach dem Administrations- und Zugriffsberechtigungen bereits bei der Installation des Verzeichnisdienstes konfiguriert werden.

## APP.2.1.A5 Sichere Konfiguration und Konfigurationsänderungen von Verzeichnisdiensten (B)

- Der Verzeichnisdienst MUSS sicher konfiguriert werden.
- Für die sichere Konfiguration einer Verzeichnisdienste-Infrastruktur MÜSSEN neben dem Server auch die Clients (IT-Systeme und Programme) einbezogen werden.
- Wird die Konfiguration der vernetzten IT-Systeme geändert, SOLLTEN die Benutzer rechtzeitig über Wartungsarbeiten informiert werden.
- Vor den Konfigurationsänderungen SOLLTEN von allen betroffenen Dateien und Verzeichnissen Datensicherungen angefertigt werden.

## APP.2.1.A6 Sicherer Betrieb von Verzeichnisdiensten (B)

- Die Sicherheit des Verzeichnisdienstes MUSS im Betrieb permanent aufrechterhalten werden.
- Alle den Betrieb eines Verzeichnisdienst-Systems betreffenden Richtlinien, Regelungen und Prozesse SOLLTEN dokumentiert werden.
- Die Arbeitsplätze von Verzeichnisdienstadministratoren MÜSSEN ausreichend gesichert sein.
- Der Zugriff auf alle Administrationswerkzeuge MUSS für normale Benutzer unterbunden werden.

## APP.2.1.A7 Erstellung eines Sicherheitskonzepts für den Einsatz von Verzeichnisdiensten (S)

- Durch das Sicherheitskonzept für Verzeichnisdienste SOLLTEN sämtliche sicherheitsbezogenen Themenbereiche eines Verzeichnisdienstes geregelt werden.
- Die daraus entwickelten Sicherheitsrichtlinien SOLLTEN schriftlich festgehalten und den Benutzern des Verzeichnisdienstes mitgeteilt werden.

## APP.2.1.A8 Planung einer Partitionierung und Replikation im Verzeichnisdienst (S)

- Bei einer Partitionierung SOLLTE auf die Verfügbarkeit und den Schutzbedarf des Verzeichnisdienstes geachtet werden.
- Die Partitionierung des Verzeichnisdienstes SOLLTE schriftlich so dokumentiert werden, dass sie manuell wieder rekonstruiert werden kann.
- Um die Replikationen zeitgerecht ausführen zu können, SOLLTE eine ausreichende Bandbreite sichergestellt werden.

## APP.2.1.A9 Geeignete Auswahl von Komponenten für Verzeichnisdienste [Fachverantwortliche] (S)

- Für den Einsatz eines Verzeichnisdienstes SOLLTEN geeignete Komponenten identifiziert werden.
- Es SOLLTE ein Kriterienkatalog erstellt werden, nach dem die Komponenten für den Verzeichnisdienst ausgewählt und beschafft werden.
- Im Rahmen der Planung und Konzeption des Verzeichnisdienstes SOLLTEN passend zum Einsatzzweck Anforderungen an dessen Sicherheit formuliert werden.

## APP.2.1.A10 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.2.1.A11 Einrichtung des Zugriffs auf Verzeichnisdienste (S)

- Der Zugriff auf den Verzeichnisdienst SOLLTE entsprechend der Sicherheitsrichtlinie konfiguriert werden.
- Wird der Verzeichnisdienst als Server im Internet eingesetzt, SOLLTE er entsprechend durch ein Sicherheitsgateway geschützt werden.
- Sollen anonymen Benutzern auf einzelne Teilbereiche des Verzeichnisbaums weitergehende Zugriffe eingeräumt werden, so SOLLTE ein gesondertes Benutzerkonto, ein sogenannter Proxy-User, für den anonymen Zugriff eingerichtet werden.
- Die Zugriffsrechte für diesen Proxy-User SOLLTEN hinreichend restriktiv vergeben werden.
- Sie SOLLTEN zudem wieder komplett entzogen werden, wenn der Account nicht mehr gebraucht wird.
- Damit nicht versehentlich schutzbedürftige Informationen herausgegeben werden, SOLLTE die Suchfunktion des Verzeichnisdienstes dem Einsatzzweck angemessen eingeschränkt werden.

## APP.2.1.A12 Überwachung von Verzeichnisdiensten (S)

- Verzeichnisdienste SOLLTEN gemeinsam mit dem Server beobachtet und protokolliert werden, auf dem sie betrieben werden.

## APP.2.1.A13 Absicherung der Kommunikation mit Verzeichnisdiensten (S)

- Die gesamte Kommunikation mit dem Verzeichnisdienst SOLLTE über SSL/TLS verschlüsselt werden.
- Der Kommunikationsendpunkt des Verzeichnisdienst-Servers SOLLTE aus dem Internet nicht erreichbar sein.
- Der Datenaustausch zwischen Client und Verzeichnisdienst-Server SOLLTE abgesichert werden.
- Es SOLLTE definiert werden, auf welche Daten zugegriffen werden darf.
- Im Falle einer serviceorientierten Architektur (SOA) SOLLTEN zum Schutz von Service-Einträgen in einer Service-Registry sämtliche Anfragen an die Registratur daraufhin überprüft werden, ob der Benutzer gültig ist.

## APP.2.1.A14 Geregelte Außerbetriebnahme eines Verzeichnisdienstes [Fachverantwortliche] (S)

- Bei einer Außerbetriebnahme des Verzeichnisdienstes SOLLTE sichergestellt sein, dass weiterhin benötigte Rechte bzw. Informationen in ausreichendem Umfang zur Verfügung stehen.
- Alle anderen Rechte und Informationen SOLLTEN gelöscht werden.
- Zudem SOLLTEN die Benutzer darüber informiert werden, wenn ein Verzeichnisdienst außer Betrieb genommen wird.
- Bei der Außerbetriebnahme einzelner Partitionen eines Verzeichnisdienstes SOLLTE darauf geachtet werden, dass dadurch andere Partitionen nicht beeinträchtigt werden.

## APP.2.1.A15 Migration von Verzeichnisdiensten (S)

- Bei einer geplanten Migration von Verzeichnisdiensten SOLLTE vorab ein Migrationskonzept erstellt werden.
- Die Schema-Änderungen, die am Verzeichnisdienst vorgenommen wurden, SOLLTEN dokumentiert werden.
- Weitreichende Berechtigungen, die dazu verwendet wurden, die Migration des Verzeichnisdienstes durchzuführen, SOLLTEN wieder zurückgesetzt werden.
- Die Zugriffsrechte für Verzeichnisdienst-Objekte bei Systemen, die von Vorgängerversionen aktualisiert bzw. von anderen Verzeichnissystemen übernommen wurden, SOLLTEN aktualisiert werden.

## APP.2.1.A16 Erstellung eines Notfallplans für den Ausfall eines Verzeichnisdienstes (H)

- Im Rahmen der Notfallvorsorge SOLLTE es eine bedarfsgerechte Notfallplanung für Verzeichnisdienste geben.
- Für den Ausfall wichtiger Verzeichnisdienst-Systeme SOLLTEN Notfallpläne vorliegen.
- Alle Notfall-Prozeduren für die gesamte Systemkonfiguration der Verzeichnisdienst-Komponenten SOLLTEN dokumentiert werden.


