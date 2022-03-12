# OPS.1.1.5: Protokollierung

## OPS.1.1.5.A1 Erstellung einer Sicherheitsrichtlinie für die Protokollierung [Fachverantwortliche] (B)

- Ausgehend von der allgemeinen Sicherheitsrichtlinie der Institution MUSS eine spezifische Sicherheitsrichtlinie für die Protokollierung erstellt werden.
- In dieser Sicherheitsrichtlinie MÜSSEN nachvollziehbar Anforderungen und Vorgaben beschrieben sein, wie die Protokollierung zu planen, aufzubauen und sicher zu betreiben ist.
- In der spezifischen Sicherheitsrichtlinie MUSS geregelt werden, wie, wo und was zu protokollieren ist.
- Dabei SOLLTEN sich Art und Umfang der Protokollierung am Schutzbedarf der Informationen orientieren.
- Die spezifische Sicherheitsrichtlinie MUSS vom ISB gemeinsam mit den Fachverantwortlichen erstellt werden.
- Sie MUSS allen für die Protokollierung zuständigen Mitarbeitern bekannt und grundlegend für ihre Arbeit sein.
- Wirddie spezifische Sicherheitsrichtlinie verändert oder wird von den Anforderungen abgewichen, MUSS dies mit dem ISB abgestimmt und dokumentiert werden.
- Es MUSS regelmäßig überprüft werden, ob die spezifische Sicherheitsrichtlinie noch korrekt umgesetzt ist.
- Die Ergebnisse der Überprüfung MÜSSEN dokumentiert werden.

## OPS.1.1.5.A2 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## OPS.1.1.5.A3 Konfiguration der Protokollierung auf System- und Netzebene (B)

- Alle sicherheitsrelevanten Ereignisse von IT-Systemen und Anwendungen MÜSSEN protokolliert werden.
- Sofern die in der Protokollierungsrichtlinie als relevant definierten IT-Systeme und Anwendungen über eine Protokollierungsfunktion verfügen, MUSS diese benutzt werden.
- Wenn die Protokollierung eingerichtet wird, MÜSSEN dabei die Herstellervorgaben für die jeweiligen IT-Systeme oder Anwendungen beachtet werden.
- In angemessenen Intervallen MUSS stichpunktartig überprüft werden, ob die Protokollierung noch korrekt funktioniert.
- Die Prüfintervalle MÜSSEN in der Protokollierungsrichtlinie definiert werden.
- Falls betriebs- und sicherheitsrelevante Ereignisse nicht auf einem IT-System protokolliert werden können, MÜSSEN zusätzliche IT-Systeme zur Protokollierung (z. B. von Ereignissen auf Netzebene) integriert werden.

## OPS.1.1.5.A4 Zeitsynchronisation der IT-Systeme (B)

- Die Systemzeit aller protokollierenden IT-Systeme und Anwendungen MUSS immer synchron sein.
- Es MUSS sichergestellt sein, dass das Datums- und Zeitformat der Protokolldateien einheitlich ist.

## OPS.1.1.5.A5 Einhaltung rechtlicher Rahmenbedingungen (B)

- Bei der Protokollierung MÜSSEN die Bestimmungen aus den aktuellen Gesetzen zum Bundes- sowie Landesdatenschutz eingehalten werden (siehe CON.2 Datenschutz).
- Darüber hinaus MÜSSEN eventuelle Persönlichkeitsrechte bzw. Mitbestimmungsrechte der Mitarbeitervertretungen gewahrt werden.
- Ebenso MUSS sichergestellt sein, dass alle weiteren relevanten gesetzlichen Bestimmungen beachtet werden.
- Protokollierungsdaten MÜSSEN nach einem festgelegten Prozess gelöscht werden.
- Es MUSS technisch unterbunden werden, dass Protokollierungsdaten unkontrolliert gelöscht oder verändert werden.

## OPS.1.1.5.A6 Aufbau einer zentralen Protokollierungsinfrastruktur (S)

