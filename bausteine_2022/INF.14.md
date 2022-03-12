# INF.14: Gebäudeautomation

## INF.14.A1 Planung der Gebäudeautomation (B) [Planer]

- Für die von der Gebäudeautomation (GA) gesteuerten Gewerke MUSS festgelegt werden, wie die GA sicher gestaltet werden kann.
- Die GA MUSS bereits bei der Planung von Neubau, Umbau, Erweiterung und Sanierung eines Gebäudes berücksichtigt werden.
- Daher MUSS die GA in den Planungs- und Bauprozessen, auch in Verbindung mit Building Information Modeling (BIM), für alle GA-relevanten Komponenten und TGA-Anlagen berücksichtigt werden.
- Im Rahmen der GA-Planung MÜSSEN die einzurichtenden GA-Systeme spezifiziert werden.
- Es MUSS festgelegt werden, in welchem Umfang TGA-Anlagen über das GA-System automatisiert gesteuert werden sollen.
- Die GA SOLLTE so geplant werden, dass zur Kopplung und Integration der TGA-Anlagen möglichst wenig unterschiedliche GA-Systeme sowie Kommunikationsprotokolle und -schnittstellen genutzt werden.
- Es SOLLTEN sichere und standardisierte Protokolle und Schnittstellen eingesetzt werden.
- Für eine Entscheidung hinsichtlich der notwendigen Systeme, Protokolle und Schnittstellen SOLLTE die erwartete Funktionalität gegenüber einem gegebenenfalls erhöhten Aufwand für Betriebs- und Informationssicherheit abgewogen werden.
- Die Planung SOLLTE dokumentiert, regelmäßig und zusätzlich bei Bedarf aktualisiert und dem Stand der Technik angepasst werden.
- Darüber hinaus SOLLTE die Planung regelmäßig und zusätzlich bei Bedarf mit der aktuellen Konfiguration verglichen werden (Soll-Ist-Vergleich).

## INF.14.A2 Festlegung eines Inbetriebnahme- und Schnittstellenmanagements für die GA (B)

- Aufgrund der Vielzahl von TGA-Anlagen und Komponenten in Gebäuden, die in GA-Systemen angebunden werden, MUSS der Ablauf zur Inbetriebnahme der involvierten TGA-Anlagen und GA-relevanten Komponenten aufeinander abgestimmt und übergreifend festgelegt werden.
- Dieser Ablauf MUSS koordiniert umgesetzt werden, um ein voll funktionsfähiges Gebäude zu gewährleisten.
- Ebenso MÜSSEN klare Schnittstellen zwischen den Betreiberorganisationen der GA und der GA-relevanten Komponenten sowie den Betreiberorganisationen der TGA-Anlagen definiert werden.
- Inbetriebnahme- und Schnittstellenmanagement MÜSSEN dokumentiert werden.
- Sowohl regelmäßig als auch zusätzlich bei Bedarf MÜSSEN die Festlegungen geprüft und gegebenenfalls nachjustiert werden.
- Insbesondere bei Änderungen innerhalb der GA-Systeme MÜSSEN die Festlegungen angepasst werden.

## INF.14.A3 Sichere Anbindung von TGA-Anlagen und GA-Systemen (B)

- Für alle TGA-Anlagen, GA-Systeme und GA-relevanten Komponenten MUSS festgelegt werden, ob durch andere TGA-Anlagen, GA-Systeme oder GA-relevante Komponenten Aktionen ausgelöst werden dürfen.
- Falls eine solche Integration zulässig ist, SOLLTE reglementiert werden, welche automatisierten Aktionen durch welche Informationen eines GA-Systems ausgelöst werden dürfen.
- Falls eine TGA-Anlage nicht in ein GA-System integriert werden kann oder darf, diese jedoch an ein GA-System gekoppelt werden soll, MUSS festgelegt werden, welche Informationen der TGA-Anlage an das GA-System gemeldet werden.
- Sowohl die Integration von TGA-Anlagen in ein GA-System als auch die rückwirkungsfreie Kopplung von TGAAnlagen an GA-Systeme MÜSSEN angemessen abgesichert sein.
- Ebenfalls MUSS die Anbindung von GA-Systemen untereinander angemessen abgesichert werden.
- Hierzu MÜSSEN insbesondere die Ablauf- und Funktionsketten innerhalb eines GA-Systems bzw. zwischen GASystemen angemessen geplant werden.
- Hierbei MÜSSEN alle Übergänge zwischen Gewerken und Techniken berücksichtigt werden.
- Diese Ablauf- und Funktionsketten MÜSSEN umfassend getestet und bei Fehlverhalten nachjustiert werden.
- Die Festlegungen MÜSSEN vollumfänglich dokumentiert werden.
- Sowohl regelmäßig als auch ergänzend bei Bedarf SOLLTE geprüft werden, ob die Dokumentation noch aktuell ist.
- Bei Abweichungen MUSS die Ursache für die Abweichungen eruiert und behoben werden.

