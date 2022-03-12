# NET.4.2: VoIP

## NET.4.2.A1 Planung des VoIP-Einsatzes (B)

- Die Bedingungen, unter denen VoIP eingesetzt werden soll, MÜSSEN festgelegt werden.
- Es MUSS unter anderem entschieden werden, ob vollständig oder partiell auf VoIP umgestiegen werden soll.
- Besondere Anforderungen an die Verfügbarkeit von VoIP oder an die Vertraulichkeit und Integrität der Telefonate bzw. der Signalisierungsinformationen SOLLTEN vorab ermittelt werden.
- Geeignete Signalisierungs- und Medientransportprotokolle MÜSSEN vor dem Einsatz ausgewählt werden.
- Es SOLLTE entschieden werden, ob und wie die VoIP-Infrastruktur an öffentliche (Daten-)Netze angebunden werden soll.
- Die Kapazitäten und das Design von vorhandenen Datennetzen SOLLTEN bei der Planung berücksichtigt werden.

## NET.4.2.A2 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## NET.4.2.A3 Sichere Administration und Konfiguration von VoIP-Endgeräten (B)

- Nicht benötigte Funktionen der Endgeräte MÜSSEN deaktiviert werden.
- Die Konfigurationseinstellungen DÜRFEN NICHT unberechtigt geändert werden.
- Alle Sicherheitsfunktionen der Endgeräte SOLLTEN vor dem produktiven Einsatz getestet werden.
- Die eingesetzten Sicherheitsmechanismen und die verwendeten Parameter SOLLTEN dokumentiert werden.

## NET.4.2.A4 Einschränkung der Erreichbarkeit über VoIP (B)

- Es MUSS entschieden werden, wie externe Gesprächspartner auf die VoIP-Architektur zugreifen können.
- Es MUSS verhindert werden, dass IT-Systeme aus unsicheren Netzen direkte Datenverbindungen auf die VoIP-Komponenten der Institution aufbauen können.
- Wenn alle ein- und ausgehenden Verbindungen über ein zentrales IT-System abgewickelt werden sollen, SOLLTE sichergestellt werden, dass alle Signalisierungs- und Sprachinformationen zwischen dem öffentlichen und dem privaten Datennetz nur über dieses autorisierte IT-System ausgetauscht werden.

## NET.4.2.A5 Sichere Konfiguration der VoIP-Middleware (B)

- Die VoIP-Komponenten MÜSSEN so konfiguriert sein, dass sie den Schutzbedarf angemessen erfüllen.
- Die DefaultKonfigurationen der VoIP-Middleware MÜSSEN vor der produktiven Inbetriebnahme angepasst werden.
- Alle Installations- und Konfigurationsschritte SOLLTEN so dokumentiert werden, dass die Installation und Konfiguration durch einen sachkundigen Dritten anhand der Dokumentation nachvollzogen und wiederholt werden können.
- Alle nicht benötigten Dienste der VoIP-Middleware MÜSSEN deaktiviert werden.

## NET.4.2.A6 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## NET.4.2.A7 Erstellung einer Sicherheitsrichtlinie für VoIP (S)

- Die zentralen sicherheitstechnischen Anforderungen an VoIP sowie das zu erreichende Sicherheitsniveau SOLLTEN in der institutionsweiten Sicherheitsrichtlinie aufgenommen werden.
- In dieser Sicherheitsrichtlinie SOLLTEN alle allgemeinen sicherheitstechnischen Vorgaben konkretisiert werden.
- Außerdem SOLLTEN in der Richtlinie die Vorgaben für den Betrieb und die Nutzung der VoIP-Komponenten geregelt sein.
- Hierbei SOLLTEN auch die verschiedenen VoIP-Funktionen, wie zum Beispiel Voicemails, betrachtet werden.
- Die VoIP-Sicherheitsrichtlinie SOLLTE allen beteiligten Personen und Gruppen zugänglich und bekannt sein.

## NET.4.2.A8 Verschlüsselung von VoIP (S)

- Es SOLLTE entschieden werden, ob und welche Sprach- und Signalisierungsinformationen verschlüsselt werden sollen.
- Generell SOLLTEN alle VoIP-Datenpakete, die das gesicherte LAN verlassen, durch geeignete Sicherheitsmechanismen geschützt werden.
- Die Benutzer SOLLTEN über die Nutzung der VoIP-Verschlüsselung informiert werden.