- Alle gesammelten sicherheitsrelevanten Protokollierungsdaten SOLLTEN an einer zentralen Stelle gespeichert werden.
- Dafür SOLLTE eine zentrale Protokollierungsinfrastruktur im Sinne eines Logserver-Verbunds aufgebaut und in einem hierfür eingerichteten Netzsegment platziert werden (siehe NET.1.1 Netzarchitektur und -design).
- Zusätzlich zu sicherheitsrelevanten Ereignissen (siehe OPS.1.1.5.A3 Konfiguration der Protokollierung auf Systemund Netzebene) SOLLTE eine zentrale Protokollierungsinfrastruktur auch allgemeine Betriebsereignisse protokollieren, die auf einen Fehler hindeuten.
- Die Protokollierungsinfrastruktur SOLLTE ausreichend dimensioniert sein.
- Die Möglichkeit einer Skalierung im Sinne einer erweiterten Protokollierung SOLLTE berücksichtigt werden.
- Dafür SOLLTEN genügend technische, finanzielle und personelle Ressourcen verfügbar sein.

## OPS.1.1.5.A7 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## OPS.1.1.5.A8 Archivierung von Protokollierungsdaten (S)

- Protokollierungsdaten SOLLTEN archiviert werden.
- Dabei SOLLTEN die gesetzlich vorgeschriebenen Regelungen berücksichtigt werden.

## OPS.1.1.5.A9 Bereitstellung von Protokollierungsdaten für die Auswertung (S)

- Die gesammelten Protokollierungsdaten SOLLTEN gefiltert, normalisiert, aggregiert und korreliert werden.
- Die so bearbeiteten Protokollierungsdaten SOLLTEN geeignet verfügbar gemacht werden, damit sie ausgewertet werden können.
- Damit sich die Daten automatisiert auswerten lassen, SOLLTEN die Protokollanwendungen über entsprechende Schnittstellen für die Auswertungsprogramme verfügen.
- Es SOLLTE sichergestellt sein, dass bei der Auswertung von Protokollierungsdaten die Sicherheitsanforderungen eingehalten werden, die in der Protokollierungsrichtlinie definiert sind.
- Auch wenn die Daten bereitgestellt werden, SOLLTEN betriebliche und interne Vereinbarungen berücksichtigt werden.
- Die Protokollierungsdaten SOLLTEN zusätzlich in unveränderter Originalform aufbewahrt werden.

## OPS.1.1.5.A10 Zugriffsschutz für Protokollierungsdaten (S)

- Es SOLLTE sichergestellt sein, dass die ausführenden Administratoren selbst keine Berechtigung haben, die aufgezeichneten Protokollierungsdaten zu verändern oder zu löschen.

## OPS.1.1.5.A11 Steigerung des Protokollierungsumfangs (H)

- Bei erhöhtem Schutzbedarf von Anwendungen oder IT-Systemen SOLLTEN grundsätzlich mehr Ereignisse protokolliert werden, sodass sicherheitsrelevante Vorfälle möglichst lückenlos nachvollziehbar sind.
- Um die Protokollierungsdaten in Echtzeit auswerten zu können, SOLLTEN sie in verkürzten Zeitabständen von den protokollierenden IT-Systemen und Anwendungen zentral gespeichert werden.
- Die Protokollierung SOLLTE eine Auswertung über den gesamten Informationsverbund ermöglichen.
- Anwendungen und IT-Systeme, mit denen eine zentrale Protokollierung nicht möglich ist, SOLLTEN bei einem erhöhten Schutzbedarf NICHT eingesetzt werden.

## OPS.1.1.5.A12 Verschlüsselung der Protokollierungsdaten (H)

- Um Protokollierungsdaten sicher übertragen zu können, SOLLTEN sie verschlüsselt werden.
- Alle gespeicherten Protokolle SOLLTEN digital signiert werden.
- Auch archivierte und außerhalb der Protokollierungsinfrastruktur gespeicherte Protokollierungsdaten SOLLTEN immer verschlüsselt gespeichert werden.

## OPS.1.1.5.A13 Hochverfügbare Protokollierungsinfrastruktur (H)

- Eine hochverfügbare Protokollierungsinfrastruktur SOLLTE aufgebaut werden.


