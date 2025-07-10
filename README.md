# steuer-calc
Die wichtigsten Toppics

✅ Diese Berechnung basiert auf den aktuellen Thüringer Steuersätzen und Beitragssätzen für 2025. Berücksichtigt werden: Gewerbesteuer mit durchschnittlichem Hebesatz von 380% für Thüringen, Kirchensteuer von 9%, Kleinunternehmerregelung bei Umsatz unter 22.000€.








# 🔍 Website Code-Analyse Report

## 📦 Externe Libraries & Dependencies

| Library | Status | URL/Quelle |
|---------|--------|-------------|
| **Tailwind CSS** | ✅ Verwendet | `https://cdn.tailwindcss.com` |
| style.css | ❌ Nicht eingebunden | Datei vorhanden aber ungenutzt |
| tailwind.css | ❌ Nicht eingebunden | Datei vorhanden aber ungenutzt |

## ⚙️ JavaScript-Funktionen

| Funktion | Zweck | Status |
|----------|-------|--------|
| `toggleTheme()` | Dark/Light Mode wechseln | ✅ Verwendet |
| `initTheme()` | Theme beim Laden initialisieren | ✅ Verwendet |
| `calculateGewerbesteuer()` | Gewerbesteuer berechnen | ✅ Verwendet |
| `calculateEinkommensteuer()` | Einkommensteuer berechnen | ✅ Verwendet |
| `calculateKrankenversicherung()` | KV-Beiträge berechnen | ✅ Verwendet |
| `formatCurrency()` | Währung formatieren | ✅ Verwendet |
| `calculate()` | Hauptberechnung starten | ✅ Verwendet |

## 🎯 Event Handler

| Handler | Element | Funktion |
|---------|---------|----------|
| `onclick="toggleTheme()"` | Theme Button | Dark/Light Mode |
| `onclick="calculate()"` | Berechnen Button | Startet Berechnung |

## 🏷️ HTML Element-IDs

### ✅ Verwendete IDs
- `moon-icon`, `sun-icon` - Theme-Icons
- `jahresgewinn`, `familienstand`, `kirchensteuer` - Input-Felder
- `umsatz`, `bundesland`, `krankenversicherung` - Input-Felder
- `alter`, `krankenkasse`, `kinder`, `zusatzbeitrag` - Input-Felder
- `results` - Ergebnisbereich

### ⚠️ Definiert aber nicht direkt über getElementById verwendet
- `themeToggle` - Verwendet über onclick
- `calculateBtn` - Verwendet über onclick

## 🌐 Verwendete Browser-APIs

| API | Zweck |
|-----|-------|
| `document.getElementById()` | Element-Zugriff |
| `document.documentElement` | HTML-Root für Theme |
| `window.matchMedia()` | Dark-Mode-Präferenz erkennen |
| `classList` | CSS-Klassen manipulieren |
| `innerHTML` | Dynamische Inhalte |
| `scrollIntoView()` | Zu Ergebnissen scrollen |
| `Intl.NumberFormat()` | Währungsformatierung |

## 🎨 CSS-Struktur

### Custom CSS Properties (Variablen)
- `--primary-color`, `--primary-hover` - Primärfarben
- `--secondary-color`, `--danger-color`, `--warning-color` - Weitere Farben
- `--bg-primary`, `--bg-secondary`, `--bg-card` - Hintergrundfarben
- `--text-primary`, `--text-secondary` - Textfarben
- `--border-color`, `--shadow` - Layout-Eigenschaften

### CSS-Klassen
- **Custom Classes**: 30 definierte Klassen (alle verwendet)
- **Tailwind Classes**: 8 Utility-Klassen verwendet
- **Dark Mode**: Implementiert über `.dark` Klasse

## 📊 Wichtige Erkenntnisse

### ✅ Positiv
- **Kein toter Code**: Alle JavaScript-Funktionen werden verwendet
- **Effiziente Struktur**: Alle HTML-IDs haben einen Zweck
- **Moderne APIs**: Gute Nutzung von Browser-Features
- **Responsive Design**: Grid-Layout mit Tailwind

### ⚠️ Optimierungsmöglichkeiten
- **Ungenutzte Dateien**: `style.css` und `tailwind.css` werden nicht eingebunden
- **Inline CSS**: Alles CSS steht im `<style>`-Tag (22KB)
- **CDN-Abhängigkeit**: Tailwind wird extern geladen

### 🔧 Empfehlungen
1. **Entferne ungenutzte Dateien** (`style.css`, `tailwind.css`)
2. **CSS externalisieren** für bessere Wartbarkeit
3. **Tailwind lokal einbinden** für bessere Performance
4. **Minimierung**: CSS und JS komprimieren für Produktion

## 📈 Statistiken

| Metrik | Wert |
|--------|------|
| Gesamtdateigröße | ~26KB |
| JavaScript-Funktionen | 7 (alle verwendet) |
| HTML-Element-IDs | 15 (alle sinnvoll) |
| CSS-Klassen definiert | 30 (alle verwendet) |
| Externe Dependencies | 1 (Tailwind CSS) |
| Browser-APIs verwendet | 7 |

---

**Fazit**: Dein Code ist sehr sauber und effizient! Es gibt praktisch keinen ungenutzten Code. Die einzigen "ungenutzten" Dateien sind die separaten CSS-Dateien, die gar nicht eingebunden sind.