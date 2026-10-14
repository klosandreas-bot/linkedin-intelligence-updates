# LinkedIn Intelligence – signierte Updates

Dieses öffentliche Repository stellt signierte Updates für das lokal ausgeführte LinkedIn Intelligence Dashboard bereit. Die Software ist unabhängig entwickelt und wird nicht von LinkedIn herausgegeben oder unterstützt.

## Aktuelle Version: 2.5.0

- [Programmarchiv V2.5.0](./LinkedIn-Intelligence-V2.5.0.zip)
- [Signiertes Versionsmanifest](./latest.json)
- [Digitale Release-Signatur](./latest.sig)

**V2.5** ergänzt den fachgebietsbezogenen Credibility-Maßnahmenplan. Jede der fünf Dimensionen wird im eigenen Score-Thema analysiert. Zeitlich neuere Kenntnisbestätigungen können bei einem späteren Datenexport als Beobachtungsfall überprüft werden. Die empfohlenen Profilmaßnahmen sind keine garantierten Ursachen für höhere LinkedIn-Scores.

Ab V2.4 prüft `Start-Dashboard.bat` automatisch auf Updates. Der lokale Updater validiert die RSA-SHA256-Signatur und die SHA-256-Prüfsumme des Archivs und ersetzt ausschließlich freigegebene Programmdateien. Offline startet die installierte Fassung weiter.

## Datenschutz und verantwortlicher Einsatz

Das Repository enthält keine Nutzerdaten, SQLite-Datenbanken, LinkedIn-Exporte, Tokens, Client Secrets oder private Signaturschlüssel. Jeder Anwender arbeitet mit seinem eigenen ZIP-Export und gegebenenfalls seiner eigenen API-Autorisierung. Die über GitHub öffentlich heruntergeladenen Programmdateien sind lesbar.

## Release-Sicherheit

Der private Release-Schlüssel darf nicht ins Repository, auch nicht in dessen Historie. `latest.json` und `latest.sig` müssen dieselben exakt signierten Bytes repräsentieren; das freigegebene Archiv muss zum hinterlegten SHA-256 passen. Bei einer Schlüsselkompromittierung ist ein kontrollierter Schlüsselwechsel erforderlich.

Die Scores aus LinkedIn-Exporten sind keine bestätigten Feed-Rankingfaktoren. Aus Veränderungen kann ohne zusätzliche Informationen keine Kausalität abgeleitet werden.
