# OPS.1.1.6: Software-Tests und -Freigaben

## OPS.1.1.6.A1 Planung der Software-Tests (B)

- Die Rahmenbedingungen für Software-Tests MÜSSEN vor den Tests innerhalb der Institution entsprechend der Schutzbedarfe, Organisationseinheiten, technischen Möglichkeiten und Test-Umgebungen festlegt sein.
- Die Software MUSS auf Basis der Anforderungen des Anforderungskatalogs zu der Software getestet werden.
- Liegt auch ein Pflichtenheft vor, dann MUSS dieses zusätzlich berücksichtigt werden.
- Die Testfälle MÜSSEN so ausgewählt werden, sodass diese möglichst repräsentativ alle Funktionen der Software überprüfen.
- Zusätzlich SOLLTEN auch Negativ-Tests berücksichtigt werden, die überprüfen, ob die Software keine ungewollten Funktionen enthält.
- Die Testumgebung MUSS so ausgewählt werden, sodass diese möglichst repräsentativ alle in der Institution eingesetzten Gerätemodelle und Betriebssystemumgebungen abdeckt.
- Es SOLLTE dabei getestet werden, ob die Software mit den eingesetzten Betriebssystemen in den vorliegenden Konfigurationen kompatibel und funktionsfähig ist.

## OPS.1.1.6.A2 Durchführung von funktionalen Software-Tests [Tester] (B)

- Mit funktionalen Software-Tests MUSS die ordnungsgemäße und vollständige Funktion der Software überprüft werden.
- Die funktionalen Software-Tests MÜSSEN so durchgeführt werden, dass sie den Produktivbetrieb nicht beeinflussen.

## OPS.1.1.6.A3 Auswertung der Testergebnisse [Tester] (B)

- Die Ergebnisse der Software-Tests MÜSSEN ausgewertet werden.
- Es SOLLTE ein Soll-Ist-Vergleich mit definierten Vorgaben durchgeführt werden.
- Die Auswertung MUSS dokumentiert werden.

## OPS.1.1.6.A4 Freigabe der Software [Fachverantwortliche] (B)

- Die fachlich zuständige Organisationseinheit MUSS die Software freigeben, sobald die Software-Tests erfolgreich durchgeführt wurden.
- Die Freigabe MUSS in Form einer Freigabeerklärung dokumentiert werden.
- Die freigebende Organisationseinheit MUSS überprüfen, ob die Software gemäß den Anforderungen getestet wurde.
- Die Ergebnisse der Software-Tests MÜSSEN mit den vorher festgelegten Erwartungen übereinstimmen.
- Auch MUSS überprüft werden, ob die rechtlichen und organisatorischen Vorgaben eingehalten wurden.

## OPS.1.1.6.A5 Durchführung von Software-Tests für nicht funktionale Anforderungen [Tester] (B)

- Es MÜSSEN Software-Tests durchgeführt werden, die überprüfen, ob alle wesentlichen nichtfunktionalen Anforderungen erfüllt werden.
- Insbesondere MÜSSEN sicherheitsspezifische Software-Tests durchgeführt werden, wenn die Anwendung sicherheitskritische Funktionen mitbringt.
- Die durchgeführten Testfälle, sowie die Testergebnisse, MÜSSEN dokumentiert werden.

## OPS.1.1.6.A11 Verwendung von anonymisierten oder pseudonymisierten Testdaten [Datenschutzbeauftragter, Tester] (B)

- Wenn Produktivdaten für Software-Tests verwendet werden, die schützenswerte Informationen enthalten, dann MÜSSEN diese Testdaten angemessen geschützt werden.
- Enthalten diese Daten personenbezogene Informationen,dann MÜSSEN diese Daten mindestens pseudonymisiert werden.
- Falls möglich, SOLLTEN die Testdaten mit Personenbezug vollständig anonymisiert werden.
- Wenn ein Personenbezug von den Testdaten abgeleitet werden könnte, MUSS der Datenschutzbeauftragte und unter Umständen die Personalvertretung hinzugezogen werden.

## OPS.1.1.6.A6 Geordnete Einweisung der Software-Tester [Fachverantwortliche] (S)

- Die Software-Tester SOLLTEN über die durchzuführenden Testarten und die zu testenden Bereiche einer Software vom Fachverantwortlichen informiert werden.
- Darüber hinaus SOLLTEN die Software-Tester über die Anwendungsfälle und mögliche weitere Anforderungen der Software informiert werden.

