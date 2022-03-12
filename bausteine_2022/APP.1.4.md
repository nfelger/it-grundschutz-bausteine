# APP.1.4: Mobile Anwendungen (Apps)

## APP.1.4.A1 Anforderungsanalyse für die Nutzung von Apps [Fachverantwortliche] (B)

- In der Anforderungsanalyse MÜSSEN insbesondere Risiken betrachtet werden, die sich aus der mobilen Nutzung ergeben.
- Die Institution MUSS prüfen, ob ihre Kontroll- und Einflussmöglichkeiten auf die Betriebssystemumgebung mobiler Endgeräte ausreichend sind, um sie sicher nutzen zu können.

## APP.1.4.A2 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.1.4.A4 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.1.4.A5 Minimierung und Kontrolle von App-Berechtigungen [Fachverantwortliche] (B)

- Sicherheitsrelevante Berechtigungseinstellungen MÜSSEN so fixiert werden, dass sie nicht durch Benutzer oder Apps geändert werden können.
- Wo dies technisch nicht möglich ist, MÜSSEN die Berechtigungseinstellungen regelmäßig geprüft und erneut gesetzt werden.
- Bevor eine App in einer Institution eingeführt wird, MUSS sichergestellt werden, dass sie nur die minimal benötigten App-Berechtigungen für ihre Funktion erhält.
- Nicht unbedingt notwendige Berechtigungen MÜSSEN hinterfragt und gegebenenfalls unterbunden werden.

## APP.1.4.A6 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.1.4.A7 Sichere Speicherung lokaler App-Daten (B)

- Wenn Apps auf interne Dokumente der Institution zugreifen können, MUSS sichergestellt sein, dass die lokale Datenhaltung der App angemessen abgesichert ist.
- Insbesondere MÜSSEN Zugriffsschlüssel verschlüsselt abgelegt werden.
- Außerdem DÜRFEN vertrauliche Daten NICHT vom Betriebssystem an anderen Ablageorten zwischengespeichert werden.

## APP.1.4.A8 Verhinderung von Datenabfluss (B)

- Um zu verhindern, dass Apps ungewollt vertrauliche Daten versenden oder aus den gesendeten Daten Profile über die Benutzer erstellt werden, MUSS die App-Kommunikation geeignet eingeschränkt werden.
- Dazu SOLLTE die Kommunikation im Rahmen des Test- und Freigabeverfahrens analysiert werden.
- Weiterhin SOLLTE überprüft werden, ob eine App ungewollte Protokollierungs- oder Hilfsdateien schreibt, die möglicherweise vertrauliche Informationen enthalten.

## APP.1.4.A3 Verteilung schutzbedürftiger Apps (S)

- Interne Apps der Institution und Apps, die schutzbedürftige Informationen verarbeiten, SOLLTEN über einen institutionseigenen App Store oder via MDM verteilt werden.

## APP.1.4.A9 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.1.4.A10 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.1.4.A11 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.1.4.A12 Sichere Deinstallation von Apps (S)

- Werden Apps deinstalliert, SOLLTEN auch Daten gelöscht werden, die auf externen Systemen, beispielsweise beim App-Anbieter, gespeichert wurden.

## APP.1.4.A13 ENTFALLEN (H)

- Diese Anforderung ist entfallen.

## APP.1.4.A14 Unterstützung zusätzlicher Authentisierungsmerkmale bei Apps (H)

- Falls möglich, SOLLTE für die Authentisierung der Benutzer in Apps ein zweiter Faktor benutzt werden.
- Hierbei SOLLTE darauf geachtet werden, dass eventuell benötigte Sensoren oder Schnittstellen in allen verwendeten Geräten vorhanden sind.
- Zusätzlich SOLLTE bei biometrischen Verfahren berücksichtigt werden, wie resistent die Authentisierung gegen mögliche Fälschungsversuche ist.

## APP.1.4.A15 Durchführung von Penetrationstests für Apps (H)

- Bevor eine App für den Einsatz freigegeben wird, SOLLTE ein Penetrationstest durchgeführt werden.
- Dabei SOLLTEN alle Kommunikationsschnittstellen zu Backend-Systemen sowie die lokale Speicherung von Daten auf mögliche Sicherheitslücken untersucht werden.
- Die Penetrationstests SOLLTEN regelmäßig und zusätzlich bei größeren Änderungen an der App wiederholt werden.

## APP.1.4.A16 Mobile Application Management (H)

- Falls möglich, SOLLTE für das zentrale Konfigurieren von dienstlichen Apps ein Mobile Application Management verwendet werden.


