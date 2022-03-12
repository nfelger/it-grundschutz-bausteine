# NET.2.1: WLAN-Betrieb

## NET.2.1.A1 Festlegung einer Strategie für den Einsatz von WLANs (B)

- Bevor in einer Institution WLANs eingesetzt werden, MUSS festgelegt sein, welche generelle Strategie die Institution im Hinblick auf die Kommunikation über WLANs plant.
- Insbesondere MUSS geklärt und festgelegt werden, in welchen Organisationseinheiten, für welche Anwendungen und zu welchem Zweck WLANs eingesetzt und welche Informationen darüber übertragen werden dürfen.
- Ebenso MUSS der Abdeckungsbereich des WLAN festgelegt werden.
- Außerdem MUSS schon in der Planungsphase festgelegt sein, wer für die Administration der unterschiedlichen WLAN-Komponenten zuständig ist, welche Schnittstellen es zwischen den am Betrieb beteiligten Verantwortlichen gibt und wann welche Informationen zwischen den Zuständigen ausgetauscht werden müssen.

## NET.2.1.A2 Auswahl eines geeigneten WLAN-Standards [Planer] (B)

- Im Rahmen der WLAN-Planung MUSS zuerst ermittelt werden, welche der von der Institution betriebenen Geräte (z. B. Mikrowellengeräte, Bluetooth-Geräte) in das ISM-Band bei 2,4 GHz sowie in das 5 GHz-Band abstrahlen.
- Außerdem MÜSSEN die vorhandenen Sicherheitsmechanismen der einzelnen WLAN-Standards gegeneinander abgewogen werden.
- Generell MUSS sichergestellt sein, dass nur als allgemein sicher anerkannte Verfahren zur Authentisierung und Verschlüsselung eingesetzt werden.
- Die Entscheidungsgründe MÜSSEN dokumentiert werden.
- Geräte, die von anerkannt sicheren Verfahren auf unsichere zurückgreifen müssen, DÜRFEN NICHT mehr eingesetzt werden.

## NET.2.1.A3 Auswahl geeigneter Kryptoverfahren für WLAN [Planer] (B)

- Die Kommunikation über die Luftschnittstelle MUSS komplett kryptografisch abgesichert werden.
- Kryptografische Verfahren, die unsicherer als WPA2 sind, DÜRFEN NICHT mehr eingesetzt werden.
- Wird WPA2 mit Pre-Shared Keys (WPA2-PSK) verwendet, dann MUSS ein komplexer Schlüssel mit einer Mindestlänge von 20 Zeichen verwendet werden.

## NET.2.1.A4 Geeignete Aufstellung von Access Points [Haustechnik] (B)

- Access Points MÜSSEN zugriffs- und diebstahlsicher montiert werden.
- Wenn sie aufgestellt werden, MÜSSEN die erforderlichen Bereiche ausreichend abgedeckt werden.
- Darüber hinaus MUSS darauf geachtet werden, dass sich die Funkwellen in Bereichen, die nicht durch das WLAN versorgt werden sollen, möglichst nicht ausbreiten.
- Außeninstallationen MÜSSEN vor Witterungseinflüssen und elektrischen Entladungen geeignet geschützt werden.

## NET.2.1.A5 Sichere Basis-Konfiguration der Access Points (B)

- Access Points DÜRFEN NICHT in der Konfiguration des Auslieferungszustandes verwendet werden.
- Voreingestellte SSIDs (Service Set Identifiers), Zugangskennwörter oder kryptografische Schlüssel MÜSSEN vor dem produktiven Einsatz geändert werden.
- Außerdem MÜSSEN unsichere Administrationszugänge abgeschaltet werden.
- Access Points DÜRFEN NUR über eine geeignet verschlüsselte Verbindung administriert werden.

## NET.2.1.A6 Sichere Konfiguration der WLAN-Infrastruktur (B)

- Es MUSS sichergestellt sein, dass mittels der WLAN-Kommunikation keine Sicherheitszonen gekoppelt werden und hierdurch etablierte Schutzmaßnahmen umgangen werden.

## NET.2.1.A7 Aufbau eines Distribution Systems [Planer] (B)

- Bevor ein kabelgebundenes Distribution System aufgebaut wird, MUSS prinzipiell entschieden werden, ob physisch oder logisch durch VLANs auf den Access Switches des kabelbasierten LANs getrennt wird.

## NET.2.1.A8 Verhaltensregeln bei WLAN-Sicherheitsvorfällen (B)

- Bei einem Sicherheitsvorfall MUSS der IT-Betrieb passende Gegenmaßnahmen einleiten:
    - Am Übergabepunkt der WLAN-Kommunikation ins interne LAN SOLLTE bei einem Angriff auf das WLAN die Kommunikation selektiv pro SSID, Access Point oder sogar für die komplette WLAN-Infrastruktur gesperrt werden.
    - Wurden Access Points gestohlen, MÜSSEN festgelegte Sicherheitsmaßnahmen umgesetzt werden, damit der Access Point oder hierauf abgespeicherte Informationen nicht missbraucht werden können.
    - Wurden WLAN-Clients entwendet und wird eine zertifikatsbasierte Authentisierung verwendet, MÜSSEN die Client-Zertifikate gesperrt werden.