## OPS.1.1.6.A7 Personalauswahl der Software-Tester [Personalabteilung, Fachverantwortliche] (S)

- Bei der Auswahl der Software-Tester SOLLTEN gesonderte Auswahlkriterien berücksichtigt werden.
- Die SoftwareTester SOLLTEN die erforderliche berufliche Qualifikation haben.
- Wird Individualsoftware auf Quellcode-Ebene überprüft, dann SOLLTEN die Tester über ausreichendes Fachwissen über die zu testenden Programmiersprache und die Entwicklungsumgebung verfügen.
- Der Quellcode SOLLTE NICHT ausschließlich von Testern überprüft werden, die auch an der Erstellung des Quellcodes beteiligt waren.

## OPS.1.1.6.A8 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## OPS.1.1.6.A9 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## OPS.1.1.6.A10 Erstellung eines Abnahmeplans (S)

- In einem Abnahmeplan SOLLTEN die durchzuführenden Testarten, Testfälle und die erwarteten Ergebnisse dokumentiert sein.
- Außerdem SOLLTE der Abnahmeplan die Freigabekriterien beinhalten.
- Es SOLLTE eine Vorgehensweise für die Situation festgelegt werden, wenn eine Freigabe abgelehnt wird.

## OPS.1.1.6.A12 Durchführung von Regressionstests [Tester] (S)

- Wenn Software verändert wurde, SOLLTEN Regressionstests durchgeführt werden.
- Hierbei SOLLTE überprüft werden, ob bisherige bestehende Sicherheitsmechanismen und -einstellungen durch das Update ungewollt verändert wurden.
- Regressionstests SOLLTEN vollständig durchgeführt werden und hierbei auch Erweiterungen sowie Hilfsmittel umfassen.
- Werden Testfälle ausgelassen, SOLLTE dies begründet und dokumentiert werden.
- Die durchgeführten Testfälle und die Testergebnisse SOLLTEN dokumentiert werden.

## OPS.1.1.6.A13 Trennung der Testumgebung von der Produktivumgebung (S)

- Software SOLLTE nur in einer hierfür vorgesehenen Testumgebung getestet werden.
- Die Testumgebung SOLLTE von der Produktivumgebung getrennt betrieben werden.
- Die in der Testumgebung verwendeten Architekturen und Mechanismen SOLLTEN dokumentiert werden.
- Es SOLLTEN Verfahren dokumentiert werden, wie mit der Testumgebung nach Abschluss des Software-Tests zu verfahren ist.

## OPS.1.1.6.A15 Überprüfung der Installation und zugehöriger Dokumentation [Tester] (S)

- Die Installation der Software SOLLTE entsprechend der Regelungen zur Installation und Konfiguration von Software (siehe Baustein APP.6 Allgemeine Software) überprüft werden.
- Falls vorhanden, SOLLTE zusätzlich die Installationsund Konfigurationsdokumentation geprüft werden.

## OPS.1.1.6.A14 Durchführung von Penetrationstests [Tester] (H)

- Für Anwendungen beziehungsweise IT-Systeme mit erhöhtem Schutzbedarf SOLLTEN Penetrationstests als Testmethode durchgeführt werden.
- Ein Konzept für Penetrationstests SOLLTE erstellt werden.
- Im Konzept für Penetrationstests SOLLTEN neben den zu verwendenden Testmethoden auch die Erfolgskriterien dokumentiert werden.
- Der Penetrationstest SOLLTE nach den Rahmenbedingungen des Penetrationstest-Konzepts erfolgen.
- Die durch den Penetrationstest aufgefundenen Sicherheitslücken SOLLTEN klassifiziert und dokumentiert sein.

## OPS.1.1.6.A16 Sicherheitsüberprüfung der Tester (H)

- Sofern Tester auf besonders schützenswerte Informationen zugreifen müssen, SOLLTE die Institution Nachweise über ihre Integrität und Reputation einholen.
- Handelt es sich dabei um klassifizierte Verschlusssachen, SOLLTEN sich die Software-Tester einer Sicherheitsüberprüfung nach dem Sicherheitsüberprüfungsgesetz (SÜG) unterziehen.
- Hierzu SOLLTE der ISB den Geheimschutzbeauftragten bzw. Sicherheitsbevollmächtigten der Institution einbeziehen.


