# CON.8: Software-Entwicklung

## CON.8.A2 Auswahl eines Vorgehensmodells (B)

- Ein geeignetes Vorgehensmodell zur Software-Entwicklung MUSS festgelegt werden.
- Anhand des gewählten Vorgehensmodells MUSS ein Ablaufplan für die Software-Entwicklung erstellt werden.
- Die Sicherheitsanforderungen des Auftraggebers an die Vorgehensweise MÜSSEN im Vorgehensmodell integriert werden.
- Das ausgewählte Vorgehensmodell, einschließlich der festgelegten Sicherheitsanforderungen, MUSS eingehalten werden.
- Das Personal SOLLTE in der Methodik des gewählten Vorgehensmodells geschult sein.

## CON.8.A3 Auswahl einer Entwicklungsumgebung (B)

- Eine Liste der erforderlichen und optionalen Auswahlkriterien für eine Entwicklungsumgebung MUSS vom Fachverantwortlichen für die Software-Entwicklung erstellt werden.
- Die Entwicklungsumgebung MUSS anhand der vorgegebenen Kriterien ausgewählt werden.

## CON.8.A4 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## CON.8.A5 Sicheres Systemdesign (B)

- Folgende Grundregeln des sicheren Systemdesigns MÜSSEN in der zu entwickelnden Software berücksichtigt werden:
    - Grundsätzlich MÜSSEN alle Eingabedaten vor der Weiterverarbeitung geprüft und validiert werden.
    - Bei Client-Server-Anwendungen MÜSSEN die Daten grundsätzlich auf dem Server validiert werden.
    - Die Standardeinstellungen der Software MÜSSEN derart voreingestellt sein, dass ein sicherer Betrieb der Software ermöglicht wird.
    - Bei Fehlern oder Ausfällen von Komponenten des Systems DÜRFEN NICHT schützenswerte Informationen preisgegeben werden.
    - Die Software MUSS mit möglichst geringen Privilegien ausgeführt werden können.
    - Schützenswerte Daten MÜSSEN entsprechend der Vorgaben des Kryptokonzepts verschlüsselt übertragen und gespeichert werden.
    - Zur Benutzer-Authentisierung und Authentifizierung MÜSSEN vertrauenswürdige Mechanismen verwendet werden, die den Sicherheitsanforderungen an die Anwendung entsprechen.
    - Falls zur Authentifizierung Passwörter gespeichert werden, MÜSSEN diese mit einem sicheren Hashverfahren gespeichert werden.
    - Sicherheitsrelevante Ereignisse MÜSSEN in der Art protokolliert werden, dass sie im Nachgang ausgewertet werden können.
    - Informationen, die für den Produktivbetrieb nicht relevant sind (z. B. Kommentare mit Zugangsdaten für die Entwicklungsumgebung), SOLLTEN in ausgeliefertem Programmcode und ausgelieferten Konfigurationsdateien entfernt werden.
- Das Systemdesign MUSS dokumentiert werden.
- Es MUSS überprüft werden, ob alle Sicherheitsanforderungen an das Systemdesign erfüllt wurden.

## CON.8.A6 Verwendung von externen Bibliotheken aus vertrauenswürdigen Quellen (B)

- Wird im Rahmen des Entwicklungs- und Implementierungsprozesses auf externe Bibliotheken zurückgegriffen, MÜSSEN diese aus vertrauenswürdigen Quellen bezogen werden.
- Bevor externe Bibliotheken verwendet werden, MUSS deren Integrität sichergestellt werden.

## CON.8.A7 Durchführung von entwicklungsbegleitenden Software-Tests [Tester, Entwickler] (B)

- Schon bevor die Software im Freigabeprozess getestet und freigegeben wird, MÜSSEN entwicklungsbegleitende Software-Tests durchgeführt und der Quellcode auf Fehler gesichtet werden.
- Hierbei SOLLTEN bereits die Fachverantwortlichen des Auftraggebers oder der beauftragenden Fachabteilung beteiligt werden.
- Die entwicklungsbegleitenden Tests MÜSSEN die funktionalen und nichtfunktionalen Anforderungen der Software umfassen.
- Die Software-Tests MÜSSEN dabei auch Negativtests abdecken.
- Zusätzlich MÜSSEN auch alle kritischen Grenzwerte der Eingabe sowie der Datentypen überprüft werden.
- Testdaten SOLLTEN dafür sorgfältig ausgewählt und geschützt werden.
- Darüber hinaus SOLLTE eine automatische statische Code-Analyse durchgeführt werden.
- Die Software MUSS in einer Test- und Entwicklungsumgebung getestet werden, die getrennt von der Produktionsumgebung ist.
- Außerdem MUSS getestet werden, ob die Systemvoraussetzungen für die vorgesehene Software ausreichend dimensioniert sind.