- Es MUSS ausgeschlossen werden, dass entwendete Geräte unberechtigt verwendet werden, um auf das Netz der Institution zuzugreifen.

## NET.2.1.A9 Sichere Anbindung von WLANs an ein LAN [Planer] (S)

- Werden WLANs an ein LAN angebunden, SOLLTE der Übergang zwischen WLANs und LAN abgesichert werden, beispielsweise durch einen Paketfilter.
- Der Access Point SOLLTE unter Berücksichtigung der Anforderung NET.2.1.A7 Aufbau eines Distribution Systems eingebunden sein.

## NET.2.1.A10 Erstellung einer Sicherheitsrichtlinie für den Betrieb von WLANs (S)

- Ausgehend von der allgemeinen Sicherheitsrichtlinie der Institution SOLLTEN die wesentlichen Kernaspekte für einen sicheren Einsatz von WLANs konkretisiert werden.
- Die Richtlinie SOLLTE allen Verantwortlichen bekannt sein, die an Aufbau und Betrieb von WLANs beteiligt sind.
- Sie SOLLTE zudem Grundlage für ihre Arbeit sein.
- Die Umsetzung der in der Richtlinie geforderten Inhalte SOLLTE regelmäßig überprüft werden.
- Werden die Inhalte der Richtlinie nicht umgesetzt, MUSS geeignet reagiert werden.
- Die Ergebnisse SOLLTEN geeignet dokumentiert werden.

## NET.2.1.A11 Geeignete Auswahl von WLAN-Komponenten (S)

- Anhand der Ergebnisse der Planungsphase SOLLTE eine Anforderungsliste erstellt werden, mithilfe derer die am Markt erhältlichen Produkte bewertet werden können.
- Werden WLAN-Komponenten beschafft, SOLLTE neben Sicherheit auch auf Datenschutz und Kompatibilität der WLAN-Komponenten untereinander geachtet werden.

## NET.2.1.A12 Einsatz einer geeigneten WLAN-Management-Lösung (S)

- Eine zentrale Managementlösung SOLLTE eingesetzt werden.
- Der Leistungsumfang der eingesetzten Lösung SOLLTE im Einklang mit den Anforderungen der WLAN-Strategie sein.

## NET.2.1.A13 Regelmäßige Sicherheitschecks in WLANs (S)

- WLANs SOLLTEN regelmäßig daraufhin überprüft werden, ob eventuell Sicherheitslücken existieren.
- Zusätzlich SOLLTE regelmäßig nach unbefugt installierten Access Points innerhalb der bereitgestellten WLANs gesucht werden.
- Weiterhin SOLLTEN die Performance und Abdeckung gemessen werden.
- Die Ergebnisse von Sicherheitschecks SOLLTEN nachvollziehbar dokumentiert und mit dem Soll-Zustand abgeglichen werden.
- Abweichungen SOLLTEN untersucht werden.

## NET.2.1.A14 Regelmäßige Audits der WLAN-Komponenten (S)

- Bei allen Komponenten der WLAN-Infrastruktur SOLLTE regelmäßig überprüft werden, ob alle festgelegten Sicherheitsmaßnahmen umgesetzt sind.
- Außerdem SOLLTE überprüft werden ob alle Komponenten korrekt konfiguriert sind.
- Öffentlich aufgestellte Access Points SOLLTEN regelmäßig stichprobenartig daraufhin geprüft werden, ob es gewaltsame Öffnungs- oder Manipulationsversuche gab.
- Die Auditergebnisse SOLLTEN nachvollziehbar dokumentiert und mit dem Soll-Zustand abgeglichen werden.
- Abweichungen SOLLTEN untersucht werden.

## NET.2.1.A15 Verwendung eines VPN zur Absicherung von WLANs (H)

- Es SOLLTE ein VPN eingesetzt werden, um die Kommunikation über die WLAN-Infrastruktur zusätzlich abzusichern.

## NET.2.1.A16 Zusätzliche Absicherung bei der Anbindung von WLANs an ein LAN (H)

- Wird eine WLAN-Infrastruktur an ein LAN angebunden, SOLLTE der Übergang zwischen WLANs und LAN entsprechend des höheren Schutzbedarfs zusätzlich abgesichert werden.

## NET.2.1.A17 Absicherung der Kommunikation zwischen Access Points (H)

- Die Kommunikation zwischen den Access Points über die Funkschnittstelle und das LAN SOLLTE verschlüsselt erfolgen.

## NET.2.1.A18 Einsatz von Wireless Intrusion Detection/Wireless Intrusion Prevention Systemen (H)

- Es SOLLTEN Wireless Intrusion Detection Systeme bzw. Wireless Intrusion Prevention Systeme eingesetzt werden.


