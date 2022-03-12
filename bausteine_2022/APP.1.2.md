# APP.1.2: Webbrowser

## APP.1.2.A1 Verwendung von grundlegenden Sicherheitsmechanismen (B)

- Der eingesetzte Webbrowser MUSS sicherstellen, dass jede Instanz und jeder Verarbeitungsprozess nur auf die eigenen Ressourcen zugreifen kann (Sandboxing).
- Webseiten MÜSSEN als eigenständige Prozesse oder mindestens als eigene Threads voneinander isoliert werden.
- Plug-ins und Erweiterungen MÜSSEN ebenfalls in isolierten Bereichen ausgeführt werden.
- Der verwendete Webbrowser MUSS die Content Security Policy (CSP) umsetzen.
- Der aktuell höchste Level der CSP SOLLTE erfüllt werden.
- Der Browser MUSS Maßnahmen zur Same-Origin-Policy und Subresource Integrity unterstützen.

## APP.1.2.A2 Unterstützung sicherer Verschlüsselung der Kommunikation (B)

- Der Webbrowser MUSS Transport Layer Security (TLS) in einer sicheren Version unterstützen.
- Verbindungen zu Webservern MÜSSEN mit TLS verschlüsselt werden, sofern dies vom Webserver unterstützt wird.
- Unsichere Versionen von TLS SOLLTEN deaktiviert werden.
- Der Webbrowser MUSS den Sicherheitsmechanismus HTTP Strict Transport Security (HSTS) gemäß RFC 6797 unterstützen und einsetzen.

## APP.1.2.A3 Verwendung von vertrauenswürdigen Zertifikaten (B)

- Falls der Webbrowser eine eigene Liste von vertrauenswürdigen Wurzelzertifikaten bereitstellt, MUSS sichergestellt werden, dass nur Administratoren diese ändern können.
- Falls dies nicht durch technische Maßnahmen möglich ist, MUSS den Benutzern verboten werden, diese Liste zu ändern.
- Außerdem MUSS sichergestellt werden, dass der Webbrowser Zertifikate lokal widerrufen kann.
- Der Webbrowser MUSS die Gültigkeit der Server-Zertifikate mithilfe des öffentlichen Schlüssels und unter Berücksichtigung des Gültigkeitszeitraums vollständig prüfen.
- Auch der Sperrstatus der Server-Zertifikate MUSS vom Webbrowser geprüft werden.
- Die Zertifikatskette einschließlich des Wurzelzertifikats MUSS verifiziert werden.
- Der Webbrowser MUSS dem Benutzer eindeutig und gut sichtbar darstellen, ob die Kommunikation im Klartext oder verschlüsselt erfolgt.
- Der Webbrowser SOLLTE dem Benutzer auf Anforderung das verwendete Serverzertifikat anzeigen können.
- Der Webbrowser MUSS dem Benutzer signalisieren, wenn Zertifikate fehlen, ungültig sind oder widerrufen wurden.
- Der Webbrowser MUSS in diesem Fall die Verbindung abbrechen, bis der Benutzer diese ausdrücklich bestätigt hat.

## APP.1.2.A4 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## APP.1.2.A6 Kennwortmanagement im Webbrowser (B)

- Wird ein Kennwortmanager im Webbrowser verwendet, MUSS er eine direkte und eindeutige Beziehung zwischen Webseite und hierfür gespeichertem Kennwort herstellen.
- Der Kennwortspeicher MUSS die Passwörter verschlüsselt speichern.
- Es MUSS sichergestellt werden, dass auf die im Kennwortmanager gespeicherten Passwörter nur nach Eingabe eines Master-Kennworts zugegriffen werden kann.
- Außerdem MUSS sichergestellt sein, dass die Authentisierung für den kennwortgeschützten Zugriff nur für die aktuelle Sitzung gültig ist.
- Der IT-Betrieb MUSS sicherstellen, dass der verwendete Browser den Benutzern die Möglichkeit bietet, gespeicherte Passwörter zu löschen.

## APP.1.2.A13 Nutzung von DNS-over-HTTPS (B)

- Die Institution MUSS prüfen, ob die verwendeten Browser DNS-over-HTTPS (DoH) einsetzen.
- Es MUSS festgelegt werden, ob die Funktion verwendet werden soll.
- Falls die Institution DNS-Server als Resolver verwendet, die über nicht vertrauenswürdige Netze angesprochen werden, SOLLTE DoH verwendet werden.
- Falls DoH verwendet wird, MUSS die Institution einen vertrauenswürdigen DoH-Server festlegen.

## APP.1.2.A5 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.1.2.A7 Datensparsamkeit in Webbrowsern [Benutzer] (S)

- Cookies von Drittanbietern SOLLTEN im Webbrowser abgelehnt werden.
- Gespeicherte Cookies SOLLTEN durch den Benutzer gelöscht werden können.
- Die Funktion zur Autovervollständigung von Daten SOLLTE deaktiviert werden.
- Wird die Funktion dennoch genutzt, SOLLTE der Benutzer diese Daten löschen können.
- Der Benutzer SOLLTE außerdem die Historiendaten des Webbrowsers löschen können.
- Sofern vorhanden, SOLLTE eine Synchronisation des Webbrowsers mit Cloud-Diensten deaktiviert werden.
- Telemetriefunktionen sowie das automatische Senden von Absturzberichten, URL-Eingaben und Sucheingaben an den Hersteller oder andere Externe SOLLTEN soweit wie möglich deaktiviert werden.
- Peripheriegeräte wie Mikrofon oder Webcam sowie Standortfreigaben SOLLTEN nur für Webseiten aktiviert werden, bei denen sie unbedingt benötigt werden.
- Der Browser SOLLTE eine Möglichkeit bieten, WebRTC, HSTS und JavaScript zu konfigurieren bzw. abzuschalten.

## APP.1.2.A8 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## APP.1.2.A9 Einsatz einer isolierten Webbrowser-Umgebung (H)

- Bei erhöhtem Schutzbedarf SOLLTEN Webbrowser eingesetzt werden, die in einer isolierten Umgebung, wie z. B. ReCoBS, oder auf dedizierten IT-Systemen ausgeführt werden.

## APP.1.2.A10 Verwendung des privaten Modus [Benutzer] (H)

- Der Webbrowser SOLLTE bei erhöhten Anforderungen bezüglich der Vertraulichkeit im sogenannten privaten Modus ausgeführt werden, sodass keine Informationen oder Inhalte dauerhaft auf dem IT-System des Benutzers gespeichert werden.
- Der Browser SOLLTE so konfiguriert werden, dass lokale Inhalte beim Beenden gelöscht werden.

## APP.1.2.A11 Überprüfung auf schädliche Inhalte (H)

- Aufgerufene Internetadressen SOLLTEN durch den Webbrowser auf potenziell schädliche Inhalte geprüft werden.
- Der Webbrowser SOLLTE den Benutzer warnen, wenn Informationen über schädliche Inhalte vorliegen.
- Eine alsschädlich klassifizierte Verbindung SOLLTE NICHT aufgerufen werden können.
- Das verwendete Verfahren zur Überprüfung DARF NICHT gegen Datenschutz- oder Geheimschutz-Vorgaben verstoßen.

## APP.1.2.A12 Zwei-Browser-Strategie (H)

- Für den Fall von ungelösten Sicherheitsproblemen mit dem verwendeten Webbrowser SOLLTE ein alternativer Browser mit einer anderen Plattform installiert sein, der dem Benutzer als Ausweichmöglichkeit dient.


