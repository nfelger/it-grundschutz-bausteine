# OPS.1.1.3: Patch- und Änderungsmanagement

## OPS.1.1.3.A1 Konzept für das Patch- und Änderungsmanagement [Fachverantwortliche] (B)

- Wenn IT-Komponenten, Software oder Konfigurationsdaten geändert werden, MUSS es dafür Vorgaben geben, die auch Sicherheitsaspekte berücksichtigen.
- Diese MÜSSEN in einem Konzept für das Patch- und Änderungsmanagement festgehalten und befolgt werden.
- Alle Patches und Änderungen MÜSSEN geeignet geplant, genehmigt und dokumentiert werden.
- Patches und Änderungen SOLLTEN vorab geeignet getestet werden (siehe hierzu auch OPS.1.1.6 Software-Tests und Freigaben).
- Wenn Patches installiert und Änderungen durchgeführt werden, MÜSSEN Rückfall-Lösungen vorhanden sein.
- Bei größeren Änderungen MUSS zudem der Informationssicherheitsbeauftragte beteiligt sein.
- Insgesamt MUSS sichergestellt werden, dass das angestrebte Sicherheitsniveau während und nach den Änderungen erhalten bleibt.
- Insbesondere SOLLTEN auch die gewünschten Sicherheitseinstellungen erhalten bleiben.

## OPS.1.1.3.A2 Festlegung der Zuständigkeiten (B)

- Für alle Organisationsbereiche MÜSSEN Zuständige für das Patch- und Änderungsmanagement festgelegt werden.
- Die definierten Zuständigkeiten MÜSSEN sich auch im Berechtigungskonzept widerspiegeln.

## OPS.1.1.3.A3 Konfiguration von Autoupdate-Mechanismen (B)

- Innerhalb der Strategie zum Patch- und Änderungsmanagement MUSS definiert werden, wie mit integrierten Update-Mechanismen (Autoupdate) der eingesetzten Software umzugehen ist.
- Insbesondere MUSS festgelegt werden, wie diese Mechanismen abgesichert und passend konfiguriert werden.
- Außerdem SOLLTEN neue Komponenten daraufhin überprüft werden, welche Update-Mechanismen sie haben.

## OPS.1.1.3.A15 Regelmäßige Aktualisierung von IT-Systemen und Software (B)

- IT-Systeme und Software SOLLTEN regelmäßig aktualisiert werden.
- Grundsätzlich SOLLTEN Patches zeitnah nach Veröffentlichung eingespielt werden.
- Basierend auf dem Konzept für das Patch- und Änderungsmanagement MÜSSEN Patches zeitnah nach Veröffentlichung bewertet und entsprechend priorisiert werden.
- Es MUSS entschieden werden, ob der Patch eingespielt werden soll.
- Wenn ein Patch eingespielt wird, SOLLTE kontrolliert werden, ob dieser auf allen relevanten Systemen zeitnah erfolgreich eingespielt wurde.
- Wenn ein Patch nicht eingespielt wird, MÜSSEN die Entscheidung und die Gründe dafür dokumentiert werden.

## OPS.1.1.3.A16 Regelmäßige Suche nach Informationen zu Patches und Schwachstellen (B)

- Der IT-Betrieb MUSS sich regelmäßig über bekannt gewordene Schwachstellen der Firmware, Betriebssysteme, eingesetzter Anwendungen und Dienste informieren.
- Die identifizierten Schwachstellen MÜSSEN so schnell wie möglich behoben werden.
- Solange keine entsprechenden Patches zur Verfügung stehen, MÜSSEN abhängig davon, wie schwerwiegend die Schwachstellen und Bedrohungen sind, andere geeignete Maßnahmen zum Schutz des IT-Systems getroffen werden.
- Falls dies nicht möglich ist, SOLLTE sichergestellt sein, dass die entsprechende Hardware, relevanten Betriebssysteme, eingesetzten Anwendungen und Dienste nicht weiter verwendet werden.

## OPS.1.1.3.A4 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## OPS.1.1.3.A5 Umgang mit Änderungsanforderungen [Fachverantwortliche] (S)

- Alle Änderungsanforderungen (Request for Changes, RfCs) SOLLTEN erfasst und dokumentiert werden.
- Die Änderungsanforderungen SOLLTEN vom Fachverantwortlichen für das Patch- und Änderungsmanagement daraufhin kontrolliert werden, ob die Aspekte der Informationssicherheit ausreichend berücksichtigt wurden.

## OPS.1.1.3.A6 Abstimmung von Änderungsanforderungen (S)

