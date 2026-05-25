# Work Session Memory

Ziel: Waehrend laufender Website-Arbeit regelmaessig Zwischenstaende speichern, damit gute Entscheidungen, Nutzerpraeferenzen und Fehler nicht im Chat verschwinden.

## Arbeitsregel

Bei jedem groesseren Website-Job speichert Codex kurze Stichpunkte:

- nach einer abgeschlossenen Design-/Code-Runde
- nach Nutzerfeedback, das eine neue Regel erkennen laesst
- vor einem Upload auf GitHub
- nach einem sichtbaren Fehler oder einer Korrektur
- am Ende einer Session

## Checkpoint-Format

```md
## YYYY-MM-DD HH:mm - <Projekt/Branche>

Status:
- ...

Gelernt:
- ...

Nutzerpraeferenz:
- ...

Naechster sinnvoller Schritt:
- ...
```

## Aktueller Stand - Berber1

Status:
- Premium-Barbershop-Demo steht lokal und auf GitHub Pages.
- Hero, Trust, Reels, WhatsApp-Anfrage, Planity-Panel, Galerie und Mobile-Menue sind vorhanden.
- GitHub-Pages-Fast-Workflow und Berber1-Sync-Skript existieren.

Gelernt:
- Nutzer will schnelle sichtbare Iterationen, keine langen Theoriepausen.
- Cache-Buster fuer CSS und JS konsequent setzen.
- Asset-Sync ist Pflicht, sobald Bilder generiert oder ersetzt werden.
- Vorher/Nachher-Reels duerfen nur die beschriebene Leistung veraendern.
- WhatsApp darf als Vorqualifizierung funktionieren, auch wenn Planity spaeter noch manuell gepflegt wird.
- Desktop- und Mobile-Varianten von Anfrage-Widgets muessen nach Aenderungen kurz auf gleiche abgefragte Infos getestet werden.
- Nutzer erwartet, dass nuetzliche Micro-Features proaktiv eingebaut werden: Toggle-Buttons, kompakte Mobile-Panels, sichtbare Pflichtfelder, klare Schliessen-Logik.

Nutzerpraeferenz:
- Premium, cinematic, aber lokal-business-tauglich.
- Direkt umsetzbare Conversion-Hebel.
- Weniger grosse Erklaerungen, mehr schneller Build/Sync/Upload.
- Bei Automatisierung ehrlich bleiben: erst Assistenz-Agent verkaufen, Vollautomation nur mit echter Schnittstelle.

Naechster sinnvoller Schritt:
- Bei neuen Branchen sofort ein Branchen-Playbook nutzen.
- Nach Nutzerfoto/URL Assets extrahieren, Demo bauen, Screenshot pruefen, dann GitHub-Ausgabe.

## 2026-05-24 21:10 - New Look Bietigheim

Status:
- Neues Projekt `demos/new-look-bietigheim` angelegt.
- Erste schwarz-goldene Premium-Demo fuer Damen- und Herrenfriseur gebaut.
- Platzhalter-Logo in schwarz/gold, bis echtes Logo fotografiert wird.
- Basisdaten aus Screenshot genutzt: New Look Damen und Herrenfriseur, Freiberger Str. 51, 74321 Bietigheim-Bissingen, 07142 9194397.
- Mobile/desktop Screenshots erstellt: `previews/new-look-bietigheim/new-look-start-5-*`.

Gelernt:
- Wenn kein Logo vorhanden ist, Markenplatzhalter bauen, der spaeter leicht gegen Foto/Logo ausgetauscht werden kann.
- Mobile Header-CTA bei engen Layouts lieber ausblenden, wenn Hero-CTA direkt sichtbar ist.
- Schwarz/gold passt zur vom Nutzer erinnerten Markenwirkung.

Naechster sinnvoller Schritt:
- Wenn Nutzer echtes Logo-Foto liefert: Farben/Typo/Logo-Card anpassen.
- Danach ggf. GitHub-Repo/Pages fuer New Look separat vorbereiten.

## 2026-05-24 21:20 - Workflow-Korrektur Phase 1 / Phase 2

Gelernt:
- Nutzer will in Phase 1 keine sichtbar unfertigen Demos, sondern echt wirkende funktionierende Websites, die man einem Betrieb verkaufen kann.
- Phase 1 muss Buttons, Links, Telefon, Navigation, lokale Daten und CTA-Logik bereits sauber enthalten. WhatsApp nur einbauen, wenn eine echte WhatsApp-Nummer sicher bekannt ist.
- Platzhalter duerfen intern existieren, aber nicht im Interface wie Platzhalter wirken.
- Phase 2 ist dann die exakte Kundenumsetzung mit echtem Logo, echten Fotos, finalen Texten, Impressum, Datenschutz, Domain/Hosting, Implementierung und Monetarisierung.

