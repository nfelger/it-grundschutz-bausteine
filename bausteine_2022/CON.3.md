# CON.3: Datensicherungskonzept

## CON.3.A1 Erhebung der Einflussfaktoren für Datensicherungen [Fachverantwortliche, IT-Betrieb] (B)

- Der IT-Betrieb MUSS für jedes IT-System und darauf ausgeführten Anwendungen die Rahmenbedingungen für die Datensicherung erheben.
- Dazu MÜSSEN die Fachverantwortlichen für die Anwendungen ihre Anforderungen an die Datensicherung definieren.
- Der IT-Betrieb MUSS mindestens die nachfolgenden Rahmenbedingungen mit den Fachverantwortlichen abstimmen:
    - zu sichernde Daten,
    - Speichervolumen,
    - Änderungsvolumen,
    - Änderungszeitpunkte,
    - Verfügbarkeitsanforderungen,
    - Vertraulichkeitsanforderungen,
    - Integritätsbedarf,
    - rechtliche Anforderungen,
    - Anforderungen an das Löschen und Vernichten der Daten sowie
    - Zuständigkeiten für die Datensicherung.
- Die Einflussfaktoren MÜSSEN nachvollziehbar und auf geeignete Weise festgehalten werden.
- Neue Anforderungen MÜSSEN zeitnah berücksichtigt werden.

## CON.3.A2 Festlegung der Verfahrensweisen für die Datensicherung [Fachverantwortliche, IT-Betrieb] (B)

- Der IT-Betrieb MUSS Verfahren festlegen, wie die Daten gesichert werden.
- Für die Datensicherungsverfahren MÜSSEN Art, Häufigkeit und Zeitpunkte der Datensicherungen bestimmt werden.
- Dies MUSS wiederum auf Basis der erhobenen Einflussfaktoren und in Abstimmung mit den jeweiligen Fachverantwortlichen geschehen.
- Auch MUSS definiert sein, welche Speichermedien benutzt werden und wie die Transport- und Aufbewahrungsmodalitäten ausgestaltet sein müssen.
- Datensicherungen MÜSSEN immer auf separaten Speichermedien für die Datensicherung gespeichert werden.
- Besonders schützenswerte Speichermedien für die Datensicherung SOLLTEN nur während der Datensicherung und Datenwiederherstellung mit dem Netz der Institution oder dem Ursprungssystem verbunden werden.
- In virtuellen Umgebungen sowie für Storage-Systeme SOLLTE geprüft werden, ob das IT-System ergänzend durch Snapshot-Mechanismen gesichert werden kann, um hierdurch mehrere schnell wiederherstellbare Zwischenversionen zwischen den vollständigen Datensicherungen zu erstellen.

## CON.3.A3 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## CON.3.A4 Erstellung von Datensicherungsplänen [IT-Betrieb] (B)

- Der IT-Betrieb MUSS Datensicherungspläne je IT-System oder Gruppe von IT-Systemen auf Basis der festgelegten Verfahrensweise für die Datensicherung erstellen.
- Diese MÜSSEN festlegen, welche Anforderungen für die Daten-sicherung mindestens einzuhalten sind.
- Die Datensicherungpläne MÜSSEN mindestens eine kurze Beschreibung dazu enthalten:
    - welche IT-Systeme und welche darauf befindlichen Daten durch welche Datensicherung gesichert werden,
    - in welcher Reihenfolge IT-System und Anwendungen wiederhergestellt werden,
    - wie die Datensicherungen erstellt und wiederhergestellt werden können,
    - wie lange Datensicherungen aufbewahrt werden,
    - wie die Datensicherungen vor unbefugtem Zugriff und Überschreiben gesichert werden,
    - welche Parameter zu wählen sind sowie
    - welche Hard- und Software eingesetzt wird.

## CON.3.A5 Regelmäßige Datensicherung [IT-Betrieb, Mitarbeiter] (B)

- Regelmäßige Datensicherungen MÜSSEN gemäß den Datensicherungsplänen erstellt werden.
- Alle Mitarbeiter MÜSSEN über die Regelungen zur Datensicherung informiert sein.
- Auch MÜSSEN sie darüber informiert werden, welche Aufgaben sie bei der Erstellung von Datensicherungen haben.

## CON.3.A12 Sichere Aufbewahrung der Speichermedien für die Datensicherungen [IT-Betrieb] (B)

- Die Speichermedien für die Datensicherung MÜSSEN räumlich getrennt von den gesicherten IT-Systemen aufbewahrt werden.
- Sie SOLLTEN in einem anderen Brandabschnitt aufbewahrt werden.
- Der Aufbewahrungsort SOLLTE so klimatisiert sein, dass die Datenträger entsprechend der zeitlichen Vorgaben des Datensicherungskonzepts aufbewahrt werden können.

## CON.3.A14 Schutz von Datensicherungen [IT-Betrieb] (B)

