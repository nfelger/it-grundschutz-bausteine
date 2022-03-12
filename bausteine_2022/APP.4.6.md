# APP.4.6: SAP ABAP-Programmierung

## APP.4.6.A1 Absicherung von Reports mit Berechtigungsprüfungen (B)

- Es MUSS sichergestellt sein, dass nur berechtigte Benutzer selbst programmierte Auswertungen (Reports) starten können.
- Deswegen MUSS jeder Report explizite, zum Kontext passende Berechtigungsprüfungen durchführen.

## APP.4.6.A2 Formal korrekte Auswertung von Berechtigungsprüfungen (B)

- Jede Berechtigungsprüfung im Code MUSS durch Abfrage des Rückgabewertes SY-SUBRC ausgewertet werden.

## APP.4.6.A3 Berechtigungsprüfung vor dem Start einer Transaktion (B)

- Wenn Entwickler den Befehl CALL TRANSACTION verwenden, MUSS vorher immer eine Startberechtigungsprüfung durchgeführt werden.

## APP.4.6.A4 Verzicht auf proprietäre Berechtigungsprüfungen (B)

- Jede Berechtigungsprüfung MUSS technisch über den dafür vorgesehenen Befehl AUTHORITY-CHECK erfolgen.
- Proprietäre Berechtigungsprüfungen, z. B. basierend auf Benutzernamen, DÜRFEN NICHT benutzt werden.

## APP.4.6.A5 Erstellung einer Richtlinie für die ABAP-Entwicklung (S)

- Es SOLLTE eine Richtlinie für die Entwicklung von ABAP-Programmen erstellt werden.
- Die Richtlinie SOLLTE neben Namenskonventionen auch Vorgaben zu ABAP-Elementen beinhalten, die verwendet bzw. nicht verwendet werden dürfen.
- Die Anforderungen aus diesem Baustein SOLLTEN in die Richtlinie aufgenommen werden.
- Die Richtlinie SOLLTE für die Entwickler verbindlich sein.

## APP.4.6.A6 Vollständige Ausführung von Berechtigungsprüfungen (S)

- Bei einer Berechtigungsprüfung im ABAP-Code (AUTHORITY-CHECK <OBJECT>) SOLLTE sichergestellt sein, dass alle Felder des relevanten Berechtigungsobjekts überprüft werden.
- Wenn einzelne Felder tatsächlich nicht benötigt werden, SOLLTEN sie als DUMMY gekennzeichnet werden.
- Zusätzlich SOLLTE am Feld der Grund für die Ausnahme dokumentiert werden.

## APP.4.6.A7 Berechtigungsprüfung während der Eingabeverarbeitung (S)

- Funktionscodes und Bildschirmelemente von ABAP-Dynpro-Anwendungen SOLLTEN konsistent sein.
- Wenn ein Bildschirmelement abgeschaltet wurde, dann SOLLTE eine Anwendung NICHT ohne adäquate Berechtigungsprüfungen auf Ereignisse dieses Elements reagieren.
- Wenn bestimmte Einträge eines Dynpro-Menüs ausgeblendet oder einzelne Schaltflächen deaktiviert werden, dann SOLLTEN auch die zugehörigen Funktionscodes nicht ausgeführt werden.

## APP.4.6.A8 Schutz vor unberechtigten oder manipulierenden Zugriffen auf das Dateisystem (S)

- Wenn Zugriffe auf Dateien des SAP-Servers von Benutzereingaben abhängen, SOLLTEN diese Eingaben vor dem Zugriff validiert werden.

## APP.4.6.A9 Berechtigungsprüfung in remote-fähigen Funktionsbausteinen (S)

- Es SOLLTE sichergestellt werden, dass alle remote-fähigen Funktionsbausteine im Programmcode explizit prüfen, ob der Aufrufer berechtigt ist, die zugehörige Businesslogik auszuführen.

## APP.4.6.A10 Verhinderung der Ausführung von Betriebssystemkommandos (S)

- Jedem Aufruf eines erlaubten Betriebssystemkommandos SOLLTE eine entsprechende Berechtigungsprüfung (Berechtigungsobjekt S_LOG_COM) vorangestellt werden.
- Benutzereingaben SOLLTEN NICHT Teil eines Kommandos sein.
- Deswegen SOLLTEN Betriebssystemaufrufe ausschließlich über dafür vorgesehene SAP-Standardfunktionsbausteine ausgeführt werden.

## APP.4.6.A11 Vermeidung von eingeschleustem Schadcode (S)

- Die ABAP-Befehle INSERT REPORT und GENERATE SUBROUTINE POOL SOLLTEN NICHT verwendet werden.