## INF.14.A4 Berücksichtigung von Gefahrenmeldeanlagen in der GA (B) [Planer]

- Gefahrenmeldeanlagen inklusive Sicherheitsanlagen MÜSSEN rückwirkungsfrei an GA-Systeme gekoppelt werden.
- Sie DÜRFEN NICHT in ein GA-System integriert werden.
- Für die netztechnische Anbindung MÜSSEN physisch getrennte Netzkomponenten und physisch getrennte Segmente genutzt werden.
- Werden Funknetze zur Kopplung genutzt, MÜSSEN solche TGA-Anlagen als Primärnutzer für die genutzten Frequenzbereiche festgelegt werden.
- Für die Kommunikation über Funknetze SOLLTEN zertifizierte Mechanismen genutzt werden.

## INF.14.A5 Dokumentation der GA (B)

- Für die GA MUSS die Vielzahl unterschiedlicher Komponenten und Zugänge dokumentiert werden.
- Die Dokumentation MUSS regelmäßig und bei Änderungen innerhalb der GA geprüft und angepasst werden.
- Insbesondere MÜSSEN auch alle deaktivierten physischen Kommunikationsschnittstellen, Protokolle und Zugänge bzw. Zugriffsmöglichkeiten zur GA dokumentiert werden.
- Darüber hinaus MÜSSEN alle Wechselwirkungen und Abhängigkeiten von GA-relevanten Komponenten sowie von TGA-Anlagen, die in GA-Systeme integriert oder mit GA-Systemen gekoppelt sind, dokumentiert werden.
- Die verfügbaren und genutzten Sicherheitseigenschaften der verwendeten Protokolle SOLLTEN dokumentiert werden.
- Die Dokumentation SOLLTE für alle GA-Systeme übergreifend hinsichtlich Inhalten und deren Datenstrukturen abgestimmt werden.

## INF.14.A6 Separierung von Netzen der GA (B) [Planer, IT-Betrieb]

- GA-Netze MÜSSEN von Büro-Netzen und sonstigen Netzen der Institution mindestens logisch getrennt werden.
- Jegliche Kommunikation zwischen GA-Systemen und sonstigen IT-Systemen MUSS kontrolliert und reglementiert werden.
- Hierfür MÜSSEN an allen Übergängen einer solchen Segmentierung entsprechende Komponenten mit Sicherheitsfunktionen, mindestens mit Firewall-Funktion, vorgesehen werden.
- Wird die GA für einen Gebäudekomplex oder eine Liegenschaft zentral eingerichtet, so MUSS die gebäudeübergreifende GA-Kommunikation über LAN-, WLAN-, WAN-, Funknetz- oder Internet-Verbindungen auch auf Ebene des Netzes separiert werden.

## INF.14.A7 Festlegung einer Sicherheitsrichtlinie für die GA (S)

