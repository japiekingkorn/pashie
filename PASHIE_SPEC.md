# Pashie - Digital Membership Card Wallet

## 📋 Projectoverzicht

**Naam:** Pashie  
**Type:** Progressive Web App (PWA)  
**Platform:** HTML/CSS/JavaScript (React + Tailwind)  
**Doel:** Digitale wallet voor membership cards die je bij winkels krijgt  
**Target devices:** Alle smartphones (iOS & Android)  
**Offline:** Ja, volledige offline functionaliteit  

## 🎯 Wat is Pashie?

Pashie is een digitale wallet app waarmee je al je membership cards (klantenkaarten, spaarpasjes, loyalty cards) van verschillende winkels op één plek kunt bewaren. Door het scannen van de barcode wordt de kaart toegevoegd aan de app, zodat je niet meer al die fysieke pasjes bij je hoeft te hebben.

### Waarom Pashie?

- 💳 **Geen dikke portemonnee meer** - Alle pasjes in één app
- 📱 **Altijd bij de hand** - Je telefoon heb je altijd bij je
- 🔍 **Geen zoeken meer** - Direct het juiste pasje vinden
- 🌍 **Werkt overal** - Op elk merk en type telefoon
- 🔒 **Privacy eerst** - Alles lokaal opgeslagen, geen cloud

## 🎨 Hoe werkt Pashie?

### Gebruikersflow

1. **Pasje toevoegen**
   - Open de Scan tab
   - Scan de barcode van je membership card
   - Geef de winkelnaam op
   - Kies of upload een logo
   - Pasje wordt opgeslagen

2. **Pasje gebruiken**
   - Open de Cards tab
   - Zie al je pasjes als knoppen met logo's
   - Tik op een pasje
   - Barcode wordt fullscreen getoond
   - Laat de kassa scannen

3. **Pasje beheren**
   - Ga naar Settings
   - Bekijk lijst van alle pasjes
   - Bewerk of verwijder pasjes

## ⚡ Minimale Functionaliteit (MVP)

### 1. Barcode Scanner
- Camera toegang voor scannen
- Ondersteuning voor meest voorkomende barcode types:
  - EAN-13 (meest gebruikt in Nederland)
  - EAN-8
  - Code 128
  - Code 39
  - QR Code
- Scan result validatie
- Feedback bij succesvolle scan

### 2. Pasje Toevoegen
- Scan barcode via camera
- **OF** handmatig invoeren van barcode nummer
- Winkelnaam invoeren
- Logo selectie:
  - Keuze uit vooraf geladen logos (~25 populaire NL winkels)
  - **OF** eigen logo uploaden via camera/galerij
  - **OF** standaard icoon met eerste letter winkelnaam

### 3. Pasjes Overzicht (Cards Tab)
- Grid layout met kaart-knoppen
- Elk pasje toont:
  - Winkel logo (prominent)
  - Winkelnaam (onder logo)
- Klik op pasje → barcode weergave
- Zoekfunctie om snel pasje te vinden
- Sorteer opties (alfabetisch, recent toegevoegd, meest gebruikt)

### 4. Barcode Weergave
- Fullscreen barcode display
- Automatische helderheid verhogen
- Barcode groot en scanbaar
- Winkelnaam + logo bovenaan
- Barcode nummer onderaan (voor handmatige invoer als scan faalt)
- Terug knop

### 5. Pasje Beheer (Settings Tab)
- Lijst van alle pasjes
- Per pasje:
  - Bewerken (naam, logo wijzigen)
  - Verwijderen (met confirmatie)
- Exporteer/Importeer functionaliteit (backup)

### 6. Help & Info
- Uitleg hoe de app werkt
- FAQ
- Tips voor beste scan resultaten
- Privacy informatie
- Versie informatie
- Feedback mogelijkheid

### 7. Technische Basis Requirements
- PWA functionaliteit (installeerbaar)
- localStorage voor data opslag
- Werkt volledig offline
- Responsive design (mobiel-first)
- Splash screen bij opstarten
- Bottom navigatie (zoals CartPal)
- Dark mode support (optioneel voor MVP)

## 🏪 Vooraf Geladen Winkel Logo's (NL)

