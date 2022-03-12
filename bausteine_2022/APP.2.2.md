# APP.2.2: Active Directory

## APP.2.2.A1 Planung des Active Directory [Fachverantwortliche] (B)

- Es MUSS ein geeignetes, möglichst hohes Domain Functional Level gewählt werden.
- Die Begründung SOLLTE geeignet dokumentiert werden.
- Ein bedarfsgerechtes Active-Directory-Berechtigungskonzept MUSS entworfen werden.
- Administrative Delegationen MÜSSEN mit restriktiven und bedarfsgerechten Berechtigungen ausgestattet sein.
- Die geplante Active-Directory-Struktur einschließlich etwaiger Schema-Änderungen SOLLTE nachvollziehbar dokumentiert sein.

## APP.2.2.A2 Planung der Active-Directory-Administration [Fachverantwortliche] (B)

- In großen Domänen MÜSSEN die administrativen Benutzer bezüglich Diensteverwaltung und Datenverwaltung des Active Directory aufgeteilt werden.
- Zusätzlich MÜSSEN hier die administrativen Aufgaben im Active Directory nach einem Delegationsmodell überschneidungsfrei verteilt sein.

## APP.2.2.A3 Planung der Gruppenrichtlinien unter Windows (B)

- Es MUSS ein Konzept zur Einrichtung von Gruppenrichtlinien vorliegen.
- Mehrfachüberdeckungen MÜSSEN beim Gruppenrichtlinienkonzept möglichst vermieden werden.
- In der Dokumentation des Gruppenrichtlinienkonzepts MÜSSEN Ausnahmeregelungen erkannt werden können.
- Alle Gruppenrichtlinienobjekte MÜSSEN durch restriktive Zugriffsrechte geschützt sein.
- Für die Parameter in allen Gruppenrichtlinienobjekten MÜSSEN sichere Vorgaben festgelegt sein.

## APP.2.2.A4 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.2.2.A5 Härtung des Active Directory (B)

- Built-in-Accounts MÜSSEN mit komplexen Passwörtern versehen werden.
- Sie DÜRFEN NUR als Notfallkonten dienen.
- Privilegierte Accounts MÜSSEN Mitglieder der Gruppe „Protected Users“ sein.
- Für Dienstkonten MÜSSEN (Group) Managed Service Accounts verwendet werden.
- Für alle Domänen-Controller MÜSSEN restriktive Zugriffsrechte auf Betriebssystemebene vergeben sein.
- Der ActiveDirectory-Restore-Modus MUSS durch ein geeignetes Passwort geschützt sein.
- Arbeiten in diesem Modus SOLLTEN nur erfolgen, wenn das Vier-Augen-Prinzip eingehalten wird.
- Ein Abbild des Domänencontrollers SOLLTE regelmäßig erstellt werden.
- Die Berechtigungen für die Gruppe „Jeder“ MUSS beschränkt werden.
- Der Domänencontroller MUSS gegen unautorisierte Neustarts geschützt sein.
- Die Richtlinien für Domänen und Domänencontroller MÜSSEN sichere Einstellungen für Kennworte, Kontensperrung, Kerberos-Authentisierung, Benutzerrechte und Überwachung umfassen.
- Es MUSS eine ausreichende Größe für das Sicherheitsprotokoll des Domänen-Controllers eingestellt sein.
- Bei externen Vertrauensstellungen zu anderen Domänen MÜSSEN die Autorisierungsdaten der Benutzer gefiltert und anonymisiert werden.

## APP.2.2.A6 Aufrechterhaltung der Betriebssicherheit von Active Directory (B)

- Alle Vertrauensbeziehungen im AD MÜSSEN regelmäßig evaluiert werden.
- Die Gruppe der Domänenadministratoren MUSS leer oder möglichst klein sein.
- Nicht mehr verwendete Konten MÜSSEN im AD deaktiviert werden.
- Sie SOLLTEN nach Ablauf einer angemessenen Aufbewahrungsfrist gelöscht werden.
- Alle notwendigen Parameter des Active Directory SOLLTEN aktuell und nachvollziehbar festgehalten werden.

## APP.2.2.A7 Umsetzung sicherer Verwaltungsmethoden für Active Directory [Fachverantwortliche] (B)