- Ausgehend von der allgemeinen Sicherheitsleitlinie der Institution und der übergreifenden Sicherheitsrichtlinie für das TGM SOLLTEN die Sicherheitsanforderungen an die GA, d. h. für alle GA-Systeme, in einer GA-Sicherheitsrichtlinie konkretisiert werden.
- Diese Richtlinie SOLLTE allen Personen, die an Planung, Beschaffung, Implementierung und Betrieb der GA-Systeme beteiligt sind, bekannt und Grundlage für deren Arbeit sein.
- Die Inhalte und die Umsetzung der geforderten Richtlinieninhalte SOLLTEN regelmäßig überprüft, gegebenenfalls angepasst und die Ergebnisse der Prüfung nachvollziehbar dokumentiert werden.
- In der Sicherheitsrichtlinie SOLLTEN auch die Vorgaben an Entwicklung und Test für den Einsatz von GA-Systemen spezifiziert werden.

## INF.14.A8 Anforderungsspezifikation für GA-Systeme (S)

- Ausgehend von der GA-Sicherheitsrichtlinie SOLLTE für die GA eine übergreifende und für jedes GA-System eine eigene Anforderungsspezifikation erstellt werden.
- Aus den Anforderungen SOLLTEN sich alle wesentlichen Elemente für Architektur und Design des jeweiligen GA-Systems und der Kopplung von GA-Systemen ableiten lassen.
- Die Anforderungsspezifikation SOLLTE dokumentiert sowie regelmäßig und zusätzlich bei Bedarf dem Stand der Technik angepasst werden.
- Darüber hinaus SOLLTE regelmäßig die Umsetzung der Anforderungen geprüft werden.
- Es SOLLTEN in der GA ausschließlich Komponenten eingesetzt werden, die eine Authentisierung mindestens über einen änderbaren Nutzernamen und ein änderbares Passwort bereitstellen.

## INF.14.A9 Entwicklung eines GA-Konzepts (S)

- Ausgehend von der GA-Sicherheitsrichtlinie und den Anforderungsspezifikationen SOLLTE für die GA ein übergreifendes GA-Konzept entwickelt werden.
- Hieraus abgeleitet SOLLTEN für alle GA-Systeme detaillierte Konzepte entwickelt werden.
- In den Konzepten SOLLTEN mindestens folgende Punkte angemessen berücksichtigt werden:
    - alle in das jeweilige GA-System integrierten TGA-Anlagen,
    - alle mit dem jeweiligen GA-System gekoppelten TGA-Anlagen,
    - alle GA-relevanten Komponenten mit den jeweiligen Kommunikationsverbindungen.
- Die Konzepte SOLLTEN alle technischen und organisatorischen Vorgaben beschreiben.
- Die erstellten Konzepte SOLLTEN regelmäßig geprüft und gegebenenfalls aktualisiert werden.

## INF.14.A10 Bildung von unabhängigen GA-Bereichen (S) [Planer]

- In der GA SOLLTEN GA-Bereiche derart geplant und umgesetzt werden, dass Abhängigkeiten zwischen den GABereichen minimiert werden und GA-Bereiche unabhängig gesteuert werden können.
- Eine Störung in einem GABereich SOLLTE keine oder nur geringe Auswirkungen auf andere GA-Bereiche haben.
- Insbesondere SOLLTEN die Gebäude innerhalb eines Gebäudekomplexes oder einer Liegenschaft separat steuerbar sein.
- Die eingerichteten GA-Bereiche SOLLTEN auch im GA-Managementsystem entsprechend sichtbar sein.

## INF.14.A11 Absicherung von frei zugänglichen Ports und Zugängen der GA (S) [Planer]

- Der Anschluss von Komponenten, speziell von unautorisierten, unbekannten Komponenten und Fremdgeräten, SOLLTE insbesondere an frei zugänglichen Ethernet-Ports, USB-Ports und anderen Schnittstellen der GA kontrolliert und eingeschränkt werden.
- Der Anschluss einer unautorisierten oder unbekannten Komponente SOLLTE in die Ereignisprotokollierung aufgenommen werden.
- Eine direkte IP-basierte Kommunikation von solchen Komponenten mit Systemen der GA SOLLTE unterbunden werden (siehe INF.14.A13 Netzsegmentierung in der GA).
- Für frei zugängliche LAN- oder WLAN-Zugänge SOLLTE eine Netzzugangskontrolle gemäß IEEE 802.1X oder vergleichbare Sicherheitsmechanismen eingesetzt werden.
- Hiermit SOLLTEN unzureichend authentisierte und autorisierte Komponenten in getrennten Netzsegmenten positioniert werden.
- Frei zugängliche Schnittstellen für temporäre Wartungszwecke, wie beispielsweise USB-Ports an GA-Komponenten, SOLLTEN nur bei Bedarf aktiviert werden.

