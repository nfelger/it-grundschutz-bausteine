# CON.10: Entwicklung von Webanwendungen

## CON.10.A1 Authentisierung bei Webanwendungen (B)

- Die Entwickler MÜSSEN sicherstellen, dass sich Benutzer gegenüber der Webanwendung sicher und angemessen authentisieren, bevor diese auf geschützte Funktionen oder Inhalte zugreifen können.
- Es MUSS eine angemessene Authentisierungsmethode ausgewählt werden.
- Der Auswahlprozess MUSS dokumentiert werden.
- Eine zentrale Authentisierungskomponente MUSS verwendet werden.
- Die zentrale Authentisierungskomponente SOLLTE mit etablierten Standardkomponenten (z. B. aus Frameworks oder Programmbibliotheken) umgesetzt werden.
- Falls eine Webanwendung Authentisierungsdaten auf einem Client speichert, MUSS der Benutzer explizit auf die Risiken der Funktion hingewiesen werden und zustimmen („Opt-In“).
- Die Webanwendung MUSS die Möglichkeit bieten, Grenzwerte für fehlgeschlagene Anmeldeversuche festzulegen.
- Die Webanwendung MUSS Benutzer sofort informieren, wenn ihr Passwort zurückgesetzt wurde.

## CON.10.A2 Zugriffskontrolle bei Webanwendungen (B)

- Die Entwickler MÜSSEN mittels einer Autorisierungskomponente sicherstellen, dass Benutzer ausschließlich solche Aktionen durchführen können, zu denen sie berechtigt sind.
- Jeder Zugriff auf geschützte Inhalte und Funktionen MUSS kontrolliert werden, bevor er ausgeführt wird.
- Die Autorisierungskomponente MUSS sämtliche Ressourcen und Inhalte berücksichtigen, die von der Webanwendung verwaltet werden.
- Ist die Zugriffskontrolle fehlerhaft, MÜSSEN Zugriffe abgelehnt werden.
- Es MUSS eine Zugriffskontrolle bei URL-Aufrufen und Objekt-Referenzen geben.

## CON.10.A3 Sicheres Session-Management (B)

- Die Entwickler MÜSSEN sicherstellen, dass Session-IDs geeignet geschützt werden.
- Session-IDs MÜSSEN zufällig und mit ausreichender Entropie erzeugt werden.
- Falls das Framework der Webanwendung sichere Session-IDs generieren kann, MUSS diese Funktion des Frameworks von den Entwicklern verwendet werden.
- Sicherheitsrelevante Konfigurationsmöglichkeiten des Frameworks MÜSSEN berücksichtigt werden.
- Wenn Session-IDs übertragen und von den Clients gespeichert werden, MÜSSEN sie ausreichend geschützt übertragen werden.
- Eine Webanwendung MUSS den Benutzern die Möglichkeit geben, eine bestehende Sitzung explizit zu beenden.
- Nachdem sich der Benutzer angemeldet hat, MUSS eine bereits bestehende Session-ID durch eine neue ersetzt werden.
- Sitzungen MÜSSEN eine maximale Gültigkeitsdauer besitzen (Timeout).
- Inaktive Sitzungen MÜSSEN automatisch nach einer bestimmten Zeit ungültig werden.
- Nachdem die Sitzung ungültig ist, MÜSSEN alle Sitzungsdaten ungültig und gelöscht sein.

## CON.10.A4 Kontrolliertes Einbinden von Inhalten bei Webanwendungen (B)

- Die Entwickler MÜSSEN sicherstellen, dass eine Webanwendung ausschließlich vorgesehene Daten und Inhalte einbindet und an den Benutzer ausliefert.
- Die Ziele der Weiterleitungsfunktion einer Webanwendung MÜSSEN ausreichend eingeschränkt werden, sodass Benutzer ausschließlich auf vertrauenswürdige Webseiten weitergeleitet werden.
- Verlässt ein Benutzer die Vertrauensdomäne, MUSS ihn die Webanwendung darüber informieren.

## CON.10.A5 Upload-Funktionen (B)