## CON.8.A8 Bereitstellung von Patches, Updates und Änderungen [Entwickler] (B)

- Es MUSS sichergestellt sein, dass sicherheitskritische Patches und Updates für die entwickelte Software zeitnah durch die Entwickler bereitgestellt werden.
- Werden für verwendete externe Bibliotheken sicherheitskritische Updates bereitgestellt, dann MÜSSEN die Entwickler ihre Software hierauf anpassen und ihrerseits entsprechende Patches und Updates zur Verfügung stellen.
- Für die Installations-, Update- oder Patchdateien MÜSSEN vom Entwickler Checksummen oder digitale Signaturen bereitgestellt werden.

## CON.8.A9 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## CON.8.A10 Versionsverwaltung des Quellcodes [Entwickler] (B)

- Der Quellcode des Entwicklungsprojekts MUSS über eine geeignete Versionsverwaltung verwaltet werden.
- Die Institution MUSS den Zugriff auf die Versionsverwaltung regeln und festlegen, wann Änderungen am Quellcode durch die Entwickler als eigene Version in der Versionsverwaltung gespeichert werden sollen.
- Es MUSS sichergestellt sein, dass durch die Versionsverwaltung alle Änderungen am Quellcode nachvollzogen und rückgängig gemacht werden können.
- Die Versionsverwaltung MUSS in dem Datensicherungskonzept berücksichtigt werden.
- Die Versionsverwaltung DARF NICHT ohne Datensicherung erfolgen.

## CON.8.A20 Überprüfung von externen Komponenten (B)

- Unbekannte externe Komponenten (bzw. Programm-Bibliotheken), deren Sicherheit nicht durch etablierte und anerkannte Peer-Reviews oder vergleichbares sichergestellt werden kann, MÜSSEN auf Schwachstellen überprüft werden.
- Alle externen Komponenten MÜSSEN auf potentielle Konflikte überprüft werden.
- Die Integrität von externen Komponenten MUSS durch Prüfsummen oder kryptographische Zertifikate überprüft werden.
- Darüber hinaus SOLLTEN keine veralteten Versionen von externen Komponenten in aktuellen Entwicklungsprojekten verwendet werden.

## CON.8.A1 Definition von Rollen und Zuständigkeiten [Zentrale Verwaltung] (S)

- Für den Software-Entwicklungsprozess SOLLTE ein Gesamtzuständiger benannt werden.
- Außerdem SOLLTEN die Rollen und Zuständigkeiten für alle Aktivitäten im Rahmen der Software-Entwicklung festgelegt werden.
- Die Rollen SOLLTEN dabei fachlich die nachfolgenden Themen abdecken:
    - Requirements-Engineering (Anforderungsmanagement) und Änderungsmanagement,
    - Software-Entwurf und -Architektur,
    - Informationssicherheit in der Software-Entwicklung,
    - Software-Implementierung in dem für das Entwicklungsvorhaben relevanten Bereichen, sowie
    - Software-Tests.
- Für jedes Entwicklungsvorhaben SOLLTE ein Zuständiger für die Informationssicherheit benannt werden.

## CON.8.A11 Erstellung einer Richtlinie für die Software-Entwicklung (S)

- Es SOLLTE eine Richtlinie für die Software-Entwicklung erstellt und aktuell gehalten werden.
- Die Richtlinie SOLLTE neben Namenskonventionen auch Vorgaben zu Elementen beinhalten, die verwendet bzw. nicht verwendet werden dürfen.
- Die relevanten Anforderungen aus diesem Baustein SOLLTEN in die Richtlinie aufgenommen werden.
- Die Richtlinie SOLLTE für die Entwickler verbindlich sein.

## CON.8.A12 Ausführliche Dokumentation (S)

- Es SOLLTEN ausreichende Projekt-, Funktions- und Schnittstellendokumentationen erstellt und aktuell gehalten werden.
- Die Betriebsdokumentation SOLLTE konkrete Sicherheitshinweise für die Installation und Konfiguration für Administratoren, sowie für die Benutzung des Produktes beinhalten.
- Die Software-Entwicklung SOLLTE so dokumentiert sein, dass ein Fachexperte mithilfe der Dokumentation den Programm-Code nachvollziehen und weiterentwickeln kann.
- Die Dokumentation SOLLTE dabei auch die Software-Architektur und Bedrohungsmodellierung umfassen.
- Die Aspekte zur Dokumentation SOLLTEN im Vorgehensmodell zur Software-Entwicklung berücksichtigt werden.

