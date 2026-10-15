# LinkedIn Intelligence – signierte Updates

Öffentlicher Updatekanal des lokal ausgeführten LinkedIn Intelligence Dashboards. Die Anwendung wurde unabhängig entwickelt und ist kein offizielles Produkt von LinkedIn.

## Aktuelle Version 2.7.0

- [Programmarchiv V2.7.0](./LinkedIn-Intelligence-V2.7.0.zip)
- [Signiertes Versionsmanifest](./latest.json)
- [Release-Signatur](./latest.sig)

**Neu in V2.7:** Die Versionsangabe wird dynamisch aus der installierten `version.json` geladen. Bei Kennzahlen werden exakt identische Datensätze nur einmal gezählt, während die unbearbeiteten Originaldaten erhalten bleiben. Im Bereich „Datenquellen & Abruf“ zeigt das Dashboard den letzten gespeicherten Datenstand je Bereich samt Quelle und Dubletten sowie separat den letzten API-Prüfstatus. Zeiten werden im Browser in deutscher Ortszeit (MEZ/MESZ) angezeigt. Der Bericht heißt „Bericht für KI Auswertung / GitHub“.

Ab V2.4 prüft `Start-Dashboard.bat` bei jedem Start auf Updates. Der lokale Updater validiert die RSA-SHA256-Signatur, prüft die SHA-256-Summe des Archivs und ersetzt nur freigegebene Programmdateien. Bei fehlender Internetverbindung startet die installierte Version weiter.

## Datenschutz und Sicherheit

Dieses öffentliche Repository enthält **keine persönlichen LinkedIn-Daten, SQLite-Datenbanken, Exporte, Nachrichten, Zugangstoken, Client Secrets oder privaten Signaturschlüssel**. Jeder Nutzer verwendet eigene Exporte beziehungsweise seine eigene LinkedIn-API-Autorisierung.

Auch ein niedriger Credibility-Score ist keine Aufforderung zu unnötigen Profileinträgen. Die internen LinkedIn-Scores sind keine nachgewiesenen Feed-Rankingfaktoren. Unveränderte Rohdaten bleiben lokal; bereinigte Zählungen sind methodisch gekennzeichnet.

Den privaten Signaturschlüssel niemals committen, auch nicht in private Repositories. Eine Kompromittierung erfordert einen kontrollierten Schlüsselwechsel.