- Der zu einer Änderung zugehörige Abstimmungsprozess SOLLTE alle relevanten Zielgruppen und die Auswirkungen auf die Informationssicherheit berücksichtigen.
- Die von der Änderung betroffenen Zielgruppen SOLLTEN sich nachweisbar dazu äußern können.
- Auch SOLLTE es ein festgelegtes Verfahren geben, wodurch wichtige Änderungsanforderungen beschleunigt werden können.

## OPS.1.1.3.A7 Integration des Änderungsmanagements in die Geschäftsprozesse (S)

- Der Änderungsmanagementprozess SOLLTE in die Geschäftsprozesse beziehungsweise Fachaufgaben integriert werden.
- Bei geplanten Änderungen SOLLTE die aktuelle Situation der davon betroffenen Geschäftsprozesse berücksichtigt werden.
- Alle relevanten Fachabteilungen SOLLTEN über anstehende Änderungen informiert werden.
- Auch SOLLTE es eine Eskalationsebene geben, deren Mitglieder der Leitungsebene der Institution angehören.
- Sie SOLLTEN in Zweifelsfällen über Priorität und Terminplanung einer Hard- oder Software-Änderung entscheiden.

## OPS.1.1.3.A8 Sicherer Einsatz von Werkzeugen für das Patch- und Änderungsmanagement (S)

- Anforderungen und Rahmenbedingungen SOLLTEN definiert werden, nach denen Werkzeuge für das Patch- und Änderungsmanagement ausgewählt werden.
- Außerdem SOLLTE eine spezifische Sicherheitsrichtlinie für die eingesetzten Werkzeuge erstellt werden.

## OPS.1.1.3.A9 Test- und Abnahmeverfahren für neue Hardware (S)

- Wenn neue Hardware ausgewählt wird, SOLLTE geprüft werden, ob die eingesetzte Software und insbesondere die relevanten Betriebssysteme mit der Hardware und dessen Treibersoftware kompatibel sind.
- Neue Hardware SOLLTE getestet werden, bevor sie eingesetzt wird.
- Diese SOLLTE ausschließlich in einer isolierten Umgebung getestet werden.
- Für IT-Systeme SOLLTE es ein Abnahmeverfahren und eine Freigabeerklärung geben.
- Der Zuständige SOLLTE die Freigabeerklärung an geeigneter Stelle schriftlich hinterlegen.
- Für den Fall, dass trotz der Abnahme- und Freigabeverfahren im laufenden Betrieb Fehler festgestellt werden, SOLLTE es ein Verfahren zur Fehlerbehebung geben.

## OPS.1.1.3.A10 Sicherstellung der Integrität und Authentizität von Softwarepaketen (S)

- Während des gesamten Patch- oder Änderungsprozesses SOLLTE die Authentizität und Integrität von Softwarepaketen sichergestellt werden.
- Dazu SOLLTE geprüft werden, ob für die eingesetzten Softwarepakete Prüfsummen oder digitale Signaturen verfügbar sind.
- Falls ja, SOLLTEN diese vor der Installation des Pakets überprüft werden.
- Ebenso SOLLTE darauf geachtet werden, dass die notwendigen Programme zur Überprüfung vorhanden sind.
- Software und Updates SOLLTEN grundsätzlich nur aus vertrauenswürdigen Quellen bezogen werden.

## OPS.1.1.3.A11 Kontinuierliche Dokumentation der Informationsverarbeitung (S)

- Änderungen SOLLTEN in allen Phasen, allen Anwendungen und allen Systemen dokumentiert werden.
- Dazu SOLLTEN entsprechende Regelungen erarbeitet werden.

## OPS.1.1.3.A12 Einsatz von Werkzeugen beim Änderungsmanagement (H)

- Bevor ein Werkzeug zum Änderungsmanagement benutzt wird, SOLLTE sorgfältig geprüft werden, ob damit die Änderungen angemessen im Informationsverbund verteilt werden können.
- Zusätzlich SOLLTEN Unterbrechungspunkte definiert werden können, an denen die Verteilung einer fehlerhaften Änderung gestoppt wird.

## OPS.1.1.3.A13 Erfolgsmessung von Änderungsanforderungen [Fachverantwortliche] (H)

- Um zu überprüfen, ob eine Änderung erfolgreich war, SOLLTE der Fachverantwortliche für das Patch- und Änderungsmanagement sogenannte Nachtests durchführen.
- Dazu SOLLTE er geeignete Referenzsysteme als Qualitätssicherungssysteme auswählen.
- Die Ergebnisse der Nachtests SOLLTEN im Rahmen des Änderungsprozesses dokumentiert werden.

## OPS.1.1.3.A14 Synchronisierung innerhalb des Änderungsmanagements (H)

- Im Änderungsmanagementprozess SOLLTE durch geeignete Mechanismen sichergestellt werden, dass auch zeitweise oder längerfristig nicht erreichbare Geräte die Patches und Änderungen erhalten.