Naechster sinnvoller Schritt:
- New-Look-Projekt von "Demo-Basis" zu Phase-1-Verkaufswebsite polieren: keine Platzhalter-Hinweise sichtbar, echte Kontaktlinks, Maps/Routenplaner, Footer-Vertrauen und mobil/desktop pruefen.

## 2026-05-24 22:55 - New Look Phase 1 Politur

Status:
- New-Look-Seite zu einer glaubwuerdigeren Phase-1-Verkaufswebsite umgebaut.
- Sichtbare Platzhalter und WhatsApp-Logik entfernt, weil nur die Festnetznummer sicher bekannt ist.
- Hero, Leistungen, Terminplanung, Anfahrt, Kontakt und Footer fuehren jetzt auf echte Telefon- und Google-Maps-Routenlinks.
- Mobile Sticky-Bar fuer Anruf und Route ergaenzt.
- JSON-LD fuer HairSalon mit Adresse und Telefonnummer hinterlegt.
- Statischer Check bestanden: keine kaputten lokalen Assets, keine fehlenden Anker, keine Platzhalter-/WhatsApp-Reste.

Gelernt:
- Phase-1-Seiten duerfen keine Formular- oder Widget-Funktion vortaeuschen. Wenn kein echter Kanal sicher ist, lieber klar auf Anruf/Routenplaner optimieren.
- Bei unbekanntem Logo reicht ein stimmiger Markenplatzhalter, aber ohne sichtbaren Hinweis auf "spaeter austauschbar".
- Headless-Screenshot kann auf dieser Windows-Chrome-Installation ausfallen; dann mindestens statische Checks laufen lassen und im offenen Browser visuell gegenpruefen.
- Wenn der Nutzer WhatsApp explizit will, das Widget wie bei Berber1 bauen: aufklappbar, erneut klickbar zum Minimieren, mit Leistung, Name, Wunschzeit und Rueckrufnummer. Nummer spaeter beim Kunden bestaetigen.

Naechster sinnvoller Schritt:
- Nach Reload im Browser optisch final pruefen.
- Wenn das echte Logo-Foto kommt: Logo, Goldton, Typografie und Hero-Card daran anpassen.
- Fuer eine oeffentliche Kundenversion spaeter Impressum, Datenschutz, finale Oeffnungszeiten und bestaetigte Kontaktkanaele einsammeln.

## 2026-05-24 23:05 - Agentur-Nutzenregel

Gelernt:
- Jede Website muss einen echten Nutzen fuer den Betrieb haben, nicht nur gut aussehen.
- Standardziel: entweder Terminbuchung/Booking so platzieren, dass sie Kunden direkt zum Abschluss fuehrt, oder Anfrage-Erfassung so bauen, dass der Betrieb sofort mit den wichtigsten Infos arbeiten kann.
- Beim Bauen immer fragen: Macht diese Funktion dem Kunden das Leben leichter, spart sie Rueckfragen oder bringt sie schneller einen Termin?

Nutzerpraeferenz:
- Der Nutzer will Webseiten als verkaufbare Arbeitserleichterung fuer lokale Unternehmen positionieren, nicht als reine Design-Demos.

## 2026-05-24 23:15 - New Look Nutzen-Optimierung

Status:
- New-Look-Seite nach der Nutzenregel ueberarbeitet.
- Hero-CTA priorisiert jetzt die vorbereitete WhatsApp-Anfrage; Telefon und Route bleiben sichtbar.
- Leistungs- und Anfrage-Bereiche oeffnen das WhatsApp-Widget mit passender Vorbelegung fuer Leistung oder Wunschzeit.
- Kontaktbereich erklaert klarer, welchen operativen Nutzen die Anfrage hat: weniger Rueckfragen, schnelle Rueckmeldung, Rueckrufnummer.

Gelernt:
- Servicekarten sollen nicht nur informieren, sondern direkt in eine qualifizierte Anfrage fuehren.
- Wenn ein Widget vorhanden ist, sollten Karten/CTAs Presets setzen, damit der Kunde weniger tippt und der Betrieb bessere Nachrichten bekommt.

## 2026-05-24 23:25 - New Look an Berber1-System angeglichen

