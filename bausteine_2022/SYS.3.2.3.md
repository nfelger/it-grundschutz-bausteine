# SYS.3.2.3: iOS (for Enterprise)

## SYS.3.2.3.A1 Strategie für die iOS-Nutzung (B)

- Wird ein MDM eingesetzt, so MÜSSEN die iOS-basierten Geräte über das MDM verwaltet und konfiguriert werden.
- Hierzu MUSS eine Strategie zur iOS-Nutzung vorliegen, in der Aspekte wie die Auswahl der Endgeräte oder Strategien für Datensicherungen festgelegt werden.
- Es MUSS geregelt werden, ob zusätzliche Apps von Drittanbietern genutzt werden sollen bzw. dürfen.
- Außerdem MÜSSEN Jailbreaks organisatorisch untersagt und nach Möglichkeit technisch verhindert werden.

## SYS.3.2.3.A2 Planung des Einsatzes von Cloud-Diensten (B)

- Bevor iOS-basierte Geräte verwendet werden, MUSS festgelegt werden, welche Cloud-Services in welchem Umfang genutzt werden sollen bzw. dürfen.
- Dabei SOLLTE berücksichtigt werden, dass iOS-basierte Geräte grundsätzlich eng mit iCloud-Diensten des Herstellers Apple verzahnt sind.
- Außerdem SOLLTE berücksichtigt werden, dass beispielsweise bereits die Aktivierung von Einzelgeräten mit einer Apple-ID hiervon betroffen ist.
- Daher SOLLTE geprüft werden, ob zur Geräteregistrierung Apple Business Manager (früher Device Enrollment Program, DEP) genutzt werden kann.

## SYS.3.2.3.A3 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## SYS.3.2.3.A4 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## SYS.3.2.3.A5 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## SYS.3.2.3.A6 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## SYS.3.2.3.A7 Verhinderung des unautorisierten Löschens von Konfigurationsprofilen (B)

- Damit Konfigurationsprofile nicht unautorisiert gelöscht werden können, MÜSSEN geeignete technische (z. B. durch den betreuten Modus) oder organisatorische Maßnahmen getroffen und umgesetzt werden.
- Benutzer von mobilen Endgeräten SOLLTEN für den Sinn und Zweck der Sicherheitsmaßnahmen sensibilisiert werden.

## SYS.3.2.3.A8 ENTFALLEN (B)

- Diese Anforderung ist entfallen.

## SYS.3.2.3.A9 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.3.2.3.A10 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.3.2.3.A11 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.3.2.3.A12 Verwendung von Apple-IDs (S)

- Statt einer persönlichen Apple-ID des Benutzers SOLLTE eine anonymisierte Apple-ID verwendet werden.
- Falls möglich, SOLLTE der Apple Business Manager für Volumenlizenzen (früher Volume Purchase Program, VPP) sowie eine zentralisierte Installation von Apps verwendet werden.

## SYS.3.2.3.A13 Verwendung der Konfigurationsoption „Einschränkungen unter iOS“ (S)

- Alle nicht benötigten oder erlaubten Funktionen bzw. Dienste von iOS SOLLTEN deaktiviert werden.
- Basierend auf dem Einsatzzweck und dem zugrundeliegenden Schutzbedarf SOLLTE geprüft werden, welche der Funktionen „Sperrbildschirm“, „Unified Communication“, „Siri“, „Hintergrundbild“, „Verbindung mit Host-Systemen“ und „Diagnose- und Nutzungsdaten“ einzusetzen sind.

## SYS.3.2.3.A14 Verwendung der iCloud-Infrastruktur (S)

- Bevor die umfängliche oder selektive Nutzung der iCloud-Infrastruktur für eine dienstliche Nutzung freigegeben wird, SOLLTE bewertet werden, ob die allgemeinen Geschäftsbedingungen der Firma Apple mit den internen Richtlinien hinsichtlich Verfügbarkeit, Vertraulichkeit, Integrität und Datenschutz vereinbar sind.
- Wird die Nutzung der iCloud-Infrastruktur erlaubt, SOLLTE die Identität am iCloud-Webservice durch eine Zwei-Faktor-Authentisierung geprüft werden.
- Ansonsten SOLLTE die iCloud-Nutzung für einen rein dienstlichen Bedarf auf ein geringes Maß reduziert oder komplett ausgeschlossen werden.

