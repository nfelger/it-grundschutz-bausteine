# DER.2.3: Bereinigung weitreichender Sicherheitsvorfälle

## DER.2.3.A1 Einrichtung eines Leitungsgremiums (B)

- Um einen APT-Vorfall zu bereinigen, MUSS ein Leitungsgremium eingerichtet werden, das alle notwendigen Aktivitäten plant, koordiniert und überwacht.
- Dem Gremium MÜSSEN alle für die Aufgaben erforderlichen Weisungsbefugnisse übertragen werden.
- Wenn ein solches Leitungsgremium zu dem Zeitpunkt, als der APT-Vorfall detektiert und klassifiziert wurde, bereits eingerichtet ist, SOLLTE dasselbe Gremium auch die Bereinigung planen und leiten.
- Wurde schon ein spezialisierter Forensik-Dienstleister hinzugezogen, um den APT-Vorfall zu analysieren, SOLLTE dieser auch bei der Bereinigung des Vorfalls miteinbezogen werden.
- Ist die IT zu stark kompromittiert, um weiter betrieben zu werden, oder sind die notwendigen Bereinigungsmaßnahmen sehr umfangreich, SOLLTE geprüft werden, ob ein Krisenstab eingerichtet werden soll.
- In diesem Fall MUSS das Leitungsgremium die Bereinigungsmaßnahmen überwachen.
- Das Leitungsgremium MUSS dann dem Krisenstab berichten.

## DER.2.3.A2 Entscheidung für eine Bereinigungsstrategie (B)

- Bevor ein APT-Vorfall tatsächlich bereinigt wird, MUSS das Leitungsgremium eine Bereinigungsstrategie festlegen.
- Dabei MUSS insbesondere entschieden werden, ob die Schadsoftware von kompromittierten IT-Systemen entfernt werden kann, ob IT-Systeme neu installiert werden müssen oder ob IT-Systeme inklusive der Hardware komplett ausgetauscht werden sollen.
- Weiterhin MUSS festgelegt werden, welche IT-Systeme bereinigt werden.
- Grundlage für diese Entscheidungen MÜSSEN die Ergebnisse einer zuvor durchgeführten forensischen Untersuchung sein.
- Es SOLLTEN alle betroffenen IT-Systeme neu installiert werden.
- Danach MÜSSEN die Wiederanlaufpläne der Institution benutzt werden.
- Bevor jedoch Backups wieder eingespielt werden, MUSS durch forensische Untersuchungen sichergestellt sein, dass dadurch keine manipulierten Daten oder Programme auf das neu installierte IT-System übertragen werden.
- Entscheidet sich eine Institution dagegen, alle IT-Systeme neu zu installieren, MUSS eine gezielte APT-Bereinigung umgesetzt werden.
- Um das Risiko übersehener Hintertüren zu minimieren, MÜSSEN nach der Bereinigung die ITSysteme gezielt daraufhin überwacht werden, ob sie noch mit dem Angreifer kommunizieren.

## DER.2.3.A3 Isolierung der betroffenen Netzabschnitte (B)

- Die von einem APT-Vorfall betroffenen Netzabschnitte MÜSSEN vollständig isoliert werden (Cut-Off).
- Insbesondere MÜSSEN die betroffenen Netzabschnitte vom Internet getrennt werden.
- Um den Angreifer effektiv auszusperren und zu verhindern, dass er seine Spuren verwischt oder noch weitere IT-Systeme sabotiert, MÜSSEN die Netzabschnitte auf einen Schlag isoliert werden.
- Welche Netzabschnitte isoliert werden müssen, MUSS vorher durch eine forensische Analyse festgelegt werden.
- Es MÜSSEN dabei sämtliche betroffenen Abschnitte identifiziert werden.
- Kann das nicht sichergestellt werden, MÜSSEN alle verdächtigen sowie alle auch nur theoretisch infizierten Netzabschnitte isoliert werden.
- Um Netzabschnitte effektiv isolieren zu können, MÜSSEN sämtliche lokalen Internetanschlüsse, z. B. zusätzliche DSL-Anschlüsse in einzelnen Subnetzen, möglichst vollständig erfasst und ebenfalls berücksichtigt werden.

## DER.2.3.A4 Sperrung und Änderung von Zugangsdaten und kryptografischen Schlüsseln (B)