Status:
- New Look strukturell naeher an Berber1 aufgebaut: Hero, mobile Navigation, Schnell-zur-Anfrage-Ablauf, Trust, Leistungen, typische Wuensche, Anfrage-System, Anfahrt, Kontakt und FAQ.
- Berber1-Prinzip verbessert umgesetzt: mehr Vorqualifizierung, Service-/Zeit-Presets und sichtbarer Kundennutzen fuer den Salon.
- Keine Berber1- oder Demo-Sprache sichtbar auf der Kundenseite.
- Statischer Check bestanden: keine kaputten lokalen Assets, keine fehlenden Anker, Script-Runtime ok.

Gelernt:
- Bewaehrte Seitenstruktur darf kopiert werden, aber sichtbarer Text und Conversion-Fokus muessen zur Marke und zum Betrieb passen.
- "Nur besser" heisst nicht mehr Deko, sondern klarerer operativer Nutzen: weniger Rueckfragen, schnellere Rueckmeldung, mehr brauchbare Anfragen.

## 2026-05-24 23:40 - New Look Planity + Bildstandard

Status:
- New Look um Planity-Profilbereich ergaenzt: Planity sichtbar, aber WhatsApp-Anfrage bleibt als funktionierender Conversion-Fallback.
- 10 neue Premium-Salonbilder generiert und ins Projekt kopiert.
- Bilder staerker eingesetzt: Hero, Leistung, Bildmosaik, typische Wuensche, Planity/Waiting-Area, Anfahrt.
- Technischer Check bestanden: keine kaputten lokalen Assets, keine fehlenden Anker, Script-Runtime ok.

Gelernt:
- Planity nur als echte Buchungsloesung darstellen, wenn online buchbar bestaetigt ist. Sonst ehrlich als Profil/Pruefpunkt integrieren und Anfrage-Erfassung als Hauptnutzen nutzen.
- Neues Projekt startet kuenftig mit 10 passenden Bildern: zuerst aus alter Website/Kundenmaterial, sonst generieren.
- Mehr Bildmaterial macht Phase-1-Seiten sofort echter und verkaufbarer, solange es nicht wie generische Stock-Deko wirkt.

## 2026-05-25 00:10 - TAO sichtbar + Bursi Thai Massage

Status:
- Nutzer moechte sichtbares TAO-Arbeiten: Thought, Action, Observation jeweils kurz ausschreiben.
- Neues Projekt `demos/bursi-thaimassage` erstellt.
- 10 echte Bilder von der alten Bursi-Website gesichert.
- Phase-1-Seite fuer TaiBurSi Traditionelle Thaimassage gebaut.
- Da keine direkte Online-Buchung sichtbar war, wurde ein Termin-Assistent gebaut: Massage, Dauer, Wunschzeit, Beschwerden, Preislogik, Kopieren und Telefon-CTA.

Gelernt:
- Massage-Seiten brauchen eine ruhigere Variante des Berber1/New-Look-Systems: Wellness-Gefuehl, echte Preis-/Dauer-Auswahl, klare Telefonbuchung, weniger aggressive CTA-Sprache.
- Wenn ein Betrieb nur telefonisch bucht, nicht so tun als gaebe es Online-Buchung. Stattdessen Terminwunsch vorbereiten und Anruf erleichtern.
- Sichtbares TAO hilft dem Nutzer, den Agenturprozess zu fuehren und zu bewerten.

## 2026-05-25 00:25 - Bursi Gutschein-Farbwelt

Status:
- Bursi farblich an Nutzerhinweis angepasst: rosa Logo-/CTA-Wirkung, babyblauer Hintergrund, grüne Bambus-Akzente.
- Termin-Assistent und Seitenstruktur unverändert funktionsfähig.
- Cache-Buster auf `bursi-gutschein-1` gesetzt.

Gelernt:
- Wenn Nutzer reale Offline-Markenhinweise nennt, haben diese Vorrang vor generischer Branchenfarbwelt.
- Bei Bestandsseiten kann ein Theme-Override am Ende der CSS die sicherste Methode sein, um Design zu ändern ohne Layout/Logik zu beschädigen.

## 2026-05-25 07:10 - Bursi echtes Gutscheinmotiv

Status:
- Nutzer lieferte `emotionheader.jpg` als echtes Markenmotiv.
- Bild als `assets/brand-emotionheader.jpg` ins Bursi-Projekt kopiert.
- Kopfleiste nutzt das Motiv dezent als Hintergrund mit dunklem Glas-Overlay.
- Palette weiter Richtung Original angepasst: kräftiges Pink, helles Wasser-/Babyblau, Bambusgrün.

Gelernt:
- Bei Offline-Material wie Gutschein/Flyer nicht nur Farben uebernehmen, sondern ein dezentes Markenfragment im UI platzieren, wenn es die Wiedererkennbarkeit erhoeht.

## 2026-05-25 07:35 - Bursi Gutschein-Shop

