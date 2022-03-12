# APP.3.6: DNS-Server

## APP.3.6.A1 Planung des DNS-Einsatzes (B)

- Der Einsatz von DNS-Servern MUSS sorgfältig geplant werden.
- Es MUSS zuerst festgelegt werden, wie der Netzdienst DNS aufgebaut werden soll.
- Es MUSS festgelegt werden, welche Domain-Informationen schützenswert sind.
- Es MUSS geplant werden, wie DNS-Server in das Netz des Informationsverbunds eingebunden werden sollen.
- Die getroffenen Entscheidungen MÜSSEN geeignet dokumentiert werden.

## APP.3.6.A2 Einsatz redundanter DNS-Server (B)

- Advertising DNS-Server MÜSSEN redundant ausgelegt werden.
- Für jeden Advertising DNS-Server MUSS es mindestens einen zusätzlichen Secondary DNS-Server geben.

## APP.3.6.A3 Verwendung von separaten DNS-Servern für interne und externe Anfragen (B)

- Advertising DNS-Server und Resolving DNS-Server MÜSSEN serverseitig getrennt sein.
- Die Resolver der internen ITSysteme DÜRFEN NUR die internen Resolving DNS-Server verwenden.

## APP.3.6.A4 Sichere Grundkonfiguration eines DNS-Servers (B)

- Ein Resolving DNS-Server MUSS so konfiguriert werden, dass er ausschließlich Anfragen aus dem internen Netz akzeptiert.
- Wenn ein Resolving DNS-Server Anfragen versendet, MUSS er zufällige Source Ports benutzen.
- Sind DNS-Server bekannt, die falsche Domain-Informationen liefern, MUSS der Resolving DNS-Server daran gehindert werden, Anfragen dorthin zu senden.
- Ein Advertising DNS-Server MUSS so konfiguriert werden, dass er Anfragen aus dem Internet immer iterativ behandelt.
- Es MUSS sichergestellt werden, dass DNS-Zonentransfers zwischen Primary und Secondary DNS-Servern funktionieren.
- Zonentransfers MÜSSEN so konfiguriert werden, dass diese nur zwischen Primary und Secondary DNS-Servern möglich sind.
- Zonentransfers MÜSSEN auf bestimmte IP-Adressen beschränkt werden.
- Die Version des verwendeten DNS-Server-Produktes MUSS verborgen werden.

## APP.3.6.A5 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.3.6.A6 Absicherung von dynamischen DNS-Updates (B)

- Es MUSS sichergestellt werden, dass nur legitimierte IT-Systeme Domain-Informationen ändern dürfen.
- Es MUSS festgelegt werden, welche Domain-Informationen die IT-Systeme ändern dürfen.

## APP.3.6.A7 Überwachung von DNS-Servern (B)

- DNS-Server MÜSSEN laufend überwacht werden.
- Es MUSS überwacht werden, wie ausgelastet die DNS-Server sind, um rechtzeitig die Leistungskapazität der Hardware anpassen zu können.
- DNS-Server MÜSSEN so konfiguriert werden, dass mindestens die folgenden sicherheitsrelevanten Ereignisse protokolliert werden:
    - Anzahl der DNS-Anfragen,
    - Anzahl der Fehler bei DNS-Anfragen,
    - EDNS-Fehler (EDNS – Extension Mechanisms for DNS),
    - auslaufende Zonen sowie
    - fehlgeschlagene Zonentransfers.

## APP.3.6.A8 Verwaltung von Domainnamen [Zentrale Verwaltung] (B)

- Es MUSS sichergestellt sein, dass die Registrierungen für alle Domains, die von einer Institution benutzt werden, regelmäßig und rechtzeitig verlängert werden.
- Ein Mitarbeiter MUSS bestimmt werden, der dafür zuständig ist, die Internet-Domainnamen zu verwalten.
- Falls ein Internetdienstleister mit der Domainverwaltung beauftragt wird, MUSS darauf geachtet werden, dass die Institution die Kontrolle über die Domains behält.

## APP.3.6.A9 Erstellen eines Notfallplans für DNS-Server (B)

- Ein Notfallplan für DNS-Server MUSS erstellt werden.
- Der Notfallplan für DNS-Server MUSS in die bereits vorhandenen Notfallpläne der Institution integriert werden.
- Im Notfallplan für DNS-Server MUSS ein Datensicherungskonzept für die Zonen- und Konfigurationsdateien beschrieben sein.
- Das Datensicherungskonzept für die Zonen- und Konfigurationsdateien MUSS in das existierende Datensicherungskonzept der Institution integriert werden.
- Der Notfallplan für DNS-Server MUSS einen Wiederanlaufplan für alle DNS-Server im Informationsverbund enthalten.

