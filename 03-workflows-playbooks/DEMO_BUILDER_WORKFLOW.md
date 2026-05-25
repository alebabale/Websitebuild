# Demo Builder Workflow

Ziel: Aus einer alten oder schwachen lokalen Website eine moderne Premium-Demo erstellen, die als Akquise-Beweisstueck dient.

## Prozess-Merkregel

Bei jedem Prompt, der auf "Website erstellen/modernisieren und auf GitHub zeigen" hinauslaeuft, zuerst den Fast Path aus `FAST_GITHUB_WEBSITE_WORKFLOW.md` verwenden. Nicht jedes Mal neu planen, sondern Analyse, Build, Preview, Publish und Pages-Check als einen Produktionslauf behandeln.

## Phasen-Merkregel

Nutze `PHASED_WEBSITE_SALES_WORKFLOW.md`.

- Phase 1: echt wirkende, funktionierende Verkaufswebsite bauen. Keine sichtbare Demo-Sprache. Buttons, Links, WhatsApp, Telefon, Navigation und lokale Orientierung muessen funktionieren.
- Phase 2: finale Kundenwebsite mit echten Kundendaten, Impressum, Datenschutz, Domain/Hosting, SEO, Testing und Monetarisierung.

## Input

- Website-URL des Zielbetriebs
- optional Branche, Ort, Ansprechpartner oder besondere Hinweise

## Schritt 1: Analyse

Extrahiere:

- Unternehmensname
- Logo
- Branche
- Standort / Region
- Leistungen
- Kontaktinformationen
- bestehende CTAs
- Trust-Elemente
- Bewertungen / Erfahrung / Historie
- Team / Personen / lokale Kompetenz
- Bilder und Assets
- rechtlich sichtbare Links wie Impressum / Datenschutz

Bewerte:

- erster Eindruck
- mobile UX
- Klarheit des Angebots
- CTA-Struktur
- Vertrauensaufbau
- Bildqualitaet
- Modernisierungshebel

## Schritt 2: Demo-Konzept

Entscheide:

- welche Leistungen im Hero priorisiert werden
- welches Bild als Hero funktioniert
- welche Trust-Elemente prominent werden
- welcher Haupt-CTA am besten passt
- welche Angebotskarten sinnvoll sind
- ob Termin, WhatsApp, Notdienst, Formular oder Anfrage im Fokus steht

## Schritt 3: Assets sichern

Speichere passende Assets unter:

`demos/<slug>/assets/`

Bild-Standard:

- pro neuem Projekt zu Beginn 10 passende Bilder sichern
- zuerst aus alter Website, Google-Unternehmensprofil, Kundenmaterial oder gelieferten Fotos uebernehmen, wenn rechtlich/inhaltlich nutzbar
- wenn nicht genug gute Bilder vorhanden sind: 10 passende neutrale Premium-Bilder generieren
- Bilder sauber nach Nutzung benennen, z.B. `hero`, `service-cut`, `service-color`, `interior`, `tools`, `team`, `exterior`, `detail`, `waiting`, `result`
- mindestens 5 Bilder sichtbar auf der Phase-1-Seite einsetzen: Hero, Leistung, Trust/Atmosphaere, Kontakt/Anfahrt, Galerie/Looks
- keine sichtbaren Wasserzeichen, keine lesbaren Fantasie-Logos, keine falschen Markenversprechen

Bevorzugt:

- Logo
- Hero-Bild
- Leistungsbilder
- Teamfoto
- echte Referenz-/Objektbilder

Nur generieren, wenn keine guten Bilder vorhanden sind oder ein atmosphaerisches Premium-Bild fehlt.

## Schritt 4: Demo bauen

Erstelle:

- `demos/<slug>/index.html`
- `demos/<slug>/styles.css`

Nutze die Design-DNA:

- cinematic Hero
- Gold/Creme/Dark
- grosse Typografie
- Premium-Buttons
- mobile first
- conversion-orientierte Struktur

## Schritt 5: Verifikation

Pruefe lokal:

- Seite laedt
- Bilder laden
- Logo sichtbar
- Mobile ohne horizontalen Overflow
- CTA im ersten Viewport sichtbar
- Kontaktlinks technisch korrekt
- Text nicht ueberlagert

Automatisierte Helfer:

```powershell
powershell -ExecutionPolicy Bypass -File .\tools\Update-CacheBuster.ps1 -HtmlPath demos\<slug>\index.html -CssFile styles.css -Token <slug>-001
powershell -ExecutionPolicy Bypass -File .\tools\Preview-Mobile.ps1 -Target http://127.0.0.1:4173/demos/<slug>/index.html -OutDir previews\<slug> -Prefix <slug>
```

## Schritt 6: Outreach vorbereiten

Erstelle kurze Akquise-Nachricht:

- persoenlich
- nicht zu aggressiv
- Demo-Link erwaehnen
- konkreter Nutzen
- Calendly/Termin-CTA

## Output

Am Ende liefern:

- Demo-URL lokal
- genutzte Inhalte / Assets
- erkannte Schwachstellen
- Verbesserungsidee in 3-5 Bulletpoints
- Outreach-Text
- Upload-Hinweis, falls relevant

## Schritt 7: Veroeffentlichen

Wenn ein GitHub-Pages-Repo existiert:

```powershell
powershell -ExecutionPolicy Bypass -File .\tools\Publish-Demo.ps1 -DemoPath demos\<slug> -RepoPath github-work\<repo> -Branch gh-pages -Message "Update <slug>"
powershell -ExecutionPolicy Bypass -File .\tools\Check-GitHubPages.ps1 -Repo <repo>
```