- Alle Zugangsdaten MÜSSEN geändert werden, nachdem das Netz isoliert wurde.
- Weiterhin MÜSSEN auch zentral verwaltete Zugangsdaten zurückgesetzt werden, z. B. in Active-Directory-Umgebungen oder wenn das Lightweight Directory Access Protocol (LDAP) benutzt wurde.
- Ist der zentrale Authentisierungsserver (Domaincontroller oder LDAP-Server) kompromittiert, MÜSSEN sämtliche dort vorhandenen Zugänge gesperrt und ihre Passwörter ausgetauscht werden.
- Dies MÜSSEN erfahrene Administratoren umsetzen, falls erforderlich, auch mithilfe interner oder externer Forensikexperten.
- Wurden TLS-Schlüssel oder eine interne Certification Authority (CA) durch den APT-Angriff kompromittiert, MÜSSEN entsprechende Schlüssel, Zertifikate und Infrastrukturen neu erzeugt und verteilt werden.
- Auch MÜSSEN die kompromittierten Schlüssel und Zertifikate zuverlässig gesperrt und zurückgerufen werden.

## DER.2.3.A5 Schließen des initialen Einbruchswegs (B)

- Wurde durch eine forensische Untersuchung herausgefunden, dass der Angreifer durch eine technische Schwachstelle in das Netz der Institution eingedrungen ist, MUSS diese Schwachstelle geschlossen werden.
- Konnten die Angreifer die IT-Systeme durch menschliche Fehlhandlungen kompromittieren, MÜSSEN organisatorische, personelle und technische Maßnahmen ergriffen werden, um ähnliche Vorfälle künftig zu verhindern.

## DER.2.3.A6 Rückführung in den Produktivbetrieb (B)

- Nachdem das Netz erfolgreich bereinigt wurde, MÜSSEN die IT-Systeme geordnet in den Produktivbetrieb zurückgeführt werden.
- Dabei MÜSSEN sämtliche zuvor eingesetzten IT-Systeme und installierten Programme, mit denen der Angriff beobachtet und analysiert wurde, entweder entfernt oder aber in den Produktivbetrieb überführt werden.
- Dasselbe MUSS mit Kommunikations- und Kollaborationssystemen erfolgen, die für die Bereinigung angeschafft wurden.
- Beweismittel und ausgesonderte IT-Systeme MÜSSEN entweder sicher gelöscht bzw. vernichtet oder aber geeignet archiviert werden.

## DER.2.3.A7 Gezielte Systemhärtung (S)

- Nach einem APT-Angriff SOLLTEN alle betroffenen IT-Systeme gehärtet werden.
- Grundlage hierfür SOLLTEN die Ergebnisse der forensischen Untersuchungen sein.
- Zusätzlich SOLLTE erneut geprüft werden, ob die betroffene Umgebung noch sicher ist.
- Wenn möglich, SOLLTEN IT-Systeme bereits während der Bereinigung gehärtet werden.
- Maßnahmen, die sich nicht kurzfristig durchführen lassen, SOLLTEN in einen Maßnahmenplan aufgenommen und mittelfristig umgesetzt werden.
- Der ISB SOLLTE den Plan aufstellen und prüfen, ob er korrekt umgesetzt wurde.

## DER.2.3.A8 Etablierung sicherer, unabhängiger Kommunikationskanäle (S)

- Es SOLLTEN sichere Kommunikationskanäle für das Leitungsgremium und die mit der Bereinigung beauftragten Mitarbeiter etabliert werden.
- Wird auf Kommunikationsdienste Dritter zurückgegriffen, SOLLTE auch hier darauf geachtet werden, dass ein sicherer Kommunikationskanal ausgewählt wird.

## DER.2.3.A9 Hardwaretausch betroffener IT-Systeme (H)

- Es SOLLTE erwogen werden, nach einem APT-Vorfall die Hardware komplett auszutauschen.
- Auch wenn nach einer Bereinigung bei einzelnen IT-Systemen noch verdächtiges Verhalten beobachtet wird, SOLLTEN die betroffenen ITSysteme ausgetauscht werden.

## DER.2.3.A10 Umbauten zur Erschwerung eines erneuten Angriffs durch denselben Angreifer (H)

- Damit derselbe Angreifer nicht noch einmal einen APT-Angriff auf die IT-Systeme der Institution durchführen kann, SOLLTE der interne Aufbau der Netzumgebung geändert werden.
- Außerdem SOLLTEN Mechanismen etabliert werden, mit denen sich ein wiederkehrender Angreifer schnell detektieren lässt.