## SYS.3.2.3.A15 Verwendung der Continuity-Funktionen (S)

- Wurde die Nutzung der iCloud-Infrastruktur nicht grundsätzlich durch das Sicherheitsmanagement der Institution untersagt, SOLLTE die Vereinbarkeit der Continuity-Funktionen mit den internen Richtlinien unter Berücksichtigung der Aspekte Vertraulichkeit und Integrität bewertet werden.
- Auf Basis der Bewertungsergebnisse SOLLTE geregelt werden, inwieweit diese Funktionen technisch bzw. organisatorisch eingeschränkt werden.

## SYS.3.2.3.A16 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.3.2.3.A17 Verwendung der Gerätecode-Historie (S)

- Im Konfigurationsprofil SOLLTE die Anzahl der eindeutigen Codes bis zur ersten Wiederholung auf einen angemessenen Wert festgelegt sein.

## SYS.3.2.3.A18 Verwendung der Konfigurationsoption für den Browser Safari (S)

- Die bereits in der Institution etablierten Browserrichtlinien SOLLTEN entsprechend auch für Safari durch technische und organisatorische Maßnahmen umgesetzt werden.
- Dabei SOLLTEN die bereits etablierten Anforderungen für Browser auf stationären und tragbaren PCs als Grundlage für die Absicherung der iOS-basierten Geräte dienen sowie die Einsatzszenarien.
- Das Einsatzumfeld der Geräte SOLLTE beachtet werden.

## SYS.3.2.3.A19 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.3.2.3.A20 ENTFALLEN (S)

- Diese Anforderung ist entfallen.

## SYS.3.2.3.A21 Installation von Apps und Einbindung des Apple App Stores (S)

- Um sicherzustellen, dass den autorisierten Benutzern die benötigten Apps zum notwendigen Zeitpunkt ausreichend zur Verfügung stehen, SOLLTE überlegt werden, den Apple Business Manager in die MDM-Infrastruktur zu integrieren.
- Zahlungen im App Store SOLLTE NICHT über biometrische Verfahren bestätigt werden.

## SYS.3.2.3.A22 ENTFALLEN (H)

- Diese Anforderung ist entfallen.

## SYS.3.2.3.A23 Verwendung der automatischen Konfigurationsprofillöschung (H)

- Geräte, die über einen klar definierten Zeitraum durchgängig offline sind, SOLLTEN ihren Zugang zur internen Infrastruktur verlieren.
- Nach Ablauf des definierten Zeitraums oder an einem bestimmten Tag, SOLLTE das Konfigurationsprofil ohne Zutun der IT-Zuständigen gelöscht werden.
- Falls der Benutzer des Geräts vor Ablauf der Frist auf das interne Netz zugreift, SOLLTE der Zeitraum bis zur automatischen Löschung des Konfigurationsprofils erneuertwerden.
- Falls sicherzustellen ist, ob der Benutzer noch im Besitz des Gerätes ist, SOLLTE der Benutzer aktiv zum Zugriff innerhalb einer Frist aufgefordert werden.
- Falls die Frist ohne Zugriff verstricht, sollte das Konfigurationsprofil dieses Benutzers automatisch gelöscht werden.

## SYS.3.2.3.A24 ENTFALLEN (H)

- Diese Anforderung ist entfallen.

## SYS.3.2.3.A25 Verwendung der Konfigurationsoption für AirPrint (H)

- Freigegebene AirPrint-Drucker SOLLTEN dem Benutzer durch ein Konfigurationsprofil bereitgestellt werden.
- Um zu vermeiden, dass Informationen auf nicht vertrauenswürdigen Druckern von Benutzern ausgedruckt werden können, SOLLTEN stets alle Kommunikationsverbindungen über die Infrastruktursysteme der Institution geführt werden.

## SYS.3.2.3.A26 Keine Verbindung mit Host-Systemen (H)

- Um zu vermeiden, dass iOS-basierte Geräte unautorisiert mit anderen IT-Systemen verbunden werden, SOLLTEN die Benutzer iOS-basierte Geräte ausschließlich mit dem MDM verbinden können.

## SYS.3.2.3.A27 ENTFALLEN (H)

- Diese Anforderung ist entfallen.