- Die Entwickler MÜSSEN sicherstellen, dass ein Benutzer Dateien nur im vorgegebenen Pfad speichern kann.
- Die Entwickler MÜSSEN sicherstellen, dass der Benutzer den Ablageort der Uploads nicht beeinflussen kann.
- Die Entwickler MÜSSEN Funktionen in die Webanwendung integrieren, mit denen der spätere Betreiber der Webanwendung die Uploads konfigurieren kann.

## CON.10.A6 Schutz vor unerlaubter automatisierter Nutzung von Webanwendungen (B)

- Die Entwickler MÜSSEN Sicherheitsmechanismen implementieren, die die Webanwendung vor automatisierten Zugriffen schützen.
- Die Entwickler MÜSSEN bei der Implementierung der Sicherheitsmechanismen berücksichtigen, wie sich diese auf die Nutzungsmöglichkeiten berechtigter Benutzer auswirken.

## CON.10.A7 Schutz vertraulicher Daten (B)

- Die Entwickler MÜSSEN sicherstellen, dass vertrauliche Daten von den Clients zu den Servern nur mit der HTTPPost-Methode übertragen werden.
- Die Entwickler MÜSSEN durch Direktiven in der Webanwendung gewährleisten, dass clientseitig keine schützenswerten Daten zwischengespeichert werden.
- Die Entwickler MÜSSEN sicherstellen, dass in Formularen keine vertraulichen Formulardaten im Klartext angezeigt werden.
- Die Webanwendung SOLLTE verhindern, dass vertrauliche Daten vom Webbrowser unerwartet gespeichert werden.
- Sämtliche Zugangsdaten der Webanwendung MÜSSEN serverseitig mithilfe von sicheren kryptografischen Algorithmen vor unbefugtem Zugriff geschützt werden (Salted Hash).
- Die Dateien mit den Quelltexten der Webanwendung MÜSSEN vor unerlaubten Abrufen geschützt werden.

## CON.10.A8 Umfassende Eingabevalidierung und Ausgabekodierung (B)

- Die Entwickler MÜSSEN sämtliche an eine Webanwendung übergebenen Daten als potenziell gefährlich behandeln und geeignet filtern.
- Sämtliche Eingabedaten sowie Datenströme und Sekundärdaten, wie z. B. Session-IDs, MÜSSEN serverseitig validiert werden.
- Fehleingaben SOLLTEN möglichst nicht automatisch behandelt werden (Sanitizing).
- Lässt es sich jedoch nicht vermeiden, MUSS Sanitizing sicher umgesetzt werden.
- Ausgabedaten MÜSSEN so kodiert werden, dass schadhafter Code auf dem Zielsystem nicht interpretiert oder ausgeführt wird.

## CON.10.A9 Schutz vor SQL-Injection (B)

- Falls Daten an ein Datenbankmanagementsystem (DBMS) weitergeleitet werden, MÜSSEN die Entwickler Stored Procedures bzw. Prepared SQL Statements einsetzen.
- Falls Daten an ein DBMS weitergeleitet werden und weder Stored Procedures noch Prepared SQL Statements von der Einsatzumgebung unterstützt werden, MÜSSEN die SQLQueries separat abgesichert werden.

## CON.10.A10 Restriktive Herausgabe sicherheitsrelevanter Informationen (B)

- Die Entwickler MÜSSEN sicherstellen, dass Webseiten, Rückantworten und Fehlermeldungen von Webanwendungen keine Informationen enthalten, die einem Angreifer Hinweise darauf geben, wie er Sicherheitsmechanismen umgehen kann.

## CON.10.A11 Softwarearchitektur einer Webanwendung (S)

- Die Entwickler SOLLTEN die Softwarearchitektur der Webanwendung mit allen Bestandteilen und Abhängigkeiten dokumentieren.
- Die Dokumentation SOLLTE bereits während des Entwicklungsverlaufs aktualisiert und angepasst werden.
- Die Dokumentation SOLLTE so gestaltet sein, dass sie schon in der Entwicklungsphase benutzt werden kann und Entscheidungen nachvollziehbar sind.
- In der Dokumentation SOLLTEN alle für den Betrieb notwendigen Komponenten gekennzeichnet werden, die nicht Bestandteil der Webanwendung sind.
- In der Dokumentation SOLLTE beschrieben sein, welche Komponenten welche Sicherheitsmechanismen umsetzen, wie die Webanwen-dung in eine bestehende Infrastruktur integriert wird und welche kryptografischen Funktionen und Verfahren eingesetzt werden.