### Supermarkten
- Albert Heijn
- Jumbo
- Lidl
- Aldi
- Plus
- Dirk van den Broek
- Hoogvliet
- Coop

### Drogisterijen & Beauty
- Etos
- Kruidvat
- DA
- ICI Paris XL

### Fashion & Lifestyle
- H&M
- Zara
- C&A
- Primark
- WE Fashion

### Electronica & Media
- MediaMarkt
- Coolblue
- Bol.com

### Overig
- Action
- HEMA
- Blokker
- Praxis
- Gamma
- IKEA

*Totaal: ~25-30 logos vooraf geladen*

## 🔮 Toekomstige Uitbreidingen

### Fase 2 - Enhanced Features
- **Favorites/Pinned cards** - Meest gebruikte pasjes bovenaan
- **Categorieën** - Groepeer pasjes (Supermarkten, Fashion, etc.)
- **Notities per pasje** - Bijv. "Saldo: €10", "Vervalt 31-12-2025"
- **Barcode types filter** - Filter op type barcode in scanner
- **Bulk import** - Meerdere pasjes achter elkaar scannen
- **Widget support** - Snelle toegang tot favoriete pasjes

### Fase 3 - Smart Features
- **Saldo tracking** - Handmatig saldo bijhouden per pasje
- **Expiry dates** - Notificatie als pasje bijna verloopt
- **Store locator** - Dichtstbijzijnde winkel vinden op kaart
- **Usage statistics** - Welke pasjes gebruik je het meest
- **NFC support** - Als pasje NFC heeft, ook digitaal gebruiken
- **Auto-brightness** - Automatisch scherm helderder bij barcode tonen

### Fase 4 - Social & Sharing
- **Gezins-sharing** - Deel pasjes met gezinsleden
- **Deals & Promoties** - Acties van winkels tonen (opt-in)
- **Pasje delen** - Tijdelijk pasje delen met iemand anders
- **Backup naar cloud** - Optioneel voor wie dat wil (Google Drive/iCloud)

### Fase 5 - Advanced
- **OCR scanning** - Scan hele pasje, niet alleen barcode
- **Wallet integration** - Toevoegen aan Apple/Google Wallet
- **Wearable support** - Apple Watch / WearOS ondersteuning
- **Multi-language** - Engels, Duits, Frans ondersteuning
- **Pasje design customization** - Eigen kleuren/layout per pasje
- **Integration met winkel apps** - API koppelingen voor real-time saldo

## 🛠️ Technische Stack

### Frontend
- **HTML5** - Basis structuur
- **React (via CDN)** - UI componenten & state management
- **Tailwind CSS** - Styling & responsive design
- **Babel Standalone** - JSX transpiling in browser

### Libraries
- **html5-qrcode** - Barcode/QR code scanning
- **JsBarcode** - Barcode generatie voor display
- **LocalForage** (optioneel) - Enhanced localStorage met IndexedDB fallback

### PWA
- **manifest.json** - App metadata & icons
  - name: "Pashie"
  - short_name: "Pashie"
  - theme_color: "#1A7B7B" (teal)
  - background_color: "#1A7B7B"
  - icons: Array met alle formaten uit `/icons/`
- **Service Worker** - Offline functionaliteit & caching
- **Apple touch icons** - iOS home screen icons
  - apple-touch-icon: `/icons/icon-192.png`
  - apple-touch-startup-image: `/icons/icon-512.png` (splash)

### Storage
- **localStorage** - Primary data storage
- JSON format voor pasje data:
  ```json
  {
    "id": "uuid",
    "storeName": "Albert Heijn",
    "barcodeValue": "1234567890123",
    "barcodeFormat": "EAN13",
    "logoType": "preset", // of "custom"
    "logoData": "ah" // preset key of base64 voor custom
    "dateAdded": "2025-11-05T10:30:00Z",
    "lastUsed": "2025-11-05T14:20:00Z",
    "usageCount": 5
  }
  ```

## 📱 UI/UX Design Principes

### Navigatie
- Bottom navigation met 4 tabs:
  - 📷 **Scan** - Barcode scannen
  - 💳 **Cards** - Pasjes overzicht
  - ⚙️ **Settings** - Beheer & instellingen
  - ℹ️ **Help** - Info & support

