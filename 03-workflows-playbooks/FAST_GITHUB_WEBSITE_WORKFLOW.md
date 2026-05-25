# Fast GitHub Website Workflow

Ziel: Vom Nutzer-Prompt bis zur veroeffentlichten GitHub-Pages-Website moeglichst wenig manuelle Zwischenschritte.

## Grundregel

Wenn der Nutzer eine lokale Business-Demo will, arbeite standardmaessig im Fast Path:

1. Ziel verstehen und Slug festlegen.
2. Vorhandene Website/Assets analysieren.
3. Demo direkt unter `demos/<slug>/` bauen.
4. Parallel eine GitHub-Pages-Arbeitskopie unter `github-work/<repo>/` vorbereiten oder nutzen.
5. Mit einem gebuendelten Tool Cache-Buster, Screenshots, Publish und Pages-Check ausfuehren.
6. Dem Nutzer am Ende nur Ergebnis, Link, Vorschauen und naechste Hebel nennen.

## Fast Path Kommandos

Nur bauen und pruefen:

```powershell
powershell -ExecutionPolicy Bypass -File .\tools\Build-Verify-Publish.ps1 `
  -DemoPath demos\<slug> `
  -RepoPath github-work\<repo> `
  -RepoName <repo> `
  -CssFile styles.css `
  -Token <slug>-001 `
  -SkipPublish
```

Bauen, pruefen, veroeffentlichen:

```powershell
powershell -ExecutionPolicy Bypass -File .\tools\Build-Verify-Publish.ps1 `
  -DemoPath demos\<slug> `
  -RepoPath github-work\<repo> `
  -RepoName <repo> `
  -CssFile styles.css `
  -Token <slug>-001 `
  -Message "Update <slug> demo"
```

Berber1 Spezial-Loop:

```powershell
powershell -ExecutionPolicy Bypass -File .\tools\Fast-Berber1.ps1 -SyncRepo -Token berber1-next
```

## Output-Standard

Am Ende kurz liefern:

- GitHub-Pages-Link
- lokale Dateien, die geaendert wurden
- Screenshot-Pfade fuer mobile und desktop
- was verbessert wurde
- was noch als naechster Conversion-Hebel offen ist

## Wichtige Arbeitsregel fuer Codex

Nicht jedes Mal neu ueber den Prozess nachdenken. Sobald klar ist, dass es eine Website-Demo mit GitHub-Ausgabe ist, diesen Ablauf verwenden und nur bei echten Blockern nachfragen.

## Before/After Reel Logik

Bei Vorher/Nachher-Reels fuer lokale Businesses gilt:

- Nur die Leistung veraendern, die im Reel versprochen wird.
- Keine Nebenverwandlungen erzeugen: Bart, Gesicht, Alter, Kleidung und Person sollen stabil bleiben, wenn sie nicht Thema sind.
- `Fade Refresh`: Seiten und Uebergaenge verbessern, Bart nicht voller oder anders machen.
- `Clean Cut`: Haarschnitt, kurze Seiten und kantige Konturen duerfen deutlich wirken.
- `Beard Line-up`: keine komplette Bart-Transformation; nur Seiten, Linien und Pflegegrad subtil verbessern, damit andere Reels nicht an Wirkung verlieren.
