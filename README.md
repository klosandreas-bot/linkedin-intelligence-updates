# LinkedIn Intelligence – signierte Updates

Dieses öffentliche Repository stellt geprüfte Updates für das lokal ausgeführte LinkedIn Intelligence Dashboard bereit. Das Dashboard wurde unabhängig entwickelt und ist nicht von LinkedIn autorisiert oder unterstützt.

## Aktuelle Version
- Version: **2.4.0**
- Programmarchiv: `LinkedIn-Intelligence-V2.4.0.zip`
- Signiertes Manifest: `latest.json`
- RSA-SHA256-Signatur: `latest.sig`

Ab V2.4 prüft `Start-Dashboard.bat` beim Start auf Updates. Das lokal installierte `updater.py` prüft die Signatur des Manifests und die SHA-256-Prüfsumme des Archivs, bevor freigegebene Programmdateien ersetzt werden. Ohne Internet läuft die lokale Software weiter. Automatische Updates lassen sich mit der Umgebungsvariablen `LINKEDIN_AUTO_UPDATE=0` deaktivieren.

## Datenschutz
Dieses Repository enthält **keine persönlichen LinkedIn-Daten, Zugangstoken, Client Secrets, SQLite-Datenbanken oder privaten Signaturschlüssel**. Jeder Anwender verwaltet seinen eigenen LinkedIn-Datenexport und gegebenenfalls seine eigene LinkedIn-Entwickleranwendung. Der vollständige ZIP-Export kann ohne API-Zugang importiert werden.

## Sicherheitsregeln für Releases
- Ausschließlich signierte und geprüfte Veröffentlichungen publizieren.
- Den privaten Signaturschlüssel niemals committen oder teilen.
- `latest.json` erst zusammen mit passendem `latest.sig` und vorhandenem Archiv bereitstellen.
- Bei vermutetem Schlüsselverlust oder -diebstahl die Auslieferung stoppen und einen kontrollierten Schlüsselwechsel vorbereiten.

Hinweis: Das GitHub-Repository ist ein öffentlicher Updatekanal, kein Speicher für Nutzerdaten. Der Quellcode im ausgelieferten ZIP ist öffentlich einsehbar.
