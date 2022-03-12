# CON.1: Kryptokonzept

## CON.1.A1 Auswahl geeigneter kryptografischer Verfahren [Fachverantwortliche] (B)

- Es MÜSSEN geeignete kryptografische Verfahren ausgewählt werden.
- Dabei MUSS sichergestellt sein, dass etablierte Algorithmen verwendet werden, die von der Fachwelt intensiv untersucht wurden und von denen keine Sicherheitslücken bekannt sind.
- Ebenso MÜSSEN aktuell empfohlene Schlüssellängen verwendet werden.

## CON.1.A2 Datensicherung bei Einsatz kryptografischer Verfahren [IT-Betrieb] (B)

- In Datensicherungen MÜSSEN kryptografische Schlüssel vom IT-Betrieb derart gespeichert bzw. aufbewahrt werden, dass Unbefugte nicht darauf zugreifen können.
- Langlebige kryptografische Schlüssel MÜSSEN außerhalb der eingesetzten IT-Systeme aufbewahrt werden.
- Bei einer Langzeitspeicherung verschlüsselter Daten SOLLTE regelmäßig geprüft werden, ob die verwendeten kryptografischen Algorithmen und die Schlüssellängen noch dem Stand der Technik entsprechen.
- Der IT-Betrieb MUSS sicherstellen, dass auf verschlüsselt gespeicherte Daten auch nach längeren Zeiträumen noch zugegriffen werden kann.
- Verwendete Kryptoprodukte SOLLTEN archiviert werden.
- Die Konfigurationsdaten von Kryptoprodukten SOLLTEN gesichert werden.

## CON.1.A3 Verschlüsselung der Kommunikationsverbindungen (S)

- Es SOLLTE geprüft werden, ob mit vertretbarem Aufwand eine Verschlüsselung der Kommunikationsverbindungen möglich und praktikabel ist.
- Ist dies der Fall, SOLLTEN Kommunikationsverbindungen geeignet verschlüsselt werden.

## CON.1.A4 Geeignetes Schlüsselmanagement (S)

- Kryptografische Schlüssel SOLLTEN immer mit geeigneten Schlüsselgeneratoren und in einer sicheren Umgebung erzeugt werden.
- Ein Schlüssel SOLLTE möglichst nur einem Einsatzzweck dienen.
- Insbesondere SOLLTEN für die Verschlüsselung und Signaturbildung unterschiedliche Schlüssel benutzt werden.
- Der Austausch von kyptografischen Schlüsseln SOLLTE mit einem als sicher geltenden Verfahren durchgeführt werden.
- Wenn Schlüssel verwendet werden, SOLLTE die authentische Herkunft und die Integrität der Schlüsseldaten überprüft werden.
- Alle kryptografischen Schlüssel SOLLTEN hinreichend häufig gewechselt werden.
- Es SOLLTE eine festgelegte Vorgehensweise für den Fall geben, dass ein Schlüssel offengelegt wurde.
- Alle erzeugten kryptografischen Schlüssel SOLLTEN sicher aufbewahrt und verwaltet werden.

## CON.1.A5 Sicheres Löschen und Vernichten von kryptografischen Schlüsseln [IT-Betrieb] (S)

- Nicht mehr benötigte Schlüssel und Zertifikate SOLLTEN sicher gelöscht bzw. vernichtet werden.

## CON.1.A6 Bedarfserhebung für kryptografische Verfahren und Produkte [IT-Betrieb, Fachverantwortliche] (S)

- Es SOLLTE festgelegt werden, für welche Geschäftsprozesse oder Fachverfahren kryptografische Verfahren eingesetzt werden sollen.
- Danach SOLLTEN die Anwendungen, IT-Systeme und Kommunikationsverbindungen identifiziert werden, die notwendig sind, um die Aufgaben zu erfüllen.
- Diese SOLLTEN durch den IT-Betrieb geeignet kryptografisch abgesichert werden.

## CON.1.A7 Erstellung einer Sicherheitsrichtlinie für den Einsatz kryptografischer Verfahren und Produkte (H)

