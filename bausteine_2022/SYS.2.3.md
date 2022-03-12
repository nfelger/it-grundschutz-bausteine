# SYS.2.3: Clients unter Linux und Unix

## SYS.2.3.A1 Authentisierung von Administratoren und Benutzern [Benutzer] (B)

- Administratoren DÜRFEN sich NICHT im Normalbetrieb als „root“ anmelden.
- Für die Systemadministrationsaufgaben SOLLTE „sudo“ oder eine geeignete Alternative mit einer geeigneten Protokollierung genutzt werden.
- Es SOLLTE verhindert werden, dass sich mehrere Benutzer auf einem Client gleichzeitig einloggen können.

## SYS.2.3.A2 Auswahl einer geeigneten Distribution (B)

- Auf Grundlage der Sicherheitsanforderungen und des Einsatzzwecks MUSS ein geeignetes Unix-Derivat bzw. eine geeignete Linux-Distribution ausgewählt werden.
- Es MUSS für die geplante Einsatzdauer des Betriebssystems Support verfügbar sein.
- Alle benötigten Anwendungsprogramme SOLLTEN als Teil der Distribution direkt verfügbar sein.
- Sie SOLLTEN NUR in Ausnahmefällen aus Drittquellen bezogen werden.
- Distributionen, bei denen das Betriebssystem selber kompiliert wird, SOLLTEN NICHT in Produktivumgebungen eingesetzt werden.

## SYS.2.3.A3 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## SYS.2.3.A4 Kernel-Aktualisierungen auf unixartigen Systemen (B)

- Der Client MUSS zeitnah rebootet werden, nachdem der Kernel des Betriebssystems aktualisiert wurde.
- Ist dies nicht möglich, MUSS alternativ Live-Patching des Kernels aktiviert werden.

## SYS.2.3.A5 Sichere Installation von Software-Paketen (B)

- Wenn zu installierende Software aus dem Quellcode kompiliert werden soll, DARF diese NUR unter einem unprivilegierten Benutzeraccount entpackt, konfiguriert und übersetzt werden.
- Anschließend DARF die zu installierende Software NICHT unkontrolliert in das Wurzeldateisystem des Betriebssystems installiert werden.
- Wird die Software aus dem Quelltext übersetzt, dann SOLLTEN die gewählten Parameter geeignet dokumentiert werden.
- Anhand dieser Dokumentation SOLLTE die Software jederzeit nachvollziehbar und reproduzierbar kompiliert werden können.
- Alle weiteren Installationsschritte SOLLTEN dabei ebenfalls dokumentiert werden, damit sich die Konfiguration im Notfall schnell reproduzieren lässt.

## SYS.2.3.A6 Kein automatisches Einbinden von Wechsellaufwerken [Benutzer] (S)

- Wechsellaufwerke SOLLTEN NICHT automatisch eingebunden werden.
- Die Einbindung von Wechsellaufwerken SOLLTE so konfiguriert sein, dass alle Dateien als nicht ausführbar markiert sind (Mountoption „noexec“).

## SYS.2.3.A7 Restriktive Rechtevergabe auf Dateien und Verzeichnisse (S)

- Es SOLLTE sichergestellt werden, dass Dienste und Anwendungen nur die ihnen zugeordneten Dateien erstellen, verändern oder löschen dürfen.
- Auf Verzeichnissen, in denen alle Benutzer Schreibrechte haben (z. B. /tmp), SOLLTE das Sticky Bit gesetzt werden.

## SYS.2.3.A8 Einsatz von Techniken zur Rechtebeschränkung von Anwendungen (S)

- Zur Beschränkung der Zugriffsrechte von Anwendungen auf Dateien, Geräte und Netze SOLLTE App-Armor oder SELinux eingesetzt werden.
- Es SOLLTEN die von dem jeweiligen Unix-Derivat bzw. der Linux-Distribution am besten unterstützten Lösungen eingesetzt werden.
- Die notwendigen Anwendungen SOLLTEN statt Blacklisting durch Whitelisting reglementiert werden.
- Erweiterungen zur Rechtebeschränkung SOLLTEN im Zwangsmodus (Enforcing Mode) oder mit geeigneten Alternativen verwendet werden.

