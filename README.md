# DnD Initiative Tracker - Android App

An Android WebView application that displays the DnD Initiative Tracker web application from [https://yigitsalihemecen.github.io/DnD_Initiative_Tracker/](https://yigitsalihemecen.github.io/DnD_Initiative_Tracker/).

## Features

- 📱 Full-screen WebView experience
- 🔄 Pull-to-refresh functionality
- 🌐 Internet connectivity error handling
- 📱 Mobile-optimized user agent
- ⬅️ Back button navigation support
- 🎨 DnD-themed UI colors (brown and gold)
- 🌙 Dark mode support
- 📊 Loading progress indicator

## Requirements

- Android Studio Flamingo | 2022.2.1 or later
- Android SDK 24 (Android 7.0) or higher
- Target SDK 34 (Android 14)
- Internet connection for loading the web app

## Setup Instructions

1. **Open in Android Studio:**
   - Open Android Studio
   - Click "Open an existing project"
   - Navigate to this project folder and select it

2. **Sync Project:**
   - Android Studio will automatically sync the project
   - Wait for the sync to complete

3. **Build and Run:**
   - Connect an Android device or start an emulator
   - Click the "Run" button or press Shift+F10
   - The app will install and launch automatically

## Project Structure

```
app/
├── src/main/
│   ├── java/com/dndinitiativetracker/app/
│   │   └── MainActivity.java          # Main activity with WebView
│   ├── res/
│   │   ├── layout/
│   │   │   └── activity_main.xml      # Main layout with WebView
│   │   ├── values/
│   │   │   ├── colors.xml             # DnD-themed colors
│   │   │   ├── strings.xml            # App strings
│   │   │   └── themes.xml             # App theme
│   │   ├── values-night/
│   │   │   └── themes.xml             # Dark theme
│   │   └── xml/
│   │       ├── backup_rules.xml       # Backup configuration
│   │       └── data_extraction_rules.xml
│   └── AndroidManifest.xml            # App permissions and config
├── build.gradle                       # App-level build config
├── proguard-rules.pro                 # ProGuard rules
build.gradle                           # Project-level build config
settings.gradle                        # Project settings
└── gradle.properties                  # Gradle properties
```

## Key Features Implemented

### WebView Configuration
- JavaScript enabled for full web app functionality
- DOM storage and app cache enabled
- Mobile user agent for optimal mobile experience
- Local storage support for the DnD tracker

### Error Handling
- Network error detection and user-friendly error dialogs
- Retry functionality when connection fails
- Graceful fallback when the website is unavailable

### User Experience
- Pull-to-refresh to reload the page
- Back button navigation within the web app
- Loading progress indicator
- Portrait orientation lock for better mobile experience

### Theming
- DnD-inspired color scheme (browns and gold)
- Dark mode support
- Material Design 3 components

## Customization

You can customize the app by modifying:

- **Colors:** Edit `app/src/main/res/values/colors.xml`
- **App Name:** Edit `app/src/main/res/values/strings.xml`
- **Theme:** Edit `app/src/main/res/values/themes.xml`
- **URL:** Change the `URL` constant in `MainActivity.java`

## Permissions

The app requires the following permissions:
- `INTERNET`: To load the web application
- `ACCESS_NETWORK_STATE`: To check network connectivity

## Troubleshooting

1. **Build Errors:** Make sure you have the latest Android SDK and build tools
2. **Network Issues:** Ensure the device has internet connectivity
3. **WebView Issues:** Clear app data and cache if the WebView doesn't load properly

## License

This project is open source and available under the MIT License. 