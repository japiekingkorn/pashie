# 🎴 Pashie - Digital Membership Card Wallet

> Stop je dikke portemonnee vol pasjes - bewaar al je membership cards digitaal in één handige app!

![Pashie Logo](icons/icon-512.png)

## 📱 Wat is Pashie?

Pashie is een Progressive Web App (PWA) waarmee je al je membership cards, klantenkaarten, spaarpasjes en loyalty cards digitaal kunt bewaren. Geen gedoe meer met zoeken naar het juiste pasje - scan je kaarten en heb ze altijd bij de hand op je telefoon!

### ✨ Features

- 📷 **Barcode Scanner** - Scan eenvoudig je membership cards
- 💳 **Digitale Wallet** - Bewaar onbeperkt pasjes
- 🔍 **Zoekfunctie** - Vind snel het juiste pasje
- 📊 **Sorteeropties** - Alfabetisch, nieuwste eerst, of meest gebruikt
- 🎨 **Preset Logo's** - 25+ Nederlandse winkels vooraf geladen
- 💾 **Export/Import** - Maak backup van je data
- 🔒 **Privacy First** - Alles lokaal opgeslagen, geen cloud
- 📴 **Offline** - Werkt zonder internet verbinding
- 🌓 **Modern Design** - Gebaseerd op het mooie Pashie logo kleurenschema

## 🚀 Installatie

### Optie 1: Direct Gebruiken (Online)
Bezoek gewoon [jouw-github-pages-url] en gebruik de app direct in je browser!

### Optie 2: Installeren als App
1. Open de app in je mobiele browser
2. Tik op het "Delen" icoon (iOS) of menu (Android)
3. Selecteer "Toevoegen aan beginscherm"
4. De app verschijnt als een normale app op je telefoon!

### Optie 3: Lokaal Draaien
```bash
# Clone de repository
git clone https://github.com/[jouw-username]/pashie.git

# Ga naar de directory
cd pashie

# Open index.html in je browser
# Of gebruik een lokale server:
python3 -m http.server 8000
# Of met Node.js:
npx serve
```

## 📖 Hoe Gebruik Je Pashie?

### Een Pasje Toevoegen
1. Open de **Scan** tab
2. Tik op "Start Scannen"
3. Geef camera permissie
4. Scan de barcode van je membership card
5. Voer de winkelnaam in
6. Kies eventueel een preset logo
7. Tik op "Opslaan"

### Een Pasje Gebruiken
1. Open de **Cards** tab
2. Zie al je pasjes als knoppen met logo's
3. Tik op het gewenste pasje
4. De barcode wordt fullscreen getoond
5. Laat de kassamedewerker scannen!

### Pasjes Beheren
1. Ga naar de **Settings** tab
2. Bekijk al je opgeslagen pasjes
3. Verwijder pasjes die je niet meer nodig hebt
4. Exporteer je data als backup
5. Importeer een backup als je van telefoon wisselt

## 🛠️ Technische Details

### Tech Stack
- **HTML5** - Basis structuur
- **React 18** - UI componenten via CDN
- **Tailwind CSS** - Styling & responsive design
- **html5-qrcode** - Barcode/QR scanning
- **JsBarcode** - Barcode display generatie
- **localStorage** - Lokale data opslag

### Ondersteunde Barcode Types
- EAN-13 (meest voorkomend in NL)
- EAN-8
- Code 128
- Code 39
- QR Codes

### Browser Compatibiliteit
- ✅ Chrome/Edge (Android & Desktop)
- ✅ Safari (iOS & macOS)
- ✅ Firefox (Android & Desktop)
- ⚠️ Camera functionaliteit vereist HTTPS of localhost

## 🎨 Kleurenschema

Gebaseerd op het Pashie logo:
- **Primary Coral:** `#FF6B5A` - Hoofdkleur, CTA buttons
- **Secondary Gold:** `#FFB84D` - Accent, highlights
- **Tertiary Turquoise:** `#4ECDC4` - Success states
- **Background Teal:** `#1A7B7B` - Splash screen, headers

## 📁 Project Structuur

```
pashie/
├── index.html              # Hoofdapplicatie
├── manifest.json           # PWA manifest
├── service-worker.js       # Offline functionaliteit
├── icons/                  # App iconen (alle formaten)
│   ├── icon-72.png
│   ├── icon-96.png
│   ├── icon-128.png
│   ├── icon-144.png
│   ├── icon-152.png
│   ├── icon-192.png
│   ├── icon-384.png
│   └── icon-512.png
├── README.md               # Deze file
├── LICENSE                 # MIT License
└── PASHIE_SPEC.md         # Volledige specificatie document
```

## 🔒 Privacy & Security

- **100% Lokaal** - Alle data blijft op je telefoon
- **Geen Account** - Geen email of wachtwoord nodig
- **Geen Tracking** - Geen analytics of tracking
- **Geen Permissies** - Alleen camera voor scannen
- **Open Source** - Code is volledig inzichtelijk

## 🚦 Roadmap

### ✅ v1.0.0 (Current - MVP)
- Barcode scanner
- Pasjes opslaan en tonen
- Zoeken en sorteren
- Export/Import functionaliteit
- PWA met offline support

### 🔮 v1.1.0 (Planned)
- Favorites/Pinned cards
- Categorieën voor pasjes
- Notities per pasje
- Dark mode
- Verbeterde zoekfunctie

### 🌟 v1.2.0 (Future)
- Saldo tracking
- Vervaldatum notificaties
- Store locator op kaart
- Usage statistics
- Widget support

## 🤝 Contributing

Contributions zijn welkom! Voel je vrij om:
- 🐛 Bugs te rapporteren
- 💡 Features voor te stellen
- 🔧 Pull requests in te dienen

Zie [PASHIE_SPEC.md](PASHIE_SPEC.md) voor de volledige specificatie.

## 📄 License

Dit project is gelicenseerd onder de MIT License - zie het [LICENSE](LICENSE) bestand voor details.

## 👨‍💻 Ontwikkelaar

Gemaakt met 💳 en ☕

## 🙏 Dankwoord

- [html5-qrcode](https://github.com/mebjas/html5-qrcode) voor de geweldige barcode scanner
- [JsBarcode](https://github.com/lindell/JsBarcode) voor barcode generatie
- [Tailwind CSS](https://tailwindcss.com) voor het styling framework
- [React](https://react.dev) voor de UI componenten

## 📞 Support

Heb je vragen of loop je tegen problemen aan?
- 📖 Lees de **Help** tab in de app
- 🐛 Open een [GitHub Issue](https://github.com/[jouw-username]/pashie/issues)
- 💬 Stuur feedback via de app

---

**Gemaakt met ❤️ voor iedereen die geen dikke portemonnee meer wil!**

*Geniet van je digitale membership cards!* 🎉