## NET.4.2.A9 Geeignete Auswahl von VoIP-Komponenten (S)

- Bevor VoIP-Komponenten beschafft werden, SOLLTE eine Anforderungsliste erstellt werden.
- Anhand der Anforderungsliste SOLLTEN die am Markt erhältlichen Produkte bewertet werden.
- Diese Anforderungsliste SOLLTE alle Merkmale zur Erreichung des angestrebten Sicherheitsniveaus umfassen.
- Es SOLLTE geregelt werden, wie die am Markt erhältlichen Produkte gemäß der Anforderungsliste bewertet werden können.

## NET.4.2.A10 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## NET.4.2.A11 Sicherer Umgang mit VoIP-Endgeräten [Benutzer] (S)

- Benutzer, die VoIP-Endgeräte einsetzen, SOLLTEN über die grundlegenden VoIP-Gefährdungen und Sicherheitsmaßnahmen informiert sein.
- Außerdem SOLLTEN sie geeignete Passwörter zur Absicherung von Voicemails auswählen.

## NET.4.2.A12 Sichere Außerbetriebnahme von VoIP-Komponenten (S)

- Wenn VoIP-Komponenten außer Betrieb genommen oder ersetzt werden, SOLLTEN alle sicherheitsrelevanten Informationen von den Geräten gelöscht werden.
- Nach dem Löschvorgang SOLLTE überprüft werden, ob die Daten auch tatsächlich erfolgreich entfernt wurden.
- Vertrauliche Informationen SOLLTEN auch von Backup-Medien gelöscht werden.
- Alle Beschriftungen, insbesondere der Endgeräte, SOLLTEN vor der Entsorgung entfernt werden.
- Es SOLLTE frühzeitig mit Herstellern, Händlern beziehungsweise Service-Unternehmen geklärt werden, welche Maßnahmen zur Löschung sicherheitsrelevanter Informationen mit den Vertrags- und Garantiebedingungen vereinbar sind.

## NET.4.2.A13 Anforderungen an eine Firewall für den Einsatz von VoIP (S)

- Es SOLLTE überprüft werden, ob die bestehende Firewall für den Einsatz von VoIP angepasst werden kann.
- Ist dies nicht der Fall, SOLLTE eine zusätzliche Firewall hierfür beschafft und installiert werden.

## NET.4.2.A14 Verschlüsselung der Signalisierung (H)

- Die Integrität und Vertraulichkeit der Signalisierungsinformationen SOLLTE durch geeignete kryptogarische Verfahren gewährleistet werden.
- Nicht nur die Nutzdaten, sondern auch die Authentisierungsdaten SOLLTEN durchgängig verschlüsselt werden.
- Der Zugriff auf das VoIP-Gateway SOLLTE durch VoIP-Adressen und H.323-Identitätenso weit wie möglich eingeschränkt werden.
- Es SOLLTEN zusätzlich Ende-zu-Ende-Sicherheitsmechanismen für den Medientransport und die Signalisierung benutzt werden.
- Es SOLLTE dokumentiert werden, wie die Signalisierung geschützt wird.

## NET.4.2.A15 Sicherer Medientransport mit SRTP (H)

- Mediendaten und Informationen zur Steuerung dieser Daten, die über das Real-Time Transport Protocol (RTP) übertragen werden, SOLLTEN in geeigneter Weise geschützt werden.
- Die Nutzdaten SOLLTEN durch den Einsatz von Secure Real-Time Transport Protocol (SRTP) beziehungsweise Secure Real-Time Control Protocol (SRTCP) geschützt werden.
- Die sicherheitsrelevanten Optionen der Implementierung des Protokolls SOLLTEN dokumentiert werden.

## NET.4.2.A16 Trennung des Daten- und VoIP-Netzes (H)

- Das VoIP-Netz SOLLTE in geeigneter Weise vom Datennetz getrennt werden.
- Es SOLLTE geregelt werden, wie mit Geräten umzugehen ist, die auf das VoIP- und Datennetz zugreifen müssen.
- VoIP-Endgeräte in einem VoIP-Netz SOLLTEN NUR die vorgesehenen VoIP-Verbindungen zu anderen IT-Systemen aufbauen können.


