# LinkedIn Intelligence – signierte Updates

Öffentlicher Updatekanal des lokal ausgeführten LinkedIn Intelligence Dashboards. Die Software ist unabhängig von LinkedIn entwickelt.

## Aktuelle Version: 2.8.0

- [Programmarchiv V2.8.0](./LinkedIn-Intelligence-V2.8.0.zip)
- [Signiertes Versionsmanifest](./latest.json)
- [Digitale Release-Signatur](./latest.sig)

### Neu in V2.8: Reichweite & Diskussion

- Neue lokale Ansicht „Reichweite & Diskussion“
- Import von LinkedIn-Einzelbeitragsstatistiken als XLSX ohne zusätzliche Python-Abhängigkeiten
- Manuelle Messstände für Privatprofil und Unternehmensseite samt tatsächlichem Messzeitpunkt
- Verlaufsvergleich von Impressionen, Kommentaren und Interaktionen für denselben Beitrag
- Fachlich substanzielle Kommentare und neue Diskussionsteilnehmer werden nur berücksichtigt, wenn der Nutzer sie ausdrücklich dokumentiert
- Keine pauschale Abwertung von Kommentaren aus dem Bekanntenkreis und keine unbelegten Behauptungen über Algorithmus-Sanktionen
- Erklärung der Datenlücke: persönliche Portabilitätsdaten enthalten überwiegend selbst verfasste Kommentare, nicht zuverlässig eingehende Diskussionen

### Softwareupdates

Ab V2.4 prüft `Start-Dashboard.bat` beim Start, ob ein neueres signiertes Update vorliegt. Der Updater prüft die RSA-SHA256-Signatur und die SHA-256-Prüfsumme des Archivs. Ohne Internet startet die lokale Version weiter. Alle Versionen einschließlich V2.7 bleiben zur nachvollziehbaren Historie erhalten.

### Datenschutz und Sicherheit

Keine persönlichen LinkedIn-Daten, SQLite-Datenbanken, ZIP-Exporte, Nachrichten, Zugangstoken, Client Secrets oder private Signaturschlüssel in diesem öffentlichen Repository. Jeder Nutzer verwaltet seine eigene Autorisierung. Der verteilte Python-Quellcode ist öffentlich lesbar.

Die neuen Messstände bleiben ausschließlich in der lokalen Datenbank und werden nicht in kuratierte Berichte oder nach GitHub übertragen. Der private Release-Signaturschlüssel darf niemals veröffentlicht werden. Weder Credibility-Scores noch Kommentarhäufigkeiten belegen eine bestimmte Wirkung auf den LinkedIn-Feed.
