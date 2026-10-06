# Schule

Editoren für Unterrichtsmaterial der Walther-Rathenau-Schulen Schweinfurt. Jede Datei läuft für sich im Browser: einfach öffnen, ohne Installation und ohne Internetverbindung.

| Datei | Wofür |
|---|---|
| `arbeitsblatt-editor.html` | Arbeitsblätter mit Schüler- und Lösungsfassung |
| `leistungsnachweis-editor.html` | Stegreifaufgaben, Kurzarbeiten und Schulaufgaben: Kopf mit Notenfeld, Bearbeitungszeit, Hilfsmitteln und Hinweisen, Teilaufgaben, BE-Lücken zum Eintragen, Gruppe A und B |

Beide Editoren sichern ihren Zwischenstand getrennt im Browser. Arbeitsblätter (`.arbeitsblatt.json`) lassen sich im Leistungsnachweis-Editor öffnen, um Aufgaben zu übernehmen.

## Regelwerk für Aufgaben und Musterlösungen

Ganz oben in `leistungsnachweis-editor.html` steht eine Anleitung für KI-Assistenten: Operatoren, Anforderungsbereiche (40 / 45 / 15 %), Umfang (1 BE je Minute), BE-Regeln für Textantworten, Rechnungen und Diagramme, Haken in der Musterlösung (`[✓]` = 1 BE, `[½]` = ½ BE) und das Dateiformat mit Beispiel. Die Zahlenwerte und die Operatorenliste stehen direkt darunter als JSON-Block `regelwerk`. Eine KI, der man die Datei zusammen mit Hefteinträgen oder Arbeitsblättern gibt, kann daraus eine `.leistungsnachweis.json` mit Musterlösung bauen.

Im Editor prüft der Überblick in der Seitenleiste Umfang, AFB-Verteilung, Operatoren und Haken. Unter „Bewertungsregeln einstellen“ lassen sich die Werte für eine Arbeit anpassen; sie werden mit der Datei gespeichert.