- Jeder Account MUSS sich eindeutig einem Mitarbeiter zuordnen lassen.
- Die Anzahl der Dienste-Administratoren und der Daten-Administratoren des Active Directory MUSS auf das notwendige Minimum vertrauenswürdiger Personen reduziert sein.
- Das Standardkonto „Administrator“ SOLLTE umbenannt werden.
- Es SOLLTE ein unprivilegiertes Konto mit dem Namen „Administrator“ erstellt werden.
- Es MUSS sichergestellt sein, dass die Dienste-Administratorkonten ausschließlich von Mitgliedern der Dienste-Administratorgruppe verwaltet werden.
- Die Gruppe „Kontenoperatoren“ SOLLTE leer sein.
- Administratoren SOLLTEN der Gruppe „Schema-Admins“ nur temporär für den Zeitraum der Schema-Änderungen zugewiesen werden.
- Für die Gruppen „Organisations-Admins“ und „Domänen-Admins“ zur Administration der Stammdomäne SOLLTE ein Vier-Augen-Prinzip etabliert sein.
- Es MUSS sichergestellt sein, dass die Gruppen „Administratoren“ bzw. „Domänenadministratoren“ auch die Besitzer des Domänenstammobjektes der jeweiligen Domäne sind.
- Der Einsatz von domänenlokalen Gruppen für die Steuerung der Leseberechtigung für Objektattribute SOLLTE vermieden werden.
- Der Papierkorb des AD SOLLTE aktiviert werden.
- In großen Institutionen SOLLTE mit einer Enterprise-Identity-Management-Lösung sichergestellt werden, dass die Rechte aller Anwender den definierten Vorgaben entsprechen.

## APP.2.2.A8 Konfiguration des „Sicheren Kanals“ unter Windows (S)

- Der „Sichere Kanal“ unter Windows SOLLTE entsprechend den Sicherheitsanforderungen und den lokalen Gegebenheiten konfiguriert sein.
- Dabei SOLLTEN alle relevanten Gruppenrichtlinienparameter berücksichtigt werden.

## APP.2.2.A9 Schutz der Authentisierung beim Einsatz von Active Directory (S)

- In der Umgebung des Active Directory SOLLTE konsequent das Authentisierungsprotokoll Kerberos eingesetzt werden.
- Wenn aus Kompatibilitätsgründen übergangsweise NTLMv2 eingesetzt wird, SOLLTE die Migration auf Kerberos geplant und terminiert werden.
- Die LM-Authentisierung SOLLTE deaktiviert sein.
- Der SMB-Datenverkehr SOLLTE signiert sein.
- Anonyme Zugriffe auf Domänencontroller SOLLTEN unterbunden sein.

## APP.2.2.A10 Sicherer Einsatz von DNS für Active Directory (S)

- Integrierte DNS-Zonen bzw. die sichere dynamische Aktualisierung der DNS-Daten SOLLTEN verwendet werden.
- Der Zugriff auf die Konfigurationsdaten des DNS-Servers SOLLTE nur von administrativen Konten erlaubt sein.
- Der DNS-Cache auf den DNS-Servern SOLLTE vor unberechtigten Änderungen geschützt sein.
- Der Zugriff auf den DNSDienst der Domänen-Controller SOLLTE auf das notwendige Maß beschränkt sein.
- Die Netzaktivitäten in Bezug auf DNS-Anfragen SOLLTEN überwacht werden.
- Der Zugriff auf die DNS-Daten im Active Directory SOLLTE mittels ACLs auf Administratoren beschränkt sein.
- Sekundäre DNS-Zonen SOLLTEN vermieden werden.
- Zumindest SOLLTE die Zonen-Datei vor unbefugtem Zugriff geschützt werden.
- Wird IPsec eingesetzt, um die DNS-Kommunikation abzusichern, SOLLTE ein ausreichender Datendurchsatz im Netz gewährleistet sein.

## APP.2.2.A11 Überwachung der Active-Directory-Infrastruktur (S)

- Änderungen auf Domänen-Ebene und an der Gesamtstruktur des Active Directory SOLLTEN überwacht, protokolliert und ausgewertet werden.

## APP.2.2.A12 Datensicherung für Domänen-Controller (S)

- Es SOLLTE eine Datensicherungs- und Wiederherstellungsrichtlinie für Domänen-Controller existieren.
- Die eingesetzte Sicherungssoftware SOLLTE explizit vom Hersteller für die Datensicherung von Domänen-Controllern freigegeben sein.
- Für die Domänen-Controller SOLLTE ein separates Datensicherungskonto mit Dienste-Administratorenrechten eingerichtet sein.
- Die Anzahl der Mitglieder der Gruppe „Sicherungs-Operatoren“ SOLLTE auf das notwendige Maß begrenzt sein.
- Der Zugriff auf das AdminSDHolder-Objekt SOLLTE zum Schutz der Berechtigungen besonders geschützt sein.
- Die Daten der Domänen-Controller SOLLTEN in regelmäßigen Abständen gesichert werden.
- Dabei SOLLTE ein Verfahren eingesetzt werden, das veraltete Objekte weitgehend vermeidet.

## APP.2.2.A13 ENTFALLEN (H)

- Diese Anforderung ist entfallen.

## APP.2.2.A14 Verwendung dedizierter privilegierter Administrationssysteme (H)

- Die Administration des Active Directory SOLLTE auf dedizierte Administrationssysteme eingeschränkt werden.
- Diese SOLLTEN durch die eingeschränkte Aufgabenstellung besonders stark gehärtet sein.

## APP.2.2.A15 Trennung von Administrations- und Produktionsumgebung (H)

- Besonders kritische Systeme wie Domaincontroller und Systeme zur Administration der Domain SOLLTEN in einen eigenen Forest ausgegliedert werden, der einen einseitigen Trust in Richtung des Produktions-Forests besitzt.