## INF.14.A12 Nutzung sicherer Übertragungsprotokolle für die GA (S)

- Für Konfiguration, Wartung und Steuerung von GA-relevanten Komponenten, die auf Ethernet und IP basieren, SOLLTEN sichere Protokolle eingesetzt werden, falls nicht über vertrauenswürdige Netzsegmente kommuniziert wird.
- Außerhalb vertrauenswürdiger Netzsegmente SOLLTE die Kommunikation über Ethernet und IP zwischen GA-Systemen verschlüsselt erfolgen.
- Die Verschlüsselung SOLLTE mit den jeweils aktuellen Verschlüsselungsmechanismen durchgeführt werden.

## INF.14.A13 Netzsegmentierung in der GA (S) [Planer]

- Innerhalb des GA-Netzes SOLLTE eine Netzsegmentierung umgesetzt werden, die bedarfsgerecht einzelne GA-Systeme, einzelne TGA-Anlagen oder einzelne Gruppen von TGA-Anlagen innerhalb eines GA-Systems voneinander trennt.
- Für die Übergänge zwischen den Segmenten SOLLTEN entsprechende Regeln definiert und zur Umsetzung Komponenten mit Sicherheitsfunktionen, mindestens zustandsbehaftete Paketfilter, genutzt werden.

## INF.14.A14 Nutzung eines GA-geeigneten Zugriffsschutzes (S)

- Für die GA SOLLTE ein Identitäts- und Berechtigungsmanagement gemäß Baustein ORP.4 Identitäts- und Berechtigungsmanagement genutzt werden, das die Anforderungen der GA angemessen umsetzt.
- Hierfür SOLLTE bedarfsabhängig eine GA-eigene Authentisierungslösung oder eine geeignete Replikation einer zentralen Authentisierungslösung der Institution realisiert werden.
- In die Authentisierungslösung SOLLTEN soweit möglich alle GA-relevanten Komponenten eingebunden werden.
- Betreiber der GA-Systeme, Betreiber der TGA-Anlagen und auch Nachfrageorganisationen SOLLTEN im Rollen- und Berechtigungskonzept hinsichtlich der GA angemessen berücksichtigt werden.
- Dies SOLLTE insbesondere dann sorgfältig geplant und abgestimmt werden, wenn die GA institutionsübergreifend bereitgestellt wird.
- Alle GA-relevanten Komponenten, inklusive der Komponenten der Feldebene und Bedienelemente, SOLLTEN geeignete Funktionen zur Absicherung von Zugriffen umsetzen können.
- Komponenten, die keinen Zugriffsschutz bieten oder für die die vom Hersteller vorgegebenen Zugangsparameter nicht änderbar sind, SOLLTEN NICHT genutzt werden.

## INF.14.A15 Absicherung von GA-spezifischen Netzen (S)

- Sind in GA-spezifischen Netzen, wie z. B. BACnet, Sicherheitsmechanismen der Kommunikation verfügbar, SOLLTEN diese genutzt werden.
- Mindestens SOLLTEN Mechanismen zur Authentisierung und Verschlüsselung genutzt werden.
- Für GA-spezifische Netze, die keine angemessenen Sicherheitsmechanismen realisieren können, SOLLTE erwogen werden, diese auf ein GA-spezifisches Netz mit angemessenen Sicherheitsmechanismen umzustellen.
- Grundsätzlich SOLLTE die Kommunikation mit GA-spezifischen Netzen durch Koppelelemente mit Sicherheitsfunktionen kontrolliert und gegebenenfalls reglementiert werden.

## INF.14.A16 Absicherung von drahtloser Kommunikation in GA-Netzen (S) [Planer]

