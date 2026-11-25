# Unser Kochbuch

Familien-Kochbuch als Web-App (eine Datei: `index.html`), gehostet über GitHub Pages.

- `data/recipes.json` – alle Rezepte (Schlüssel = Rezept-ID)
- `data/history.json` – Verlauf der bestätigten Rezepte

## Speichern auf dem Handy

Lesen geht ohne Anmeldung. Zum Speichern braucht jedes Gerät einmal einen GitHub-Schlüssel
(Fine-grained personal access token, nur für dieses Repository, Berechtigung „Contents: Read and write“).
Unten auf der Seite „GitHub-Schlüssel für dieses Gerät“ antippen und einfügen.
Jede Änderung wird als Commit gespeichert, damit ist alles versioniert.

## Kochbuch als PDF (`buch.html`)

Erreichbar über „Kochbuch als PDF“ in der Übersicht oder „Als PDF“ bei einem Rezept.
Aufbau: Titelseite, Inhaltsverzeichnis nach Kapitel (`chapter`) und Unterkapitel (`subchapter`),
jedes Rezept als Doppelseite (links Foto mit optionaler Hinweis-Box `photoNote`, Titel, Einleitung, Notizen;
rechts Zutaten, Eckdaten `prepTime`/`restTime`/`cookTime`/`time`/`servings`, Schritte),
hinten ein Stichwortverzeichnis (Titel, Themen, Hauptzutaten, `keywords`).
Fotos liegen in `images/`, das Rezept speichert nur den Pfad (`photo`).

## Kapitelansicht
Unterkapitel und ihre Abschnitte (`section`) sind aufklappbare Felder. Beim Öffnen eines Unterkapitels sind seine Abschnitte offen.
