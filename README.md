# DMT Medical App - Proms

Patient-Reported Outcomes Measurement System (PROMS) medical application built with Kotlin for capturing and analyzing patient health data.

## Features

- **Patient Questionnaires**: Structured PROMS collection
- **Health Metrics**: Track symptoms, pain, quality of life
- **Data Analysis**: Visualize trends over time
- **Doctor Integration**: Share reports with healthcare providers
- **Multi-language Support**: Support for multiple languages
- **Offline Mode**: Works without internet connection
- **Secure Storage**: Encrypted patient data
- **Cloud Sync**: Automatic backup to secure server

## Tech Stack

- **Language**: Kotlin
- **Platform**: Android (Native)
- **Architecture**: MVVM + Clean Architecture
- **Database**: Room (local), Firebase (cloud)
- **UI Framework**: Jetpack Compose / Material Design
- **Security**: Encryption, secure storage
- **Build Tool**: Gradle

## Project Structure

```
├── app/src/
│   ├── main/
│   │   ├── java/
│   │   │   ├── data/           # Data layer
│   │   │   ├── domain/         # Business logic
│   │   │   ├── presentation/   # UI layer
│   │   │   └── di/             # Dependency injection
│   │   └── res/                # Resources
│   └── test/                   # Unit tests
├── build.gradle
└── AndroidManifest.xml
```

## Getting Started

### Requirements

- Android Studio Hedgehog+
- Android SDK 24+
- Kotlin 1.9+

### Setup

```bash
# Clone repository
git clone https://github.com/eranCat/DMT---Proms.git

# Open in Android Studio
# Sync Gradle
# Run on emulator or device
```

### Configuration

1. Firebase setup:
   - Create Firebase project
   - Download `google-services.json`
   - Place in `app/` directory

2. Enable services:
   - Realtime Database
   - Cloud Storage
   - Authentication

## Features in Detail

### Questionnaire System
- Pre-built PROMS templates
- Customizable question types (MCQ, Likert, open-ended)
- Progress tracking
- Timed questionnaires

### Data Visualization
- Charts and graphs
- Trend analysis
- Comparison views
- Export to PDF

### Patient Dashboard
- Health overview
- Upcoming questionnaires
- Medical history
- Appointment scheduling

### Doctor Portal
- View patient responses
- Analyze trends
- Generate reports
- Send messages

## API Endpoints

- `GET /patients/:id/responses` - Get patient responses
- `POST /responses` - Submit questionnaire response
- `GET /analytics/:patientId` - Get analytics
- `POST /reports/generate` - Generate report

## Testing

```bash
# Unit tests
./gradlew test

# UI tests
./gradlew connectedAndroidTest

# Code coverage
./gradlew jacocoTestReport
```

## Privacy & Security

- HIPAA compliant
- End-to-end encryption
- Secure authentication
- Data anonymization options
- Regular security audits

## Deployment

```bash
# Build release APK
./gradlew assembleRelease

# Build app bundle for Play Store
./gradlew bundleRelease
```

---

**Empowering patients through health data** 🏥