- In GA-Netzen, die auf einer drahtlosen Kommunikation wie z. B. EnOcean basieren, SOLLTEN die Sicherheitsmechanismen der jeweiligen Funktechnik zur Absicherung der Kommunikation genutzt werden.
- Insbesondere SOLLTEN eine angemessene Authentisierung und eine Verschlüsselung auf der Luftschnittstelle umgesetzt werden.
- Ist dies für die entsprechenden Endgeräte nicht möglich, SOLLTE für diese Endgeräte die Kommunikation am Übergang in kabelgebundene Netze kontrolliert werden, z. B. durch eine Komponente mit Firewall-Funktion.
- Darüber hinaus SOLLTEN mögliche Störungen für die Ausbreitung der Funkwellen, beispielsweise durch Abschattungen, bei der Planung der GA-Netze berücksichtigt werden.

## INF.14.A17 Absicherung von Mobilfunkkommunikation in GA-Netzen (S) [Planer]

- Wird im Rahmen der GA Mobilfunk eingesetzt, SOLLTEN für solche GA-Netze die Sicherheitsmechanismen der jeweiligen Mobilfunknetze genutzt werden.
- Werden öffentliche Mobilfunknetze wie 5G oder Sigfox in der GA verwendet, SOLLTE eine unkontrollierte direkte IP-basierte Kommunikation mit GA-relevanten Komponenten unterbunden werden.
- GA-Komponenten SOLLTEN nur dann mit einem dedizierten Anschluss an ein öffentliches Mobilfunknetz ausgestattet werden, falls dieser für deren Betrieb essenziell ist.
- Hierfür SOLLTE geprüft und festgelegt werden, für welche GA-Komponenten ein Anschluss an öffentliche Mobilfunknetze notwendig ist.
- Sofern im öffentlichen Mobilfunknetz keine Trennung der GA-Netze möglich ist, wie z. B. bei 5G mit Slicing, SOLLTE im Kommunikationspfad eine Entkopplung der IP-Kommunikation durch ein Application Layer Gateway (ALG) stattfinden.
- Falls Mobilfunktechniken in der GA als Bestandteil der öffentlichen Mobilfunkinfrastruktur eines Mobilfunkbetreibers eingesetzt werden, SOLLTEN mit den Mitteln der entsprechenden Mobilfunktechnik ein oder mehrere virtuelle Mobilfunknetze realisiert werden, die ausschließlich der GA zur Verfügung stehen.
- Falls in der GA mit Hilfe von Mobilfunktechniken wie LTE und 5G autarke private Mobilfunknetze lokal auf dem Campus eingerichtet werden, SOLLTE der Übergang zwischen diesen Mobilfunknetzen und den sonstigen Netzen durch ein Koppelelement mit Firewall-Funktion abgesichert werden.
- Auch für private Mobilfunknetze SOLLTE eine Segmentierung in mehrere virtuelle Mobilfunknetze umgesetzt werden.

## INF.14.A18 Sichere Anbindung von GA-externen Systemen (S)

- Die Kommunikation von GA-Systemen mit GA-externen Systemen SOLLTE ausschließlich über definierte Schnittstellen und mit definierten IT-Systemen möglich sein.
- Die Kommunikation SOLLTE authentisiert und verschlüsselt werden.
- Die möglichen Schnittstellen zu GA-externen Systemen SOLLTEN auf das notwendige Maß beschränkt werden.

## INF.14.A19 Nutzung dedizierter Adressbereiche für GA-Netze (S) [Planer]

- Für die GA SOLLTEN dedizierte Adressbereiche genutzt werden, die sich insbesondere von den Adressbereichen der Büro-IT und der OT unterscheiden.
- Für diese Adressbereiche SOLLTE festgelegt werden, aus welchen Bereichen statische Adressen vergeben werden und welche GA-relevanten Komponenten statische Adressen erhalten.
- Falls an die GA angebundene Netzbereiche wie TGA-Anlagen identische Adressbereiche nutzen (Replizieren von Anlagenkonfigurationen), MÜSSEN diese in getrennten Segmenten positioniert werden, um Adresskonflikte zu unterbinden.
- In diesem Fall MUSS die segmentübergreifende Kommunikation durch entsprechende Mechanismen abgesichert werden, beispielsweise durch den Einsatz eines ALG oder von Network Address Translation (NAT).

