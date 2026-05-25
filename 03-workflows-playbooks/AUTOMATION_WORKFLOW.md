# Automation Workflow

Ziel: Demo-Websites schneller anpassen, mobil pruefen und auf GitHub Pages veroeffentlichen.

## Fast Path

Fuer neue Demo-Websites oder schnelle Iterationen bevorzugt den gebuendelten Ablauf nutzen:

```powershell
powershell -ExecutionPolicy Bypass -File .\tools\Build-Verify-Publish.ps1 `
  -DemoPath demos\<slug> `
  -RepoPath github-work\<repo> `
  -RepoName <repo> `
  -CssFile styles.css `
  -Token <slug>-001 `
  -Message "Update <slug> demo"
```

Ohne Push, nur Cache-Buster und Screenshots:

```powershell
powershell -ExecutionPolicy Bypass -File .\tools\Build-Verify-Publish.ps1 `
  -DemoPath demos\<slug> `
  -RepoPath github-work\<repo> `
  -RepoName <repo> `
  -CssFile styles.css `
  -Token <slug>-001 `
  -SkipPublish
```

## Standard-Loop

1. Demo lokal bearbeiten:

```powershell
# Beispiel
demos\berber1-barbershop\index.html
demos\berber1-barbershop\concepts.css
```

2. Cache-Buster erhoehen, damit Handy/Browser wirklich die neue CSS-Version laden:

```powershell
powershell -ExecutionPolicy Bypass -File .\tools\Update-CacheBuster.ps1 -HtmlPath demos\berber1-barbershop\index.html -CssFile concepts.css -Token berber1-mobile-003
```

3. Mobile/desktop Screenshots erzeugen:

```powershell
powershell -ExecutionPolicy Bypass -File .\tools\Preview-Mobile.ps1 -Target http://127.0.0.1:4173/demos/berber1-barbershop/index.html -OutDir previews\berber1 -Prefix berber1
```

4. Verzeichnis auf GitHub Pages veroeffentlichen:

```powershell
powershell -ExecutionPolicy Bypass -File .\tools\Publish-Demo.ps1 `
  -DemoPath demos\berber1-barbershop `
  -RepoPath github-work\Berber1 `
  -Branch gh-pages `
  -Message "Update Berber1 mobile layout"
```

5. Pages-Status pruefen:

```powershell
powershell -ExecutionPolicy Bypass -File .\tools\Check-GitHubPages.ps1 -Repo Berber1
```

## Repo-Regel

Das GitHub-Pages-Repo muss direkt diese Struktur haben:

```text
index.html
styles.css oder concepts.css
script.js
assets/
```

Keine zusaetzliche `demos/...` Ebene in GitHub Pages.

## Mobile Checkliste

- Header-CTA nicht abgeschnitten
- Kein horizontaler Overflow
- Hero-Headline im ersten Viewport lesbar
- Floating CTA verdeckt keine wichtigen Inhalte
- Booking/WhatsApp/Planity auf dem Handy nutzbar
- Bilder laden, Logo sichtbar
- CSS-Link hat neuen `?v=` Token

## Naechster Ausbau

- pro Zielbetrieb eine `site.json` anlegen
- automatische Asset-Liste und Kontaktlinks pruefen
- nach dem Push automatisch Pages-Status pollen
- optional Lighthouse/Performance-Check ergaenzen