### Logo & Branding
- **Logo:** Moderne cirkel met vloeiende vormen
- **Logo locatie:** `/icons/` directory in GitHub
- **Beschikbare formaten:**
  - 72x72px - `icon-72.png`
  - 96x96px - `icon-96.png`
  - 128x128px - `icon-128.png`
  - 144x144px - `icon-144.png`
  - 152x152px - `icon-152.png`
  - 192x192px - `icon-192.png`
  - 384x384px - `icon-384.png`
  - 512x512px - `icon-512.png`
  - 1024x1024px - `icon-1024.png`

### Kleurenschema
Gebaseerd op het Pashie logo:
- **Primary Coral:** `#FF6B5A` - Hoofdkleur, CTA buttons
- **Secondary Gold:** `#FFB84D` - Accent, highlights
- **Tertiary Turquoise:** `#4ECDC4` - Success states, active states
- **Background Teal:** `#1A7B7B` - Splash screen, headers
- **Neutral Gray:** `#6B7280` - Text, borders
- **Light Background:** `#F9FAFB` - Card backgrounds, main bg
- **White:** `#FFFFFF` - Cards, modals
- **Dark Text:** `#1F2937` - Primary text

**Dark Mode Palette:**
- **Background:** `#111827` - Main background
- **Surface:** `#1F2937` - Cards, elevated surfaces
- **Primary:** `#FF8A7A` - Lighter coral for dark mode
- **Secondary:** `#FFC870` - Lighter gold for dark mode
- **Tertiary:** `#6EDDD4` - Lighter turquoise for dark mode

### Interactie
- Touch-friendly (minimum 44x44px touch targets)
- Swipe gestures (bijv. swipe om pasje te verwijderen)
- Haptic feedback (vibratie bij scan success)
- Smooth transitions & animations
- Loading states & skeletons

### Toegankelijkheid
- High contrast mode support
- Screen reader friendly
- Keyboard navigation (voor web versie)
- Error messages duidelijk en behulpzaam

## 📊 Data Structuur

### Stored Data
```javascript
{
  "cards": [
    {
      "id": "uuid-string",
      "storeName": "string",
      "barcodeValue": "string",
      "barcodeFormat": "EAN13 | EAN8 | CODE128 | CODE39 | QRCODE",
      "logoType": "preset | custom | default",
      "logoData": "string", // preset key, base64, or color
      "dateAdded": "ISO date string",
      "lastUsed": "ISO date string",
      "usageCount": number,
      "notes": "string (optional)",
      "category": "string (optional - future)"
    }
  ],
  "settings": {
    "sortBy": "alphabetical | dateAdded | mostUsed",
    "darkMode": boolean,
    "hapticFeedback": boolean,
    "autoScan": boolean
  },
  "appVersion": "1.0.0"
}
```

## 🚀 Development Roadmap

