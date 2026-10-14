# LinkedIn Intelligence – signierte Updates

Öffentlicher Updatekanal des lokal ausgeführten LinkedIn Intelligence Dashboards. Die Software ist unabhängig von LinkedIn entwickelt und wird nicht von LinkedIn herausgegeben oder unterstützt.

## Aktuell: Version 2.6.0

- [LinkedIn Intelligence V2.6.0](./LinkedIn-Intelligence-V2.6.0.zip)
- [Signiertes Versionsmanifest](./latest.json)
- [Digitale Release-Signatur](./latest.sig)

**Neu in V2.6:** Profilbewusste Credibility-Empfehlungen statt mechanischer Score-Jagd. Ein niedriger Score löst nicht automatisch eine Profiländerung aus. Die Auswertung unterscheidet konkrete Prüfpunkte, Beobachtung, fehlende Exportdaten und keinen belegbaren Handlungsbedarf. Sie stellt zeitliche Score-Änderungen dar, ohne daraus Kausalität abzuleiten. Zusätzliche alte Seminare, Zertifikate oder Bestätigungen allein zur Score-Optimierung werden nicht empfohlen.

Ab V2.4 prüft `Start-Dashboard.bat` automatisch auf signierte Updates. Eine fehlende Internetverbindung verhindert den lokalen Start nicht. Die Installation verändert keine persönliche Datenbank, LinkedIn-Exporte, Berichte, Nachrichten oder OAuth-Zugangsdaten.

## Datenschutz und Sicherheit

Dieses Repository enthält **keine privaten Nutzerdaten, Zugangstoken, Client Secrets, SQLite-Datenbanken oder privaten Signaturschlüssel**. Jeder Anwender importiert eigene LinkedIn-Daten und betreibt gegebenenfalls eine eigene Entwickleranwendung. Der verteilte Python-Quellcode ist öffentlich lesbar.

Der private Signaturschlüssel darf niemals hochgeladen oder veröffentlicht werden. `latest.json` und `latest.sig` müssen zur Archiv-Prüfsumme passen. Änderungen an veröffentlichten Releases nur kontrolliert und signiert durchführen.

Die historischen Scores aus dem Datenexport sind keine nachgewiesenen LinkedIn-Feed-Rankingfaktoren. Aus der zeitlichen Überschneidung von Aktivitäten und Score-Änderungen kann keine Ursache abgeleitet werden.
