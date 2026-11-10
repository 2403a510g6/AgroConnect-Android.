# AgroConnect Android app

This Android Studio project wraps the existing AgroConnect website:
https://agroconnect-6hff.onrender.com/

## Build the APK on Windows

1. Install **Android Studio** (stable version) and open it.
2. Choose **Open** and select the `AgroConnectAndroid` folder extracted from this ZIP.
3. Allow Android Studio to install the required Android SDK and accept the Gradle sync prompt.
4. Wait until Gradle sync completes.
5. For a test APK, choose **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
6. When the build finishes, click **locate** in the notification.
   The APK is normally at `app/build/outputs/apk/debug/app-debug.apk`.
7. Transfer the APK to your Android phone and install it. If prompted, allow installing apps from that file manager.

## App behavior

- Loads the hosted AgroConnect site rather than copying/replacing its backend.
- JavaScript, local storage, cookies and session persistence are enabled.
- Website navigation stays inside the app.
- Android back button navigates backward through website pages.
- File chooser and download handling are included.
- Camera, microphone and location permissions are requested only if the website asks for them.

## Important

This project source is prepared, but an APK has **not** been compiled in this environment because the Android SDK/Gradle build toolchain is not installed here. You must build it with Android Studio using the steps above. The app requires an internet connection and the hosted website must remain online. Test login, uploads, location, camera and any payment flows on your device before distribution.