- Ausgehend von der allgemeinen Sicherheitsrichtlinie der Institution SOLLTE eine spezifische Richtlinie für den Einsatz von Kryptoprodukten erstellt werden.
- In der Sicherheitsrichtlinie SOLLTE geregelt werden, wer für den sicheren Betrieb der kryptografischen Produkte zuständig ist.
- Für die benutzten Kryptoprodukte SOLLTE es Vertretungsregelungen geben.
- Auch SOLLTEN notwendige Schulungs- und Sensibilisierungsmaßnahmen für Benutzer sowie Verhaltensregeln und Meldewege bei Problemen oder Sicherheitsvorfällen festgelegt werden.
- Weiter SOLLTE die Richtlinie definieren, wie sichergestellt wird, dass Kryptomodule sicher konfiguriert, korrekt eingesetzt und regelmäßig gewartet werden.
- Die Richtlinie SOLLTE allen relevanten Mitarbeitern bekannt und grundlegend für ihre Arbeit sein.
- Wird die Richtlinie verändert oder wird von ihr abgewichen, SOLLTE dies mit dem ISB abgestimmt und dokumentiert werden.
- Es SOLLTE regelmäßig überprüft werden, ob die Richtlinie noch korrekt umgesetzt wird.
- Die Ergebnisse SOLLTEN sinnvoll dokumentiert werden.

## CON.1.A8 Erhebung der Einflussfaktoren für kryptografische Verfahren und Produkte (H)

- Bevor entschieden werden kann, welche kryptografischen Verfahren und Produkte bei erhöhtem Schutzbedarf eingesetzt werden, SOLLTEN unter anderem folgende Einflussfaktoren ermittelt werden:
    - Sicherheitsaspekte (siehe CON.1.A6 Bedarfserhebung für kryptografische Verfahren und Produkte),
    - technische Aspekte,
    - personelle und organisatorische Aspekte,
    - wirtschaftliche Aspekte,
    - Lebensdauer von kryptografischen Verfahren und der eingesetzten Schlüssellängen,
    - Zulassung von kryptografischen Produkten sowie
    - gesetzliche Rahmenbedingungen.

## CON.1.A9 Auswahl eines geeigneten kryptografischen Produkts [IT-Betrieb, Fachverantwortliche] (H)

- Bevor ein kryptografisches Produkt ausgewählt wird, SOLLTE die Institution festlegen, welche Anforderungen das Produkt erfüllen muss.
- Dabei SOLLTEN Aspekte wie Funktionsumfang, Interoperabilität, Wirtschaftlichkeit sowie Fehlbedienungs- und Fehlfunktionssicherheit betrachtet werden.
- Es SOLLTE geprüft werden, ob zertifizierte Produkte vorrangig eingesetzt werden sollen.
- Auch die zukünftigen Einsatzorte SOLLTEN bei der Auswahl beachtet werden, da es z. B. Export- und Importbeschränkungen für kryptografische Produkte gibt.
- Auf Produkte mit unkontrollierbarer Schlüsselablage SOLLTE generell verzichtet werden.

## CON.1.A10 Entwicklung eines Kryptokonzepts (H)

- Es SOLLTE ein Kryptokonzept entwickelt werden, das in das Sicherheitskonzept der Institution integriert wird.
- Im Konzept SOLLTEN alle technischen und organisatorischen Vorgaben für die eingesetzten kryptografischen Produkte beschrieben werden.
- Auch SOLLTEN alle relevanten Anwendungen, IT-Systeme und Kommunikationsverbindungen aufgeführt sein.
- Das erstellte Kryptokonzept SOLLTE regelmäßig aktualisiert werden.

## CON.1.A11 Sichere Konfiguration der Kryptomodule [IT-Betrieb] (H)

- Kryptomodule SOLLTEN sicher installiert und konfiguriert werden.
- Alle voreingestellten Schlüssel SOLLTEN geändert werden.
- Anschließend SOLLTE getestet werden, ob die Kryptomodule korrekt funktionieren und vom Benutzer auch bedient werden können.
- Weiterhin SOLLTEN die Anforderungen an die Einsatzumgebung festgelegt werden.
- Wenn ein IT-System geändert wird, SOLLTE getestet werden, ob die eingesetzten kryptografischen Verfahren noch greifen.
- Die Konfiguration der Kryptomodule SOLLTE dokumentiert und regelmäßig überprüft werden.

