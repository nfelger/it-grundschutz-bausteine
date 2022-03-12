# SYS.1.3: Server unter Linux und Unix

## SYS.1.3.A1 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## SYS.1.3.A2 Sorgfältige Vergabe von IDs (B)

- Jeder Login-Name, jede Benutzer-ID (User-ID, UID) und jede Gruppen-ID (GID) DARF NUR einmal vorkommen.
- Jeder Benutzer MUSS Mitglied mindestens einer Gruppe sein.
- Jede in der Datei /etc/passwd vorkommende GID MUSS in der Datei /etc/group definiert sein.
- Jede Gruppe SOLLTE nur die Benutzer enthalten, die unbedingt notwendig sind.
- Bei vernetzten Systemen MUSS außerdem darauf geachtet werden, dass die Vergabe von Benutzer- und Gruppennamen, UID und GID im Systemverbund konsistent erfolgt, wenn beim systemübergreifenden Zugriff die Möglichkeit besteht, dass gleiche UIDs bzw. GIDs auf den Systemen unterschiedlichen Benutzer- bzw. Gruppennamen zugeordnet werden könnten.

## SYS.1.3.A3 Kein automatisches Einbinden von Wechsellaufwerken (B)

- Wechseldatenträger wie z. B. USB-Sticks oder CDs/DVDs DÜRFEN NICHT automatisch eingebunden werden.

## SYS.1.3.A4 Schutz vor Ausnutzung von Schwachstellen in Anwendungen (B)

- Um die Ausnutzung von Schwachstellen in Anwendungen zu erschweren, MUSS ASLR und DEP/NX im Kernel aktiviert und von den Anwendungen genutzt werden.
- Sicherheitsfunktionen des Kernels und der Standardbibliotheken, wie z. B. Heap- und Stackschutz, DÜRFEN NICHT deaktiviert werden.

## SYS.1.3.A5 Sichere Installation von Software-Paketen (B)

- Wenn zu installierende Software aus Quellcode kompiliert werden soll, DARF diese NUR unter einem unprivilegierten Benutzeraccount entpackt, konfiguriert und übersetzt werden.
- Anschließend DARF die zu installierende Software NICHT unkontrolliert in das Wurzeldateisystem des Servers installiert werden.
- Wird die Software aus dem Quelltext übersetzt, SOLLTEN die gewählten Parameter geeignet dokumentiert werden.
- Anhand dieser Dokumentation SOLLTE die Software jederzeit nachvollziehbar und reproduzierbar kompiliert werden können.
- Alle weiteren Installationsschritte SOLLTEN dabei ebenfalls dokumentiert werden.

## SYS.1.3.A6 Verwaltung von Benutzern und Gruppen (S)

- Zur Verwaltung von Benutzern und Gruppen SOLLTEN die entsprechenden Verwaltungswerkzeuge genutzt werden.
- Von einer direkten Bearbeitung der Konfigurationsdateien /etc/passwd, /etc/shadow, /etc/group und /etc/ sudoers SOLLTE abgesehen werden.

## SYS.1.3.A7 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.1.3.A8 Verschlüsselter Zugriff über Secure Shell (S)

- Um eine verschlüsselte und authentisierte, interaktive Verbindung zwischen zwei IT-Systemen aufzubauen, SOLLTE ausschließlich Secure Shell (SSH) verwendet werden.
- Alle anderen Protokolle, deren Funktionalität durch Secure Shell abgedeckt wird, SOLLTEN vollständig abgeschaltet werden.
- Für die Authentifizierung SOLLTEN Benutzer vorrangig Zertifikate anstatt eines Passwortes verwenden.

## SYS.1.3.A9 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.1.3.A10 Verhinderung der Ausbreitung bei der Ausnutzung von Schwachstellen (S)

- Dienste und Anwendungen SOLLTEN mit einer individuellen Sicherheitsarchitektur geschützt werden (z. B. mit AppArmor oder SELinux).
- Auch chroot-Umgebungen sowie LXC- oder Docker-Container SOLLTEN dabei berücksichtigt werden.
- Es SOLLTE sichergestellt sein, dass mitgelieferte Standardprofile bzw. -regeln aktiviert sind.

## SYS.1.3.A11 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.1.3.A12 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.1.3.A13 ENTFALLEN (H)

- Diese Anforderung ist entfallen.

## SYS.1.3.A14 Verhinderung des Ausspähens von System- und Benutzerinformationen (H)

- Die Ausgabe von Informationen über das Betriebssystem und der Zugriff auf Protokoll- und Konfigurationsdateien SOLLTE für Benutzer auf das notwendige Maß beschränkt werden.
- Außerdem SOLLTEN bei Befehlsaufrufen keine vertraulichen Informationen als Parameter übergeben werden.

## SYS.1.3.A15 ENTFALLEN (H)

- Diese Anforderung ist entfallen.

## SYS.1.3.A16 Zusätzliche Verhinderung der Ausbreitung bei der Ausnutzung von Schwachstellen (H)

- Die Nutzung von Systemaufrufen SOLLTE insbesondere für exponierte Dienste und Anwendungen auf die unbedingt notwendige Anzahl beschränkt werden.
- Die Standardprofile bzw. -regeln von z. B. SELinux, AppArmor SOLLTEN manuell überprüft und unter Umständen an die eigenen Sicherheitsrichtlinien angepasst werden.
- Falls erforderlich, SOLLTEN neue Regeln bzw. Profile erstellt werden.

## SYS.1.3.A17 Zusätzlicher Schutz des Kernels (H)

- Es SOLLTEN speziell gehärtete Kernels (z. B. grsecurity, PaX) und geeignete Schutzmaßnahmen wie Speicherschutz oder Dateisystemabsicherung umgesetzt werden, die eine Ausnutzung von Schwachstellen und die Ausbreitung im Betriebssystem verhindern.


