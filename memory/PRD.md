# Flamingo Feedback WBA App - PRD

## Original Problem Statement
Repair the Feedback Formular WBA App. Data was wiped and design was broken.

## Latest Updates (2026-01-28)
- ✅ Notizfeld pro Task
- ✅ Deaktivierte Sektionen: grau, nicht anklickbar, nicht berechnet
- ✅ Responsive: Große Sterne auf Handy (44px), 2-spaltig auf Widescreen
- ✅ Professioneller PDF Export mit page-break-avoid
- ✅ Splash-Sequenz: FFF Logo (2500ms) → Taktikboard (2000ms) → Hero

## User Personas
- **Shop-Mitarbeiter**: Selbstbewertung während Kundengesprächen
- **Team-Leads/Coaches**: Mitarbeiter-Performance bewerten
- **Training-Manager**: Reports exportieren

## Core Requirements (Implemented)
1. ✅ 8 Sektionen mit 73+ Tasks
2. ✅ Sektionen deaktivierbar (grau, nicht anklickbar, nicht berechnet)
3. ✅ Splash Screen Sequenz (FFF Logo 2500ms → Taktikboard 2000ms → Hero)
4. ✅ PDF Export 2 Optionen (Ausgefüllt + Blanko)
5. ✅ Design: Schwarz/Magenta/Weiß
6. ✅ Notizfeld pro Task
7. ✅ Responsive: Mobile große Sterne, Widescreen 2-spaltig
8. ✅ TXT Export mit Notizen
9. ✅ Reset-Funktion
10. ✅ Warnung für Entwicklungsfelder (<70%)
11. ✅ Service Worker für Offline

## Architecture
- **Frontend**: Standalone HTML/CSS/JavaScript
- **Storage**: localStorage (state, sections, notes)
- **PWA**: manifest.json, sw.js
- **Responsive**: Mobile-first, 2-column breakpoint at 1200px

## Test Results
- Frontend: 95% (1 Playwright-Limitation, keine echte Bugs)
- All features working correctly

## Files
- `/app/index.html` - Hauptanwendung
- `/app/splash.png` - FFF Logo
- `/app/taktikboard.jpg` - Hero/Splash Bild
- `/app/manifest.json` - PWA Manifest
- `/app/sw.js` - Service Worker

## Backlog
### P1 (High)
- [ ] Historische Bewertungen speichern
- [ ] Datums-Tracking für Sessions

### P2 (Medium)
- [ ] Vergleichs-Reports
- [ ] Excel Export

### P3 (Future)
- [ ] Team-Dashboard
- [ ] Cloud-Sync
