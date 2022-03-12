# SYS.3.2.2: Mobile Device Management (MDM)

## SYS.3.2.2.A1 Festlegung einer Strategie für das Mobile Device Management (B)

- Es MUSS eine Strategie erarbeitet werden, die festlegt, wie Mitarbeiter mobile Endgeräte benutzen dürfen und wie die Geräte in die IT-Strukturen der Institution integriert sind.
- Grundlage MUSS dabei der Schutzbedarf der zu verarbeitenden Informationen sein.
- Die Strategie MUSS mindestens folgende Aspekte abdecken:
    - Darf das MDM als Cloud-Dienst betrieben werden?
    - Soll das MDM durch die Institution selbst betrieben werden?
    - Soll das MDM alle Apps bereitstellen oder darf der Beutzer selber Apps installieren? Welche Restriktionen gibt die Institution bei bereitgestellten oder selbst installierten Apps vor?
    - Soll das MDM in eine weitere Infrastruktur eingebunden werden?
    - Welche Anforderungen bezüglich Supportleistungen und Reaktionszeiten sind an den Anbieter des MDM zu stellen?
    - Welche Compliance-Anforderungen müssen durchgesetzt werden?
    - Welche mobilen Geräte und welche Betriebssysteme muss das MDM unterstützen?
    - Muss die MDM-Lösung mandantenfähig sein? Gewährleistet sie die notwendige Mandantentrennung?
    - Müssen Cloud-Dienste eingebunden werden?
    - Müssen Dokumentenmanagementsysteme eingebunden werden?
    - Muss das MDM auch Peripheriegeräte einbinden und verwalten?
    - Welches Betriebsmodell soll eingesetzt werden: private Endgeräte (Bring Your Own Device, BYOD), personalisierte Endgeräte (Eigentum der Institution) oder nicht personalisierte Endgeräte (Eigentum der Institution, gemeinsam genutzt)?
- Die Strategie MUSS schriftlich fixiert und vom ISB freigegeben werden.

## SYS.3.2.2.A2 Festlegung erlaubter mobiler Endgeräte (B)

- Es MUSS festgelegt werden, welche mobilen Endgeräte und Betriebssysteme in der Institution zugelassen sind.
- Alle erlaubten Geräte und Betriebssysteme MÜSSEN den Anforderungen der MDM-Strategie genügen und die technischen Sicherheitsanforderungen der Institution vollständig erfüllen.
- Das MDM MUSS so konfiguriert werden, dass nur mit freigegebenen Geräten auf Informationen der Institution zugegriffen werden kann.
- Es DÜRFEN nur von der Institution zugelassene mobile Endgeräte beschafft werden.

## SYS.3.2.2.A3 Auswahl eines MDM-Produkts (B)

- Wenn eine geeignete MDM-Software beschafft werden soll, MUSS sichergestellt sein, dass sich mit ihr alle in der MDM-Strategie festgelegten Anforderungen erfüllen lassen.
- Auch MUSS sie sämtliche technischen und organisatorischen Sicherheitsmaßnahmen umsetzen können und alle zugelassenen mobilen Endgeräte unterstützen.

## SYS.3.2.2.A4 Verteilung der Grundkonfiguration auf mobile Endgeräte (B)

- Alle mobilen Endgeräte MÜSSEN, bevor sie eingesetzt werden, in das MDM integriert werden.
- Wenn die Geräte die Grundkonfiguration erhalten, MÜSSEN sie sich im Werkszustand befinden.
- Die Verbindung der mobilen Endgeräte zum MDM MUSS angemessen abgesichert werden.
- Bei bereits benutzten Geräten MÜSSEN vorher alle institutionsbezogenen Daten gelöscht werden.
- Ein nicht über MDM konfiguriertes Endgerät DARF NICHT auf Informationen der Institution zugreifen können.

## SYS.3.2.2.A5 Installation des MDM Clients (B)

- Wenn mobile Endgeräte an Mitarbeiter übergeben werden, MUSS, wenn vom Betriebssystem nicht bereits bereitgestellt, darauf der MDM-Client installiert und konfiguriert sein.

## SYS.3.2.2.A20 Regelmäßige Überprüfung des MDM (B)

- Sicherheitseinstellungen MÜSSEN regelmäßig überprüft werden.
- Bei neuen Betriebssystemversionen der mobilen Endgeräte MUSS vorab geprüft werden, ob das MDM diese vollständig unterstützt und die Konfigurationsprofile und Sicherheitseinstellungen weiterhin wirksam und ausreichend sind.
- Abweichungen MÜSSEN korrigiert werden.
- Die zugeteilten Berechtigungen für Benutzer und Administratoren MÜSSEN regelmäßig daraufhin überprüft werden, ob sie weiterhin angemessen sind (Minimalprinzip).

## SYS.3.2.2.A6 Protokollierung des Gerätestatus (S)

- Der Lebenszyklus einschließlich der Konfigurationshistorie eines mobilen Endgerätes SOLLTE ausreichend protokolliert und zentral abrufbar sein.
- Bei Bedarf SOLLTE der aktuelle Status der verwalteten Endgeräte durch den Administrator ermittelt werden können (Device Audit).

## SYS.3.2.2.A7 Installation von Apps (S)