Status:
- Nutzer lieferte echtes Gutschein-Foto als Referenz.
- Bursi-Seite um integrierten Gutschein-Shop erweitert: Wertauswahl, Massageart, Empfaenger, Absender, Abholhinweis, Vorschau und kopierbare Telefonanfrage.
- Keine Fake-Zahlung eingebaut. Der Shop bereitet die Gutscheinbestellung vor und fuehrt zum Telefon, weil der Betrieb sichtbar telefonisch/analog arbeitet.
- Mobile Schnellleiste hat jetzt einen direkten Gutschein-Einstieg.
- Statischer Check bestanden: keine fehlenden lokalen Assets, keine fehlenden Anker, Gutschein-Script initialisiert korrekt.

Gelernt:
- Gutscheine sind bei Wellness/Massage ein echter Zusatzumsatz und sollten als eigener Conversion-Weg gebaut werden, nicht nur als FAQ-Hinweis.
- Wenn ein Betrieb offline Gutscheine ausstellt, wirkt ein "Reservieren und abholen"-Flow ehrlicher und verkaufbarer als ein unechter Checkout.

## 2026-05-25 08:05 - Bursi WhatsApp-Auswahlseite

Status:
- Privates, ausgefuelltes Gutschein-Foto aus der sichtbaren Seite entfernt.
- Bursi auf zentrale Auswahl umgebaut: Besucher waehlen am Ende immer zwischen Termin und Gutschein.
- Termin- und Gutscheinformular erzeugen direkte WhatsApp-Links mit vorausgefuellter Nachricht.
- Floating-WhatsApp-Widget und mobile Schnellleiste integriert.
- Gutschein wird als sauberer leerer UI-Entwurf gezeigt, nicht als Foto eines echten privaten Gutscheins.
- Runtime-Check bestanden: keine fehlenden Assets, keine fehlenden Anker, WhatsApp-Links fuer Termin und Gutschein werden korrekt erzeugt.

Gelernt:
- Bei Massage/Wellness sollte die Website nicht in mehrere lose CTAs zerfallen. Hauptlogik: Erst inspirieren, dann klar zwischen Termin und Gutschein entscheiden lassen.
- Private Kundenfotos duerfen nicht als sichtbarer Website-Content genutzt werden, wenn sie ausgefuellt oder persoenlich wirken. Besser als Designreferenz verwenden und eine saubere leere Vorschau neu bauen.
- WhatsApp ist fuer Phase-1-Seiten ein guter operativer Abschluss, wenn keine echte Onlinebuchung vorhanden ist: strukturierte Anfrage statt loser Nachricht.

## 2026-05-25 08:20 - Premium-Webdesign-Workflow

Status:
- Nutzer lieferte Cliptics-Artikel zu Premium-Webdesign als neuen Qualitaetsanker.
- Playbook angelegt: `C:\Users\aleza\Documents\Codex\_AI_AGENCY\04_Playbooks\PREMIUM_WEBSITE_WORKFLOW.md`.
- Arbeitsweise angepasst: Premium wird kuenftig als Ausfuehrungsqualitaet bewertet, nicht als mehr Dekoration.

Gelernt:
- Premium-Sites muessen psychologisch Qualitaet signalisieren: klare visuelle Hierarchie, Liebe zum Detail, Vertrauen, hochwertige Bildwirkung und ruhige Exklusivitaet.
- Erst Grundlagen perfekt machen: Typografie, Spacing, echte Bilder, klare lokale Daten, mobile CTA-Fuehrung, Performance.
- Effekte nur verwenden, wenn sie Wert erzeugen. Subtile Bewegung und Microinteractions ja, Spielerei nein.
- Jede lokale Business-Seite braucht einen eindeutigen operativen Abschluss: Termin, Anfrage, Gutschein, Anruf oder Route.
- Vor Abschluss immer pruefen: Premium-Wirkung in 5 Sekunden, mobile/desktop Konsistenz, echte Links, Assets, Anker, Script-Runtime.

## 2026-05-25 08:35 - Bursi Premium-Nachpruefung

Status:
- Bursi mit Premium-Workflow erneut geprueft.
- Relevante Schwachstellen gefunden und bereinigt: Meta-Text, Header-CTA, alte Telefon-/Anruf-Sprache im Trust-/Kontakt-/FAQ-Bereich.
- Privates Gutscheinbild endgueltig aus dem Projektordner entfernt.
- Runtime-Check bestanden: keine fehlenden Assets, keine fehlenden Anker, WhatsApp-Links funktionieren, alte Telefon-Wording-Reste entfernt.

