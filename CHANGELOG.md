# Changelog

All notable changes to MooTracker will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [Unreleased]

### Added
- Planned: Multi-farm management support
- Planned: Push notification alerts via PWA service worker
- Planned: Offline-first mode with IndexedDB caching
- Planned: ESP32 OTA (over-the-air) firmware update support

---

## [1.2.0] - 2026-09-22

### Added
- Mobile Android APK (`MooTracker.apk`) release for field use
- `mobile.html` companion page with Figma mobile design integration
- `mobile-app/` directory with native-style mobile UI components
- In-page interactive Mobile App Simulator modal in the Command Center
- Figma Integration Bar with direct button link to Figma Make URL

### Changed
- Signal Orbit illustration updated with additional telemetry path animations
- Farm context signal now weighted more heavily in mastitis risk scoring
- Bilingual toggle (EN/हिं) now persists across page navigations via `localStorage`

### Fixed
- Temperature sensor spike false-positives in the `ml_engine.js` risk calculator
- Herd animal list pagination breaking on datasets larger than 50 entries
- IST clock display misalignment on Safari mobile browsers

---

## [1.1.0] - 2026-09-10

### Added
- Live Prototype Command Center (`#dashboard`) with real-time data
- Farm Console Sidebar with Overview, Active Alerts counter, Signal health
- Summary Stats Cards (Animals tracked, Needs attention, Watch, Last sync)
- Herd Animals List with search and risk-level filter dropdown
- Interactive Detail Panel with dynamic risk score gauge (0-100)
- Alerts Stream with one-click "Acknowledge" action
- PWA manifest (`manifest.json`) and service worker (`sw.js`) for installability
- Progressive Web App icons: `icon-192.png`, `icon-512.png`, `icon.svg`

### Changed
- Migrated backend data layer to Supabase real-time database
- `app.js` refactored for cleaner signal pipeline separation
- `data.js` now serves as the canonical dataset adapter layer

### Fixed
- Supabase connection dropping after 30 minutes of inactivity
- Risk gauge not updating on animal selection in Detail Panel
- `robots.txt` missing, now added for proper crawler control

---

## [1.0.0] - 2026-09-01

### Added
- Initial public release of MooTracker Landing Page & Command Center
- Hero section with Signal Orbit illustration and CTA group
- "The Signal Field" 4-column signal strip (Milk, Movement, Temperature, Context)
- "From Noise to Action" 3-step timeline story band
- "Built for the Field" principles section
- Sticky navigation with anchor links
- Bilingual EN/हिं toggle (initial implementation)
- ESP32 Arduino firmware (`MooTracker_ESP32.ino`) for IoT sensor integration
- Python ML engine stub (`ml_engine.js` predecessor) for cattle health inference
- `requirements.txt` for Python ML dependencies
- `server.js` local Node.js server for development

---

## Version History Summary

| Version | Date | Highlights |
|---------|------|-----------|
| 1.2.0 | 2026-09-22 | Mobile APK, Figma integration, offline prep |
| 1.1.0 | 2026-09-10 | Full Command Center, Supabase, PWA support |
| 1.0.0 | 2026-09-01 | Initial landing page & ESP32 firmware |

---

[Unreleased]: https://github.com/embeddedriders/MooTracker/compare/v1.2.0...HEAD
[1.2.0]: https://github.com/embeddedriders/MooTracker/compare/v1.1.0...v1.2.0
[1.1.0]: https://github.com/embeddedriders/MooTracker/compare/v1.0.0...v1.1.0
[1.0.0]: https://github.com/embeddedriders/MooTracker/releases/tag/v1.0.0