## INF.14.A20 Vermeidung von Broadcast-Kommunikation in GA-Netzen (S) [Planer]

- In GA-Netzen SOLLTE die Broadcast-Last auf OSI Layer 2 oder OSI Layer 3 für unbeteiligte Systeme und Komponenten minimiert werden, um eine Überlastung zu vermeiden.
- Hierzu SOLLTE die Kommunikation auf gruppenspezifische Multicasts umgestellt oder in der Planung der Segmentierung entsprechend berücksichtigt werden.

## INF.14.A21 Anzeigen der Gültigkeit von Informationen in GA-Systemen (S)

- Ein GA-System SOLLTE visualisieren, ob die angezeigten Informationen bezüglich Zeit, Ort, Wert, Zustand oder Ereignis auf planmäßig erhaltenen Informationen basieren.
- Informationen, die simulierte oder „eingefrorene“ Werte anzeigen, SOLLTEN abhängig vom Schutzbedarf der TGA-Anlagen erkennbar sein oder einen Alarm auslösen.

## INF.14.A22 Sicherstellung von autark funktionierenden GA-Systemen und TGA-Anlagen (S) [Planer]

- Innerhalb eines GA-Systems SOLLTE sichergestellt werden, dass TGA-Anlagen gemäß ihrem Schutzbedarf auch unabhängig von der Anbindung an das GA-System autark funktionieren.
- Insbesondere SOLLTEN GA-Systeme so konfiguriert werden, dass keine betriebsverhindernden Abhängigkeiten zum TGM, zu anderen GA-Systemen oder TGA-Anlagen bestehen.
- Eine TGA-Anlage SOLLTE auch bei Ausfall der Verbindung zur GA für einen bestimmten Zeitraum gemäß dem jeweiligen Schutzbedarf betriebsfähig bleiben und ihre Funktion wahrnehmen.

## INF.14.A23 Einsatz von physisch robusten Komponenten für die GA (S) [Planer]

- Abhängig von den Einsatzbedingungen der Komponenten in der GA SOLLTEN entsprechend physisch robuste Komponenten eingesetzt werden, die besonders auch für harsche Umgebungsbedingungen vorgesehen bzw. ausgewiesen sind.
- Sind angemessen robuste Komponenten nicht verfügbar, SOLLTEN entsprechende Kompensationsmaßnahmen ergriffen werden.

## INF.14.A24 Zeitsynchronisation für die GA (S)

- Alle in einem GA-System angebundenen Komponenten und TGA-Anlagen SOLLTEN eine synchrone Uhrzeit nutzen, um ein automatisiertes Messen, Steuern und Regeln zu gewährleisten (siehe auch APP.3.7 NTP-Zeitsynchronisation).
- Auch GA-Systeme, die miteinander verbunden sind, SOLLTEN eine synchrone Uhrzeit nutzen.
- Erstreckt sich die GA über Gebäudekomplexe oder Liegenschaften, SOLLTE die Zeitsynchronisation für alle Gebäude gewährleistet werden.
- Falls innerhalb eines GA-Systems eine Kommunikation mit Echtzeit-Anforderungen erforderlich ist, SOLLTE für die Zeitsynchronisation PTP oder ein vergleichbarer Mechanismus anstelle von NTP genutzt werden.

## INF.14.A25 Dediziertes Monitoring in der GA (S)

- Für alle Komponenten, die für die GA betriebsrelevant sind, SOLLTE ein geeignetes Monitoringkonzept erstellt und umgesetzt werden.
- Hierbei SOLLTEN die Verfügbarkeit sowie bedeutsame Parameter der GA-relevanten Komponenten laufend überwacht werden.
- Fehlerzustände sowie die Überschreitung definierter Grenzwerte SOLLTEN automatisch an die Betreiberorganisation gemeldet werden.
- Es SOLLTEN durch die GA mindestens Alarme ausgelöst werden, wenn TGA-Anlagen ausfallen oder wichtige Funktionen zum automatisierten Steuern und Regeln nicht verfügbar sind.
- Zudem SOLLTE festgelegt werden, für welche besonders sicherheitsrelevanten Ereignisse und für welche weiteren Ereignisse automatische Alarmmeldungen generiert werden.
- Statusmeldungen und Monitoringdaten SOLLTEN NUR über sichere Kommunikationswege übertragen werden.

