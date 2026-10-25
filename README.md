<p align="center">
  <img src=".github/logo.svg" width="72" height="72" alt="">
</p>

<h1 align="center">BlueProceedings ISMS</h1>

<p align="center"><b>Ein ISMS-Werkzeug für Grundschutz++, das mitläuft.</b><br>
On-Premises per Docker · ohne Hersteller-Cloud · Pre-Alpha</p>

<p align="center">
  <a href="https://blueproceedings.de">Website</a> ·
  <a href="https://www.linkedin.com/company/blueproceedings">LinkedIn</a> ·
  <a href="https://github.com/BlueProceedings/blueproceedings-community">Community</a>
</p>

---

> **Stand: Pre-Alpha.** Dieses Repository ist bis zur ersten Version ein Platzhalter. Container-Image und
> Installationsanleitung sind für **Januar 2027** geplant. Wer die Entwicklung verfolgen möchte: oben rechts auf
> **Watch → Custom → Releases** klicken, dann meldet GitHub die erste Version.

## Worum es geht

Tabellen, Vorlagen und One-Pager halten einen Stand fest. Mit der Freigabe ist ein ISMS nicht fertig: Prozesse ändern sich,
Nachweise laufen ab, eine Maßnahme ist erledigt, aber niemand hat geprüft, ob sie wirkt. Das Sicherheitskonzept sieht
weiter grün aus, weil keine alte Tabelle widerspricht.

BlueProceedings ISMS setzt die Grundschutz++-Methodik als verbundene Arbeitskette um:

```
Prozesse und Informationen → Komponenten und Dienstleister → Schutzbedarf → Anforderungen
→ Risiken → Maßnahmen → Nachweise → Wirksamkeit → Freigabe
```

Jede Angabe weiß, woher sie kommt und was von ihr abhängt. Ändert sich ein Glied, zeigt BlueProceedings ISMS, was neu zu
bewerten ist, und Berichte sagen, seit wann und warum sie veraltet sind.

## Was die Pre-Alpha heute abbildet

| Bereich | Beispiele |
|---|---|
| Kontext | Stakeholder, interne und externe Faktoren, Compliance, Geltungsbereich |
| Struktur | Prozesse, Informationen, Komponenten, Dienstleister, Standorte, Schutzbedarf (normal, hoch) |
| Anforderungen | Grundschutz++-Katalog und weitere OSCAL-Kataloge, Blaupausen, Parameter, Nachweise, Fristen, Katalog-Migration |
| Risiken | Risikoregister mit Historie, Ausbreitungsprüfung über Abhängigkeiten, Akzeptanz mit Wiedervorlage |
| Verantwortung | Rollen, RACI, Vertretungen, Vier-Augen-Freigaben, Kleinunternehmen-Modus |
| Überwachung | Kennzahlen, Auditprogramm, Prüfpaket, Wirksamkeitsprüfung, Managementbewertung |
| Notfall (BCM) | Sicherheitsvorfälle, BIA, Notfallorganisation, Notfallszenarien, Krisenläufe, Übungen |
| Berichte | Veraltet-Warnung mit Ursache, Konsistenzprüfungen, OSCAL-Export |
| Schneller Start | Vorlagen, Einrichtungsassistent, Lern-Modus |

Bilder aus der Pre-Alpha mit fiktiven Daten zeigt die [Website](https://blueproceedings.de/#funktionen).

## Fahrplan

| Zeitpunkt | Schritt |
|---|---|
| Anfang 2026 | Entwicklung beginnt, von Grundschutz++ gibt es erst Umrisse |
| Oktober 2026 | Pre-Alpha; Feinschliff in Teilen öffentlich, Fortschritte regelmäßig auf [LinkedIn](https://www.linkedin.com/company/blueproceedings) |
| 27.10.2026 | Das BSI stellt Grundschutz++ auf der it-sa vor |
| 11.11.2026 | Testphase: bis zu elf Personen aus der ISMS-Praxis testen die Pre-Alpha, Bewerbung per E-Mail, manuelle Auswahl, kein Anspruch auf Teilnahme ([Bewerben](mailto:info@blueproceedings.de?subject=Interessiert%20an%20der%20Testteilnahme)) |
| 01.01.2027 | Grundschutz++ wird laut BSI zertifizierbar |
| Januar 2027 (geplant) | Erste Version: Container-Image, `docker-compose.yml`, Alpha-Lizenzbedingungen (Termin ist eine Planung, keine Zusage) |

## Betrieb (ab der ersten Version)

- Auslieferung als Container-Image über `ghcr.io`, Start per `docker compose`.
- Läuft auf eigener Infrastruktur. Für den Regelbetrieb ist keine Hersteller-Cloud nötig.
- Verschlüsselte Datenbank. BlueProceedings hat keinen Zugriff auf die Produktdaten, und die Anwendung übermittelt im
  Standardbetrieb keine Produktdaten an BlueProceedings. Daten verlassen sie nur durch einen bewusst erzeugten Export; ab
  dann verantwortet der Betreiber Transport, Empfänger und Aufbewahrung.

## Kosten und Lizenz

Die Alpha wird mit einer unentgeltlichen Alpha-Lizenz bereitgestellt; alle Alpha-Lizenzen enden spätestens zwei Jahre nach dem allgemeinen Veröffentlichungsdatum der Alpha. Enddatum und Bedingungen werden vor dem Download angezeigt, für spätere Versionen sind keine Preise zugesagt. Kostenpflichtige Unterstützung kann gesondert vereinbart werden. Das Angebot richtet sich ausschließlich an Unternehmer im Sinne des § 14 BGB, juristische Personen des öffentlichen Rechts und öffentlich-rechtliche Sondervermögen; Verträge mit Verbrauchern werden nicht geschlossen. Dieses Repository enthält keinen Quelltext und gewährt keine Nutzungsrechte.

## Einordnung

BlueProceedings ISMS unterstützt die Vorbereitung auf Grundschutz++: Es hält Anforderungen, Nachweise, Prüfungen und
Entscheidungen nachvollziehbar zusammen. Es macht keine Aussage über Konformität oder Zertifizierung; Bewertung,
Freigabe, Audit und Zertifizierung bleiben Aufgabe der zuständigen Personen und Stellen.

BlueProceedings ISMS ist ein unabhängiges Projekt von BlueProceedings, einem Einzelunternehmen in Bonn. Es wird nicht im
Auftrag eines Arbeitgebers entwickelt. Der Grundschutz++-Katalog stammt aus dem
Repository [BSI-Bund/Stand-der-Technik-Bibliothek](https://github.com/BSI-Bund/Stand-der-Technik-Bibliothek)
(CC BY-SA 4.0).

## Mitmachen und Kontakt

- Vorlagen und Erfahrungen: [blueproceedings-community](https://github.com/BlueProceedings/blueproceedings-community)
  mit offenen Diskussionen.
- Interesse an BlueProceedings ISMS für deine Institution: [info@blueproceedings.de](mailto:info@blueproceedings.de?subject=Interesse%20an%20BlueProceedings%20ISMS)
- Sicherheitslücken bitte nicht öffentlich melden, sondern wie in [SECURITY.md](SECURITY.md) beschrieben.

[Impressum](https://blueproceedings.de/impressum/) · [Datenschutz](https://blueproceedings.de/datenschutz/)