Gelernt:
- Nach groesseren Flow-Umbauten muss die gesamte Microcopy gegen den neuen Hauptprozess geprueft werden. Ein Premium-Flow wirkt schwach, wenn einzelne Texte noch den alten Prozess verraten.
- Private Referenzbilder nicht nur aus dem HTML entfernen, sondern auch aus dem Kundenprojekt loeschen.

## 2026-05-25 08:50 - Kreativere Font-Auswahl

Status:
- Nutzer lieferte BSC-Webdesign-Artikel zu Font-Finder/Schriftwahl.
- Premium-Playbook erweitert: pro Marke bewusste Font-Auswahl statt Standard-Kombi.
- Bursi-Headerlogo von rundem Badge zu laengerem ovalem Markenstempel umgebaut.
- Logo nutzt jetzt `DM Serif Display` als charaktervollere Markenstimme, Body bleibt bei Manrope.

Gelernt:
- Schriftwahl ist Teil der Markenpositionierung. Lokale Business-Seiten sollen nicht alle dieselbe Typografie tragen.
- Maximal zwei bis drei Fonts, aber eine davon darf bewusst Charakter tragen: Logo/Headline anders als Body.

## 2026-05-25 09:00 - Branchen-Erkundung als Pflichtschritt

Status:
- Nutzer moechte, dass neue Branchen nicht blind mit bestehendem Template gebaut werden.
- Premium-Playbook erweitert: Bei jeder neuen Branche automatisch herausfinden, wie diese Website gebaut werden sollte.

Gelernt:
- Vor dem Design fuer neue Branchen immer erst Branchenlogik klaeren: Kaufmotiv, Vertrauenssignale, typische Buchungs-/Anfragewege, relevante Wettbewerber, erwartete Inhalte.
- Ergebnis muss eine kurze Branchen-Hypothese sein: Warum genau diese Struktur, dieser CTA und diese Bild-/Font-Sprache fuer diese Branche passt.

## 2026-05-24 22:00 - Codex-Ordnerstruktur

Status:
- Zentraler Agentur-Hub erstellt: `C:\Users\aleza\Documents\Codex\_AI_AGENCY`.
- Root-Hinweis erstellt: `C:\Users\aleza\Documents\Codex\START_HERE.md`.
- Kundenakten fuer Berber1 und New Look angelegt.
- Business-Angebotsmodell fuer Phase 1 / Phase 2 angelegt.

Gelernt:
- Datumsordner sind technische Codex-Arbeitsbereiche, aber nicht die richtige mentale Ordnung fuer den Nutzer.
- Der Nutzer braucht eine Agenturstruktur nach Kunden, Branchen, Assets, Playbooks, Angeboten und Checkpoints.

## 2026-05-25 09:25 - GI Nails Tamm, erste Nagelstudio-Branche

Status:
- Neue Demo angelegt: `C:\Users\aleza\Documents\Codex\2026-05-23\du-bist-mein-pers-nlicher-ai\demos\gi-nails-tamm`.
- Originaldaten von GI Nails genutzt: Adresse, Telefon, Oeffnungszeiten, Preise, Instagram/Facebook und echte Galerie-Bilder.
- Seite branchengerecht aufgebaut: Hero mit Lookbook, Branchenlogik, Leistungen, transparente Preise, Qualitaets-/Vertrauensbereich, Terminnotiz, Anfahrt, FAQ und mobile Schnellleiste.
- Keine unechte WhatsApp- oder Onlinebuchung eingebaut, weil auf der Originalseite kein bestaetigter WhatsApp-Kanal sichtbar war.
- Demo-Uebersicht ergaenzt und Nagelstudio-Muster im Premium-Workflow gespeichert.
- Statischer Check bestanden: keine fehlenden lokalen Assets, keine fehlenden Anker, Script-Runtime ok.
- Desktop- und Mobile-Screenshot geprueft; mobile Hero-Schrift und CTA-Fuehrung danach kompakter gemacht.

Gelernt:
- Nagelstudio ist visuell entscheidungsgetrieben: Ergebnisse muessen frueh sichtbar sein, weil Kundinnen Form, Farbe, Laenge und Detailgefuehl zuerst pruefen.
- Preisstruktur muss besonders klar sein, weil Leistungen schnell verwechselbar werden: Manikuere, Gellack, Auffuellen, Neumodellage, French/Babyboomer, Extras, Fuss Pflege.
- Phase-1-Seite muss trotzdem einen echten Nutzen haben: strukturierte Terminnotiz spart dem Betrieb Rueckfragen und macht aus einem alten Webauftritt einen funktionierenden Anfrageweg.

## 2026-05-25 09:40 - Ersatzseite statt Demo-Akzente

