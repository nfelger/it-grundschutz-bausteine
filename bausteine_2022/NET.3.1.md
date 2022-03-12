# NET.3.1: Router und Switches

## NET.3.1.A1 Sichere Grundkonfiguration eines Routers oder Switches (B)

- Bevor ein Router oder Switch eingesetzt wird, MUSS er sicher konfiguriert werden.
- Alle Konfigurationsänderungen SOLLTEN nachvollziehbar dokumentiert sein.
- Die Integrität der Konfigurationsdateien MUSS in geeigneter Weise geschützt werden.
- Bevor Zugangspasswörter abgespeichert werden, MÜSSEN sie mithilfe eines zeitgemäßen kryptografischen Verfahrens abgesichert werden (siehe CON.1 Kryptokonzept).
- Router und Switches MÜSSEN so konfiguriert sein, dass nur zwingend erforderliche Dienste, Protokolle und funktionale Erweiterungen genutzt werden.
- Nicht benötigte Dienste, Protokolle und funktionale Erweiterungen MÜSSEN deaktiviert oder ganz deinstalliert werden.
- Ebenfalls MÜSSEN nicht benutzte Schnittstellen auf Routern und Switches deaktiviert werden.
- Unbenutzte Netzports MÜSSEN nach Möglichkeit deaktiviert oder zumindest einem dafür eingerichteten Unassigned-VLAN zugeordnet werden.
- Wenn funktionale Erweiterungen benutzt werden, MÜSSEN die Sicherheitsrichtlinien der Institution weiterhin erfüllt sein.
- Auch SOLLTE begründet und dokumentiert werden, warum solche Erweiterungen eingesetzt werden.
- Informationen über den internen Konfigurations- und Betriebszustand MÜSSEN nach außen verborgen werden.
- Unnötige Auskunftsdienste MÜSSEN deaktiviert werden.

## NET.3.1.A2 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## NET.3.1.A3 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## NET.3.1.A4 Schutz der Administrationsschnittstellen (B)

- Alle Administrations- und Managementzugänge der Router und Switches MÜSSEN auf einzelne Quell-IP-Adressen bzw. -Adressbereiche eingeschränkt werden.
- Es MUSS sichergestellt sein, dass aus nicht vertrauenswürdigen Netzen heraus nicht direkt auf die Administrationsschnittstellen zugegriffen werden kann.
- Um Router und Switches zu administrieren bzw. zu überwachen, SOLLTEN geeignet verschlüsselte Protokolle eingesetzt werden.
- Sollte dennoch auf unverschlüsselte Protokolle zurückgegriffen werden, MUSS für die Administration ein eigenes Administrationsnetz (Out-of-Band-Management) genutzt werden.
- Die Managementschnittstellen und die Administrationsverbindungen MÜSSEN durch eine separate Firewall geschützt werden.
- Für die Schnittstellen MÜSSEN geeignete Zeitbeschränkungen für z. B. Timeouts vorgegeben werden.
- Alle für das Management-Interface nicht benötigten Dienste MÜSSEN deaktiviert werden.
- Verfügt eine Netzkomponente über eine dedizierte Hardwareschnittstelle, MUSS der unberechtigte Zugriff darauf in geeigneter Weise unterbunden werden.

## NET.3.1.A5 Schutz vor Fragmentierungsangriffen (B)

- Am Router und Layer-3-Switch MÜSSEN Schutzmechanismen aktiviert sein, um IPv4- sowie IPv6-Fragmentierungsangriffe abzuwehren.

## NET.3.1.A6 Notfallzugriff auf Router und Switches (B)

- Es MUSS für die Administratoren immer möglich sein, direkt auf Router und Switches zuzugreifen, sodass diese weiterhin lokal administriert werden können, auch wenn das gesamte Netz ausfällt.

## NET.3.1.A7 Protokollierung bei Routern und Switches (B)

- Ein Router oder Switch MUSS so konfiguriert werden, dass er unter anderem folgende Ereignisse protokolliert:
    - Konfigurationsänderungen (möglichst automatisch),
    - Reboot,
    - Systemfehler,
    - Statusänderungen pro Interface, System und Netzsegment sowie
    - Login-Fehler.

## NET.3.1.A8 Regelmäßige Datensicherung (B)

- Die Konfigurationsdateien von Routern und Switches MÜSSEN regelmäßig gesichert werden.
- Die Sicherungskopien MÜSSEN so abgelegt werden, dass im Notfall darauf zugegriffen werden kann.

## NET.3.1.A9 Betriebsdokumentationen (B)