### Sprint 1 - MVP Core (Week 1-2)
- [ ] Project setup & basic HTML structure
- [ ] Bottom navigation implementatie
- [ ] Scan tab met html5-qrcode integratie
- [ ] Basic localStorage setup
- [ ] Pasje toevoegen flow (zonder logo's)

### Sprint 2 - Cards Display (Week 2-3)
- [ ] Cards tab met grid layout
- [ ] Barcode display met JsBarcode
- [ ] Fullscreen barcode view
- [ ] Logo system (preset logos)
- [ ] Custom logo upload functionaliteit

### Sprint 3 - Management (Week 3-4)
- [ ] Settings tab implementatie
- [ ] Edit pasje functionaliteit
- [ ] Delete pasje met confirmatie
- [ ] Search & sort functionaliteit
- [ ] Export/Import backup

### Sprint 4 - Polish & PWA (Week 4-5)
- [ ] Help tab met documentatie
- [ ] Splash screen met Pashie logo (`/icons/icon-512.png`)
  - Teal achtergrond (#1A7B7B)
  - Gecentreerd logo
  - Fade-in animatie (0.5s)
  - Fade-out naar app (0.5s na 1.5s)
- [ ] PWA manifest & icons (alle formaten uit `/icons/`)
- [ ] Service worker voor offline
- [ ] Testing op verschillende devices
- [ ] Bug fixes & optimalisaties

### Sprint 5 - Launch Prep (Week 5-6)
- [ ] Final testing & QA
- [ ] Performance optimalisatie
- [ ] GitHub repository opzetten
- [ ] README.md met installatie instructies
- [ ] Deployment naar GitHub Pages
- [ ] Launch! 🎉

## 📝 Gebruik Cases

### Use Case 1: Nieuwe gebruiker
1. Installeert Pashie op telefoon
2. Opent app, ziet splash screen
3. Komt op Scan tab
4. Tikt "Scan Card" knop
5. Geeft camera permissie
6. Scant barcode van AH bonuskaart
7. App herkent barcode
8. Voert "Albert Heijn" in
9. Selecteert AH logo uit lijst
10. Pasje opgeslagen!
11. Gaat naar Cards tab, ziet pasje

### Use Case 2: Pasje gebruiken in winkel
1. Staat bij kassa
2. Opent Pashie
3. Cards tab is al open
4. Ziet Albert Heijn pasje
5. Tikt erop
6. Barcode verschijnt fullscreen
7. Kassamedewerker scant barcode
8. Klaar!

### Use Case 3: Pasje bewerken
1. Gaat naar Settings
2. Ziet lijst van pasjes
3. Tikt op "Edit" bij een pasje
4. Wijzigt winkelnaam of logo
5. Saved
6. Terug naar Cards tab
7. Wijziging is zichtbaar

## 🔒 Privacy & Security

### Data Opslag
- **Alles lokaal** - Geen data naar servers
- **Geen account vereist** - Geen email/wachtwoord
- **Geen tracking** - Geen analytics (optioneel later opt-in)
- **Geen permissies** - Alleen camera voor scannen

### Gebruiker Controle
- Volledige controle over eigen data
- Export functionaliteit voor backup
- Delete functionaliteit voor elk pasje
- Clear all data optie in settings

## 📖 Documentation Needs

### User Documentation
- **Quickstart guide** - Eerste pasje toevoegen
- **FAQ** - Veel gestelde vragen
- **Troubleshooting** - Scan problemen, barcode niet herkend
- **Tips & Tricks** - Best practices

### Developer Documentation
- **README.md** - Project overview, installatie, development
- **CONTRIBUTING.md** - Voor toekomstige contributors
- **Code comments** - Inline documentatie
- **API documentation** - Als we externe APIs gaan gebruiken

## 🎯 Success Metrics (voor later)

### Engagement Metrics
- Aantal pasjes per gebruiker (gemiddeld)
- Scan success rate (percentage)
- Daily active users
- Pasje gebruik frequency

### Technical Metrics
- App load time
- Scan to save time
- PWA install rate
- Crash/error rate

### User Satisfaction
- App store ratings (als gepubliceerd)
- User feedback submissions
- Feature requests
- Bug reports

## 🤝 Samenwerking

### GitHub Setup
- **Repository:** github.com/[username]/pashie
- **Branches:**
  - `main` - Stable production code
  - `develop` - Development branch
  - `feature/*` - Feature branches
- **Issues:** Voor bugs & feature requests
- **Projects:** Kanban board voor tracking

### Communication
- Nieuwe chat per feature/bug fix
- Gebruik dit MD bestand als referentie
- Update dit document bij wijzigingen

## 📅 Version History (Planned)

- **v1.0.0** - MVP Launch (Q1 2025)
  - Core functionaliteit
  - 25 preset logos
  - Basic PWA
  
- **v1.1.0** - Quality of Life (Q2 2025)
  - Search & sort improvements
  - Dark mode
  - Performance optimizations
  
- **v1.2.0** - Smart Features (Q2 2025)
  - Favorites
  - Categories
  - Usage statistics
  
- **v2.0.0** - Major Update (Q3 2025)
  - Cloud backup (optional)
  - Widget support
  - Advanced barcode types

---

## 🎨 Design References

Inspiratie apps voor UI/UX:
- CartPal (eigen app - bottom nav, clean design)
- Apple Wallet (card display)
- Google Pay (barcode display)
- Stocard (competitor analysis)

---

**Laatst bijgewerkt:** 5 november 2025  
**Status:** Specification fase  
**Volgende stap:** Development Sprint 1 starten
