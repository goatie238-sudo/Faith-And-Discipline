# Faith & Discipline Android app

This is an Android Studio project wrapping the Faith & Discipline tracker in an Android WebView. It loads the app locally, and habit data is stored on the device by the web app.

## Build an APK with GitHub Actions (no Android SDK needed on your computer)
1. Create a new GitHub repository.
2. Upload the contents of this folder to the repository (make sure `.github/workflows/build-apk.yml` is included).
3. Open the repository's **Actions** tab and run **Build Android APK** (or push to the `main` branch).
4. When the workflow finishes, open its run and download the `faith-discipline-debug-apk` artifact.
5. Extract the downloaded artifact ZIP to get `app-debug.apk`, then transfer it to your Android phone and install it. Android may ask you to allow installation from that source.

## Build locally
Open this folder in Android Studio and build the `app` debug APK, or run `gradle assembleDebug` with a compatible Gradle installation and Android SDK configured.

## Notes
- This is a debug APK, not a Play Store release.
- The app stores data locally on the device; there is no account/cloud sync.
- Bible verses shown are public-domain King James Version text with references.