## APP.4.6.A12 Vermeidung von generischer Modulausführung (S)

- Transaktionen, Programme, Funktionsbausteine und Methoden SOLLTEN NICHT generisch ausführbar sein.
- Sollte es wichtige Gründe für eine generische Ausführung geben, SOLLTE detailliert dokumentiert werden, wo und warum dies geschieht.
- Zusätzlich SOLLTE eine Whitelist definiert werden, die alle erlaubten Module enthält.
- Bevor ein Modul aufgerufen wird, SOLLTE die Benutzereingabe mit der Whitelist abgeglichen werden.

## APP.4.6.A13 Vermeidung von generischem Zugriff auf Tabelleninhalte (S)

- Tabelleninhalte SOLLTEN NICHT generisch ausgelesen werden.
- Sollte es wichtige Gründe dafür geben, dies doch zu tun, SOLLTE detailliert dokumentiert werden, wo und warum dies geschieht.
- Außerdem SOLLTE dann gewährleistet sein, dass sich der dynamische Tabellenname auf eine kontrollierbare Liste von Werten beschränkt.

## APP.4.6.A14 Vermeidung von nativen SQL-Anweisungen (S)

- Die Schnittstelle ABAP Database Connectivity (ADBC) SOLLTE NICHT verwendet werden.
- Benutzereingaben SOLLTEN NICHT Teil von ADBC-Befehlen sein.

## APP.4.6.A15 Vermeidung von Datenlecks (S)

- Es SOLLTE eine ausreichend sichere Berechtigungsprüfung durchgeführt werden, bevor geschäftskritische Daten angezeigt, übermittelt oder exportiert werden.
- Vorgesehene (gewollte) Möglichkeiten des Exports SOLLTEN dokumentiert werden.

## APP.4.6.A16 Verzicht auf systemabhängige Funktionsausführung (S)

- ABAP-Programme SOLLTEN NICHT systemabhängig programmiert werden, sodass sie nur auf einem bestimmten SAP-System ausgeführt werden können.
- Sollte dies jedoch unbedingt erforderlich sein, SOLLTE es detailliert dokumentiert werden.
- Außerdem SOLLTE der Code dann manuell überprüft werden.

## APP.4.6.A17 Verzicht auf mandantenabhängige Funktionsausführung (S)

- ABAP-Programme SOLLTEN NICHT mandantenabhängig programmiert werden, sodass sie nur von einem bestimmten Mandanten ausgeführt werden können.
- Sollte dies jedoch unbedingt erforderlich sein, SOLLTE es detailliert dokumentiert werden.
- Außerdem SOLLTEN dann zusätzliche Sicherheitsmaßnahmen ergriffen werden, wie beispielsweise eine manuelle Code-Überprüfung (manuelles Code-Review) oder eine Qualitätssicherung auf dem entsprechenden Mandanten.

## APP.4.6.A18 Vermeidung von Open-SQL-Injection-Schwachstellen (S)

- Dynamisches Open SQL SOLLTE NICHT verwendet werden.
- Falls Datenbankzugriffe mit dynamischen SQL-Bedingungen notwendig sind, SOLLTEN KEINE Benutzereingaben in der jeweiligen Abfrage übertragen werden.
- Wenn das dennoch der Fall ist, SOLLTE die Benutzereingabe zwingend geprüft werden (Output Encoding).

## APP.4.6.A19 Schutz vor Cross-Site-Scripting (S)

- Auf selbst entwickeltes HTML in Business-Server-Pages-(BSP)-Anwendungen oder HTTP-Handlern SOLLTE möglichst verzichtet werden.

## APP.4.6.A20 Keine Zugriffe auf Daten eines anderen Mandanten (S)

- Die automatische Mandantentrennung SOLLTE NICHT umgangen werden.
- Auf Daten anderer Mandanten SOLLTE NICHT mittels EXEC SQL oder der Open SQL Option CLIENT SPECIFIED zugegriffen werden.

## APP.4.6.A21 Verbot von verstecktem ABAP-Quelltext (S)

- Der Quelltext eines selbst erstellten ABAP-Programms SOLLTE immer lesbar sein.
- Techniken, die das verhindern (Obfuskation), SOLLTEN NICHT verwendet werden.

## APP.4.6.A22 Einsatz von ABAP-Codeanalyse Werkzeugen (H)

- Zur automatisierten Überprüfung von ABAP-Code auf sicherheitsrelevante Programmierfehler, funktionale und technische Fehler sowie auf qualitative Schwachstellen SOLLTE ein ABAP-Codeanalyse-Werkzeug eingesetzt werden.


