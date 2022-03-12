# OPS.1.2.6: NTP-Zeitsynchronisation

## OPS.1.2.6.A1 Planung des NTP- Einsatzes (B)

- Der IT-Betrieb MUSS planen, wo und wie NTP eingesetzt wird.
- Dies SOLLTE vollständig dokumentiert werden.
- Dabei MUSS ermittelt werden, welche Anwendungen auf eine genaue Zeitinformation angewiesen sind.
- Die Anforderungen des Informationsverbunds hinsichtlich genauer Zeit der IT-Systeme MÜSSEN definiert und dokumentiert werden.
- Der IT-Betrieb MUSS definieren, welche NTP-Server von welchen NTP-Clients genutzt werden sollen.
- Es MUSS festgelegt werden, ob NTP-Server im Client-Server- oder im Broadcast-Modus arbeiten.

## OPS.1.2.6.A2 Sichere Nutzung fremder Zeitquellen (B)

- Falls Zeitinformationen von einem NTP-Server außerhalb des Netzes der Institution bezogen werden, dann MUSS der IT-Betrieb beurteilen, ob der NTP-Server des Betreibers hinreichend verlässlich ist.
- Der IT-Betrieb MUSS sicherstellen, dass nur als verlässlich eingestufte NTP-Server verwendet werden.
- Der IT-Betrieb MUSS die Nutzungsregeln des Betreibers kennen und beachten.

## OPS.1.2.6.A3 Sichere Konfiguration von NTP-Servern (B)

- Der IT-Betrieb MUSS den NTP-Server so konfigurieren, dass Clients nur dann Einstellungen des NTP-Servers verändern können, wenn dies explizit vorgesehen ist.
- Darüber hinaus MUSS sichergestellt werden, dass nur vertrauenswürdige Clients Status-Informationen abfragen können.
- Falls die internen NTP-Server der Institution nicht selbst hinreichend genaue Zeitquellen nutzen, dann MUSS der ITBetrieb diese NTP-Server so konfigurieren, dass sie regelmäßig genaue Zeitinformationen von externen NTP-Servern abfragen.

## OPS.1.2.6.A4 Nichtberücksichtigung unaufgeforderter Zeitinformationen (B)

- Der IT-Betrieb MUSS alle NTP-Clients so konfigurieren, dass sie Zeitinformationen verwerfen, die sie unaufgefordert von anderen IT-Systemen erhalten.

## OPS.1.2.6.A5 Nutzung des Client-Server-Modus für NTP (S)

- Der IT-Betrieb SOLLTE alle IT-Systeme so konfigurieren, dass sie den NTP-Dienst im Client-Server-Modus nutzen.
- NTP-Server SOLLTEN Zeitinformationen nur dann an Clients versenden, wenn diese aktiv anfragen.

## OPS.1.2.6.A6 Überwachung von IT-Systemen mit NTP-Nutzung (S)

- Der IT-Betrieb SOLLTE die Verfügbarkeit, die Kapazität und die Systemzeit der internen NTP-Server überwachen.
- Der IT-Betrieb SOLLTE IT-Systeme, die ihre Zeit per NTP synchronisieren, so konfigurieren, dass sie folgende Ereignisse protokollieren:
    - unerwartete Neustarts des IT-Systems,
    - unerwartete Neustarts des NTP-Dienstes,
    - Fehler im Zusammenhang mit dem NTP-Dienst sowie
    - ungewöhnliche Zeitinformationen.
- Falls der NTP-Server von sich aus regelmäßig Zeitinformationen versendet (Broadcast-Modus), dann SOLLTE der ITBetrieb die NTP-Clients daraufhin überwachen, ob sie ungewöhnliche Zeitinformationen erhalten.

## OPS.1.2.6.A7 Sichere Konfiguration von NTP-Clients (S)

- Der IT-Betrieb SOLLTE festlegen, welche Zeitinformationen ein IT-System verwenden soll, wenn es neu gestartet wurde.
- Der IT-Betrieb SOLLTE festlegen, welche Zeitinformationen ein IT-System verwenden soll, wenn sein NTPDienst neu gestartet wurde.
- Der IT-Betrieb SOLLTE festlegen, wie NTP-Clients auf stark abweichende Zeitinformationen reagieren.
- Insbesondere SOLLTE entschieden werden, ob stark abweichende Zeitinformationen von NTP-Servern nach einem Systemneustart akzeptiert werden.
- Der IT-Betrieb SOLLTE Grenzwerte für stark abweichende Zeitinformationen festlegen.
- Der IT-Betrieb SOLLTE sicherstellen, dass NTP-Clients auch dann noch ausreichende Zeitinformationen erhalten, wenn sie von einem NTP-Server aufgefordert werden weniger oder gar keine Anfragen zu senden.

## OPS.1.2.6.A8 Einsatz sicherer Protokolle zur Zeitsynchronisation (S)

- Der IT-Betrieb SOLLTE prüfen, ob sichere Protokolle zur Zeitsynchronisation eingesetzt werden können (z. B. Network Time Security (NTS)).
- Falls dies möglich ist, SOLLTEN sichere Protokolle eingesetzt werden.

## OPS.1.2.6.A9 Verfügbarkeit ausreichend vieler genauer Zeitquellen (H)

- Falls korrekte Systemzeiten von erheblicher Bedeutung sind, dann SOLLTE eine Institution über mehrere Stratum1-NTP-Server in ihrem Netz verfügen.
- Die IT-Systeme des Informationsverbunds mit NTP-Dienst SOLLTEN die Stratum-1-NTP-Server direkt oder indirekt als Zeitreferenz nutzen.
- Die Straum-1-Server SOLLTEN jeweils über verschiedene Zeitquellen verfügen.

## OPS.1.2.6.A10 Ausschließlich interne NTP-Server (H)

- Jedes IT-System des Informationsverbunds mit NTP-Dienst SOLLTE Zeitinformationen ausschließlich von NTP-Servern innerhalb des Netzes der Institution beziehen.

## OPS.1.2.6.A11 Redundante NTP-Server (H)

- IT-Systeme, bei denen die Genauigkeit der Systemzeit von erheblicher Bedeutung ist, SOLLTEN Zeitinformationen von mindestens vier unabhängigen NTP-Servern beziehen.

## OPS.1.2.6.A12 NTP-Server mit authentifizierten Auskünften (H)

- NTP-Server SOLLTEN sich bei der Kommunikation gegenüber Clients authentisieren.
- Dies SOLLTE auch für die Server gelten, von denen der NTP-Server seinerseits Zeitinformationen erhält.
- Die NTP-Clients SOLLTEN nur authentifizierte NTP-Daten akzeptieren.