- Die wichtigsten betrieblichen Aufgaben eines Routers oder Switches MÜSSEN geeignet dokumentiert werden.
- Es SOLLTEN alle Konfigurationsänderungen sowie sicherheitsrelevante Aufgaben dokumentiert werden.
- Die Dokumentation SOLLTEN vor unbefugten Zugriffen geschützt werden.

## NET.3.1.A10 Erstellung einer Sicherheitsrichtlinie (S)

- Ausgehend von der allgemeinen Sicherheitsrichtlinie der Institution SOLLTE eine spezifische Sicherheitsrichtlinie erstellt werden.
- In der Sicherheitsrichtlinie SOLLTEN nachvollziehbar Anforderungen und Vorgaben beschrieben sein, wie Router und Switches sicher betrieben werden können.
- Die Richtlinie SOLLTE allen Administratoren bekannt und grundlegend für ihre Arbeit sein.
- Wird die Richtlinie verändert oder wird von den festgelegten Anforderungen abgewichen, SOLLTE das mit dem ISB abgestimmt und dokumentiert werden.
- Es SOLLTE regelmäßig überprüft werden, ob die Richtlinie noch korrekt umgesetzt ist.
- Die Ergebnisse SOLLTEN geeignet dokumentiert werden.

## NET.3.1.A11 Beschaffung eines Routers oder Switches (S)

- Bevor Router oder Switches beschafft werden, SOLLTE basierend auf der Sicherheitsrichtlinie eine Anforderungsliste erstellt werden, anhand derer die am Markt erhältlichen Produkte bewertet werden.
- Es SOLLTE darauf geachtet werden, dass das von der Institution angestrebte Sicherheitsniveau mit den zu beschaffenden Geräten erreicht werden kann.
- Grundlage für die Beschaffung SOLLTEN daher die Anforderungen aus der Sicherheitsrichtlinie sein.

## NET.3.1.A12 Erstellung einer Konfigurations-Checkliste für Router und Switches (S)

- Es SOLLTE eine Konfigurations-Checkliste erstellt werden, anhand derer die wichtigsten sicherheitsrelevanten Einstellungen auf Routern und Switches geprüft werden können.
- Da die sichere Konfiguration stark vom Einsatzzweck abhängt, SOLLTEN die unterschiedlichen Anforderungen der Geräte in der Konfigurations-Checkliste berücksichtigt werden.

## NET.3.1.A13 Administration über ein gesondertes Managementnetz (S)

- Router und Switches SOLLTEN ausschließlich über ein separates Managementnetz (Out-of-Band-Management) administriert werden.
- Eine eventuell vorhandene Administrationsschnittstelle über das eigentliche Datennetz (InBand) SOLLTE deaktiviert werden.
- Die verfügbaren Sicherheitsmechanismen der eingesetzten Managementprotokolle zur Authentisierung, Integritätssicherung und Verschlüsselung SOLLTEN aktiviert werden.
- Alle unsicheren Managementprotokolle SOLLTEN deaktiviert werden.

## NET.3.1.A14 Schutz vor Missbrauch von ICMP-Nachrichten (S)

- Die Protokolle ICMP und ICMPv6 SOLLTEN restriktiv gefiltert werden.

## NET.3.1.A15 Bogon- und Spoofing-Filterung (S)

- Es SOLLTE verhindert werden, dass Angreifer mithilfe gefälschter, reservierter oder noch nicht zugewiesener IP-Adressen in die Router und Switches eindringen können.

## NET.3.1.A16 Schutz vor „IPv6 Routing Header Type-0“-Angriffen (S)

- Beim Einsatz von IPv6 SOLLTEN Mechanismen eingesetzt werden, die Angriffe auf den Routing-Header des Type-0 erkennen und verhindern.

## NET.3.1.A17 Schutz vor DoS- und DDoS-Angriffen (S)

- Es SOLLTEN Mechanismen eingesetzt werden, die hochvolumige Angriffe sowie TCP-State-Exhaustion-Angriffe erkennen und abwehren.

## NET.3.1.A18 Einrichtung von Access Control Lists (S)

- Der Zugriff auf Router und Switches SOLLTE mithilfe von Access Control Lists (ACLs) definiert werden.
- In der ACL SOLLTE anhand der Sicherheitsrichtlinie der Institution festgelegt werden, über welche IT-Systeme oder Netze mit welcher Methode auf einen Router oder Switch zugegriffen werden darf.
- Für den Fall, dass keine spezifischen Regeln existieren, SOLLTE generell der restriktivere Whitelist-Ansatz bevorzugt werden.