## SYS.2.3.A9 Sichere Verwendung von Passwörtern auf der Kommandozeile [Benutzer] (S)

- Passwörter SOLLTEN NICHT als Parameter an Programme übergeben werden.

## SYS.2.3.A10 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.2.3.A11 Verhinderung der Überlastung der lokalen Festplatte (S)

- Es SOLLTEN Quotas für Benutzer bzw. Dienste eingerichtet werden, die ausreichend Freiraum für das Betriebssystem lassen.
- Generell SOLLTEN unterschiedliche Partitionen für Betriebssystem und Daten genutzt werden.
- Alternativ SOLLTEN auch Mechanismen des verwendeten Dateisystems genutzt werden, die ab einem geeigneten Füllstand nur noch dem Benutzer „root“ Schreibrechte einräumen.

## SYS.2.3.A12 Sicherer Einsatz von Appliances (S)

- Es SOLLTE sichergestellt werden, dass Appliances ein ähnliches Sicherheitsniveau wie Clients auf Standard-IT-Systemen erfüllen.
- Es SOLLTE dokumentiert werden, wie entsprechende Sicherheitsanforderungen mit einer eingesetzten Appliance erfüllt werden.
- Wenn die Anforderungen nicht zweifelsfrei erfüllt werden können, SOLLTE eine Konformitätserklärung vom Hersteller angefordert werden.

## SYS.2.3.A13 ENTFALLEN (H)

- Diese Anforderung ist entfallen.

## SYS.2.3.A14 Absicherung gegen Nutzung unbefugter Peripheriegeräte (H)

- Peripheriegeräte SOLLTEN nur nutzbar sein, wenn sie auf einer zentral verwalteten Whitelist geführt sind.
- Kernelmodule für Peripheriegeräte SOLLTEN nur geladen und aktiviert werden, wenn das Gerät auf der Whitelist steht.

## SYS.2.3.A15 Zusätzlicher Schutz vor der Ausführung unerwünschter Dateien (H)

- Partitionen und Verzeichnisse, in denen Benutzer Schreibrechte haben, SOLLTEN so gemountet werden, dass keine Dateien ausgeführt werden können (Mountoption „noexec“).

## SYS.2.3.A16 ENTFALLEN (H)

- Diese Anforderung ist entfallen.

## SYS.2.3.A17 Zusätzliche Verhinderung der Ausbreitung bei der Ausnutzung von Schwachstellen (H)

- Die Nutzung von Systemaufrufen SOLLTE insbesondere für exponierte Dienste und Anwendungen auf die unbedingt notwendige Anzahl beschränkt werden (z. B. durch seccomp).
- Die vorhandenen Standardprofile bzw. -regeln von SELinux, AppArmor sowie alternativen Erweiterungen SOLLTEN manuell überprüft und gegebenenfalls an die eigene Sicherheitsrichtlinie angepasst werden.
- Falls erforderlich, SOLLTEN neue Regeln bzw. Profile erstellt werden.

## SYS.2.3.A18 Zusätzlicher Schutz des Kernels (H)

- Es SOLLTEN mit speziell gehärteten Kernels (z. B. grsecurity, PaX) geeignete Schutzmaßnahmen wie Speicherschutz, Dateisystemabsicherung und rollenbasierte Zugriffskontrolle umgesetzt werden, die eine Ausnutzung von Schwachstellen und die Ausbreitung im Betriebssystem verhindern.

## SYS.2.3.A19 Festplatten- oder Dateiverschlüsselung (H)

- Festplatten oder die darauf abgespeicherten Dateien SOLLTEN verschlüsselt werden.
- Die dazugehörigen Schlüssel SOLLTEN NICHT auf dem IT-System gespeichert werden.
- Es SOLLTEN AEAD-Verfahren (Authenticated Encryption with Associated Data) bei der Festplatten- und Dateiverschlüsselung eingesetzt werden.
- Alternativ SOLLTE „dmcrypt“ in Kombination mit „dm-verity“ genutzt werden.

## SYS.2.3.A20 Abschaltung kritischer SysRq-Funktionen (H)

- Es SOLLTE festgelegt werden, welche SysRq-Funktionen von den Benutzern ausgeführt werden dürfen.
- Generell SOLLTEN keine kritischen SysRq-Funktionen von den Benutzern ausgelöst werden können.