- Die erstellten Datensicherungen MÜSSEN in geeigneter Weise vor unbefugtem Zugriff geschützt werden.
- Hierbei MUSS insbesondere sichergestellt werden, dass Datensicherungen nicht absichtlich oder unbeabsichtigt überschrieben werden können.
- IT-Systeme, die für die Datensicherung eingesetzt werden, SOLLTEN einen schreibenden Zugriff auf die Speichermedien für die Datensicherung nur für autorisierte Datensicherungen oder autorisierte Administrationstätigkeiten gestatten.
- Alternativ SOLLTEN die Speichermedien für die Datensicherung nur für autorisierte Datensicherungen oder autorisierte Administrationstätigkeiten mit den entsprechenden IT-Systemen verbunden werden.

## CON.3.A15 Regelmäßiges Testen der Datensicherungen [IT-Betrieb] (B)

- Es MUSS regelmäßig getestet werden, ob die Datensicherungen wie gewünscht funktionieren, vor allem, ob gesicherte Daten einwandfrei und in angemessener Zeit zurückgespielt werden können.

## CON.3.A6 Entwicklung eines Datensicherungskonzepts [Fachverantwortliche, IT-Betrieb] (S)

- Die Institution SOLLTE ein Datensicherungskonzept erstellen, dass mindestens die nachfolgenden Punkte umfasst:
    - Definitionen zu wesentlichen Aspekten der Datensicherung (z. B. unterschiedliche Verfahrensweisen zur Datensicherung),
    - Gefährdungslage,
    - Einflussfaktoren je IT-System oder Gruppe von IT-Systemen,
    - Datensicherungspläne je IT-System oder Gruppe von IT-Systemen sowie
    - relevante Ergebnisse des Notfallmanagements/BCM, insbesondere die Recovery Point Objective (RPO) je IT-System oder Gruppe von IT-Systemen.
- Der IT-Betrieb SOLLTE das Datensicherungskonzept mit den jeweiligen Fachverantwortlichen der betreffenden Anwendungen abstimmen.
- Wird ein zentrales Datensicherungssystem für die Sicherung der Daten eingesetzt, SOLLTEbeachtet werden, dass sich aufgrund der Konzentration der Daten ein höherer Schutzbedarf ergeben kann.
- Datensicherungen SOLLTEN regelmäßig gemäß dem Datensicherungskonzept durchgeführt werden.
- Das Datensicherungskonzept selbst SOLLTE auch in einer Datensicherung enthalten sein.
- Die im Datensicherungskonzept enthaltenen technischen Informationen, um Systeme und Datensicherungen wiederherzustellen (Datensicherungspläne), SOLLTEN in der Art gesichert werden, dass Sie auch verfügbar sind, wenn die Datensicherungssysteme selbst ausfallen.
- Die Mitarbeiter SOLLTEN über den Teil des Datensicherungskonzepts unterrichtet werden, der sie betrifft.
- Regelmäßig SOLLTE kontrolliert werden, ob das Datensicherungskonzept korrekt umgesetzt wird.

## CON.3.A7 Beschaffung eines geeigneten Datensicherungssystems [IT-Betrieb] (S)

- Bevor ein Datensicherungssystem beschafft wird, SOLLTE der IT-Betrieb eine Anforderungsliste erstellen, nach der die am Markt erhältlichen Produkte bewertet werden.
- Die angeschafften Datensicherungssysteme SOLLTEN die Anforderungen des Datensicherungskonzepts der Institution erfüllen.

## CON.3.A8 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## CON.3.A9 Voraussetzungen für die Online-Datensicherung [IT-Betrieb] (S)

- Wenn für die Datensicherung ein Online-Speicher genutzt werden soll, SOLLTEN mindestens folgende Punkte vertraglich geregelt werden:
    - Gestaltung des Vertrages,
    - Ort der Datenspeicherung,
    - Vereinbarungen zur Dienstgüte (SLA), insbesondere in Hinsicht auf die Verfügbarkeit,
    - geeignete Authentisierungsmethoden für den Zugriff,
    - Verschlüsselung der Daten auf dem Online-Speicher sowie
    - Verschlüsselung auf dem Transportweg.
- Zudem SOLLTEN Sicherungssystem und Netzanbindung so beschaffen sein, dass die zulässigen Sicherungs- bzw. Wiederherstellungszeiten nicht überschritten werden.

## CON.3.A10 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## CON.3.A11 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## CON.3.A13 Einsatz kryptografischer Verfahren bei der Datensicherung [IT-Betrieb] (H)

- Um die Vertraulichkeit der gesicherten Daten zu gewährleisten, SOLLTE der IT-Betrieb alle Datensicherungen verschlüsseln.
- Es SOLLTE sichergestellt werden, dass sich die verschlüsselten Daten auch nach längerer Zeit wieder einspielen lassen.
- Verwendete kryptografische Schlüssel SOLLTEN mit einer getrennten Datensicherung geschützt werden.


