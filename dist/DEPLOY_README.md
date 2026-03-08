# 🚀 Deployment-Anleitung - Vox Draconis Crafting Manager

## 📁 Was ist im dist-Ordner?

```
dist/
├── index.html          ← Hauptdatei (Crafting Manager)
├── assets/
│   └── bg-blacksmith.jpg  ← Hintergrundbild
└── DEPLOY_README.md    ← Diese Datei
```

## 🔥 Schritt 1: Netlify Upload

### Option A: Drag & Drop (Einfachste)

1. Öffne https://app.netlify.com/drop
2. Ziehe den **dist-Ordner** auf die Seite
3. Warten...
4. Fertig! 🎉

### Option B: Über Projekt-Seite

1. Gehe zu https://app.netlify.com/
2. Wähle dein Projekt: `creative-panda-4b65fc`
3. Klicke auf "Deploys"
4. "Deploy manually" → "Upload folder"
5. Wähle den **dist-Ordner**
6. Warten...
7. Fertig!

## 🌐 Schritt 2: URL überprüfen

Nach dem Upload bekommst du eine URL wie:
```
https://creative-panda-4b65fc.netlify.app/
```

**Wichtig**: Die Crafting-Seite ist dann erreichbar unter:
```
https://creative-panda-4b65fc.netlify.app/crafting/
```

## ⚙️ Schritt 3: Firebase prüfen

Die Firebase-Verbindung sollte automatisch funktionieren, da:
- Die Konfiguration ist in `index.html` eingebaut
- Firebase arbeitet mit allen Domains

**Test:**
1. Öffne die URL im Browser
2. Trage einen Test-Namen ein
3. Öffne die Seite in einem anderen Browser/Fenster
4. Die Daten sollten synchronisiert sein!

## 🎨 Optional: Eigene Domain

Falls du eine eigene Domain hast:

1. Netlify → Domain settings
2. "Add custom domain"
3. DNS-Einstellungen anpassen

## 🆘 Fehlerbehebung

### Seite ist leer/weiß?
→ Browser-Cache leeren (Strg+F5)

### Bild wird nicht angezeigt?
→ Prüfe ob `assets/bg-blacksmith.jpg` existiert

### Firebase funktioniert nicht?
→ Browser-Konsole öffnen (F12) → Nach roten Fehlermeldungen suchen

### 404 Fehler?
→ Stelle sicher, dass du den **dist-Ordner** hochlädst, nicht den übergeordneten crafting-Ordner

## ✅ Checkliste vor dem Upload

- [ ] index.html ist vorhanden
- [ ] assets/bg-blacksmith.jpg ist vorhanden
- [ ] Firebase-Konfiguration ist eingetragen (API-Key, etc.)
- [ ] Alte Version wurde gelöscht (falls vorhanden)

## 📞 Support

Bei Problemen:
1. Browser-Konsole prüfen (F12)
2. Netlify-Logs prüfen
3. Firebase-Console prüfen

---

**Viel Erfolg!** 🎉

Vox Draconis - Midnight Crafting Manager