## CON.1.A12 Sichere Rollenteilung beim Einsatz von Kryptomodulen [IT-Betrieb] (H)

- Bei der Konfiguration eines Kryptomoduls SOLLTEN Benutzerrollen festgelegt werden.
- Es SOLLTE mit Zugriffskontroll- und Authentisierungsmechanismen verifiziert werden, ob ein Mitarbeiter den gewünschten Dienst auch tat-sächlich benutzen darf.
- Das Kryptomodul SOLLTE so konfiguriert sein, dass bei jedem Rollenwechsel oder bei Inaktivität nach einer bestimmten Zeitdauer die Authentisierungsinformationen erneut eingegeben werden müssen.

## CON.1.A13 Anforderungen an die Betriebssystem-Sicherheit beim Einsatz von Kryptomodulen (H)

- Das Zusammenwirken von Betriebssystem und Kryptomodulen SOLLTE gewährleisten, dass
    - die installierten Kryptomodule nicht unbemerkt abgeschaltet oder umgangen werden können,
    - die angewendeten oder gespeicherten Schlüssel nicht kompromittiert werden können,
    - die zu schützenden Daten nur mit Wissen und unter Kontrolle des Benutzers auch unverschlüsselt auf Datenträgern abgespeichert werden bzw. das informationsverarbeitende System verlassen können sowie
    - Manipulationsversuche am Kryptomodul erkannt werden.

## CON.1.A14 Schulung von Benutzern und Administratoren [Vorgesetzte, Fachverantwortliche, IT-Betrieb] (H)

- Es SOLLTE Schulungen geben, in denen Benutzern und Administratoren der Umgang mit den für sie relevanten Kryptomodulen vermittelt wird.
- Den Benutzern SOLLTE genau erläutert werden, was die spezifischen Sicherheitseinstellungen von Kryptomodulen bedeuten und warum sie wichtig sind.
- Außerdem SOLLTEN sie auf die Gefahren hingewiesen werden, die drohen, wenn diese Sicherheitseinstellungen aus Bequemlichkeit umgangen oder deaktiviert werden.
- Die Schulungsinhalte SOLLTEN immer den jeweiligen Einsatzszenarien entsprechend angepasst werden.
- Die Administratoren SOLLTEN zudem gezielt dazu geschult werden, wie die Kryptomodule zu administrieren sind.
- Auch SOLLTEN sie einen Überblick über kryptografische Grundbegriffe erhalten.

## CON.1.A15 Reaktion auf praktische Schwächung eines Kryptoverfahrens (H)

- Es SOLLTE ein Prozess etabliert werden, der im Falle eines geschwächten kryptografischen Verfahrens herangezogen werden kann.
- Dabei SOLLTE sichergestellt werden, dass das geschwächte kryptografische Verfahren abgesichert werden kann oder durch eine geeignete Alternative abgelöst wird.

## CON.1.A16 Physische Absicherung von Kryptomodulen [IT-Betrieb] (H)

- Der IT-Betrieb SOLLTE sicherstellen, dass nicht unautorisiert physisch auf Modulinhalte des Kryptomoduls zugegriffen wird.
- Hard- und Softwareprodukte, die als Kryptomodule eingesetzt werden, SOLLTEN einen Selbsttest durchführen können.

## CON.1.A17 Abstrahlsicherheit [IT-Betrieb] (H)

- Es SOLLTE untersucht werden, ob zusätzliche Maßnahmen hinsichtlich der Abstrahlsicherheit notwendig sind.
- Dies SOLLTE insbesondere dann geschehen, wenn staatliche Verschlusssachen (VS) der Geheimhaltungsgrade VS-VERTRAULICH und höher verarbeitet werden.

## CON.1.A18 Kryptografische Ersatzmodule [IT-Betrieb] (H)

- Es SOLLTEN Ersatzkryptomodule vorrätig sein.