Status:
- Nutzer hat zurecht markiert: Bei neuen Branchen duerfen keine sichtbaren Demo-/Agentur-Akzente auf der Kundenseite bleiben.
- GI Nails bereinigt: "Branchenlogik" und interne Erklaertexte entfernt, sichtbare Texte auf echte Salon-Sprache umgestellt.
- Terminanfrage von "Terminnotiz kopieren" auf kundenfaehigen E-Mail-Prozess umgestellt: Formular oeffnet eine vorbereitete Mail an `gpileczky@gmail.com`; Telefon und Instagram bleiben direkte Alternativen.
- Premium-Workflow erweitert: Interne Analyse gehoert ins Playbook, nicht in die sichtbare Website.

Gelernt:
- Jede Phase-1-Seite muss wie eine uebernahmefaehige Ersatzseite wirken. Auch kleine Begriffe wie "Demo", "Branchenlogik", "keine direkte Onlinebuchung sichtbar" oder "Notiz kopieren" brechen diese Wirkung.
- Wenn ein echter Kanal unsicher ist, nicht erklaeren, was fehlt. Stattdessen den vorhandenen Kanal professionell nutzen: Anrufen, E-Mail, Instagram, Route oder Gutschein-/Termin-Auswahl.

## 2026-05-25 09:55 - Planity als Beauty-Verkaufsanker

Status:
- Nutzer will Planity bei passenden Branchen immer sichtbar mitdenken, auch wenn der Betrieb es noch nicht aktiv nutzt.
- GI Nails um Planity-Navigation, Hero-Link, eigene Planity-Section, Terminbereich-Link, mobile Planity-Leiste und Schema-sameAs erweitert.
- Planity-Text bewusst ehrlich gehalten: "Planity-Profil oeffnen" statt "Online buchen", solange aktive Buchung nicht bestaetigt ist.
- Premium-Workflow erweitert: Beauty/Friseur/Barber/Kosmetik/Nagelstudio immer auf Planity pruefen und sauber integrieren.

Gelernt:
- Planity ist nicht nur Kundennutzen, sondern Verkaufshebel fuer den Betrieb: Die Website wirkt moderner, und die spaetere Einrichtung kann als Zusatzleistung angeboten werden.
- Sichtbar darf die Seite trotzdem nichts vortaeuschen. Unterschied merken: aktives Planity = "Online buchen"; nur Profil = "Planity-Profil oeffnen" plus echter Anfrage-Fallback.

## 2026-05-25 10:05 - Planity bevorzugt eingebettet

Status:
- Nutzer erlaubt und wuenscht Planity ruhig eingebettet zu nutzen.
- GI Nails Planity-Section von reiner Profilkarte auf eingebetteten Iframe-Bereich mit externem Fallback-Link umgebaut.
- Premium-Workflow aktualisiert: Bei Beauty/Salon/Nails Planity bevorzugt eingebettet verwenden, wenn technisch moeglich.

Gelernt:
- Ein eingebetteter Planity-Bereich wirkt verkaufsstaerker als nur ein Link, weil der Betrieb sofort ein modernes Buchungssystem auf der Ersatzseite sieht.
- Trotzdem Fallback-Link sichtbar lassen, falls der Anbieter Embedding oder Buchung im Iframe blockiert.

## 2026-05-25 10:15 - GI Nails WhatsApp statt E-Mail

Status:
- Nutzer findet E-Mail-Anfrage fuer GI Nails zu schwach und will WhatsApp wie bei Berber1.
- Oeffentlich gelistete mobile Nummer fuer GI Nails gefunden: `0163 2070766`; WhatsApp-Link nutzt `+491632070766`.
- GI Nails Anfragebereich von E-Mail auf WhatsApp umgestellt.
- Anfrage sammelt jetzt Leistung, Mitarbeiterin, Name, Rueckrufnummer, Wunschzeit und Hinweis; mobile Schnellleiste nutzt WhatsApp.
- Premium-Workflow erweitert: Bei Beauty/Salon-Seiten WhatsApp bevorzugen, wenn eine oeffentliche Mobil-/WhatsApp-Nummer auffindbar ist.

Gelernt:
- E-Mail wirkt bei schnellen Beauty-Terminen weniger verkaufsstark. WhatsApp ist naeher am realen Kundenverhalten und nimmt dem Betrieb direkt Rueckfragen ab.
- Mitarbeiterin/keine Praeferenz ist ein starker Zusatzpunkt im Formular, auch wenn nur eine Person sicher bekannt ist.

## 2026-05-25 10:25 - Planity-Bereich nicht wie Demo wirken lassen

