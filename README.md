# 🎮 palkoli - Fanseite

Professionelle League of Legends Streamer Fanseite mit Live-Status und Highlights.

![Status](https://img.shields.io/badge/Status-Live-brightgreen?style=flat-square)
![League of Legends](https://img.shields.io/badge/Game-League%20of%20Legends-blue?style=flat-square)
![GitHub Pages](https://img.shields.io/badge/Hosting-GitHub%20Pages-333?style=flat-square)

---

## 🌐 Live ansehen

👉 **[palkoli.github.io/palkoli-fanseite](https://palkoli.github.io/palkoli-fanseite/)**

---

## ✨ Features

- 🔴 **Live-Status Badge** - Zeigt an, ob du gerade streamst
- 🎬 **Highlights Galerie** - Deine besten Clips und Videos
- 📺 **Twitch & YouTube Integration** - Direkte Links zu deinen Kanälen
- 📱 **Responsive Design** - Funktioniert auf Desktop, Tablet & Handy
- 🎨 **LoL-Theme** - Hextech-Farben und professionelles Design
- ⚡ **Super schnell** - Hosted auf GitHub Pages (kostenlos!)

---

## 📁 Dateistruktur

```
palkoli-fanseite/
├── index.html          # Die Fanseite
├── clips.json          # Deine Clips & Videos
├── status.json         # Live-Status
└── README.md           # Diese Datei
```

---

## 🚀 Quick Start

### 1. Clips hinzufügen

Öffne `clips.json` und füge deine Videos hinzu:

```json
{
  "title": "Dein Clip-Titel",
  "description": "Kurze Beschreibung",
  "url": "https://www.youtube.com/watch?v=VIDEO_ID",
  "thumbnail": "https://img.youtube.com/vi/VIDEO_ID/maxresdefault.jpg",
  "source": "YouTube",
  "date": "2026-08-29"
}
```

**YouTube Video ID finden:** 
- URL: `https://www.youtube.com/watch?v=dQw4w9WgXcQ`
- ID: `dQw4w9WgXcQ`

**Thumbnail URL:** `https://img.youtube.com/vi/dQw4w9WgXcQ/maxresdefault.jpg`

### 2. Live-Status aktualisieren

Bearbeite `status.json` wenn du live gehst:

```json
{
  "live": true,
  "title": "Ranked Grind - Master Push",
  "game": "League of Legends",
  "viewers": 1523,
  "uptime": "1 Std 45 Min",
  "lastUpdate": "2026-08-29T18:30:00Z"
}
```

Und wenn offline:

```json
{
  "live": false,
  "title": "Stream offline",
  "game": "League of Legends",
  "viewers": 0,
  "uptime": "",
  "lastUpdate": "2026-08-29T20:00:00Z"
}
```

---

## 🎨 Design anpassen

### Farben ändern

Öffne `index.html` und bearbeite die `:root` CSS-Variablen:

```css
:root {
    --void-ink: #0B0E14;           /* Hintergrund */
    --hextech-blue: #2C5C8F;       /* Blau */
    --noxus-crimson: #8C2F3A;      /* Rot */
    --rune-gold: #C8A24B;          /* Gold */
    --parchment: #EDE6D6;          /* Helles Weiß */
    --ash: #8A8F98;                /* Grau */
}
```

### Text ändern

Suche nach `PALKOLI` und ändere es überall wo du willst.

---

## 🤖 Automatisierung (Optional)

### GitHub Actions für Auto-Update

Erstelle `.github/workflows/update-status.yml` um den Stream-Status automatisch alle 5 Minuten zu checken.

**Benötigt:**
- Twitch API Token (https://dev.twitch.tv/console)
- GitHub Secrets für Token-Speicherung

Siehe `SETUP_GITHUB_PAGES.md` für detaillierte Anleitung.

---

## 📱 Mobile-Test

1. Öffne die Seite im Browser
2. Drücke `F12` (Developer Tools)
3. Klick auf "Toggle device toolbar" (oben links)
4. Teste verschiedene Geräte

---

## 🔗 Links

- **Twitch:** https://twitch.tv/palkoli
- **YouTube:** https://youtube.com/@WFLMPwned

---

## 📋 Changelog

### v1.0 (2026-08-29)
- ✅ Initial Release
- ✅ Live-Status Integration
- ✅ Clips-Galerie
- ✅ Responsive Design
- ✅ GitHub Pages Hosting

---

## 🐛 Problembehebung

| Problem | Lösung |
|---------|--------|
| Seite wird nicht angezeigt | Warte 1-2 Minuten, dann F5 drücken |
| Clips laden nicht | Checke `clips.json` mit https://jsonlint.com/ |
| JSON Error | Überprüfe auf fehlende Kommas oder Klammern |
| Status aktualisiert sich nicht | GitHub braucht 30-60 Sekunden zum Deploy |

---

## 💡 Pro-Tipps

- **Neue Clips regelmäßig hinzufügen** - Macht die Seite interessant
- **Gute Thumbnails nutzen** - YouTube liefert automatisch gute Bilder
- **Mobile testen** - Viele Zuschauer nutzen Handys
- **Meta-Daten aktualisieren** - Description und Daten sind wichtig
- **Backup machen** - GitHub speichert alles automatisch

---

## 📞 Support

Probleme oder Fragen?
- Check die Logs (Browser F12)
- Schau in `SETUP_GITHUB_PAGES.md`
- GitHub Issues erstellen

---

## 📄 Lizenz

Frei verwendbar und erweiterbar für deinen Stream! 🎮

---

**Viel Erfolg mit deinem Stream!** 🚀

Made with ⚔️ for League of Legends Streamers