## NET.3.1.A19 Sicherung von Switch-Ports (S)

- Die Ports eines Switches SOLLTEN vor unberechtigten Zugriffen geschützt werden.

## NET.3.1.A20 Sicherheitsaspekte von Routing-Protokollen (S)

- Router SOLLTEN sich authentisieren, wenn sie Routing-Informationen austauschen oder Updates für Routing-Tabellen verschicken.
- Es SOLLTEN ausschließlich Routing-Protokolle eingesetzt werden, die dies unterstützen.
- Dynamische Routing-Protokolle SOLLTEN ausschließlich in sicheren Netzen verwendet werden.
- Sie DÜRFEN NICHT in demilitarisierten Zonen (DMZs) eingesetzt werden.
- In DMZs SOLLTEN stattdessen statische Routen eingetragen werden.

## NET.3.1.A21 Identitäts- und Berechtigungsmanagement in der Netzinfrastruktur (S)

- Router und Switches SOLLTEN an ein zentrales Identitäts- und Berechtigungsmanagement angebunden werden (siehe ORP.4 Identitäts- und Berechtigungsmanagement).

## NET.3.1.A22 Notfallvorsorge bei Routern und Switches (S)

- Es SOLLTE geplant und vorbereitet werden, welche Fehler bei Routern oder Switches in einem Notfall diagnostiziert werden könnten.
- Außerdem SOLLTE geplant und vorbereitet werden, wie die identifizierten Fehler behoben werden können.
- Für typische Ausfallszenarien SOLLTEN entsprechende Handlungsanweisungen definiert und in regelmäßigen Abständen aktualisiert werden.
- Die Notfallplanungen für Router und Switches SOLLTEN mit der übergreifenden Störungs- und Notfallvorsorge abgestimmt sein.
- Die Notfallplanungen SOLLTEN sich am allgemeinen Notfallvorsorgekonzept orientieren (siehe DER.4 Notfallmanagement).
- Es SOLLTE sichergestellt sein, dass die Dokumentationen zur Notfallvorsorge und die darin enthaltenen Handlungsanweisungen in Papierform vorliegen.
- Das im Rahmen der Notfallvorsorge beschriebene Vorgehen SOLLTE regelmäßig geprobt werden.

## NET.3.1.A23 Revision und Penetrationstests (S)

- Router und Switches SOLLTEN regelmäßig auf bekannte Sicherheitsprobleme hin überprüft werden.
- Auch SOLLTEN regelmäßig Revisionen durchgeführt werden.
- Dabei SOLLTE unter anderem geprüft werden, ob der Ist-Zustand der festgelegten sicheren Grundkonfiguration entspricht.
- Die Ergebnisse SOLLTEN nachvollziehbar dokumentiert und mit dem Soll-Zustand abgeglichen werden.
- Abweichungen SOLLTE nachgegangen werden.

## NET.3.1.A24 Einsatz von Netzzugangskontrollen (H)

- Eine Port-based Access Control SOLLTE nach IEEE 802.1x auf Basis von EAP-TLS implementiert werden.
- Es SOLLTE KEINE Implementierung nach den Standards IEEE 802.1x-2001 und IEEE 802.1x-2004 erfolgen.

## NET.3.1.A25 Erweiterter Integritätsschutz für die Konfigurationsdateien (H)

- Stürzt ein Router oder Switch ab, SOLLTE sichergestellt werden, dass bei der Wiederherstellung bzw. beim Neustart keine alten oder fehlerhaften Konfigurationen (unter anderem ACLs) benutzt werden.

## NET.3.1.A26 Hochverfügbarkeit (H)

- Die Realisierung einer Hochverfügbarkeitslösung SOLLTE den Betrieb der Router und Switches bzw. deren Sicherheitsfunktionen NICHT behindern oder das Sicherheitsniveau senken.
- Router und Switches SOLLTEN redundant ausgelegt werden.
- Dabei SOLLTE darauf geachtet werden, dass die Sicherheitsrichtlinie der Institution eingehalten wird.

## NET.3.1.A27 Bandbreitenmanagement für kritische Anwendungen und Dienste (H)

- Router und Switches SOLLTEN Funktionen enthalten und einsetzen, mit denen sich die Applikationen erkennen und Bandbreiten priorisieren lassen.

## NET.3.1.A28 Einsatz von zertifizierten Produkten (H)

- Es SOLLTEN Router und Switches mit einer Sicherheitsevaluierung nach Common Criteria eingesetzt werden, mindestens mit der Stufe EAL4.


