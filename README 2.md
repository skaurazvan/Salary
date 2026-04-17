# 💰 Salary Tracker Pro

A professional, feature-rich salary and tax tracking application for UK employees with cumulative PAYE calculations.

![Version](https://img.shields.io/badge/version-3.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Size](https://img.shields.io/badge/size-~70KB-orange)

## ✨ Features

### 🔐 Security
- **SHA-256 PIN Protection** - Secure authentication with hashed PINs
- **Auto-lock Timer** - Configurable inactivity timeout
- **Session Management** - Secure session-based access
- **Forgot PIN Recovery** - Reset to default PIN if needed

### 📊 Salary Tracking
- **12-Month View** - Complete tax year tracking (April - March)
- **Dual Modes**:
  - **Prediction Mode** - Estimate pay based on OT, sick days, bonuses
  - **Actual Mode** - Enter real payslip values for accuracy
- **Cumulative PAYE** - Accurate UK tax calculations across months
- **Automatic Calculations** - Tax, NI, pension computed in real-time

### 📈 Visualization
- **Interactive Charts** - Bar charts showing gross, net, and tax
- **Tax Band Progress** - Visual indicators of basic/higher/additional rates
- **Statistics Dashboard** - Annual totals and averages
- **Month-by-Month Breakdown** - Detailed view of all periods

### 💾 Data Management
- **Auto-save** - Changes saved automatically to browser storage
- **Export to CSV** - Spreadsheet-compatible format
- **Export to JSON** - Full backup including settings
- **Import from JSON** - Restore from previous backup
- **Copy from Previous** - Quick-fill prediction data

### 🎨 User Experience
- **Dark/Light Modes** - Switch themes or use system preference
- **Responsive Design** - Works on mobile, tablet, and desktop
- **Smooth Animations** - Professional transitions and feedback
- **Interactive Elements** - Hover effects, focus states, tooltips
- **Contextual Tips** - Helpful hints (can be disabled)

### ⚙️ Customization
- **Theme Selection** - Dark, Light, or Auto (system)
- **Notifications** - Optional browser notifications for paydays
- **Auto-lock Settings** - 1, 5, 10, 30 minutes, or never
- **Show/Hide Tips** - Toggle helpful hints throughout app

## 🚀 Getting Started

### Installation
1. Download `index.html`
2. Open in a modern web browser
3. That's it! No installation or build process required

### First Time Setup
1. **Set PIN**: Create your 5-digit security PIN
2. **Confirm PIN**: Re-enter to confirm
3. **Start Tracking**: Begin entering your salary data

### Daily Usage
1. **Unlock**: Enter your PIN
2. **Edit Month**: Tap any month to enter OT, sick days, or bonuses
3. **View Summary**: Check YTD totals and tax status
4. **Review Charts**: Visualize your income over time
5. **Export**: Backup your data regularly

## 📱 Interface Overview

### Tabs
- **📅 Months** - View and edit all 12 months
- **📊 Summary** - Year-to-date totals and forecasts
- **📈 Charts** - Visual data representation
- **🗓️ Schedule** - Pay dates and OT cut-off periods

### Month Card
```
April (M1)                      £2,902.09
✓ ACTUAL    📅 Pay: 2nd Apr    Gross £3,757.20
⏰ 5h OT • 🤒 1d sick
```

### Action Buttons
- **📊** - Export/Import menu
- **⚙️** - Settings panel

## 💡 Tips & Tricks

### For Accuracy
1. ✅ Update months to "Actual" after receiving payslip
2. ✅ Enter exact values from payslip for tax calculations
3. ✅ Use predictions for future planning
4. ✅ Export data monthly as backup

### For Efficiency
1. 🚀 Use "Copy from previous" for similar months
2. 🚀 Set up notifications for payday reminders
3. 🚀 Enable auto-lock for security
4. 🚀 Use keyboard Tab to navigate between fields

### For Planning
1. 📈 Check tax band utilization to avoid surprises
2. 📈 Review over/underpayment status regularly
3. 📈 Use predictions to plan for extra OT or sick days
4. 📈 Compare actual vs predicted for accuracy

## 🔧 Configuration

### Tax Settings (2025-26)
```javascript
TAX_CONFIG = {
  year: "2025-26",
  personalAllowance: £12,630,
  basicRate: 20% (£12,630 - £50,270),
  higherRate: 40% (£50,270 - £125,140),
  additionalRate: 45% (above £125,140),
  NI: 8% / 2% (threshold £12,570 / £50,270)
}
```

### Salary Components
```javascript
SALARY_CONFIG = {
  monthlyBase: £3,055.36,
  hourlyRate: £16.79,
  shiftAllowance: £458.29/month,
  overtimeMultiplier: 1.33x,
  pensionRate: 4%
}
```

## 📖 FAQ

### Q: Is my data secure?
**A**: Yes! All data is stored locally in your browser. No cloud storage or external servers. PIN is hashed with SHA-256.

### Q: What if I forget my PIN?
**A**: Click "Forgot PIN?" on the lock screen to reset to default (22222), then change it immediately.

### Q: Can I use this on multiple devices?
**A**: Export to JSON and import on another device. Data is device-specific by default.

### Q: How accurate are tax calculations?
**A**: Very accurate for standard UK PAYE. Doesn't account for student loans, Scotland rates, or other special cases.

### Q: Can I customize for my company?
**A**: Yes! Edit `SALARY_CONFIG` and `TAX_CONFIG` in the HTML file to match your situation.

### Q: Does it work offline?
**A**: Yes! Once loaded, it works completely offline. Consider saving as PWA (future feature).

## 🛠️ Technical Details

### Technologies
- **React 18.3.1** - UI framework
- **Chart.js 4.4.0** - Data visualization
- **Vanilla CSS** - Styling with CSS variables
- **Web Crypto API** - PIN hashing
- **LocalStorage** - Data persistence

### Browser Support
- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+

### File Size
- **Uncompressed**: ~70KB
- **Gzipped**: ~20KB
- **Single file deployment**

## 🎯 Roadmap

### Planned Features
- [ ] PWA support (offline mode, install prompt)
- [ ] Print-friendly view
- [ ] Student loan calculations
- [ ] Scotland tax rates
- [ ] Multi-year tracking
- [ ] Calendar integration (.ics export)

### Under Consideration
- [ ] Cloud sync (optional)
- [ ] Spending budget tracker
- [ ] Tax optimization suggestions
- [ ] Multi-currency support

## 🤝 Contributing

This is a personal project, but suggestions are welcome!

1. Fork the repository
2. Make your changes
3. Test thoroughly
4. Submit a pull request

## 📄 License

MIT License - Use freely for personal or commercial projects.

## ⚠️ Disclaimer

This tool provides estimates only. Actual tax calculations may vary based on individual circumstances. Always verify with official payslips and HMRC documentation. Not a substitute for professional financial advice.

## 🙏 Credits

- **Design Inspiration**: Modern financial apps
- **Icons**: Emoji (no external dependencies)
- **Fonts**: Inter & JetBrains Mono (Google Fonts)

## 📞 Support

For issues or questions:
1. Check the FAQ above
2. Review the tips in the app
3. Examine the code (it's well-commented!)

---

**Made with ❤️ for UK employees tracking their salary**

*Last updated: April 2026*