- Apps SOLLTEN gemäß den Anforderungen des geplanten Einsatzszenarios über das MDM installiert, deinstalliert und aktualisiert werden.
- Das MDM SOLLTE die Installation, Deinstallation und Aktualisierung erzwingen, sobald eine Verbindung zum mobilen Endgerät besteht.
- Über das MDM installierte Apps SOLLTEN NICHT durch den Benutzer deinstalliert werden können.
- Das MDM SOLLTE eine Black- oder White-List für die Installation von Apps ermöglichen.

## SYS.3.2.2.A8 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.3.2.2.A9 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.3.2.2.A10 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.3.2.2.A11 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.3.2.2.A12 Absicherung der MDM-Betriebsumgebung (S)

- Das MDM selbst SOLLTE durch technische Maßnahmen abgesichert werden, um dem Schutzbedarf der hinterlegten oder verarbeiteten Informationen zu genügen.
- Das zugrundeliegende Betriebssystem SOLLTE gehärtet werden.

## SYS.3.2.2.A21 Verwaltung von Zertifikaten (S)

- Zertifikate zur Nutzung von Diensten auf dem mobilen Endgerät SOLLTEN zentral über das MDM installiert, deinstalliert und aktualisiert werden.
- Die Installation von nicht vertrauenswürdigen und nicht verifizierbaren (Root-) Zertifikaten durch den Benutzer SOLLTE durch das MDM verhindert werden.
- Das MDM SOLLTE Mechanismen unterstützen, um die Gültigkeit von Zertifikaten zu überprüfen.

## SYS.3.2.2.A22 Fernlöschung und Außerbetriebnahme von Endgeräten (S)

- Das MDM SOLLTE sicherstellen, dass sämtliche dienstliche Daten auf dem mobilen Endgerät aus der Ferne gelöscht werden können (Remote Wipe bei bestehender Datenverbindung).
- Werden in dem mobilen Endgerät externe Speicher genutzt, SOLLTE geprüft werden, ob diese bei einem Remote Wipe ebenfalls gelöscht werden sollen.
- Diese Funktion SOLLTE vom MDM unterstützt werden.
- Der Prozess zur Außerbetriebnahme des mobilen Endgerätes (Unenrollment) SOLLTE sicherstellen, dass keine schutzbedürftigen Daten auf dem mobilen Endgerät oder eingebundenen Speichermedien verbleiben.
- Dies SOLLTE insbesondere dann gelten, wenn das Unenrollment aus der Ferne ausgeführt wird.

## SYS.3.2.2.A13 ENTFALLEN (H)

- Diese Anforderung ist entfallen.

## SYS.3.2.2.A14 Benutzung externer Reputation-Services für Apps (H)

- Wenn die Administratoren einer Institution die erlaubten Apps nicht selbst auswählen können und Benutzer selbstständig Apps auf ihren Geräten installieren dürfen, SOLLTE ein sogenannter Reputation-Service eingesetzt werden.
- Das MDM SOLLTE dann mithilfe dieser Informationen aus dem Reputation-Service die Installation von Apps zumindest einschränken.

## SYS.3.2.2.A15 ENTFALLEN (H)

- Diese Anforderung ist entfallen.

## SYS.3.2.2.A16 ENTFALLEN (H)

- Diese Anforderung ist entfallen.

## SYS.3.2.2.A17 Kontrolle der Nutzung von mobilen Endgeräten (H)

- Es SOLLTEN angemessene Kriterien definiert werden, aufgrund derer die Geräte zu überwachen sind, ohne gegen gesetzliche oder interne Regelungen zu verstoßen.
- Insbesondere SOLLTEN sogenannte Jailbreaks oder sogenanntes Routen erkannt werden.

## SYS.3.2.2.A18 ENTFALLEN (H)

- Diese Anforderung ist entfallen.

## SYS.3.2.2.A19 Einsatz von Geofencing (H)

- Durch die Hinterlegung einer Geofencing-Richtlinie SOLLTE sichergestellt werden, dass Geräte mit schutzbedürftigen Informationen nicht außerhalb eines zuvor festgelegten geografischen Bereichs verwendet werden können.
- Wird der geografische Bereich verlassen, SOLLTEN entsprechend klassifizierte Informationen oder das Gerät vollständig gelöscht werden.
- Bevor das Gerät selektiv oder vollständig gelöscht wird, SOLLTEN die verantwortlichen Administratoren und das Sicherheitsmanagement sowie der Benutzer informiert werden.
- Erst mit einer angemessenen zeitlichen Verzögerung SOLLTE das Gerät selektiv oder vollständig gelöscht werden.
- Die Bereiche, an denen diese zusätzlichen Sicherheitsmaßnahmen nötig sind, SOLLTEN identifiziert werden.
- Anschließend SOLLTEN die Sicherheitsmaßnahmen unter Beachtung gesetzlicher und interner Regelungen umgesetzt werden.

## SYS.3.2.2.A23 Durchsetzung von Compliance-Anforderungen (H)

- Verstöße gegen die Regelungen der Institution oder sogar eine Manipulation des Betriebssystems SOLLTEN mit einer geeigneten Lösung erkannt werden.
- Die folgenden Aktionen SOLLTEN bei Verdacht auf Verstoß gegen Regelungen oder Manipulation des Betriebssystems ausgeführt werden.
- Hierzu SOLLTEN entsprechende Funktionen bereitgestellt werden:


