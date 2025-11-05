# Contributing to Pashie

Bedankt voor je interesse om bij te dragen aan Pashie! 🎉

## 🐛 Bug Reports

Als je een bug vindt:
1. Check eerst of de bug al gerapporteerd is in de [Issues](https://github.com/[jouw-username]/pashie/issues)
2. Als het een nieuwe bug is, open een issue met:
   - Een duidelijke titel
   - Beschrijving van de bug
   - Stappen om de bug te reproduceren
   - Verwacht gedrag vs. actueel gedrag
   - Screenshots indien relevant
   - Je browser en OS informatie

## 💡 Feature Requests

Heb je een idee voor een nieuwe feature?
1. Check eerst of het al voorgesteld is in de [Issues](https://github.com/[jouw-username]/pashie/issues)
2. Open een issue met het "feature request" label en beschrijf:
   - Wat wil je kunnen doen?
   - Waarom zou dit nuttig zijn?
   - Hoe zou het kunnen werken?

## 🔧 Pull Requests

### Voordat je begint
1. Fork de repository
2. Clone je fork lokaal
3. Maak een nieuwe branch voor je feature/fix:
   ```bash
   git checkout -b feature/jouw-feature-naam
   ```

### Development Workflow
1. Maak je wijzigingen
2. Test lokaal of alles werkt
3. Commit met duidelijke messages:
   ```bash
   git commit -m "feat: voeg zoekfunctie toe voor pasjes"
   ```
4. Push naar je fork:
   ```bash
   git push origin feature/jouw-feature-naam
   ```
5. Open een Pull Request

### Commit Message Guidelines
Gebruik het volgende formaat:
- `feat:` voor nieuwe features
- `fix:` voor bug fixes
- `docs:` voor documentatie wijzigingen
- `style:` voor code formatting (geen functionaliteit wijziging)
- `refactor:` voor code refactoring
- `test:` voor test toevoegingen
- `chore:` voor maintenance taken

Voorbeelden:
```
feat: voeg dark mode toggle toe
fix: herstel barcode scanner op iOS
docs: update README met nieuwe screenshots
style: format code volgens style guide
```

### Code Style
- Gebruik **functionele React componenten** met hooks
- Gebruik **Tailwind CSS** classes voor styling
- Houd code leesbaar met duidelijke variabele namen
- Voeg comments toe bij complexe logica
- Gebruik Nederlandse teksten in de UI
- Gebruik Engelse namen voor code/variabelen

### Testing
Test je wijzigingen op:
- ✅ Chrome/Edge (Desktop)
- ✅ Safari (iOS - indien mogelijk)
- ✅ Chrome (Android - indien mogelijk)
- ✅ Firefox (Desktop)

## 📋 Development Setup

```bash
# Clone je fork
git clone https://github.com/[jouw-username]/pashie.git
cd pashie

# Start een lokale server
python3 -m http.server 8000
# Of:
npx serve

# Open http://localhost:8000 in je browser
```

## 🎨 Design Guidelines

- Volg het bestaande kleurenschema (zie PASHIE_SPEC.md)
- Houd de interface simpel en intuïtief
- Zorg dat touch targets minimaal 44x44px zijn
- Test op verschillende schermgroottes
- Behoud de "mobile-first" aanpak

## 📄 Documentation

Bij het toevoegen van features:
- Update de README.md indien relevant
- Update PASHIE_SPEC.md voor grote wijzigingen
- Voeg code comments toe voor complexe logica
- Update de Help tab in de app indien nodig

## 🤝 Code Review Process

1. Je Pull Request wordt gereviewd door de maintainers
2. Er kunnen vragen of suggesties voor wijzigingen komen
3. Maak de gevraagde wijzigingen
4. Na goedkeuring wordt je PR gemerged!

## ❓ Vragen?

Heb je vragen over het contributing proces?
- Open een [Discussion](https://github.com/[jouw-username]/pashie/discussions)
- Of plaats een comment in een bestaande Issue

## 🎉 Erkenning

Alle contributors worden vermeld in de README! Bedankt voor je bijdrage! 🙏

## 📜 License

Door bij te dragen aan Pashie, ga je akkoord dat je bijdragen gelicenseerd worden onder de MIT License.
