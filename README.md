# LinkedIn Intelligence – signierte Updates

Öffentlicher Updatekanal für das lokal ausgeführte LinkedIn Intelligence Dashboard. Die Software ist unabhängig von LinkedIn entwickelt und wird nicht von LinkedIn herausgegeben.

## Aktuelle Version: 2.9.0

- [Programmarchiv V2.9.0](./LinkedIn-Intelligence-V2.9.0.zip)
- [Signiertes Versionsmanifest](./latest.json)
- [Release-Signatur](./latest.sig)

### V2.9 – Firmenstatistiken, API-Status und Dubletten

**Unternehmensseite:** Neues eigenständiges Dashboard für LinkedIn-Seitenanalysen. XLS (altes Excel-/BIFF8-Format), XLSX und CSV der Bereiche Inhalte/Beiträge, Follower und Besucher werden lokal eingelesen. Erkannte tägliche Kennzahlen und beitragsbezogene Daten erscheinen getrennt vom Privatprofil. Wiederholte Dateiuploads werden nicht doppelt gezählt; überlappende Zeiträume werden pro Messdatum/Kennzahl anhand des neueren Exports zusammengeführt. Unbekannte Blätter werden ausdrücklich gemeldet, nicht erraten. Demografische Blätter ohne Datum werden derzeit nicht als zeitliche Kennzahlen importiert.

**API-Prüfstatus:** Korrekter letzter Prüflauf und Einzelstatus pro Datenbereich im lokalen Dashboard. Erfolgreicher Import ist von späterer leerer/fehlgeschlagener API-Prüfung unterscheidbar.

**Speicherung:** Exakt identische API-Ereignisse liegen für Auswertungen nur einmal vor. Vollständige Rohantworten mit allen wiederholten Zeilen werden weiterhin lokal in komprimierten, per SHA-256 überprüfbaren Archivdateien vorgehalten. Identische API-Seiten während der Paginierung werden als Fehler erkannt; ein unvollständiger Download überschreibt keinen früheren Datenstand.

**Optionaler Altbestands-Fix:** Mit ausdrücklicher Zustimmung und vorheriger vollständiger SQLite-Sicherung können ältere API-Snapshots platzsparend archiviert werden. Historische Snapshots, Score-Werte, ZIP-Importe, Unternehmensdaten und Originale bleiben erhalten.

### Automatische Updates

Ab V2.4 prüft `Start-Dashboard.bat` bei jedem Start das signierte Manifest und aktualisiert bei Bedarf das Programm. Bei fehlender Verbindung startet die vorhandene lokale Version weiter. Die RSA-SHA256-Signatur und der SHA-256-Hash des Archivs werden geprüft. Alte Releases bleiben in diesem Repository erhalten.

### Datenschutz

Dieses öffentliche Repository enthält **keine persönlichen LinkedIn-Daten, SQLite-Datenbanken, Exporte, Berichte, Nachrichten, Tokens, Client Secrets oder privaten Signaturschlüssel**. Jeder Nutzer verwendet eigene Daten und bei Bedarf eine eigene LinkedIn-API-Autorisierung. Lokale Daten werden vom Softwareupdate nicht ersetzt; Firmenexporte werden nicht an GitHub übertragen.

Die LinkedIn-internen Credibility-Scores sind keine nachgewiesenen Feed-Rankingfaktoren. Ein Zusammenhang zwischen Kommentaren, API-Abfragen oder Profiländerungen und der Beitragsverteilung kann aus den exportierten Daten nicht kausal abgeleitet werden.