## CON.10.A12 Verifikation essenzieller Änderungen (S)

- Falls wichtige Einstellungen mit der Anwendung geändert werden sollen, dann SOLLTEN die Entwickler sicherstellen, dass die Änderungen durch die Eingabe eines Passworts erneut verifiziert werden.
- Falls dies nicht möglich ist, dann SOLLTE die Webanwendung auf andere geeignete Weise sicherstellen, dass sich die Benutzer authentisieren.
- Die Benutzer SOLLTEN über Änderungen mithilfe von Kommunikationswegen außerhalb der Webanwendung informiert werden.

## CON.10.A13 Fehlerbehandlung (S)

- Treten während der Laufzeit einer Webanwendung Fehler auf, SOLLTEN Entwickler diese so behandeln, dass die Webanwendung weiter in einem konsistenten Zustand bleibt.
- Die Webanwendung SOLLTE Fehlermeldungen protokollieren.
- Falls eine veranlasste Aktion einen Fehler verursacht, SOLLTE die Webanwendung diese Aktion abbrechen.
- Die Webanwendung SOLLTE im Fehlerfall den Zugriff auf eine angeforderte Ressource oder Funktion verweigern.
- Zuvor reservierte Ressourcen SOLLTEN im Rahmen der Fehlerbehandlung wieder freigegeben werden.
- Der Fehler SOLLTE möglichst von der Webanwendung selbst behandelt werden.

## CON.10.A14 Sichere HTTP-Konfiguration bei Webanwendungen (S)

- Zum Schutz vor Clickjacking, Cross-Site-Scripting und anderen Angriffen SOLLTEN die Entwickler geeignete HTTPResponse-Header setzen.
- Es SOLLTEN mindestens die folgenden HTTP-Header verwendet werden: Content-Security-Policy, Strict-Transport-Security, Content-Type, X-Content-Type-Options sowie Cache-Control.
- Die verwendeten HTTP-Header SOLLTEN auf die Webanwendung abgestimmt werden.
- Die verwendeten HTTP-Header SOLLTEN so restriktiv wie möglich sein.
- Cookies SOLLTEN grundsätzlich mit den Attributen secure, SameSite und httponly gesetzt werden.

## CON.10.A15 Verhinderung von Cross-Site-Request-Forgery (S)

- Die Entwickler SOLLTEN die Webanwendung mit solchen Sicherheitsmechanismen ausstatten, die eine Unterscheidung zwischen beabsichtigten Seitenaufrufen des Benutzers von unbeabsichtigt weitergeleiteten Befehlen Dritter ermöglichen.
- Dabei SOLLTE mindestens geprüft werden, ob neben der Session-ID ein geheimes Token für den Zugriff auf geschützte Ressourcen und Funktionen benötigt wird.

## CON.10.A16 Mehr-Faktor-Authentisierung (S)

- Die Entwickler SOLLTEN eine Mehr-Faktor-Authentisierung implementieren.

## CON.10.A17 Verhinderung der Blockade von Ressourcen (H)

- Zum Schutz vor Denial-of-Service (DoS)-Angriffen SOLLTEN ressourcenintensive Operationen vermieden werden.
- Falls ressourcenintensive Operationen notwendig sind, dann SOLLTEN diese besonders abgesichert werden.
- Bei Webanwendungen SOLLTE ein möglicher Überlauf von Protokollierungsdaten überwacht und verhindert werden.

## CON.10.A18 Kryptografische Absicherung vertraulicher Daten (H)

- Entwickler SOLLTEN sicherstellen, dass vertrauliche Daten einer Webanwendung durch sichere, kryptografische Algorithmen abgesichert werden.