## CON.8.A13 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## CON.8.A14 Schulung des Entwicklungsteams zur Informationssicherheit (S)

- Die Entwickler und die übrigen Mitglieder des Entwicklungsteams SOLLTEN zu generellen Informationssicherheitsaspekten und zu den jeweils speziell für sie relevanten Aspekten geschult sein:
    - Anforderungsanalyse,
    - Projektmanagement allgemein sowie speziell bei der Software-Entwicklung,
    - Risikomanagement bzw. Bedrohungsmodellierung in der Software-Entwicklung,
    - Qualitätsmanagement und Qualitätssicherung,
    - Modelle und Methoden für die Software-Entwicklung,
    - Software-Architektur,
    - Software-Tests,
    - Änderungsmanagement sowie
    - Informationssicherheit, Sicherheitsvorgaben in der Institution und Sicherheitsaspekte in speziellen Bereichen.

## CON.8.A15 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## CON.8.A16 Geeignete Steuerung der Software-Entwicklung (S)

- Bei einer Software-Entwicklung SOLLTE ein geeignetes Steuerungs- bzw. Projektmanagementmodell auf Basis des ausgewählten Vorgehensmodells verwendet werden.
- Das Steuerungs- bzw. Projektmanagementmodell SOLLTE in die Richtlinie zur Software Entwicklung integriert werden.
- Dabei SOLLTEN insbesondere die benötigten Qualifikationen beim Personal und die Abdeckung aller relevanten Phasen während des Lebenszyklus der Software berücksichtigt werden.
- Für das Vorgehensmodell SOLLTE ein geeignetes Risikomanagement festgelegt werden.
- Außerdem SOLLTEN geeignete Qualitätsziele für das Entwicklungsprojekt definiert werden.

## CON.8.A21 Bedrohungsmodellierung (S)

- In der Entwurfsphase der Software-Entwicklung SOLLTE eine Bedrohungsmodellierung durchgeführt werden.
- Hierzu SOLLTEN auf Basis des Sicherheitsprofils, des Anforderungskatalogs und der geplanten Einsatzumgebung bzw. Einsatzszenarios potentielle Bedrohungen identifiziert werden.
- Die Bedrohungen SOLLTEN hinsichtlich ihrer Eintrittswahrscheinlichkeit und Auswirkung bewertet werden.

## CON.8.A22 Sicherer Software-Entwurf (S)

- Der Software-Entwurf SOLLTE den Anforderungskatalog, das Sicherheitsprofil und die Ergebnisse der Bedrohungsmodellierung berücksichtigen.
- Im Rahmen des sicheren Software-Entwurfs SOLLTE eine sichere Software-Architektur entwickelt werden, auf deren Grundlage der Quellcode der Anwendung zu entwickeln ist.
- Hierbei SOLLTEN möglichst zukünftige Standards und Angriffstechniken berücksichtigt werden, damit die zu entwickelnde Software auch zukünftig leicht gewartet werden kann.

## CON.8.A17 Auswahl vertrauenswürdiger Entwicklungswerkzeuge (H)

- Zur Entwicklung der Software SOLLTEN nur Werkzeuge mit nachgewiesenen Sicherheitseigenschaften verwendet werden.
- An die Hersteller von Hardware oder Software SOLLTEN hinreichende Anforderungen zur Sicherheit ihrer Werkzeuge gestellt werden.

## CON.8.A18 Regelmäßige Sicherheitsaudits für die Entwicklungsumgebung (H)

- Es SOLLTEN regelmäßige Sicherheitsaudits der Software-Entwicklungsumgebung und der Software-Testumgebung durchgeführt werden.

## CON.8.A19 Regelmäßige Integritätsprüfung der Entwicklungsumgebung [IT-Betrieb] (H)

- Die Integrität der Entwicklungsumgebung SOLLTE regelmäßig mit kryptographischen Mechanismen entsprechend dem Stand der Technik geprüft werden.
- Die Prüfsummendateien und das Prüfprogramm selbst SOLLTEN ausreichend vor Manipulationen geschützt sein.
- Wichtige Hinweise auf einen Integritätsverlust SOLLTEN nicht in einer Fülle irrelevanter Warnmeldungen (false positives) untergehen.


