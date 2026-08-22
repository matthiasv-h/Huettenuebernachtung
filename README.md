# Vier Hütten zur Auswahl

Eine Seite, die vier SAC-Hütten vorstellt. Läuft ohne Server – reines HTML.

## Auf GitHub Pages veröffentlichen

1. Auf github.com ein neues Repository anlegen, z. B. `huettenwahl`. **Public**, ohne README.
2. Dateien hochladen: auf der Repo-Seite **Add file → Upload files**, dann `index.html` und den Ordner `fotos/` hineinziehen und **Commit changes**.
3. **Settings → Pages** öffnen. Bei *Source* **Deploy from a branch** wählen, Branch `main`, Ordner `/ (root)`, **Save**.
4. Nach ein bis zwei Minuten ist die Seite unter `https://DEINBENUTZERNAME.github.io/huettenwahl/` erreichbar.

Alternativ per Kommandozeile:

```bash
git init
git add .
git commit -m "Hüttenwahl"
git branch -M main
git remote add origin https://github.com/DEINBENUTZERNAME/huettenwahl.git
git push -u origin main
```

## Fotos einsetzen

In den Ordner `fotos/` legen, exakt so benannt:

| Datei | Hütte |
|---|---|
| `sewen.jpg` | Sewenhütte |
| `glattalp.jpg` | Glattalphütte |
| `lidernen.jpg` | Lidernenhütte |
| `rugghubel.jpg` | Rugghubelhütte |

Fehlt ein Foto, zeigt die Karte einfach ein farbiges Feld – die Seite funktioniert trotzdem.

Querformat ist ideal (etwa 1600 × 1000 Pixel), pro Bild möglichst unter 500 KB, damit die Seite auf dem Handy schnell lädt.

**Achtung Urheberrecht:** Eine öffentliche GitHub-Pages-Seite ist für alle sichtbar. Nur eigene Fotos verwenden oder solche, für die eine Erlaubnis vorliegt. Bilder von den Hüttenseiten vorher kurz anfragen.

## Ändern

Texte stehen direkt in `index.html`. Die Farbe einer Karte steckt im `style="--c: …"` des jeweiligen `<article>`.
