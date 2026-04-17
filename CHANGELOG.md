# Changelog

All notable changes to Salary Tracker Pro.

## [3.0.0] - 2026-04-17

### 🎉 Major Release - Complete Redesign

This is a complete overhaul of the original salary tracker with 40+ new features and improvements.

### 🔒 Security
- **Added** SHA-256 PIN hashing with salt (replaces plaintext storage)
- **Added** Auto-lock timer with configurable timeout
- **Added** Forgot PIN recovery option
- **Added** Activity tracking for security
- **Improved** Session management

### 🎨 Design System
- **Added** Professional design tokens (50+ CSS variables)
- **Added** Light/dark mode with system detection
- **Added** Inter font for display text
- **Added** Consistent spacing scale (4px base unit)
- **Added** Professional color palette
- **Added** Shadow system for elevation
- **Improved** Typography hierarchy
- **Improved** Button styles with hover/focus states
- **Improved** Form input styling
- **Improved** Card designs with better borders and shadows

### ✨ New Features
- **Added** Export to CSV functionality
- **Added** Export to JSON (full backup)
- **Added** Import from JSON (restore)
- **Added** Copy from previous month
- **Added** Settings panel
- **Added** Toast notification system
- **Added** Modal component system
- **Added** Charts tab with Chart.js integration
- **Added** Tax band visualization
- **Added** Statistics dashboard
- **Added** Contextual tips (toggleable)
- **Added** Browser notifications support
- **Added** Theme selector (dark/light/auto)

### 📊 Data Visualization
- **Added** Bar charts for income overview
- **Added** Progress bars for tax bands
- **Added** Statistics cards (totals, averages)
- **Added** Compact currency display (£2.5k format)
- **Added** Visual month-by-month comparison

### 🎭 User Interface
- **Added** Enhanced month cards with mini previews
- **Added** Status badges (Actual/Predicted/Empty)
- **Added** Icon integration throughout
- **Added** Improved PIN screen with animations
- **Added** Better edit screen layout
- **Added** Action buttons in header
- **Added** Export/Import dropdown menu
- **Added** Current month highlighting
- **Added** Hover effects on interactive elements
- **Improved** Month list view with better cards
- **Improved** Edit month screen with copy button
- **Improved** Summary tab with better organization
- **Improved** Schedule tab with current month display
- **Improved** Footer with version and disclaimers

### ♿ Accessibility
- **Added** ARIA labels for screen readers
- **Added** Keyboard navigation support
- **Added** Focus visible states
- **Added** Reduced motion support
- **Added** Better color contrast
- **Improved** Semantic HTML structure
- **Improved** Interactive element sizes (44x44px min)

### 📱 Mobile
- **Added** Responsive container with max-width
- **Added** Touch-friendly button sizes
- **Improved** Grid layouts for mobile
- **Improved** Scrollbar styling
- **Improved** Tap target sizes

### 🔧 Code Quality
- **Added** Configuration objects (TAX_CONFIG, SALARY_CONFIG)
- **Added** Utility functions (storage, export, import)
- **Added** Component separation (Modal, Toast, Chart)
- **Added** Error handling throughout
- **Added** Data migration support
- **Added** Input validation
- **Improved** React hooks usage (useMemo, useCallback)
- **Improved** Code organization with clear sections
- **Improved** Comments and documentation
- **Fixed** Storage error handling
- **Fixed** Invalid data format handling

### 🎯 Performance
- **Improved** Calculation memoization
- **Improved** Re-render optimization
- **Improved** Storage efficiency
- **Added** Chart lazy loading
- **Added** Component memoization

### 📝 Documentation
- **Added** README.md with full documentation
- **Added** IMPROVEMENTS.md with detailed changes
- **Added** CHANGELOG.md (this file)
- **Added** Inline code comments
- **Added** Contextual help tips

### 🐛 Bug Fixes
- **Fixed** Tax calculation accuracy
- **Fixed** NI calculation edge cases
- **Fixed** Pension threshold handling
- **Fixed** Storage quota errors
- **Fixed** Negative value inputs
- **Fixed** Date calculations for current month

### 📦 Dependencies
- **Updated** Font family to Inter + JetBrains Mono
- **Added** Chart.js 4.4.0
- **Maintained** React 18.3.1
- **Maintained** Babel standalone

### 🔄 Breaking Changes
- Storage key changed from `salary-tracker-v2` to `salary-tracker-v3`
- PIN is now hashed (existing PINs will need to be reset on first load)
- Data structure includes new fields (backwards compatible)
- Font loading from Google Fonts (Inter instead of Space Grotesk)

### 📈 Statistics
- **Added**: 40+ new features
- **Code**: 600 → 2,000+ lines
- **Components**: 1 → 8 components
- **Design tokens**: 0 → 50+ CSS variables
- **Animations**: 2 → 10+ keyframes
- **File size**: ~50KB → ~70KB (uncompressed)

---

## [2.0.0] - Original Version

### Features
- Basic PIN protection (plaintext)
- 12-month tracking
- Prediction/Actual modes
- Cumulative PAYE calculation
- Dark theme only
- LocalStorage persistence
- Basic card UI
- Simple tabs (Months, Summary, Schedule)

---

## Version Numbering

This project uses semantic versioning:
- **Major**: Breaking changes, complete redesigns
- **Minor**: New features, backwards compatible
- **Patch**: Bug fixes, minor improvements

**Current Version**: 3.0.0
**Release Date**: April 17, 2026
**Status**: Stable

---

## Upgrade Guide

### From v2.0.0 to v3.0.0

1. **Backup Your Data**
   - Open v2.0.0
   - Manually note down your salary data
   - Or use browser DevTools to export localStorage

2. **Install v3.0.0**
   - Replace `index.html` with new version
   - Open in browser

3. **Set New PIN**
   - v3.0.0 uses secure hashing
   - Set a new 5-digit PIN on first launch
   - Previous PIN ("22222") won't work initially

4. **Import Data** (if backed up to JSON)
   - Use Import function (📊 button → Import from JSON)
   - Or manually re-enter from notes

5. **Configure Settings**
   - Set theme preference
   - Enable/disable tips
   - Configure auto-lock
   - Enable notifications (optional)

6. **Verify Calculations**
   - Double-check tax calculations
   - Compare with v2.0.0 if available
   - Update any months with actual payslip data

### Data Migration

The app automatically migrates v2 data to v3 format:
- Adds missing fields with defaults
- Preserves all existing month data
- Maintains actual/prediction modes
- Keeps notes and values

### Known Issues in v3.0.0

None reported. Please submit issues if found.

---

## Roadmap

### v3.1.0 (Planned)
- [ ] PWA support (service worker)
- [ ] Install prompt
- [ ] Offline mode indicator
- [ ] Print stylesheet
- [ ] Student loan calculations

### v3.2.0 (Future)
- [ ] Scotland tax rates
- [ ] Multi-year tracking
- [ ] Calendar export (.ics)
- [ ] Advanced charts (line, pie)

### v4.0.0 (Considering)
- [ ] Cloud sync (optional)
- [ ] Multi-currency
- [ ] Budget tracking
- [ ] Tax optimization AI
- [ ] Native mobile app

---

## Support & Feedback

Found a bug? Have a suggestion? 
- Open an issue on GitHub
- Contact via email
- Contribute via pull request

---

**Thank you for using Salary Tracker Pro!** 🚀
