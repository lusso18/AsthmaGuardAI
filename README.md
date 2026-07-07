# AsthmaGuardAI

<div align="center">

**An intelligent iOS app with Apple Watch integration for asthma monitoring, management, and emergency response.**

[![iOS](https://img.shields.io/badge/iOS-17%2B-blue)](https://www.apple.com/ios/)
[![Swift](https://img.shields.io/badge/Swift-5.5%2B-orange)](https://swift.org/)
[![License](https://img.shields.io/badge/License-MIT-green)](#license)

</div>

---

## 📋 Overview

AsthmaGuardAI is a comprehensive asthma management solution that leverages AI, real-time health data, and environmental awareness to help users:

- **Monitor** breathing patterns and asthma triggers
- **Predict** asthma attack risk before symptoms worsen
- **Manage** medications and inhaler usage
- **Respond** to emergencies with one-tap emergency contacts
- **Track** health data via Apple Watch and HealthKit
- **Generate** health reports in PDF format

---

## 🎯 Key Features

### 📱 iOS App
- **Dashboard** - Real-time health overview
- **Breathing Check** - AI-powered breathing assessment
- **Inhaler Log** - Track medication usage
- **Risk Assessment Engine** - Predict asthma attacks
- **Emergency Contacts** - Quick access to help
- **PDF Reports** - Share health data with doctors
- **HealthKit Integration** - Connect to Apple Health

### ⌚ Apple Watch App
- **Watch Dashboard** - Quick health status
- **Watch Alerts** - Real-time notifications
- **HealthKit Manager** - Background health data sync

### 🔧 Backend Services
- **Firebase Integration** - Cloud storage & authentication
- **AI Assistant Service** - Intelligent recommendations
- **Push Notifications** - Alert users to risks
- **Environmental Data** - Track air quality & triggers

### 🧠 Shared Components
- **Risk Scoring Engine** - ML-based risk calculation
- **Medication Models** - Drug interaction data
- **User Profiles** - Personalized settings
- **Constants & Models** - Shared across app & watch

---

## 🏗️ Project Structure

```
AsthmaGuardAI/
├── WatchApp/
│   ├── WatchAlerts/               # Alert handling
│   ├── WatchHealth/               # HealthKit for watch
│   └── WatchScreens/              # Watch UI
├── Backend/
│   ├── Firebase/                  # Cloud backend
│   ├── AI/                        # AI services
│   ├── Notifications/             # Push notifications
│   └── Environment/               # Environmental data
├── iOSApp/
│   ├── Emergency/                 # Emergency features
│   ├── Reports/                   # PDF generation
│   ├── Medication/                # Med tracking
│   ├── RiskEngine/                # Risk assessment
│   ├── Screens/                   # UI screens
│   └── Health/                    # Health integration
├── Shared/
│   ├── Models/                    # Data models
│   ├── Constants/                 # App-wide constants
│   └── RiskScoring/               # Scoring logic
├── README.md
└── .gitignore
```

---

## 🚀 Getting Started

### Prerequisites
- **Xcode 14.0+**
- **iOS 17.0+**
- **Swift 5.5+**
- **CocoaPods** (for dependency management)
- **Firebase account** (for backend services)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/lusso18/AsthmaGuardAI.git
   cd AsthmaGuardAI
   ```

2. **Install dependencies** (if using CocoaPods)
   ```bash
   pod install
   open AsthmaGuardAI.xcworkspace
   ```

3. **Configure Firebase**
   - Add `GoogleService-Info.plist` to the project
   - Update Firebase configuration in `FirebaseService.swift`

4. **Build & Run**
   ```bash
   # For iOS
   xcodebuild -scheme AsthmaGuardAI build
   
   # For Watch
   xcodebuild -scheme AsthmaGuardAI_Watch build
   ```

---

## 📲 Core Modules

### 🩺 Risk Assessment Engine
- Analyzes user health data
- Calculates asthma attack risk score
- Triggers alerts based on thresholds

### 💊 Medication Tracking
- Log inhaler usage
- Track medication adherence
- Drug interaction warnings

### 📊 Health Reporting
- Generate PDF reports
- Track trends over time
- Export data for healthcare providers

### 🔔 Smart Notifications
- Real-time alerts via push notifications
- Watch alerts for urgent updates
- Customizable notification preferences

### 🌍 Environmental Integration
- Air quality monitoring
- Weather-based trigger tracking
- Pollen alerts

---

## 🔧 Development

### Code Structure
- **Swift** for iOS and watchOS development
- **SwiftUI** for modern UI components
- **Combine** for reactive programming
- **HealthKit** for health data integration

### Testing
```bash
# Run unit tests
xcodebuild test -scheme AsthmaGuardAI

# Run watch tests
xcodebuild test -scheme AsthmaGuardAI_Watch
```

### Debugging
- Enable detailed logging in `AppConstants.swift`
- Use Xcode debugger for breakpoints
- Check Firebase console for backend logs

---

## 🔐 Security & Privacy

- ✅ HealthKit data encrypted locally
- ✅ Firebase security rules configured
- ✅ HIPAA-compliant data handling
- ✅ No unnecessary data collection
- ✅ User consent for data access

---

## 📝 Contributing

Contributions are welcome! Please:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 🐛 Known Issues

- [ ] Watch app sync delay on cellular connections
- [ ] PDF export performance on large datasets
- [ ] Dark mode inconsistencies in some screens

See [Issues](https://github.com/lusso18/AsthmaGuardAI/issues) for more.

---

## 📄 License

This project is licensed under the **MIT License** - see [LICENSE](LICENSE) file for details.

---

## 👥 Authors

- **lusso18** - Initial development

---

## 🙏 Acknowledgments

- HealthKit framework documentation
- Firebase community support
- asthma.org.uk for medical guidelines
- Apple Developer community

---

## 📞 Support

For issues, questions, or suggestions:
- 📧 [Open an Issue](https://github.com/lusso18/AsthmaGuardAI/issues)
- 💬 [Start a Discussion](https://github.com/lusso18/AsthmaGuardAI/discussions)

---

**Last Updated:** July 2026  
**Status:** Active Development 🔄