Status:
- Nutzer zeigte Screenshot: Planity-Sektion wirkte noch zu sehr wie Demo, vor allem durch grosse Verkaufsheadline und leere Iframe-Flaeche.
- GI Nails Planity-Sektion umgebaut: keine leere Embed-Flaeche mehr, sondern kompakter Buchungsblock mit konkreten Leistungen, Preisen, Planity-Profil und WhatsApp-Anfrage.
- Premium-Workflow erweitert: blockierte/leere Embeds nie als sichtbare Hauptflaeche stehen lassen.

Gelernt:
- Eingebettet wirkt nur verkaufsstaerker, wenn es wirklich geladen und fertig aussieht. Ein leeres Iframe ist schlimmer als ein sauberer nativer Buchungsblock.
- Die sichtbare Sprache muss aus Kundensicht formuliert sein: "Termin bequem vorbereiten" statt "Planity als moderner Weg".

## 2026-05-25 10:40 - Planity + WhatsApp nebeneinander

Status:
- Nutzer markierte "Klare Preisorientierung" als erneut zu intern wirkend.
- GI Nails Trust-Karten auf Kundensprache umgestellt: sorgfaeltige Vorbereitung, vorher klar besprochen, gut erreichbar in Tamm.
- Terminbereich zusammengefuehrt: Planity links als kleines eingebettetes Widget, WhatsApp rechts als Anfrage-Assistent.
- Anker bleiben sauber: `#planity` springt zum Widget, `#termin` zum gemeinsamen Buchungsbereich.
- Validierung bestanden: keine internen/Demo-Begriffe, keine fehlenden Assets/Anker, WhatsApp-URL funktioniert, Planity-Iframe vorhanden.

Gelernt:
- Interne Bewertungsbegriffe fallen dem Nutzer sofort auf. Sichtbare Trust-Karten muessen wie Salonberatung klingen, nicht wie unsere Analyse.
- Beauty-Buchung sollte als Zweiklang gedacht werden: Planity fuer moderne Buchungswirkung, WhatsApp fuer unmittelbare Rueckfragen und echte Abschlusskraft.

## 2026-05-25 10:55 - Seitenfluss bis zum Ende pruefen

Status:
- Nutzer wies zurecht darauf hin, dass nicht nur einzelne Sections, sondern der gesamte logische Verlauf geprueft werden muss.
- GI Nails FAQ korrigiert: geoeffnete Antwort nennt jetzt Planity/WhatsApp und alle relevanten WhatsApp-Felder inklusive Name und Hinweis.
- Zusaetzliche FAQ zu hilfreichen Angaben ergaenzt.
- Final-CTA und Footer hinzugefuegt, damit die Seite nach FAQ wieder zu WhatsApp, Planity, Anruf, Route und Kontakt zusammenlaeuft.
- Premium-Workflow erweitert: Vor Uebergabe immer Seitenfluss, FAQ-Konsistenz und finalen Abschluss pruefen.

Gelernt:
- Eine Seite kann technisch sauber sein und trotzdem logisch offen enden. Besonders FAQ und Footer muessen mit Formularfeldern, CTAs und realen Kontaktwegen zusammenpassen.
- Nach FAQ braucht eine verkaufbare Ersatzseite fast immer einen finalen Handlungsbereich, sonst verliert die Seite am Ende Abschlusskraft.

## 2026-05-25 11:15 - Nagelstudio Mielke Besigheim

Status:
- Zweites Nagelstudio-Projekt erstellt: `C:\Users\aleza\Documents\Codex\2026-05-23\du-bist-mein-pers-nlicher-ai\demos\nagelstudio-mielke-besigheim`.
- Originalseite erfolgreich gelesen: Startseite, Studio, Leistungen, Kontakt und Assets.
- Echte Inhalte uebernommen: Rosemarie Mielke, lizenziertes Institut fuer Hand- und Nagelpflege, Nailmaster, zertifizierte Manicure-Stylistin, alessandro-Bezug, Adresse, Telefon, Mobilnummer, Leistungen und Preise.
- Sichtbarer Stil anders als GI Nails: klassischer, ruhiger, schwarz/creme/rot, institutartiger mit Studiofotos und Beratung statt Trend-Lookbook.
- Planity geprueft: kein eindeutiges Profil fuer dieses Studio gefunden; deshalb kein unsicherer Planity-Button auf der Kundenseite. Termine stattdessen ueber WhatsApp/Telefon als echte Wege.
- Demo-Uebersicht um Mielke ergaenzt.
- Validierung bestanden: keine internen Begriffe, keine fehlenden Assets/Anker, FAQ passt zu Formularfeldern, finaler Abschluss vorhanden, WhatsApp-Link korrekt.
- Desktop- und Mobile-Screenshots geprueft; mobilen Header nachpoliert.

