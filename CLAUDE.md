# Portfolio-Website Aline Piazza

## Was dieses Projekt ist

Ein persönliches Portfolio als Website, um Alines Arbeit als Videoproduzentin und Storytellerin sichtbar zu machen – Zielgruppe: potenzielle Arbeitgeber und Kunden. Gezeigt werden Videos (meist Hochformat), Foto-Projekte und Texte.

## Arbeitsweise (wichtig!)

- Aline hat keinen Programmierhintergrund. Sie ist offen fürs Mitarbeiten am Code, braucht aber Erklärungen.
- **Strikt ein Schritt nach dem anderen.** Vor jeder Aktion kurz erklären, was passiert und warum. Keine grossen Sprünge, keine fünf Dinge auf einmal.
- Kommunikation auf Deutsch.
- Bei Entscheidungen: Optionen kurz erklären, Empfehlung geben, Aline entscheiden lassen.

## Bereits getroffene Entscheidungen

- **Hosting:** GitHub Pages (statische Website, kostenlos). Aline hat bereits ein GitHub-Konto.
- **Eigene Domain:** geplant, aber noch nicht gekauft (voraussichtlich .ch, z.B. via Infomaniak). Kommt als späterer Schritt.
- **Sprachen:** Zweisprachig Deutsch und Englisch. Die Sprachstruktur von Anfang an sauber anlegen (z.B. `/de/` und `/en/` oder gleichwertige Lösung – Optionen mit Aline besprechen).
- **Videos:** werden NICHT direkt gehostet, sondern auf Vimeo hochgeladen und eingebettet. Wichtig: Hochformat (9:16 bzw. 4:5) muss sauber eingebettet dargestellt werden.
- **Technik:** So einfach wie möglich. Statisches HTML/CSS (ggf. wenig JS) ist völlig ausreichend – kein Framework, kein Build-Tool, ausser es gibt einen sehr guten Grund (dann mit Aline besprechen). Aline soll später selbst neue Projekte hinzufügen können.

## Design

Das Design lebt in einem Claude-Design-Projekt (Design-System „Classical") und wird dort ggf. noch weiterentwickelt. **Erster Schritt in Claude Code: das Design von dort importieren.** Anweisung aus Claude Design (im Original belassen):

> Use the claude_design MCP (https://api.anthropic.com/v1/design/mcp, auth via /design-login) to import this project:
> https://claude.ai/design/p/07436125-21ec-4a2e-be5c-808541c9071e?file=Aline+Piazza+Portfolio.dc.html
> Implement: Aline Piazza Portfolio.dc.html

Der Design-Entwurf enthält mehrere Varianten. Gewählte Richtung: **Variante 1a „Das Editorial"** (nur diese umsetzen, ggf. in aktualisierter Form, falls Aline sie im Design-App weiterentwickelt hat):

- Warmer heller Hintergrund (#f3f2f2), Text #201f1d, goldener Akzent (#b68235-Ramp)
- Schriften: Cormorant Garamond (Überschriften), Lora (Fliesstext), via Google Fonts
- Struktur der Startseite: Navigation → grosser Serifen-Hero mit persönlichem Einleitungstext → durchscrollbares 3×3-Raster mit Hochformat-Tafeln (4:5) für alle Arbeiten → „Über mich" mit Porträt → Kontakt → Footer
- Die CSS-Variablen aus dem importierten Design-System (`styles.css` von „Classical") als Grundlage übernehmen

## Noch zu bauen / offene Punkte

1. **Startseite** als saubere, mobiltaugliche Umsetzung des Designs (Raster bricht auf Mobile auf 1–2 Spalten um; der Entwurf ist bisher nur Desktop).
2. **Projekt-Detailseiten:** Klick auf eine Tafel öffnet das Projekt – eingebettetes Hochformat-Video (Vimeo) bzw. Artikeltext, plus Beschreibung. Eine wiederverwendbare Vorlage bauen.
3. **Inhalte:** Aktuell Platzhalter-Projekte aus dem Design-Entwurf. Echte Titel, Texte, Bilder und Videos liefert Aline nach und nach.
4. **Kontakt:** Das Formular aus dem Entwurf funktioniert auf einer statischen Seite nicht ohne Backend. Einfachste Lösung: mailto-Link; Alternative: Formulardienst (z.B. Formspree). Mit Aline besprechen.
5. **Deployment:** GitHub-Repository anlegen, GitHub Pages aktivieren, später Domain verbinden.
6. **Pflege-Anleitung:** Am Ende soll Aline verstehen und dokumentiert haben, wie sie selbst ein neues Projekt hinzufügt.

## Was NICHT tun

- Keine E-Mail-Adressen, Namen oder Platzhalterdaten aus dem Design-Entwurf ungeprüft übernehmen (z.B. „aline@piazza.example" ersetzen).
- Keine Komplexität einführen, die Aline später nicht selbst pflegen kann.
- Nichts veröffentlichen/pushen ohne Alines ausdrückliches Okay.