## APP.3.6.A10 Auswahl eines geeigneten DNS-Server-Produktes (S)

- Wird ein DNS-Server-Produkt beschafft, dann SOLLTE darauf geachtet werden, dass es sich in der Praxis ausreichend bewährt hat.
- Das DNS-Server-Produkt SOLLTE die aktuellen RFC-Standards unterstützen.
- Das DNS-Server-Produkt SOLLTE den Zuständigen dabei unterstützen, syntaktisch korrekte Master Files zu erstellen.

## APP.3.6.A11 Ausreichende Dimensionierung der DNS-Server (S)

- Die Hardware des DNS-Servers SOLLTE ausreichend dimensioniert sein.
- Die Hardware des DNS-Servers SOLLTE ausschließlich für den Betrieb dieses DNS-Servers benutzt werden.
- Die Netzanbindungen sämtlicher DNS-Server im Informationsverbund SOLLTEN ausreichend bemessen sein.

## APP.3.6.A12 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.3.6.A13 Einschränkung der Sichtbarkeit von Domain-Informationen (S)

- Der Namensraum eines Informationsverbunds SOLLTE in einen öffentlichen und einen institutionsinternen Bereich aufgeteilt werden.
- Im öffentlichen Teil SOLLTEN nur solche Domain-Informationen enthalten sein, die von Diensten benötigt werden, die von extern erreichbar sein sollen.
- IT-Systeme im internen Netz SOLLTEN selbst dann keinen von außen auflösbaren DNS-Namen erhalten, wenn sie eine öffentliche IP-Adresse besitzen.

## APP.3.6.A14 Platzierung der Nameserver (S)

- Primary und Secondary Advertising DNS-Server SOLLTEN in verschiedenen Netzsegmenten platziert werden.

## APP.3.6.A15 Auswertung der Logdaten (S)

- Die Logdateien des DNS-Servers SOLLTEN regelmäßig überprüft werden.
- Die Logdateien des DNS-Servers SOLLTEN regelmäßig ausgewertet werden.
- Mindestens die folgenden sicherheitsrelevanten Ereignisse SOLLTEN ausgewertet werden:
    - Anzahl der DNS-Anfragen,
    - Anzahl der Fehler bei DNS-Anfragen,
    - EDNS-Fehler,
    - auslaufende Zonen,
    - fehlgeschlagene Zonentransfers sowie
    - Veränderungen im Verhältnis von Fehlern zu DNS-Anfragen.

## APP.3.6.A16 Integration eines DNS-Servers in eine „P-A-P“-Struktur (S)

- Die DNS-Server SOLLTEN in eine „Paketfilter – Application-Level-Gateway – Paketfilter“-(P-A-P)-Struktur integriert werden (siehe auch NET.1.1 Netzarchitektur und -design).
- Der Advertising DNS-Server SOLLTE in diesem Fall in einer demilitarisierten Zone (DMZ) des äußeren Paketfilters angesiedelt sein.
- Der Resolving DNS-Server SOLLTE in einer DMZ des inneren Paketfilters aufgestellt sein.

## APP.3.6.A17 Einsatz von DNSSEC (S)

- Die DNS-Protokollerweiterung DNSSEC SOLLTE sowohl auf Resolving DNS-Servern als auch auf Advertising DNSServern aktiviert werden.
- Die dabei verwendeten Schlüssel Key-Signing-Keys (KSK) und Zone-Signing-Keys (ZSK) SOLLTEN regelmäßig gewechselt werden.

## APP.3.6.A18 Erweiterte Absicherung von Zonentransfers (S)

- Um Zonentransfers stärker abzusichern, SOLLTEN zusätzlich Transaction Signatures (TSIG) eingesetzt werden.

## APP.3.6.A19 Aussonderung von DNS-Servern (S)

- Der DNS-Server SOLLTE sowohl aus dem Domain-Namensraum als auch aus dem Netzverbund gelöscht werden.

## APP.3.6.A20 Prüfung des Notfallplans auf Durchführbarkeit (H)

- Es SOLLTE regelmäßig überprüft werden, ob der Notfallplan für DNS-Server durchführbar ist.

## APP.3.6.A21 Hidden Master (H)

- Um Angriffe auf den primären Advertising DNS-Server zu erschweren, SOLLTE eine sogenannte Hidden-MasterAnordnung vorgenommen werden.

## APP.3.6.A22 Anbindung der DNS-Server über unterschiedliche Provider (H)

- Extern erreichbare DNS-Server SOLLTEN über unterschiedliche Provider angebunden werden.


