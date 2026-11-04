# LinkedIn Intelligence – signierte Updates

## Aktuelle Version: 2.9.6 (04.11.2026)

- [Programmarchiv V2.9.6](./LinkedIn-Intelligence-V2.9.6.zip)
- [Signiertes Versionsmanifest](./latest.json)
- [Release-Signatur](./latest.sig)

### V2.9.6 – Reichweitenstatistiken und Auto-Update
- Die persönlichen AggregateAnalytics-XLSX enthalten bis zu 50 TOP-Beiträge mit Impressionen; diese werden nun vollständig importiert und über LinkedIn-Beitragskennungen zugeordnet.
- Mehrere offizielle XLSX-Dateien können gemeinsam importiert werden. Der wiederholte Import derselben Datei ergänzt frühere unvollständige Datensätze.
- Der Extended Report zeigt die Messquelle und den Bezugszeitraum; Zuwächse werden nur zwischen vergleichbaren Exportfenstern berechnet.
- Update wird über den bestehenden RSA-signierten Auto-Updater verteilt, ohne zusätzliche Programme oder Änderung persönlicher Daten.

### V2.9.5 – Erweiterter Beitragsbericht

- Neuer optionaler **Extended Report** mit allen lokal verfügbaren eigenen LinkedIn-Beiträgen, Volltexten, Daten, Links und Datenherkunft.
- Zuordnung verfügbarer Beitrags- und Wochenstatistiken; keine künstlich ergänzten Kennzahlen.
- Lokale Vergleiche zwischen gespeicherten API-/ZIP-Snapshots und Anzeige neu erkannter Beiträge.
- Textmerkmale für den Vergleich von Beitragslänge, Themen und Unicode-Formatierung.
- Der bisherige datensparsame Report bleibt Standard. Keine personenbezogenen Daten, Tokens oder Datenbanken im öffentlichen Repo.
- Signiertes Update kompatibel zu V2.9.1–V2.9.4; alle Tests und die Archivvalidierung erfolgreich.

Öffentlicher Updatekanal für das lokal ausgeführte LinkedIn Intelligence Dashboard. Die Software ist unabhängig von LinkedIn entwickelt und wird nicht von LinkedIn herausgegeben.

### V2.9.1 – Import der Original-Seitenanalyse korrigiert

- Der native deutsche LinkedIn-XLS-Export unter „Inhalte“ wird korrekt gelesen: **„Kennzahlen“** und **„Alle Beiträge“**.
- Die echten Spaltenüberschriften für organische, gesponserte und gesamte Tageswerte, individuelle Impressionen, Klicks, Reaktionen, Kommentare und Interaktionsraten werden erkannt. Die Kategorien werden **nicht addiert**, da „insgesamt“ organisch und gesponsert bereits enthält.
- Veröffentlichungsdatum, dauerhafter Beitragslink und lesbarer Beitragstitel werden getrennt gespeichert. Wiederholte Exporte desselben Beitrags überschreiben pro Kennzahl den früheren Messstand, statt neue Beiträge zu erzeugen.
- US-Datumswerte im Format Monat/Tag/Jahr werden erkannt, ohne mehrdeutige Angaben als Tag/Monat/Jahr zu interpretieren. Deutsche Datumsformate bleiben unterstützt.
- Getestet gegen einen echten, unveränderten LinkedIn-XLS-Inhalteexport mit 30 Tagesdatensätzen und neun Beiträgen sowie durch einen lokalen HTTP-Importtest. Die Originaldatei und privaten Daten sind **nicht Teil dieses Repositorys**.
- Frühere Unternehmensdaten, persönliche SQLite-Datenbank, lokale Exporte und OAuth-Zugangsdaten bleiben unberührt.

### V2.9 – Firmenstatistiken, API-Status und Dubletten

Der eigenständige Bereich „Unternehmensseite“ importiert lokal XLS, XLSX und CSV für Inhalte, Follower und Besucher. Überlappende Zeiträume werden pro Datum und Kennzahl zusammengeführt. Der letzte API-Prüfstatus ist getrennt vom letzten erfolgreichen Import sichtbar.

Neue API-Daten werden in der auswertbaren Kopie um exakt identische Datensätze bereinigt; die vollständigen Originalantworten bleiben komprimiert und lokal abrufbar. Die freiwillige Optimierung vorhandener Snapshots sichert die SQLite-Datenbank vor Änderungen.

### Automatische Updates

Ab V2.4 prüft `Start-Dashboard.bat` beim Programmstart den signierten Updatekanal. Das Update wird nur bei gültiger RSA-SHA256-Signatur und korrektem Archiv-Hash installiert. Bei fehlender Internetverbindung startet die lokale Anwendung weiter.

Dieses öffentliche Repository enthält **keine personenbezogenen LinkedIn-Daten, SQLite-Datenbanken, privaten Exporte, Berichte, Tokens, Client Secrets oder privaten Signaturschlüssel**. Der private Release-Signaturschlüssel darf niemals veröffentlicht werden.

Credibility-Scores und Kommentardaten belegen keine bestimmte Wirkung auf den LinkedIn-Feed.
