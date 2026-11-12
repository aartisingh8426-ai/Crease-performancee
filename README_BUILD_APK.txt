CREASE PERFORMANCE — ANDROID APK PROJECT

This is an Android Studio project that wraps the existing Crease Performance app in a native Android WebView.
It keeps the app's HTML/CSS/JavaScript bundled locally. The app's browser localStorage is used for on-device data persistence.

BUILD THE APK
1. Install Android Studio on a computer.
2. Extract this ZIP.
3. In Android Studio choose: File > Open, then select the "crease_performance_android" folder.
4. Allow Gradle sync and install the Android SDK Platform 35 if Android Studio asks.
5. Wait for sync to finish.
6. Choose Build > Build Bundle(s) / APK(s) > Build APK(s).
7. When complete, click "locate" in the notification.
   Expected output: app/build/outputs/apk/debug/app-debug.apk

INSTALL ON YOUR ANDROID PHONE
1. Transfer app-debug.apk to your phone.
2. Open it and allow installation from that file manager if Android asks.
3. Install and launch "Crease Performance".

NOTES
- This is a project ready for Android Studio, not a precompiled APK.
- A real APK must be built with Android SDK + Gradle, which are not installed in the current build environment.
- Data is stored locally on this device/browser profile. Clearing app data will erase it; use the app's export/backup feature regularly.
- Cloud sync and external biometric integrations are not included.
- The current Coach is based on locally recorded data/rules; it is not a connected generative AI service.


OPTIONAL: BUILD AUTOMATICALLY ON GITHUB
A GitHub Actions workflow is included at .github/workflows/build-apk.yml.
1. Create a GitHub repository and upload/push the contents of this project.
2. Open the repository's Actions tab.
3. Run "Build Crease Performance APK" (or push to main).
4. Open the successful workflow run and download the artifact named "crease-performance-debug-apk".