## INF.14.A26 Protokollierung in der GA (S)

- Ergänzend zu OPS.1.1.5 Protokollierung SOLLTEN Statusänderungen an GA-relevanten Komponenten und sicherheitsrelevante Ereignisse protokolliert werden.
- Zusätzlich SOLLTEN alle schreibenden Konfigurationszugriffe auf TGA-Anlagen und gegebenenfalls GA-relevante Komponenten sowie alle manuellen und automatisierten Änderungen der Zustände von diesen protokolliert werden.
- Es SOLLTE festgelegt werden, welche Protokollierungsdaten auf einer zentralen Protokollierungsinstanz zusammengeführt werden.
- Protokollierungsdaten SOLLTEN NUR über sichere Kommunikationswege übertragen werden.

## INF.14.A27 Berücksichtigung von Wechselwirkungen zwischen Komponenten der GA in der Notfallplanung (S)

- Es SOLLTE initial und in regelmäßigen Abständen nachvollziehbar analysiert werden, wie sich die GA und die abgeleiteten Planungen und Konzepte auf die Notfallplanung auswirken.
- Insbesondere SOLLTE festgelegt werden, wie bei einem Ausfall von TGA-Anlagen oder GA-relevanten Komponenten durch technischen Defekt oder Angriff die Wechselwirkungen auf andere TGA-Anlagen, GA-relevante Systeme und TGM minimiert werden können.
- Im Rahmen der Notfallplanung SOLLTE auch festgelegt werden, welches Wartungspersonal für die betroffenen TGA-Anlagen und GA-relevanten Systeme zuständig ist und über welche Meldewege dieses erreicht werden kann.
- Außerdem SOLLTE festgelegt werden, welche Berechtigungen das Wartungspersonal zur Behebung von Notfällen hat.
- Es SOLLTE in der Notfallplanung auch spezifiziert werden, wie bei Ausfall der GA-Systeme ein gegebenenfalls erforderlicher Notbetrieb von TGA-Anlagen sichergestellt wird.
- Dabei SOLLTE für alle TGA-Anlagen und GA-Systeme inklusive aller GA-relevanten Komponenten eine Wiederanlaufreihenfolge festgelegt und in den entsprechenden Wiederanlaufplänen dokumentiert werden.

## INF.14.A28 Physische Trennung der GA (H) [Planer]

- Bei erhöhtem Schutzbedarf SOLLTEN GA-Netze als physisch getrennte Zonen gemäß Baustein NET.1.1 Netzarchitektur und -design realisiert werden.
- Abhängig vom Schutzbedarf SOLLTE für die Anbindung beispielsweise an Hersteller-Clouds ein dedizierter, restriktiv reglementierter Internet-Zugang bereitgestellt werden.
- Ebenfalls SOLLTEN, abhängig vom Schutzbedarf der GA-Systeme, Anbindungen an nicht vertrauenswürdige Netze, gegebenenfalls auch Anbindungen an institutionseigene Büro- oder OT-Netze, unterbunden werden.

## INF.14.A29 Trennung einzelner TGA-Anlagen (H)

- Um einzelne TGA-Anlagen mit erhöhtem Schutzbedarf innerhalb eines GA-Systems abzusichern, SOLLTEN solche TGA-Anlagen in separaten Netzsegmenten positioniert werden.
- Zur Kontrolle der Kommunikation SOLLTEN Firewall-Funktionen unmittelbar vor dem Anlagennetz positioniert werden.

## INF.14.A30 Bereitstellung eines GA-eigenen Zeitservers zur Zeitsynchronisation (H)

- Bei erhöhtem Schutzbedarf SOLLTE für die GA oder auch für einzelne GA-Systeme ein eigener GA-Zeitserver bereitgestellt werden, der direkt mit einer Atom- oder Funkuhr (Stratum 0) gekoppelt ist und an den gegebenenfalls weitere nachgelagerte GA-Zeitserver angebunden werden.


