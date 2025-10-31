# Mobile Development with React Native

## Development Environment Setup
1. System Requirements
 - Operating System
 - Node.js
 - Npm
 - Git

### Step 1: Install Node.js and npm
```
node --version
npm --version
```

### Step 2: Install Expo CLI
```
npm install -g expo-cli
or
npx create-expo-app@latest
```

### Step 3: Create First Project
```
# Using npx (recommended)
npx create-expo-app myApp
cd myApp
```

### Step 4: Start the development server (Metro) and open Expo
```
# start Metro + Expo dev server
npx expo start
```

### Step 5: Set Up Mobile Device
 - Install Expo Go app in mobile phone
 - Open Expo Go → Scan QR code from terminal/browser

### Step 6: Set up emulators / simulators
 - Install Android Studio and the Android SDK + at least one AVD (Android Virtual Device).
 - Start the emulator, then in Expo Dev Tools click Run on Android device/emulator, or from terminal:
```
npx expo start
# then press 'a' in the terminal (or use Dev Tools)
```

## Challenges in Setting Up Development Environment
 - **“App won’t load on device”** — check both dev machine and phone are on the same Wi-Fi; try switching Expo’s connection mode to tunnel in Dev Tools if network blocks local connections.
 - **QR scan fails on iOS** — iOS camera can scan QR; if not, use the built-in scanner in Expo Go app. Also ensure Local Network permission is allowed.
 - **Node incompatibilities / weird errors** — use Node LTS and clear node_modules + reinstall (rm -rf node_modules && npm install or yarn). Consider nvm to switch Node versions. 
 - **Emulator won’t start** — ensure Android Studio SDK is installed, AVD system image matches API level, and environment variables (ANDROID_HOME/ANDROID_SDK_ROOT) are set. For iOS: Xcode must be installed and up to date.
 - **Expo Go SDK mismatch** — if your project uses a newer/older Expo SDK than the version of Expo Go installed on your device, you may need a matching Expo Go or use a development build. The Expo docs list SDK versions and matching Expo Go builds.
