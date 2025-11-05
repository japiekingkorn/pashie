# 🚀 GitHub Setup Guide voor Pashie

## Stap 1: Repository Aanmaken

1. Ga naar [GitHub](https://github.com)
2. Klik op de **+** knop rechtsboven
3. Selecteer **New repository**
4. Vul in:
   - **Repository name:** `pashie`
   - **Description:** `🎴 Digital Membership Card Wallet - Bewaar al je pasjes in één handige app`
   - **Public** of **Private** (naar keuze)
   - **NIET** aanvinken: "Add a README file" (we hebben al een README)
   - **NIET** aanvinken: "Add .gitignore" (we hebben al een .gitignore)
   - **NIET** aanvinken: "Choose a license" (we hebben al een LICENSE)
5. Klik op **Create repository**

## Stap 2: Logo's Toevoegen

1. Zorg dat je alle logo formaten hebt gegenereerd:
   - icon-72.png
   - icon-96.png
   - icon-128.png
   - icon-144.png
   - icon-152.png
   - icon-192.png
   - icon-384.png
   - icon-512.png
   - icon-1024.png

2. Plaats deze bestanden in de `icons/` folder van je project

## Stap 3: Code Uploaden naar GitHub (SUPER SIMPEL!)

**Geen terminal nodig! Gewoon slepen en neerzetten! 🎉**

1. **Download de ZIP** met alle Pashie bestanden
2. **Unzip** de bestanden op je computer (dubbelklik op de ZIP)
3. **Voeg je logo's toe** aan de `icons/` folder (alle PNG bestanden)
4. Ga naar je **nieuwe repository op GitHub** (die je net in stap 1 hebt gemaakt)
5. Klik op **"uploading an existing file"** (staat in de blauwe tekst)
6. **Sleep** ALLE bestanden uit de pashie folder naar het GitHub venster
   - Of klik op "choose your files" en selecteer alles
7. Scroll naar beneden
8. Typ bij "Commit changes": `Initial commit - Pashie v1.0.0`
9. Klik op de groene knop **"Commit changes"**
10. **Klaar!** 🎉 Al je bestanden staan nu op GitHub!

**Let op:** Zorg dat je ook de `icons` folder met alle logo's uploadt!

## Stap 4: GitHub Pages Activeren

1. Ga naar je repository op GitHub
2. Klik op **Settings** (tandwiel icoon)
3. Scroll naar beneden naar **Pages** in het linker menu
4. Bij **Source** selecteer: **Deploy from a branch**
5. Bij **Branch** selecteer: **main** en **/ (root)**
6. Klik op **Save**
7. Wacht een paar minuten
8. Je app is nu live op: `https://[jouw-username].github.io/pashie/`

## Stap 5: Repository Instellingen Optimaliseren

### About Sectie Updaten
1. Ga naar je repository homepage
2. Klik op het tandwiel icoon bij "About" rechtsboven
3. Vul in:
   - **Description:** `🎴 Digital Membership Card Wallet`
   - **Website:** `https://[jouw-username].github.io/pashie/`
   - **Topics:** `pwa`, `membership-cards`, `javascript`, `react`, `tailwindcss`, `offline-first`, `dutch`
4. Klik op **Save changes**

### Topics/Tags Toevoegen
Klik op het tandwiel bij About en voeg deze topics toe:
- `pwa`
- `progressive-web-app`
- `membership-cards`
- `loyalty-cards`
- `barcode-scanner`
- `offline-first`
- `javascript`
- `react`
- `tailwindcss`
- `dutch`
- `mobile-app`

## Stap 6: README Badges Toevoegen (Optioneel)

Voeg deze badges toe aan je README.md:

```markdown
![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.0.0-green.svg)
![PWA](https://img.shields.io/badge/PWA-enabled-purple.svg)
```

## Stap 7: Testen

1. Bezoek je GitHub Pages URL: `https://[jouw-username].github.io/pashie/`
2. Test of de app correct laadt
3. Test de camera scanner (geef permissie)
4. Probeer een pasje toe te voegen
5. Test of de app installeerbaar is (Toevoegen aan startscherm)

## 🎉 Klaar!

Je Pashie app is nu live en klaar voor gebruik!

## 📱 Installatie Instructies voor Gebruikers

### iOS (iPhone/iPad)
1. Open de app in Safari
2. Tik op het "Delen" icoon (vierkant met pijltje omhoog)
3. Scroll naar beneden en tik op "Zet op beginscherm"
4. Tik op "Voeg toe"

### Android
1. Open de app in Chrome
2. Tik op de drie puntjes (⋮) rechtsboven
3. Selecteer "App installeren" of "Toevoegen aan startscherm"
4. Tik op "Installeren"

## 🔄 Updates Maken (Later)

Als je later iets wilt wijzigen:

**Makkelijke manier (via GitHub website):**
1. Ga naar je repository op GitHub
2. Klik op het bestand dat je wilt wijzigen (bijv. `index.html`)
3. Klik op het potlood icoon ✏️ (rechtsboven)
4. Maak je wijzigingen
5. Scroll naar beneden
6. Typ een beschrijving van je wijziging
7. Klik op **"Commit changes"**
8. Na een paar minuten is de wijziging live!

**Of upload nieuwe bestanden:**
1. Ga naar je repository
2. Klik op **"Add file"** → **"Upload files"**
3. Sleep je nieuwe/gewijzigde bestanden naar het venster
4. Klik op **"Commit changes"**

## 🐛 Troubleshooting

### App laadt niet
- Check of alle bestanden correct zijn geüpload
- Controleer of GitHub Pages correct is ingesteld
- Wacht 5-10 minuten na eerste deploy

### Logo's worden niet getoond
- Controleer of de icons folder bestaat
- Check of alle logo bestanden de juiste namen hebben
- Controleer de bestandsextensies (.png)

### Camera werkt niet
- GitHub Pages gebruikt HTTPS (✅ veilig)
- Localhost werkt ook (✅)
- Geef browser permissie voor camera
- Test eerst op een ander device

## 📞 Hulp Nodig?

- Check de [Issues](https://github.com/[jouw-username]/pashie/issues) op GitHub
- Open een nieuwe Issue als je problemen hebt
- Lees de volledige documentatie in PASHIE_SPEC.md

---

**Veel succes met Pashie! 🎴**