Gelernt:
- Zweites Nagelstudio darf nicht wie GI Nails aussehen. Mielke braucht mehr Lizenz/Vertrauen/Bestand, weniger Trend-Reel-Feeling.
- Wenn kein echtes Planity-Profil existiert, nicht sichtbar so tun als waere es aktiv. Widget-Suche bleibt Pflicht, aber sichtbare Seite muss echte Kundenwege nutzen.
- Lange Original-Logos auf Mobile koennen Header/Navigation sprengen. Bei Bedarf kompakter Header und mobile Actionbar statt sichtbares Menue.

## 2026-05-25 11:25 - Mobile Buttons frueher sauber planen

Status:
- Nutzer weist auf wiederkehrende Fehler wie zu breite Buttons in der Mobile-Version hin.
- Premium-Workflow erweitert: Mobile-Buttons, Sticky-Bars, Hero-CTAs und Widget-Buttons muessen vor Uebergabe gezielt auf Breite, Textumbruch und optische Schwere geprueft werden.

Gelernt:
- Mobile darf nicht erst nach Screenshot-Kritik repariert werden. Buttons brauchen von Anfang an kompakte, responsive Grenzen: kurze Labels, Icon-Text-Segmente, `max-width`, sinnvoller Umbruch und genug Touch-Flaeche ohne den Screen zu dominieren.
- Besonders bei lokalen Business-Seiten entscheiden kleine Mobile-Details darueber, ob die Seite fertig oder nach Baukasten aussieht.

## 2026-05-25 11:45 - Mielke zweite Qualitaetsrunde

Status:
- Nutzer fand den ersten Mielke-Wurf fast gut und wollte eine genauere Nachpruefung.
- Mielke-Seite nachpoliert: sichtbare Kundensprache mit echten deutschen Umlauten, Aiperturmstraße korrekt, WhatsApp-Anfrage sauberer, mobile CTAs kompakter, Sticky-Bar schmaler und Proof-Chips robuster.
- Desktop- und Mobile-Screenshots erneut geprueft; Assets und Anker ohne Fehler; keine internen Demo-/Agenturbegriffe gefunden.

Gelernt:
- Bei deutschen Ersatzseiten wirken ASCII-Ersatzformen wie `fuer`, `Naegel`, `Rueckrufnummer` schnell unfertig. Wenn die Seite kundenseitig uebernehmbar wirken soll, muessen echte Umlaute in sichtbaren Texten benutzt werden.
- Die zweite Qualitaetsrunde muss bewusst auf kleine Mobile-Kanten gehen: Header, Sticky-Bar, Buttonbreiten, lange Badges, echte Ortsdaten und FAQ-/CTA-Sprache.

## 2026-05-25 11:55 - Visuelle Checks vor Praesentation

Status:
- Nutzer will die visuellen Checks plus Anpassungen eingebaut haben, bevor eine Seite praesentiert wird.
- Premium-Workflow erweitert: Vor jeder Praesentation muessen Desktop-Hero, Mobile-Hero und mobiler Termin-/Anfragebereich visuell geprueft und sichtbare Probleme direkt behoben werden.

Gelernt:
- Desktop und Mobile sind zwei verschiedene Verkaufssituationen. Desktop darf grosszuegig, editorial und bildstark sein; Mobile muss schneller, enger, tappbar und abschlussorientiert sein.
- Eine Seite gilt nicht als praesentationsbereit, nur weil Code/Links/Assets stimmen. Erst Screenshot/Viewport-Check plus Nachpolitur macht sie bereit fuer den Nutzer.

## 2026-05-25 12:05 - Container-Overflow bei langen Leistungsnamen

Status:
- Nutzer markierte bei Mielke zwei Stellen, an denen Schrift aus Karten/Containern lief.
- Refill-Kartentitel gekuerzt, Karten-/Preis-Typografie mit Umbruchregeln abgesichert und Desktop-Floating-Button deaktiviert, damit er keine Karte ueberdeckt.
- Premium-Workflow erweitert: Lange deutsche Leistungsnamen und Floating-CTAs muessen gezielt auf Container-Overflow geprueft werden.

Gelernt:
- Beauty-/Nagelstudio-Leistungen enthalten oft sehr lange Komposita. Sichtbare Titel muessen verkaufsstark und kurz sein; Details gehoeren in den Beschreibungstext.
- Schwebende Buttons sind nur gut, wenn sie nichts verdecken. Header-CTA plus Mobile-Sticky-Bar reichen oft aus.
